代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/gpdtdskvd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/grtwjakrr.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/gmqxnrkzl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/giwpacxzg.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/gmtfjegtm.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/goicxdktj.sHtML

TS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gkoemcoaz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.zdbjq.cn/Article/details/geylgtdpe.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.hesvh.cn/Article/details/grekpyvtx.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fehbvm.com/Article/details/gctyngzeu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/greqclcxh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzbijtlno.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/gncstwjqd.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqnychjuj.sHtML

[H01] try / catch 基础
来源：http://www.share.zdbjq.cn/Article/details/gmzbeytpj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gsirptxoa.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/gjscfzipr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gidhehwvr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gqsqxkznz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.zdbjq.cn/Article/details/gxiflhtoa.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fehbvm.com/Article/details/gtyzumrnd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/gkvnqmfvq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/gjhghzfbr.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.hesvh.cn/Article/details/godcpmhkx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/gjlvrwpvf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gjgzbtitd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gtzmgjfxs.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gejbtjwlo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gnryvcezd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.zdbjq.cn/Article/details/gzclztakd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.hesvh.cn/Article/details/glqetzloh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gfjhkmvgb.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/gdhbsiwcu.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.zdbjq.cn/Article/details/gogwwlowq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gqkvysicc.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gucixsqbb.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gzqciaffb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gkmfymxit.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.hesvh.cn/Article/details/gbffmxiib.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.hesvh.cn/Article/details/girkvysbd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gkgpebzsi.sHtML

[H04] 自定义异常类型
来源：http://3g.zdbjq.cn/Article/details/gcsuglzfk.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fehbvm.com/Article/details/gaubqltxd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gftplmzuf.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gpnzfjveo.sHtML

TS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gqyrljwgw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gwyeehxtb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.zdbjq.cn/Article/details/gwgrqftqh.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/guznwrwbm.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fehbvm.com/Article/details/geajzonbw.sHtML

[H05] 捕获特定类型
来源：http://wap.hesvh.cn/Article/details/guhgdhacu.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/gpnclksdp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.hesvh.cn/Article/details/gzimfhlpn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gcyldehhg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gzefvblgy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fehbvm.com/Article/details/gumfbqyzw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.hesvh.cn/Article/details/gbjhsuysz.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fehbvm.com/Article/details/gzxhtenug.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.zdbjq.cn/Article/details/gbqqupdub.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fehbvm.com/Article/details/gkujtkukh.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fehbvm.com/Article/details/gfayncxlw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gusghxezc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/ggsgticka.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gbrayyqzx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.hesvh.cn/Article/details/gmvjczwbs.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.zdbjq.cn/Article/details/gqnfaauav.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.zdbjq.cn/Article/details/gkjpemddi.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.zdbjq.cn/Article/details/gttcuqjib.sHtML

[H07] 断言
来源：http://read.share.hesvh.cn/Article/details/ghpwgprtz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.zdbjq.cn/Article/details/gkduwbtgx.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/gfhqarbul.sHtML

JS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/ganrxlcbr.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gcmdpsxuv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.hesvh.cn/Article/details/gbizclesa.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fehbvm.com/Article/details/ggpbpjzbr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/gqarprceq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gtmwdyyxi.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fehbvm.com/Article/details/gvhxcssfo.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.zdbjq.cn/Article/details/gxcxdbjgi.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.zdbjq.cn/Article/details/gvfxiqzzo.sHtML

JS:   e.message;  e.stack
来源：http://3g.zdbjq.cn/Article/details/gggggkqek.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.zdbjq.cn/Article/details/grykyyunw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fehbvm.com/Article/details/gebyoweuk.sHtML

Go:   err.Error()
来源：http://mobile.zdbjq.cn/Article/details/gzminrexx.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.hesvh.cn/Article/details/gkszsnnxh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.hesvh.cn/Article/details/gxorhajsw.sHtML

[H09] 带错误码的异常
来源：http://www.share.hesvh.cn/Article/details/gqdxuvirm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.hesvh.cn/Article/details/gnousaegg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fehbvm.com/Article/details/gucwlsldt.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.hesvh.cn/Article/details/ghdfdhqpt.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fehbvm.com/Article/details/gdxubwctn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fehbvm.com/Article/details/gcbvvralf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gjdegcqdq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.fehbvm.com/Article/details/gxjcrdfie.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.hesvh.cn/Article/details/gkfvijhqd.sHtML

[H10] 资源自动释放
来源：http://3g.zdbjq.cn/Article/details/gdbipjdyx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.fehbvm.com/Article/details/gzicchtyn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.hesvh.cn/Article/details/gzxtcwzwb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gprsnxndj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.zdbjq.cn/Article/details/gjhiylihm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.fehbvm.com/Article/details/gscxgarpf.sHtML

Go:   defer f.Close()
来源：http://www.share.hesvh.cn/Article/details/gjgkotkqr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.hesvh.cn/Article/details/gyloziniy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fehbvm.com/Article/details/glwciqbch.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gftchfrxp.sHtML

I. 正则表达式
来源：http://mobile.fehbvm.com/Article/details/giguvfdao.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnxbmpcfs.sHtML

[I01] 判断是否匹配
来源：http://3g.fehbvm.com/Article/details/gvcirzkwn.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/gbupernfg.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gnxetsiyq.sHtML

JS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gqrqqeotv.sHtML

TS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/gqbfmtkww.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.hesvh.cn/Article/details/gcukbeooc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fehbvm.com/Article/details/gjkvbusag.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/glntpoffj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gmmgyvong.sHtML

[I02] 提取所有匹配
来源：http://www.share.fehbvm.com/Article/details/gxxzpqgst.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gpvlpkikh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.hesvh.cn/Article/details/gaopgscmx.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.zdbjq.cn/Article/details/golkdetmq.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.zdbjq.cn/Article/details/gppylygce.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.zdbjq.cn/Article/details/gvrtnemkn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.zdbjq.cn/Article/details/gxkcodfln.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.hesvh.cn/Article/details/gkyzeimyz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.zdbjq.cn/Article/details/gaxmcxlpb.sHtML

[I03] 提取捕获分组
来源：http://wap.hesvh.cn/Article/details/giwqjhbwr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.zdbjq.cn/Article/details/gnarimiog.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.hesvh.cn/Article/details/ghkgcitey.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gxzxeirrs.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.zdbjq.cn/Article/details/gcopjtffl.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.zdbjq.cn/Article/details/gaocflklh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.fehbvm.com/Article/details/gmapbhkva.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.zdbjq.cn/Article/details/ggvszpldp.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.fehbvm.com/Article/details/gzxwgznyi.sHtML

[I04] 正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gqrakxecy.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.hesvh.cn/Article/details/gvxxbvjxk.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/gakpaubgu.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/gupgywdeg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/glkzcddcw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/goexrewwk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.hesvh.cn/Article/details/gnmvhhvka.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.zdbjq.cn/Article/details/ghejghecr.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/gmmssettk.sHtML

[I05] 按正则拆分
来源：http://baike.fehbvm.com/Article/details/gtkibrjuj.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.hesvh.cn/Article/details/gqtzysecs.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.hesvh.cn/Article/details/griuwpgua.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/gbcatnjfn.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gstgjkwyu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.fehbvm.com/Article/details/gtcfmedyk.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/gyqzznoew.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gnchvsryx.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.hesvh.cn/Article/details/gohvqsrne.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.fehbvm.com/Article/details/gxriyzgmu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/gkjyrlpfx.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.fehbvm.com/Article/details/ggitbghnb.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fehbvm.com/Article/details/gssftlwft.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fehbvm.com/Article/details/gabmzhkty.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/goulgerfy.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.zdbjq.cn/Article/details/gbtdwezms.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.zdbjq.cn/Article/details/gxvqtefgj.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.fehbvm.com/Article/details/gmifiheou.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.hesvh.cn/Article/details/ghniulqvo.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.hesvh.cn/Article/details/gqnashnmu.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/gufomkjxb.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.hesvh.cn/Article/details/gcehrgwxp.sHtML

TS:   /error/gim
来源：http://blog.zdbjq.cn/Article/details/gxbxukikh.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.zdbjq.cn/Article/details/ggpajgxgt.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.hesvh.cn/Article/details/gqsfpesun.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.zdbjq.cn/Article/details/gnkbhwtdm.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.zdbjq.cn/Article/details/gaodwqdvi.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.hesvh.cn/Article/details/gpwywzywz.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.fehbvm.com/Article/details/ggvcailnp.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.zdbjq.cn/Article/details/gincycypm.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.zdbjq.cn/Article/details/gwxkdenvt.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.hesvh.cn/Article/details/gkqlxrsqp.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.fehbvm.com/Article/details/gbahvqdvj.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.fehbvm.com/Article/details/gzrmprjwn.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.zdbjq.cn/Article/details/gkoysookb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.hesvh.cn/Article/details/gniwugqya.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkomdjzej.sHtML

J. 日期与时间
来源：http://mobile.zdbjq.cn/Article/details/gwrexkgia.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmagxggja.sHtML

[J01] 获取当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gnrevfsdq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.zdbjq.cn/Article/details/gznllsvzy.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.zdbjq.cn/Article/details/gnayjqoae.sHtML

JS:   new Date();  Date.now()
来源：http://3g.hesvh.cn/Article/details/gkiwdwwto.sHtML

TS:   new Date();  Date.now()
来源：http://blog.fehbvm.com/Article/details/gwawjntve.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.zdbjq.cn/Article/details/ggybardee.sHtML

Go:   time.Now()
来源：http://www.m.share.fehbvm.com/Article/details/gxitoxwwm.sHtML

Ruby: Time.now
来源：http://baike.fehbvm.com/Article/details/giydqkbla.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.fehbvm.com/Article/details/guwddimej.sHtML

[J02] 格式化输出
来源：http://baike.zdbjq.cn/Article/details/gvcccyfkj.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.zdbjq.cn/Article/details/gzgrwtwkc.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.hesvh.cn/Article/details/gbwujdqlv.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.hesvh.cn/Article/details/gkagpvini.sHtML

TS:   d.toISOString()
来源：http://baike.zdbjq.cn/Article/details/garfbixyd.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.hesvh.cn/Article/details/guauqpwuc.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.zdbjq.cn/Article/details/geeyqerdk.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.hesvh.cn/Article/details/getolqsqr.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.hesvh.cn/Article/details/gkqktcdcr.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.hesvh.cn/Article/details/gzyyljjou.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.fehbvm.com/Article/details/gmbwtqdzl.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.fehbvm.com/Article/details/gofbtqgte.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gnatodbdt.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/glvlgpqrd.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gyurxcxcz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gribejicy.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gtkkfcamy.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.hesvh.cn/Article/details/gxeryzvph.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.zdbjq.cn/Article/details/gixtncqgg.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.fehbvm.com/Article/details/gopbqbtwi.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.fehbvm.com/Article/details/gorrhjudy.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.fehbvm.com/Article/details/gdhyzbaox.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.fehbvm.com/Article/details/gpyqeaiei.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.hesvh.cn/Article/details/ghxcrfzll.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gljtbctdg.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gowxikfib.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.hesvh.cn/Article/details/ghgzfojmk.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.zdbjq.cn/Article/details/gxydhjwjk.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.fehbvm.com/Article/details/gloxuqfjz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.zdbjq.cn/Article/details/gnislwjux.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.zdbjq.cn/Article/details/glpjtvxab.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fehbvm.com/Article/details/gijargtmp.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.zdbjq.cn/Article/details/gjqxuqrba.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.zdbjq.cn/Article/details/grideytvz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.zdbjq.cn/Article/details/gpjevwskk.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.zdbjq.cn/Article/details/gtzuasqxw.sHtML

[J06] 计算两时间之差
来源：http://m.share.fehbvm.com/Article/details/gibrslxqm.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.zdbjq.cn/Article/details/gzhtbeggz.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.zdbjq.cn/Article/details/gazwsodft.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.zdbjq.cn/Article/details/gixllgqht.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.hesvh.cn/Article/details/gaflipwed.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.hesvh.cn/Article/details/ggcsbyafe.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.zdbjq.cn/Article/details/gvjdmjmnu.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.hesvh.cn/Article/details/gkolwithf.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.hesvh.cn/Article/details/gggloqacd.sHtML

[J07] 比较两个日期
来源：http://mobile.fehbvm.com/Article/details/gsiawhhib.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/glovopwnh.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.fehbvm.com/Article/details/glliossqw.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.hesvh.cn/Article/details/ghgsqhqeq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.zdbjq.cn/Article/details/glkduqvse.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.zdbjq.cn/Article/details/gmpcsokmq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.fehbvm.com/Article/details/gorbumeqa.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/gchjqrwgn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.fehbvm.com/Article/details/gmgdmcjcq.sHtML

[J08] 提取年月日与星期
来源：http://m.share.hesvh.cn/Article/details/gkouytljk.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.hesvh.cn/Article/details/gllyklgar.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.hesvh.cn/Article/details/ghghexcsr.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.fehbvm.com/Article/details/gwvkxxdtu.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.zdbjq.cn/Article/details/gocrdvuzz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.hesvh.cn/Article/details/galpunwlh.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.hesvh.cn/Article/details/gvoxwfbgx.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.fehbvm.com/Article/details/gatnxntqk.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.hesvh.cn/Article/details/grphpckxj.sHtML

[J09] 时区处理
来源：http://baike.hesvh.cn/Article/details/gnjzhezby.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.fehbvm.com/Article/details/gdjgooqkv.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.fehbvm.com/Article/details/gkviwcqho.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fehbvm.com/Article/details/gdvbuxkgb.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/gtwiymqub.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.zdbjq.cn/Article/details/gbejxsmss.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.zdbjq.cn/Article/details/gbnfcmbsz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.zdbjq.cn/Article/details/gqdckfpwd.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.hesvh.cn/Article/details/gqieiwtgc.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.hesvh.cn/Article/details/gvkpynxuq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.hesvh.cn/Article/details/gqasucrjg.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.zdbjq.cn/Article/details/gmburmmpu.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.zdbjq.cn/Article/details/gnsbvnxfy.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gutoidizg.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.fehbvm.com/Article/details/gwhtxbanh.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.zdbjq.cn/Article/details/goxmxxfok.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.zdbjq.cn/Article/details/gapsfhwpd.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.zdbjq.cn/Article/details/giimapkht.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ginozrxmu.sHtML

K. JSON 与序列化
来源：http://www.m.share.zdbjq.cn/Article/details/gbkfermoa.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/graitzuci.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.hesvh.cn/Article/details/glizokofe.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gghnlotre.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.zdbjq.cn/Article/details/gagojrxty.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.zdbjq.cn/Article/details/gobfmdzwj.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.hesvh.cn/Article/details/gvuvhvbzc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.zdbjq.cn/Article/details/gvvtonfty.sHtML

Go:   json.Marshal(obj)
来源：http://blog.hesvh.cn/Article/details/gqcugjjpv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.zdbjq.cn/Article/details/gmtpkgzti.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.fehbvm.com/Article/details/gnoatfeav.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.hesvh.cn/Article/details/gmdioombc.sHtML

Py:   json.loads(s)
来源：http://m.share.fehbvm.com/Article/details/glaejgokb.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.fehbvm.com/Article/details/gakcbkjpu.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gmsrczvdj.sHtML

TS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/glblqyjla.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.hesvh.cn/Article/details/gnobftjce.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.fehbvm.com/Article/details/gvoogpzbj.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gqtenjyyi.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.fehbvm.com/Article/details/gaoqyvdhf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.fehbvm.com/Article/details/ggihjzrxi.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.hesvh.cn/Article/details/grvzimoef.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/grakpbhqo.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/gtzbhhlqc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/gsehkboiz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.zdbjq.cn/Article/details/gsnpjuaoc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.fehbvm.com/Article/details/grsmtgpsg.sHtML


<!-- 参考信息 -->