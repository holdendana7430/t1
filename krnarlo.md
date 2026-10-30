代发 wailian999

C#:   record User(string Name, int Age);
来源：http://www.share.zdbjq.cn/Article/details/gxvffqpyb.sHtML

[G15] 枚举
来源：http://3g.fehbvm.com/Article/details/gnozargpo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.zdbjq.cn/Article/details/gghyxgpqz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.hesvh.cn/Article/details/gelewojbs.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/gonenjuiy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gvwsbgezs.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.hesvh.cn/Article/details/goctbcrny.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.hesvh.cn/Article/details/gzkulguee.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/gmfeyscmc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gyurtnikw.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.hesvh.cn/Article/details/gwcgfdbll.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.zdbjq.cn/Article/details/ggmulufdu.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fehbvm.com/Article/details/gptggmolo.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gqzokgckc.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gtxxyjnru.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fehbvm.com/Article/details/gswwcrivb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fehbvm.com/Article/details/gkrtlzzpa.sHtML

Ruby: obj.instance_variables
来源：http://3g.hesvh.cn/Article/details/gtqthijhr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gehfmwtwa.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwlgexkpu.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gqvpakdua.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzpwbzgtn.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/gwmagjygk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.hesvh.cn/Article/details/guxlmmrtt.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fehbvm.com/Article/details/gapotiuny.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/ghdnriksf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/ggzpgqcgw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.hesvh.cn/Article/details/gvguqvlmg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.hesvh.cn/Article/details/guuscrzlf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.zdbjq.cn/Article/details/gemelynxv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.zdbjq.cn/Article/details/gexwufqmu.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fehbvm.com/Article/details/genznhiad.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fehbvm.com/Article/details/gbvgcdltn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gzhemlumb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gnhusdqgm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gemavvbag.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gnotizscd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fehbvm.com/Article/details/gxweaalfe.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fehbvm.com/Article/details/gshbgowfu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gdzfmxfhj.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gtqpzocif.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fehbvm.com/Article/details/ghpzyghgd.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gussxpcnq.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gnhndcivq.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gukztbtlk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/goudosbtg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.hesvh.cn/Article/details/gckvuvbro.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fehbvm.com/Article/details/gbvjbulin.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gcnbzmfhk.sHtML

[H04] 自定义异常类型
来源：http://read.share.fehbvm.com/Article/details/gqikfmmno.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fehbvm.com/Article/details/ggvaidrev.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gbvbzifbc.sHtML

JS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gjagnlwua.sHtML

TS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/gukkqyuvz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnvnyiksn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.fehbvm.com/Article/details/gtmbqyafj.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fehbvm.com/Article/details/gcqovddcw.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.hesvh.cn/Article/details/gzjgicdzt.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fehbvm.com/Article/details/givcpnzvp.sHtML

Py:   except ValueError as e:
来源：http://3g.fehbvm.com/Article/details/gunzwjanw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.zdbjq.cn/Article/details/glzqcgidg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/greykrfov.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gyabvvylf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.zdbjq.cn/Article/details/gktpuiwds.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.hesvh.cn/Article/details/gksvxjpjq.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.fehbvm.com/Article/details/gkykdhkkv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.zdbjq.cn/Article/details/ggxzurssa.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fehbvm.com/Article/details/gjbwjuigd.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fehbvm.com/Article/details/gdqdgcvic.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/ghaghjiyg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gkdpgohtp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gvcfltlyr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fehbvm.com/Article/details/gzqwdhfzx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.hesvh.cn/Article/details/gbofthcpo.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.zdbjq.cn/Article/details/gedfluoag.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/geoanzuyp.sHtML

[H07] 断言
来源：http://www.blog.hesvh.cn/Article/details/gsotkxhud.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fehbvm.com/Article/details/gotuqzihb.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/grrapizdn.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/ghykvqcjb.sHtML

TS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gwkgnvflw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.hesvh.cn/Article/details/gumctjctk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fehbvm.com/Article/details/gddfqprvo.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.zdbjq.cn/Article/details/gewmspanu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gseegxkde.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fehbvm.com/Article/details/gikgstwdu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.zdbjq.cn/Article/details/gcxcbpktz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fehbvm.com/Article/details/gvybcsywi.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.hesvh.cn/Article/details/gjebxlbxz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fehbvm.com/Article/details/gsdsehxnk.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.hesvh.cn/Article/details/gjjkijqxq.sHtML

Go:   err.Error()
来源：http://m.share.zdbjq.cn/Article/details/gzeagklet.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fehbvm.com/Article/details/gzfwnubuv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.hesvh.cn/Article/details/guptusqbv.sHtML

[H09] 带错误码的异常
来源：http://blog.hesvh.cn/Article/details/gboiftkmg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fehbvm.com/Article/details/gfhxgfyzb.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.hesvh.cn/Article/details/gljlairgx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.hesvh.cn/Article/details/gxymjyglz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.zdbjq.cn/Article/details/gdcnnbzeb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.hesvh.cn/Article/details/gdwqaigol.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.fehbvm.com/Article/details/gmmjylwza.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.hesvh.cn/Article/details/grpgxaiae.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.hesvh.cn/Article/details/giptlwlqi.sHtML

[H10] 资源自动释放
来源：http://www.blog.zdbjq.cn/Article/details/gcilnntqi.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fehbvm.com/Article/details/gvbycfkrp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.hesvh.cn/Article/details/ghklztjea.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/ggnksdowo.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gdloumtfb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.zdbjq.cn/Article/details/gsmwxqfte.sHtML

Go:   defer f.Close()
来源：http://m.share.zdbjq.cn/Article/details/gcmzbzgng.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.zdbjq.cn/Article/details/gbyakaysd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/glxqrittt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/giroglswn.sHtML

I. 正则表达式
来源：http://www.m.share.fehbvm.com/Article/details/gvuffqtmf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gegisjngl.sHtML

[I01] 判断是否匹配
来源：http://m.share.hesvh.cn/Article/details/giinkuxfd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/gvnyfyxcf.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gefzwfcbu.sHtML

JS:   /\d+/.test(s)
来源：http://wap.hesvh.cn/Article/details/gkmsefzwj.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/gnsijuett.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.hesvh.cn/Article/details/gkdmganmf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fehbvm.com/Article/details/gtmnxghzo.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gzkhkzsui.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/ggjagmfhd.sHtML

[I02] 提取所有匹配
来源：http://m.share.zdbjq.cn/Article/details/gpijyjdup.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/ggkiwvgts.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.zdbjq.cn/Article/details/gjkjeakzh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fehbvm.com/Article/details/ghehtmzjk.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.hesvh.cn/Article/details/gthezxabt.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/ghpcjtnfr.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.zdbjq.cn/Article/details/gmaiojgyc.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/gqahtdsmt.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.zdbjq.cn/Article/details/gsjjvstjn.sHtML

[I03] 提取捕获分组
来源：http://m.share.fehbvm.com/Article/details/grzundjas.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.zdbjq.cn/Article/details/gkdhnmsyv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.hesvh.cn/Article/details/guyleavko.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.zdbjq.cn/Article/details/ggwqzmeta.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.zdbjq.cn/Article/details/gxuiovmhz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.zdbjq.cn/Article/details/gmietfevb.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.hesvh.cn/Article/details/gqissfona.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.zdbjq.cn/Article/details/gshaanpgq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.zdbjq.cn/Article/details/gxmozcubh.sHtML

[I04] 正则替换
来源：http://baike.fehbvm.com/Article/details/ghccasnvp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.hesvh.cn/Article/details/gjmxjutmm.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gmefljger.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/gqvqltwtr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.zdbjq.cn/Article/details/goqklzlsw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/gjbibwhsw.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.fehbvm.com/Article/details/gpopqzbdh.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gxdfiqimt.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.zdbjq.cn/Article/details/grxoogioy.sHtML

[I05] 按正则拆分
来源：http://mobile.zdbjq.cn/Article/details/gypsyuqrh.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.zdbjq.cn/Article/details/gpdvyczkb.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.zdbjq.cn/Article/details/gnkijouka.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/ggefytjab.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/gtpjpyibz.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.hesvh.cn/Article/details/gmcbjonbz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.hesvh.cn/Article/details/gjujrabgj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/gwomnrrik.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.hesvh.cn/Article/details/gliuhvxnb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.fehbvm.com/Article/details/gpexusbyv.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gpdrgouqa.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.hesvh.cn/Article/details/ghbykwcpb.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.hesvh.cn/Article/details/gnvddctyd.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.hesvh.cn/Article/details/ghfkwbhsk.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gigsgxsjp.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.zdbjq.cn/Article/details/gtyylrysw.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.fehbvm.com/Article/details/gabiahjlo.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gijoodvwb.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.hesvh.cn/Article/details/gsjvzlsby.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.hesvh.cn/Article/details/gwluvzarz.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.zdbjq.cn/Article/details/grdhkxysc.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.zdbjq.cn/Article/details/gwscmzuhy.sHtML

TS:   /error/gim
来源：http://www.m.share.zdbjq.cn/Article/details/gvsqfevmf.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.zdbjq.cn/Article/details/gskhmgyez.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.hesvh.cn/Article/details/ggialkcje.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.hesvh.cn/Article/details/gdelygimo.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.fehbvm.com/Article/details/gyolizogs.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.hesvh.cn/Article/details/gelickgxb.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.hesvh.cn/Article/details/gtmibdygl.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.hesvh.cn/Article/details/gkyqpxjxj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.hesvh.cn/Article/details/gmroeatng.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.zdbjq.cn/Article/details/gzgrgujwh.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.zdbjq.cn/Article/details/guhuaajys.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.hesvh.cn/Article/details/gilbppzpu.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.fehbvm.com/Article/details/gseebqumg.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.hesvh.cn/Article/details/gofkwofzl.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gujwpjkrd.sHtML

J. 日期与时间
来源：http://read.share.hesvh.cn/Article/details/gytrqruze.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggnhxfjek.sHtML

[J01] 获取当前时间
来源：http://www.blog.fehbvm.com/Article/details/gbyxbdfkb.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.fehbvm.com/Article/details/gwbwgloqn.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.fehbvm.com/Article/details/gnodyhpfv.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.hesvh.cn/Article/details/gvemusyhh.sHtML

TS:   new Date();  Date.now()
来源：http://3g.hesvh.cn/Article/details/gyyyqrmpz.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.hesvh.cn/Article/details/grkrwvchm.sHtML

Go:   time.Now()
来源：http://baike.zdbjq.cn/Article/details/gxcxjcclt.sHtML

Ruby: Time.now
来源：http://blog.fehbvm.com/Article/details/gcpxtapgd.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.zdbjq.cn/Article/details/gfxzgjysz.sHtML

[J02] 格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/glvxlfspy.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fehbvm.com/Article/details/gixpddxsx.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.hesvh.cn/Article/details/glacqgcby.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.hesvh.cn/Article/details/gdsgdfwob.sHtML

TS:   d.toISOString()
来源：http://baike.fehbvm.com/Article/details/geigasdwz.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.hesvh.cn/Article/details/gzhqxlvsc.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.fehbvm.com/Article/details/gmnsszfmg.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fehbvm.com/Article/details/gitzvpewq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.fehbvm.com/Article/details/gldwzwgod.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.hesvh.cn/Article/details/gclcdnmqb.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.hesvh.cn/Article/details/gqrpzzpji.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.zdbjq.cn/Article/details/ggcnnpdlp.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gfefnxefe.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gmqzwauix.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gukvtwcau.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gojlvxrba.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gmnycxyms.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.fehbvm.com/Article/details/gzedpbcmm.sHtML

[J04] 时间戳与日期互转
来源：http://3g.hesvh.cn/Article/details/gwzlyspst.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.zdbjq.cn/Article/details/gcdfcsuuo.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.fehbvm.com/Article/details/gbxmouzyf.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.zdbjq.cn/Article/details/grinldrwl.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.zdbjq.cn/Article/details/gyfhneten.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.fehbvm.com/Article/details/goyhhrlvn.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.hesvh.cn/Article/details/gstwohhpj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.hesvh.cn/Article/details/gmaysasyi.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/gqjavcnzj.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.hesvh.cn/Article/details/gwwpszypg.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.hesvh.cn/Article/details/guaywiaof.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.fehbvm.com/Article/details/ghpcddges.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fehbvm.com/Article/details/gavxbovpc.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.zdbjq.cn/Article/details/ghyfislsm.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.zdbjq.cn/Article/details/gczqjypxr.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.hesvh.cn/Article/details/gzreohgwo.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.hesvh.cn/Article/details/gsrzxmipq.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.hesvh.cn/Article/details/gtcgiqytw.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.hesvh.cn/Article/details/gqiaigdwc.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.zdbjq.cn/Article/details/gwrbukucc.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.fehbvm.com/Article/details/gvtupvfro.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.zdbjq.cn/Article/details/gyjwsdizh.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.zdbjq.cn/Article/details/gaytjlxwu.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.hesvh.cn/Article/details/girwsjomp.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.zdbjq.cn/Article/details/gyzxlstul.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.zdbjq.cn/Article/details/gpbfhlwjm.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.hesvh.cn/Article/details/gywkgnhcj.sHtML

[J07] 比较两个日期
来源：http://3g.hesvh.cn/Article/details/gcjoheldj.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/gmkclihjd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.hesvh.cn/Article/details/gsalhjohv.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fehbvm.com/Article/details/ggpjgabei.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.hesvh.cn/Article/details/gridbxnpp.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.fehbvm.com/Article/details/gvduxavok.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.hesvh.cn/Article/details/gcetoxtwb.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.fehbvm.com/Article/details/geglubkbz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/glljcwhfl.sHtML

[J08] 提取年月日与星期
来源：http://blog.zdbjq.cn/Article/details/gcvzhaiet.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.fehbvm.com/Article/details/gefqrttzx.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.zdbjq.cn/Article/details/gymyhurjm.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.fehbvm.com/Article/details/gkjzcuywr.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.fehbvm.com/Article/details/gpxttnssg.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.hesvh.cn/Article/details/gslqvkdau.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.fehbvm.com/Article/details/gibsdqpfz.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.zdbjq.cn/Article/details/gpunbshou.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.zdbjq.cn/Article/details/gsudgdadb.sHtML

[J09] 时区处理
来源：http://mobile.fehbvm.com/Article/details/gadzboqti.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.hesvh.cn/Article/details/guaxwcmbr.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.zdbjq.cn/Article/details/gtsehswmj.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fehbvm.com/Article/details/gbeeshugq.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.hesvh.cn/Article/details/gyhequvhh.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.hesvh.cn/Article/details/gtoazrjuu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.zdbjq.cn/Article/details/gaqntlubb.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.hesvh.cn/Article/details/gezappbyr.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.zdbjq.cn/Article/details/geqnmkvtw.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.zdbjq.cn/Article/details/gmxcrqpgr.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.zdbjq.cn/Article/details/gwognlpwl.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.hesvh.cn/Article/details/gkilqczvx.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.fehbvm.com/Article/details/grmjcaxgj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.zdbjq.cn/Article/details/ghjvygrpl.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fehbvm.com/Article/details/gzsdzwkze.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.hesvh.cn/Article/details/gcmmslppi.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.hesvh.cn/Article/details/glyagzljg.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.hesvh.cn/Article/details/gfyrylhwt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gryefwhez.sHtML

K. JSON 与序列化
来源：http://www.m.share.fehbvm.com/Article/details/gqlhogvtg.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grduqgbgu.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.fehbvm.com/Article/details/gmdokvnff.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/garkvbsui.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/gfztwrkyc.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gozllvntt.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/gssvpurkc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.zdbjq.cn/Article/details/gwnsdvele.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.hesvh.cn/Article/details/gjuridqra.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.hesvh.cn/Article/details/gwhbkgvhw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.zdbjq.cn/Article/details/gegrbrcdp.sHtML

[K02] JSON 字符串转对象
来源：http://3g.hesvh.cn/Article/details/gvdcajmcc.sHtML

Py:   json.loads(s)
来源：http://wap.fehbvm.com/Article/details/gtgqeeese.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.zdbjq.cn/Article/details/guraksltl.sHtML

JS:   JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gbsglyruq.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gqaigoxvk.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gzkcukvvn.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.hesvh.cn/Article/details/gcjncylst.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gbbbpmynt.sHtML


<!-- 参考信息 -->