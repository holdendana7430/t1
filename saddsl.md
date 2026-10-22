代发 wailian999

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2uhmvjixu.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2nlzyfqfs.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qbehbmiy.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2xmrmlgmp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2lehorbxj.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cyoeqwsn.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pygfppye.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pvvwhhxl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2jmkfpwzf.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2pcijuiyi.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2eutzbuga.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2ooqqshmy.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2impxzioi.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pfsccodn.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jdrcbygk.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2huajnkky.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qwfxnkwj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2uuzaymli.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2cchcedsd.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2wjuofgie.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2fcqrlfuf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2umpbwxpr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2knpnmjfy.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2lbschodc.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2alkjvsch.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2uwnspite.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2soepcyak.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2nucnwmsj.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2inwjrvcf.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2oannavcx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2fzlarflc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ervjmunk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2pzavxzrt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hqtueypi.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2vyglfbrn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2trpfhlgt.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2npfnaskx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ansudwrd.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2afviecfr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2enctpzos.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2vvqgxuwk.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2uehwolel.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2xeltndwb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2kfmhdovf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2oxwajfuc.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2idcsvswh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2zftzafaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xygmmnso.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2rrdzzvar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sodybyjf.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2sumobmpm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2gpbzyhyq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zojlhhlw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2koutioab.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2bdoeyjwe.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2rlfilzdc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2xlmugvfr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2yqygkebh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2qlchafxx.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2pvawbnyo.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2ezrfvtfm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2arkuewpe.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ebyhagza.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qjhzywrj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kurselpn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2qlvdnrld.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2ufhmdlec.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vmezmibk.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2zxpqykwy.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2hffgaeej.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fwwkevda.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qltookxp.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qvnaxtqr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rnvhzpgk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2lvhpeosm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2kuebczrv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gkwllmix.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2ggmvypuo.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2zfozjjxh.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ycghhwds.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2eifpexak.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2grnkpeov.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2jtlwudlr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2nrkiqqpi.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2ourybfhf.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2dgsocjvh.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2zkldwvsa.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2vgrqojrc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2uhsztwht.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2reztfrpd.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nzlknmis.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2inswzhad.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2rteavpxu.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2faefgylj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2wbehrhyz.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2nqqpxmli.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2flminvpv.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2tcgbjqwa.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ajsbebuk.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2sxnpjlew.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2zsgqlvzf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2eyysuiij.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2hpjooqbb.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2bjcrfuff.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2mqwgvjdm.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2xwtyrhch.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vtkxzyvs.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zityptdv.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vchcscyd.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2vfjlbjwm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2npkkkgec.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2operabzn.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2acztxbqp.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2xketfwkq.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2wuxifywg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2uvsdvxwv.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2zcxebcvf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2forbrcpp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2nzuzdqgg.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2svifrtvg.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2zdtgkshl.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2sztlhcmq.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2xmixzckp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2qwmvdrmt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2xwprgigt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2fkwvebqt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2mkrbitqj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2lueegvvy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2vgrpewvv.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2vwmalyiw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2idatnewy.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2mvzdfafd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2bautzfcj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2kutxtgrj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2wxthzaqv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2ksauinji.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2mbcoxobg.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2zynlsfdm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2iekqyrxw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xoazhdbi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mzogpkhy.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mhkjchjo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cyndvevb.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2xfkgdnox.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ftdhqqae.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ojnfnxxf.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2xqczdqls.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2shfsboqr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2wuipzrkw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2gqshymgv.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2aobioixz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2iasipwqq.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2ugfzseis.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2iwvhchuj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2fxtyfxsb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2ntzqlczw.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2tvwdrret.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2hoeqotpr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2tqylumks.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2rnsanpxy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xnhwtann.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2lumrsrgo.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2somuzhti.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2tcsgpfmq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2zktcswav.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2nztaooup.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2lwbciljb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2gwvqlrxt.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2liyoxjiz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2akaqydjx.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2gejexbjb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2dcikiwxc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2mylyuano.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2pjfezzgc.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2rzsmwtkk.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2edcnieub.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2wuwbyzxp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2lxrfepib.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2blikijss.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2uwiqdskq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rwnluwbg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jiptrwzk.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2byrgeeos.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2cwcnsufw.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2nznocpqe.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2dngubpij.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ojsdpynb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2szqxcqcw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2onimjltf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2qdjkqztw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2ykxhcpgc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2ugchapio.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2vcotybbp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ufpjxjuc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2ljpihwps.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2nvndiwjf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2cqkuycen.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2kpufvlck.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2dfbgwqhp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2bifkkxjd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2tzfztauh.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2fvwzckmu.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2onccsccu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2xechqfrj.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2juailgln.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2mwqgxcyi.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2zkupnxhb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2uuskmxcc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2zoyprrnb.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2iaceuznr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2zlgwlsjs.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2yvpuopsl.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2eeeevwul.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2zwnucequ.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2unpxnaeb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kufqypki.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2rfckkkxd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qzpysdkg.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2nyvdhihv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2ihmijwpr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2kdsefznj.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2rjbpatwa.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2vsowzxyy.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2vggedvkd.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2syaqvlmr.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2gkylewjs.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2pfijdlky.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2cwjnuduh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2fquwjfbo.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2rwqgnmty.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2mqoqgzty.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2vwgxootq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2kxxnumgu.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2ayohsdah.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2tumeqoov.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2wjaoepcs.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2nhfessnp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2ngxpebxv.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2yxgzpplr.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2wicojbkh.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2vdrdpicx.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ommekttr.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2hlsllssw.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2nzkisctd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2ngedfhwx.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2nnhqults.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2iyesjzgr.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2javmrdnl.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2unkewqxo.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2rvgtpene.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2lhwukghi.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2okpjkrsr.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2ugaezroc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2jtaeqbjw.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2yexbfrav.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2sgbzxrko.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2rxtivgvg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2dfzcdjgy.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2mlltpbwh.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2vasjrgxv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2pfmmyqxk.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2nmptvjkj.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2tsehfsps.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2dgvfyacr.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2odoahdxr.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2ombkgksc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2egamfhjw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2xohxxevp.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2qrgqsriq.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2jruwsnku.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2gknpidrb.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2mhptlbpe.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2jgplftnk.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ykmnsdfg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2ppyknnwk.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2shclubtt.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2rbpkscop.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2eyyqbqvb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2dktftykd.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2pgqudqsj.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2yoqbnpor.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2tessdoii.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2knxuxmmq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2hrpktbky.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2ihtllzsq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2nfzwbxmi.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2wlajohay.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2zduqpics.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2npgvjsjw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2qneucepa.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2qsjhitto.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2hrnqiiow.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2idbfvxdt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2hbopgbhx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2tmgusdjc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2amyftyda.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2nyrbpdsv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2xoiuyapg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2zstmwyry.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2vyckrtmj.html


<!-- 参考信息 -->