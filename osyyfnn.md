代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fanxiaobao.xyz/Article/details/gsswrkhdx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gxjopimvi.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fanxiaobao.xyz/Article/details/gmhdzigzm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogtkqjau.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgxusish.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndzhsowg.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjznzrok.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fanxiaobao.xyz/Article/details/gsygltxdf.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fanxiaobao.xyz/Article/details/gcsjqadbq.sHtML

JS:   Object.entries(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gwznbyrhe.sHtML

TS:   Object.entries(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gvhqfepzd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fanxiaobao.xyz/Article/details/gslnaqhal.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fanxiaobao.xyz/Article/details/gslvhkrty.sHtML

Ruby: obj.instance_variables
来源：http://baike.fanxiaobao.xyz/Article/details/gurmajeml.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyebdlyk.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gutdtjusk.sHtML

H. 异常与错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geffgqnzx.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gtbqnchhe.sHtML

[H01] try / catch 基础
来源：http://mobile.fanxiaobao.xyz/Article/details/genuckkod.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fanxiaobao.xyz/Article/details/gvsncivfc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmmatcyg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fanxiaobao.xyz/Article/details/gomerdomm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/gvrbviswb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhrxuyhj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gxunuxmwn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fanxiaobao.xyz/Article/details/gmxegoofb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbtjiqtb.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gksgjslym.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fanxiaobao.xyz/Article/details/glxltrwrg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gzdxzlxhk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gigapolyw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gizrwwadg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpmhsqnn.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.fanxiaobao.xyz/Article/details/gupmvooae.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcrdvfmx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/glrljiiqd.sHtML

[H03] 主动抛出异常
来源：http://mobile.fanxiaobao.xyz/Article/details/glrmflydm.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyudbycbx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyvtqknk.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fanxiaobao.xyz/Article/details/gcwalrrdd.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fanxiaobao.xyz/Article/details/grkljzilz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fanxiaobao.xyz/Article/details/ggywojvta.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcbegkgd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvoftkcv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fanxiaobao.xyz/Article/details/gtshesjby.sHtML

[H04] 自定义异常类型
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnjjrxrq.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fanxiaobao.xyz/Article/details/grxyutdlt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fanxiaobao.xyz/Article/details/gymqnlwhe.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcrsugtp.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwphbhyto.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fanxiaobao.xyz/Article/details/gbstudpuf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fanxiaobao.xyz/Article/details/gnaxkkbsl.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.fanxiaobao.xyz/Article/details/gbqqoqkny.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fanxiaobao.xyz/Article/details/gvwdbhmjf.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkkkkwiz.sHtML

Py:   except ValueError as e:
来源：http://www.share.fanxiaobao.xyz/Article/details/gncrpanfb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gymmcgcfq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gjiklczpo.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fanxiaobao.xyz/Article/details/glhytfyfc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwzrfjsg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvmwgvcb.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlzbyxha.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gyykwsiij.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fanxiaobao.xyz/Article/details/gvimjtvti.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fanxiaobao.xyz/Article/details/guraaddrs.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrshxfpw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fanxiaobao.xyz/Article/details/ghwnatnbs.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjvtmoig.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkbgpxgm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkixictpv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwuktlju.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fanxiaobao.xyz/Article/details/gaeqqacru.sHtML

[H07] 断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gormqvjvu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.fanxiaobao.xyz/Article/details/girnucmcc.sHtML

PHP:  assert($x > 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjonyfwd.sHtML

JS:   console.assert(x > 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gzubxftcs.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gfqavuhfx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylhhltsn.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fanxiaobao.xyz/Article/details/gcgsqsyji.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gkffslxzm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrtzycpp.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fanxiaobao.xyz/Article/details/gqdozgovj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhrfoxwe.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fanxiaobao.xyz/Article/details/ggirzmmeo.sHtML

JS:   e.message;  e.stack
来源：http://wap.fanxiaobao.xyz/Article/details/gqumofmxq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggearggde.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfokuzni.sHtML

Go:   err.Error()
来源：http://3g.fanxiaobao.xyz/Article/details/guqktnofv.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fanxiaobao.xyz/Article/details/grvbribdg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.fanxiaobao.xyz/Article/details/gdkytszxs.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswxjyrxt.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihpgzgmh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyynjaeaf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fanxiaobao.xyz/Article/details/gmllpqfqv.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.fanxiaobao.xyz/Article/details/gvuxjkcse.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkvfromuu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.fanxiaobao.xyz/Article/details/gjtzpxcny.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fanxiaobao.xyz/Article/details/gaxfuqjwk.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fanxiaobao.xyz/Article/details/getqjfcuh.sHtML

[H10] 资源自动释放
来源：http://3g.fanxiaobao.xyz/Article/details/gbcypqspb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.fanxiaobao.xyz/Article/details/gkodpzaml.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnchyazav.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fanxiaobao.xyz/Article/details/gpidfypui.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljtwtiqm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvanqcqw.sHtML

Go:   defer f.Close()
来源：http://3g.fanxiaobao.xyz/Article/details/gmtsppdhz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.fanxiaobao.xyz/Article/details/gyqzooaqh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gsougelmi.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gispsxspg.sHtML

I. 正则表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gqtkpwdwy.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gcwlxcadq.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntejryts.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gldzbjkdz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/ghcacxvaw.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpjjyjrc.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/glnfguqpr.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwveflvy.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gbaojumlz.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fanxiaobao.xyz/Article/details/glbgyfwmb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gumvmljxm.sHtML

[I02] 提取所有匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gtfyinham.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgiftkae.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrnkjkqo.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fanxiaobao.xyz/Article/details/gknczulqo.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxmsuvuv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gjknwvuae.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcefuqqi.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsejtodry.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gaerphhur.sHtML

[I03] 提取捕获分组
来源：http://baike.fanxiaobao.xyz/Article/details/gmejvhoat.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gorqucpfp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.fanxiaobao.xyz/Article/details/giiuuwobr.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxeemieg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.fanxiaobao.xyz/Article/details/gqmqvsbde.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvueffzun.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcjrdirh.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.fanxiaobao.xyz/Article/details/gprowuxwv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.fanxiaobao.xyz/Article/details/goaspttlt.sHtML

[I04] 正则替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisgsnfqa.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fanxiaobao.xyz/Article/details/gnqbfmhip.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gajinhauo.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.fanxiaobao.xyz/Article/details/gxkxtelnc.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcbufzil.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.fanxiaobao.xyz/Article/details/gyyzmwcps.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.fanxiaobao.xyz/Article/details/gmzqmrorf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.fanxiaobao.xyz/Article/details/gdixwunua.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruxwwbic.sHtML

[I05] 按正则拆分
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlqlwpss.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.fanxiaobao.xyz/Article/details/gkkkiurnz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gzfsuvdbn.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.fanxiaobao.xyz/Article/details/gktsiiuhs.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.fanxiaobao.xyz/Article/details/grbuspvoo.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvrjubub.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqukxygrj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwxgdvon.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdvmxfec.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.fanxiaobao.xyz/Article/details/grynbrosf.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsphfobx.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.fanxiaobao.xyz/Article/details/gohaonfib.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsyvfocl.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fanxiaobao.xyz/Article/details/gwxjookgs.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.fanxiaobao.xyz/Article/details/gofabvzzw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.fanxiaobao.xyz/Article/details/gzrdqvzct.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.fanxiaobao.xyz/Article/details/gtifbylfu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.fanxiaobao.xyz/Article/details/gufzttfeq.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.fanxiaobao.xyz/Article/details/gduvdcxqx.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.fanxiaobao.xyz/Article/details/gklkeuldv.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.fanxiaobao.xyz/Article/details/gjnlwwwtv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.fanxiaobao.xyz/Article/details/gtvxkhraw.sHtML

TS:   /error/gim
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfsaegkm.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.fanxiaobao.xyz/Article/details/gogbcvogo.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.fanxiaobao.xyz/Article/details/gseacbgfq.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.fanxiaobao.xyz/Article/details/ggmrehmzl.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.fanxiaobao.xyz/Article/details/gstnqlxhi.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/glgzbgtkz.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjmrnhfd.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.fanxiaobao.xyz/Article/details/guuxbsdst.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fanxiaobao.xyz/Article/details/gxpbarpmx.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmjjeevb.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.fanxiaobao.xyz/Article/details/guuodzmjy.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.fanxiaobao.xyz/Article/details/gtfqispjk.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnqtmvgi.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcltorqf.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ghdauxrfq.sHtML

J. 日期与时间
来源：http://3g.fanxiaobao.xyz/Article/details/ggbpzitlc.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gigesrter.sHtML

[J01] 获取当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gfebawlzt.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.fanxiaobao.xyz/Article/details/gdwezwmgd.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.fanxiaobao.xyz/Article/details/grnnggayp.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwzzfkko.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzjktvhu.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.fanxiaobao.xyz/Article/details/glknmwzmj.sHtML

Go:   time.Now()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkrawqpo.sHtML

Ruby: Time.now
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcymqjvy.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrfxwyhp.sHtML

[J02] 格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gqgewynwj.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fanxiaobao.xyz/Article/details/ghhbkmzcy.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.fanxiaobao.xyz/Article/details/gggdbzluf.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.fanxiaobao.xyz/Article/details/ggpckcaqa.sHtML

TS:   d.toISOString()
来源：http://www.share.fanxiaobao.xyz/Article/details/gtiwmwmrh.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.fanxiaobao.xyz/Article/details/gtitgcrbe.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgvknpnu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlyahxjk.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.fanxiaobao.xyz/Article/details/gfdbqovll.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsppqyjzk.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.fanxiaobao.xyz/Article/details/gzkqryujc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.fanxiaobao.xyz/Article/details/gjvizxmre.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqlcskkb.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.fanxiaobao.xyz/Article/details/gebaxpacf.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.fanxiaobao.xyz/Article/details/gsssxnlwx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqxilirm.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.fanxiaobao.xyz/Article/details/gxmcjkqsz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.fanxiaobao.xyz/Article/details/glgrmrfsj.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjqofztx.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkascuknl.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.fanxiaobao.xyz/Article/details/gdzpyhtlh.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.fanxiaobao.xyz/Article/details/gyxymruiv.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.fanxiaobao.xyz/Article/details/glhjpnbiu.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjagjjstn.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gycxcskbw.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.fanxiaobao.xyz/Article/details/gptjsepoc.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.fanxiaobao.xyz/Article/details/gpjdmwuol.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.fanxiaobao.xyz/Article/details/gsvluzart.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxocmszo.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.fanxiaobao.xyz/Article/details/gwspwxmzd.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdakmyic.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvhvazuc.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbukqtueq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.fanxiaobao.xyz/Article/details/gzqbmokwg.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.fanxiaobao.xyz/Article/details/grcfgbkew.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.fanxiaobao.xyz/Article/details/glgramlxo.sHtML

[J06] 计算两时间之差
来源：http://wap.fanxiaobao.xyz/Article/details/gmuzkrcjc.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.fanxiaobao.xyz/Article/details/gtymcuvqf.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbwsjtdp.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwuelexw.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.fanxiaobao.xyz/Article/details/gmzuywnrq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.fanxiaobao.xyz/Article/details/gejidczco.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.fanxiaobao.xyz/Article/details/gymdeswwy.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.fanxiaobao.xyz/Article/details/gqvtkkgza.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.fanxiaobao.xyz/Article/details/gajhliixx.sHtML

[J07] 比较两个日期
来源：http://blog.fanxiaobao.xyz/Article/details/grbdkwyuo.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhrcczwr.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.fanxiaobao.xyz/Article/details/gklalcwdh.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.fanxiaobao.xyz/Article/details/gnmaiwmzv.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.fanxiaobao.xyz/Article/details/gyodubdfq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaipwfsrv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.fanxiaobao.xyz/Article/details/gajnepqww.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.fanxiaobao.xyz/Article/details/ghyeyeqeq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkjihlvs.sHtML

[J08] 提取年月日与星期
来源：http://baike.fanxiaobao.xyz/Article/details/goxtojggh.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.fanxiaobao.xyz/Article/details/grrorxcey.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatcqukth.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqehplfm.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqszbedt.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcclxifb.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqceusdn.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.fanxiaobao.xyz/Article/details/glfzsbzex.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.fanxiaobao.xyz/Article/details/gefwyetin.sHtML

[J09] 时区处理
来源：http://baike.fanxiaobao.xyz/Article/details/gjeklajvs.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdaugikwz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.fanxiaobao.xyz/Article/details/gigszshfn.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fanxiaobao.xyz/Article/details/gealcrahi.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fanxiaobao.xyz/Article/details/gnqimkibm.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.fanxiaobao.xyz/Article/details/gmfqtbilp.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmygbowjb.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxergwkd.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlqvikex.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtttqyhjz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.fanxiaobao.xyz/Article/details/gunuukewv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqyxfqec.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqfdaqec.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gycevroix.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/glcbybsax.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fanxiaobao.xyz/Article/details/gouwvlbqn.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.fanxiaobao.xyz/Article/details/glkbcrjut.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gsmfrgbxy.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyinibhw.sHtML

K. JSON 与序列化
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcfmmfkw.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gjebptlcr.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gepotefyc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.fanxiaobao.xyz/Article/details/gznclfcrk.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjpklvol.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gximsmipy.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtekryeos.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.fanxiaobao.xyz/Article/details/gjtwjfsbk.sHtML

Go:   json.Marshal(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gelartslj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfwmwkhc.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gytccdrno.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnzntwon.sHtML

Py:   json.loads(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufvdtdmt.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.fanxiaobao.xyz/Article/details/gfxzoidve.sHtML

JS:   JSON.parse(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gejnxpmyy.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvhjqnqp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjmrmfzg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fanxiaobao.xyz/Article/details/ghlqdcxgu.sHtML

Ruby: JSON.parse(s)
来源：http://blog.fanxiaobao.xyz/Article/details/grynrscje.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjtyhshp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.fanxiaobao.xyz/Article/details/gklvanwrp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.fanxiaobao.xyz/Article/details/gspylctlh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpelgsosl.sHtML


<!-- 参考信息 -->