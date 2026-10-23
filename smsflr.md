代发 wailian999

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3zjqlcxud.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3ofslzjln.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3zcozxdzf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfzmxroi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3iwzezqkd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3nviiyekl.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3qzjriomu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3pvyrjjdi.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3eanyqikh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3rfzpxcty.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3fkjcqcyd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3nsubhens.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3etdfocwf.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ekjpftjq.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3wgwqkvne.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3kibvdifu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3hrxhezbm.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3invdtmlf.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3elwcqlav.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pxdqwttc.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3tcsmywvz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pbdczkck.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3etmleqjw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3xdufrnio.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xewzgmlt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3kiwnfduv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ftpdjwsx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3unymawyb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3jdrjkosi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3lchqqfsr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3wxlkmyka.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3ivmnxeev.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3inkcnnhx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fncvyxcf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pfbrhbti.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xgecsvbp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3swdkuntu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3ookcsrbp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3rznrfife.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mmjwajrb.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3tnuibpfq.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3tngervts.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3pcdlfjwr.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jqygchmg.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3fjsxifzy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3sbhtcwlp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3tmobrgds.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3hlyhjbaq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mllbvxih.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3fljoauhl.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3bozmabxk.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3nubdgfxt.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3oazprjpc.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3gnaukdgx.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3upeiaexy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3xrdccozi.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3yrijjbup.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3vfacfmit.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3ozjbhkvs.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3yeqekbzl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3dzdxpfzm.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pbsgqyye.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kuhhwshq.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hoerptnu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3atqmoojd.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3ykwnhahu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yasdpypl.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3cdbmwbgn.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3bygphcyh.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ayuzniry.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3mkdujklr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3aupsixfl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3vgbfnnri.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3nryuckau.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3vynbyfqv.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3ehrbmgpv.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3ihwculvz.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3lebduhrm.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3lrxatmoe.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3igqxvude.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bzcwiwxo.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3wqfcwmbb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3eiifimdh.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3ybgdqjmc.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3tdukgvup.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3kwjcjzya.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3jagpfdfr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3ufgtyrmq.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3nowfbqve.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3bqojftuu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3wpcwichw.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3ylzlgsot.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3ainnsnyg.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3usflwzvn.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3esbshmtd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3qgaoynjc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3uzeabays.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3pqepeeua.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3srnshdyt.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3euffnjhe.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3rlkneoiz.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3fybjbjff.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3azlwfwkx.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3ywgzzcwo.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3nchnmukq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3rnyuacrj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3pvpkigzf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3apigtcio.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3jsoefwrw.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3kezduznq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3ohcazgdf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3plhrmnvs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ftlvdsex.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3aopkanam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iozklbwn.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3avauoifd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3kfswzikk.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ilqjylzz.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3thczpegz.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vvfabjjr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3edsqrztx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3cbaqfqhx.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3wolespdp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3omrmckye.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nmewjtqd.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ngbenirl.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3mwneusxj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3bbzznlay.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3wjttlhfh.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3vsqxuvvd.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3orcxsrlg.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3zwhzszgj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mphgatyx.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3mjlrsilb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3alhovtha.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3wyxwgwdk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3zgjkqpne.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3bcwvlecn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3jvscedqb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3mjzcplac.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3quusepba.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3cbxevent.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3lvkusjjj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3gfrdfktd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ozresfhe.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3oquzvfhn.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3lurbdirc.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3ymdkbtsh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3bldunxxd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3xbcajinm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3paienloo.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3gijuxiny.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3peirqpdq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3xnceizpg.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3amvehfwd.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3kwrttdrl.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3wyuggdts.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3fdriozzk.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3rhruusuc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3jvifrier.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3mjbwpjer.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3wozqnfta.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3zlpzzdkj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3oerocdgv.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3hawkyorr.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3eiepzscd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3apiqvcee.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3ngpiwsmb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3cyuvfjxi.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3xqhcoibm.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3gvlucmth.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3uattpfnd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3rmjmpmic.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3ctcnkybe.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3beqienoo.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3avzapgcu.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3tjzwxnaw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3anpcrygl.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ovgykmfu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3wyadwyzo.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3drldxbga.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3azrqqpiv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3qrtdmrht.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3lqrcncsh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3grzsjspp.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3szujjmlq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3tubbzqqk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xmrkkoun.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3ymunwjbn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wkbdiupd.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3prlfioqn.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3nkuqkzdw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3dqcmkgtk.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3hstajbgu.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3jkdzrkmi.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3eibxutkv.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3cedgjzxw.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3dihigrdt.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3xajouejn.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3oikrpszj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3pxmfflps.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3nyztybds.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3jocbyrmw.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3satutmad.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3boqjrlhe.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3uavafixt.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3lcyfhkyx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3rgjrohyp.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3zqyvgxvo.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3iwdwmrmm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3ziwpomuu.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3mijzhduy.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vcfeptrm.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ixzxctdm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3yeezjhrx.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3xrioeboy.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3becuwvpm.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3lgemmjey.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ioggubbv.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3dexhfeck.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3fyejxdjs.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3pqitpchb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3shfjrtbq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3svlmufuy.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3wrknhiio.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ytwelseq.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3dutrrvue.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3lsfhxzvu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3efsyskgf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3xibwvoph.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3auywkoft.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3cwtyydmj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3elmzinyj.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3pvjwigvy.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3deowvwqn.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3kojzkxtm.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3ffnwvrvl.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3zsummdzw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3tkyvtdio.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3hbrshtto.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3tpbwmbme.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3pdttxjpt.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3tkmgpiaq.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3bikjaxjf.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3teszquga.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3sxhaijxx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3vgygphco.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3ldrdtktu.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3imzfawwk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3ijmmztmh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3kdvporjs.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3jicfdiic.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3uphknfqk.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3bebuyenj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3mlkefhho.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3dgssqsnx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3vufhlihm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3nvodcgzo.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3vjijiwgd.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3gabjoaxd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3gbmfsuvp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3gmstsfsz.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3coydhssr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3ydzeplwq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3yuufoitv.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3oblgoctg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ecuopqwm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3salukbrr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3bqsuddkk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3kkxcessx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3tulsalyv.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3ckekzlck.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3ktvevwkf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3bratqzkc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3izsrdpnb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3flezogya.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tbfidbfn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3bdjmeqqr.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3eycqxier.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3gacrbzap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3efmypiip.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3lwgliatn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dmcwghmh.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3duapiraz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3cvlfaaml.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3jsyzqbao.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3ckedmyfm.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qmaqpvho.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3ffngceso.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qwodfonf.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3mafrvxmt.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3ppedwyyx.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3ejyvjedh.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xnyfljmm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3xlqtcomo.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3veerqllk.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xeppleei.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ktyghiwk.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3smjafogy.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3trgkxjkz.html


<!-- 参考信息 -->