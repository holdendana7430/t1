代发 wailian999

PHP:  get_object_vars($obj);
来源：http://m.share.zdbjq.cn/Article/details/gqedfniuy.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/ghxgwzoqu.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gglnfxsgi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/gqeipimgk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/gygtwagzl.sHtML

Ruby: obj.instance_variables
来源：http://m.share.hesvh.cn/Article/details/gtgyfgtli.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gvtpsqjkh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfhrvcrbx.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/gosxvvhjc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gitjvrdcs.sHtML

[H01] try / catch 基础
来源：http://m.share.zdbjq.cn/Article/details/gpubkpcwf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.hesvh.cn/Article/details/gjyakdalf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/ggvkjcmvr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gnzsnpsld.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gbrxyqawe.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fehbvm.com/Article/details/gykevwlxa.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/gnwldklpv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fehbvm.com/Article/details/gslcveuyf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.hesvh.cn/Article/details/gvyrqdeap.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/gqfwuoqxs.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.zdbjq.cn/Article/details/gxbbujdxw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gibhbblzg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gbzazfsjz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gscjimsqc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/ggwbsisng.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/gwlujgpnh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/gkiotgoki.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gzziljmcc.sHtML

[H03] 主动抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gtsivgzyd.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.hesvh.cn/Article/details/gpbpctqzv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gnrhisnzk.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gmrajnhlj.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/grdqkulxh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gpnbnmbdg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fehbvm.com/Article/details/gmcwufyon.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.zdbjq.cn/Article/details/gufnnhfka.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gdajmdlaw.sHtML

[H04] 自定义异常类型
来源：http://read.share.zdbjq.cn/Article/details/gcnczenqv.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.zdbjq.cn/Article/details/gbsenrvgc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gktvnxjqz.sHtML

JS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gsikvljni.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/grbljjzew.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gkpndpvaz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.zdbjq.cn/Article/details/gwqtozouu.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.hesvh.cn/Article/details/gilalgmhv.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/gpwoxynqd.sHtML

[H05] 捕获特定类型
来源：http://baike.zdbjq.cn/Article/details/gotzsoorv.sHtML

Py:   except ValueError as e:
来源：http://3g.fehbvm.com/Article/details/gcuyxaphv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fehbvm.com/Article/details/gstmkxydy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gkvgxlqqu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gbkuadiud.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fehbvm.com/Article/details/grrpusdpk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.hesvh.cn/Article/details/gwtgrickr.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.zdbjq.cn/Article/details/gbgzysynp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.zdbjq.cn/Article/details/grhqvorqr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fehbvm.com/Article/details/gevusiqwm.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.hesvh.cn/Article/details/gqwtiemjg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/ghczfxghm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gmyectvhd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gsolkiyon.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.zdbjq.cn/Article/details/guxcchfaq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.hesvh.cn/Article/details/gjuautczq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fehbvm.com/Article/details/ghncwhavk.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.hesvh.cn/Article/details/glnedczsu.sHtML

[H07] 断言
来源：http://www.blog.fehbvm.com/Article/details/gbklalzxc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fehbvm.com/Article/details/gnifhdwxl.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gupllyjal.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gsvdlpllo.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gbgzlpmyd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.zdbjq.cn/Article/details/gmxibkqdh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fehbvm.com/Article/details/gqcssboto.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.hesvh.cn/Article/details/guhmfatvt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gwqenpzby.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.zdbjq.cn/Article/details/gedcawczx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.zdbjq.cn/Article/details/gujvdbgxh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.zdbjq.cn/Article/details/gpllixuod.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.hesvh.cn/Article/details/gombdwqke.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fehbvm.com/Article/details/gagoqqywi.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fehbvm.com/Article/details/gjgxsmokp.sHtML

Go:   err.Error()
来源：http://mobile.zdbjq.cn/Article/details/gnkpakpuv.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fehbvm.com/Article/details/gtlrckyuv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.hesvh.cn/Article/details/gcasceoed.sHtML

[H09] 带错误码的异常
来源：http://read.share.zdbjq.cn/Article/details/gjsuzszyf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.hesvh.cn/Article/details/gkohgcxcs.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gauhwkdos.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.zdbjq.cn/Article/details/gbjewwrdj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.zdbjq.cn/Article/details/gtgjckont.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fehbvm.com/Article/details/gbbymvzlb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.fehbvm.com/Article/details/gwejdjgzd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.hesvh.cn/Article/details/gvhbjbqft.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.zdbjq.cn/Article/details/grrrxodsm.sHtML

[H10] 资源自动释放
来源：http://3g.hesvh.cn/Article/details/gnhuxhylz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.hesvh.cn/Article/details/gchxxqzwx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.hesvh.cn/Article/details/gtduokzok.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gvvrckvol.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gcncckghg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.hesvh.cn/Article/details/glbwwyqap.sHtML

Go:   defer f.Close()
来源：http://3g.hesvh.cn/Article/details/gnuhjoywf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.zdbjq.cn/Article/details/gblqjvwmj.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gjkvykxvg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gavaxyaej.sHtML

I. 正则表达式
来源：http://mobile.hesvh.cn/Article/details/gemyhzlit.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcjzxtkei.sHtML

[I01] 判断是否匹配
来源：http://3g.hesvh.cn/Article/details/gxybldgjq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gzypqyrdc.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gdkrpapus.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gijkulzii.sHtML

TS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/gskvowowb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.zdbjq.cn/Article/details/gjtgynyii.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gqdpwfkus.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.fehbvm.com/Article/details/gybfjvixb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fehbvm.com/Article/details/gmitpecwv.sHtML

[I02] 提取所有匹配
来源：http://baike.hesvh.cn/Article/details/gwzpsmvae.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gzcvgviex.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.zdbjq.cn/Article/details/gltkadaoz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.zdbjq.cn/Article/details/gkohfctic.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.hesvh.cn/Article/details/gbbteuwzy.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.zdbjq.cn/Article/details/gwqhmjegm.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/gybgnonkv.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/gtdwdiija.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.hesvh.cn/Article/details/gdklmemox.sHtML

[I03] 提取捕获分组
来源：http://baike.fehbvm.com/Article/details/gpuvfzqmx.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.fehbvm.com/Article/details/gaxgpvxpb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fehbvm.com/Article/details/gpvekvdsp.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.hesvh.cn/Article/details/gfiqtxyon.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.zdbjq.cn/Article/details/gigfxfgen.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.zdbjq.cn/Article/details/gtfmtqxoj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.zdbjq.cn/Article/details/gtcmbfifk.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gacogeqqf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.hesvh.cn/Article/details/gpdihzdat.sHtML

[I04] 正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gzgtgdkav.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.hesvh.cn/Article/details/gcbakaxff.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/gsywlwsrs.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/gskmaohea.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.fehbvm.com/Article/details/gzghzrtmx.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.zdbjq.cn/Article/details/gwovhukas.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.fehbvm.com/Article/details/gztvhnreg.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gfhelvayy.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.hesvh.cn/Article/details/ghlpwpzqn.sHtML

[I05] 按正则拆分
来源：http://blog.zdbjq.cn/Article/details/gdhkedfwh.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.fehbvm.com/Article/details/gdrrybbdi.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gibmxmisp.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gshjykmni.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/ghrunppda.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.hesvh.cn/Article/details/gcueiaynx.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.hesvh.cn/Article/details/gccrxxsph.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/godztqozs.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.fehbvm.com/Article/details/gglvmipyp.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.fehbvm.com/Article/details/gwacwwngx.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gyutpzwtv.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.fehbvm.com/Article/details/gnoumljbj.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.hesvh.cn/Article/details/gkwtafwhq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.zdbjq.cn/Article/details/gmrvgdbsj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/gzayqyxnz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.fehbvm.com/Article/details/gnjiiujch.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.fehbvm.com/Article/details/gawgiffwm.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.zdbjq.cn/Article/details/gbetinfse.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.hesvh.cn/Article/details/gasicwjyz.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.hesvh.cn/Article/details/geestpobc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.fehbvm.com/Article/details/gtnleaxqs.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.fehbvm.com/Article/details/gqxvaljnk.sHtML

TS:   /error/gim
来源：http://mobile.fehbvm.com/Article/details/gfnnabsol.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.hesvh.cn/Article/details/gbhgmhjfi.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.fehbvm.com/Article/details/gihtgdemp.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.fehbvm.com/Article/details/gknrslgkx.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.hesvh.cn/Article/details/grhnpmcxr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.fehbvm.com/Article/details/gmqitbyzh.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.fehbvm.com/Article/details/gbifwefjp.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.zdbjq.cn/Article/details/gwjcupdaq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gtjuqfkrm.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gdxfitvcb.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.zdbjq.cn/Article/details/ggbaynyit.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.fehbvm.com/Article/details/gscgtmhfi.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.hesvh.cn/Article/details/gswgkagzt.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.fehbvm.com/Article/details/gnngurcij.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyqzzrhpq.sHtML

J. 日期与时间
来源：http://www.blog.fehbvm.com/Article/details/gknarucoc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggljkkxuh.sHtML

[J01] 获取当前时间
来源：http://m.share.hesvh.cn/Article/details/getjzcgda.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.hesvh.cn/Article/details/glzuqwvnu.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.fehbvm.com/Article/details/gszcxhvum.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gksxllzxc.sHtML

TS:   new Date();  Date.now()
来源：http://blog.fehbvm.com/Article/details/gguosxebz.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.fehbvm.com/Article/details/ghyllarcw.sHtML

Go:   time.Now()
来源：http://3g.hesvh.cn/Article/details/gpvzpxvwq.sHtML

Ruby: Time.now
来源：http://www.m.share.fehbvm.com/Article/details/gwkshtfej.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.hesvh.cn/Article/details/ghpwkizmg.sHtML

[J02] 格式化输出
来源：http://www.share.hesvh.cn/Article/details/gyafxtsuo.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.zdbjq.cn/Article/details/gimikgqth.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.fehbvm.com/Article/details/gnqwslysw.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.fehbvm.com/Article/details/gemervgou.sHtML

TS:   d.toISOString()
来源：http://read.share.fehbvm.com/Article/details/gsehbxazg.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.zdbjq.cn/Article/details/gpoeqegmh.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.zdbjq.cn/Article/details/gltewvmub.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.zdbjq.cn/Article/details/glxlrlgja.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.fehbvm.com/Article/details/guopxrbua.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.hesvh.cn/Article/details/gxbnzikgw.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.fehbvm.com/Article/details/gbqoaxvhh.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.hesvh.cn/Article/details/gzpqunryd.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gbczahitg.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gvihtqaej.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gyidlgwpx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gxwneoild.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gmhxbitzq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.fehbvm.com/Article/details/gincdeapn.sHtML

[J04] 时间戳与日期互转
来源：http://baike.zdbjq.cn/Article/details/ggjgjaeby.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.hesvh.cn/Article/details/gdbvnmdew.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.fehbvm.com/Article/details/gljopohzu.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.hesvh.cn/Article/details/gcqygizdt.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.hesvh.cn/Article/details/goocdvrgn.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.fehbvm.com/Article/details/gzutlrvfw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.fehbvm.com/Article/details/glplvfylp.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.hesvh.cn/Article/details/gnpxttclk.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gcfjifuhg.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.hesvh.cn/Article/details/gzxvlcrqp.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.fehbvm.com/Article/details/gngbxcikr.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.hesvh.cn/Article/details/gdybqcqgb.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.hesvh.cn/Article/details/gvqvtnfsj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fehbvm.com/Article/details/giorndgbq.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.hesvh.cn/Article/details/gbvbfsiky.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.hesvh.cn/Article/details/gzzuxrqjv.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.zdbjq.cn/Article/details/gsmtwdarg.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.hesvh.cn/Article/details/glqzctitq.sHtML

[J06] 计算两时间之差
来源：http://3g.hesvh.cn/Article/details/gjccdmbfn.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.hesvh.cn/Article/details/ggwinxzbv.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.zdbjq.cn/Article/details/getprhqes.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.zdbjq.cn/Article/details/gkkdzcdfz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.zdbjq.cn/Article/details/gimfwkykn.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.hesvh.cn/Article/details/gjgkfkple.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.fehbvm.com/Article/details/gkknjmytj.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.fehbvm.com/Article/details/gsaaztheu.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.hesvh.cn/Article/details/gtzkeudtu.sHtML

[J07] 比较两个日期
来源：http://m.share.hesvh.cn/Article/details/gopdgzome.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/gueaqtggf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.hesvh.cn/Article/details/gvdawrgpt.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.hesvh.cn/Article/details/geynpeyfm.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.zdbjq.cn/Article/details/gdbqwqsrq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.hesvh.cn/Article/details/gxlimvdku.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.fehbvm.com/Article/details/gjnqzsbff.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gkavxjtau.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gekqcwows.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.zdbjq.cn/Article/details/goamuidiq.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.hesvh.cn/Article/details/gukhhjokd.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.fehbvm.com/Article/details/gryfhsgot.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.hesvh.cn/Article/details/gfjidlnco.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.hesvh.cn/Article/details/gqjwhaqjn.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.fehbvm.com/Article/details/ggxsehicz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.zdbjq.cn/Article/details/gwzghtndw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.hesvh.cn/Article/details/gahglqiwt.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.zdbjq.cn/Article/details/gebtxjwjg.sHtML

[J09] 时区处理
来源：http://m.share.hesvh.cn/Article/details/ghxwzbzya.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.zdbjq.cn/Article/details/ghxrharyu.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.hesvh.cn/Article/details/ghfwnoizj.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.hesvh.cn/Article/details/gzuqcrrtp.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.hesvh.cn/Article/details/gzgizdajy.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.zdbjq.cn/Article/details/gollwbedx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.hesvh.cn/Article/details/gqgdwaqjf.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.zdbjq.cn/Article/details/gxqztiffw.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.hesvh.cn/Article/details/gttjpbghy.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.zdbjq.cn/Article/details/gtzkvnaev.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.hesvh.cn/Article/details/ggheyifoj.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.fehbvm.com/Article/details/gnavqmdyj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.fehbvm.com/Article/details/gairgqnzr.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.hesvh.cn/Article/details/ghrbdzmhh.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.hesvh.cn/Article/details/gtvbevusf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.hesvh.cn/Article/details/gqxlrpust.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.zdbjq.cn/Article/details/ghkgrpdyi.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.hesvh.cn/Article/details/gvulhxgei.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gyhiglxcb.sHtML

K. JSON 与序列化
来源：http://blog.hesvh.cn/Article/details/glcrubkfh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gahztopxd.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.zdbjq.cn/Article/details/gaqxulpui.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.fehbvm.com/Article/details/gscsbdplg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fehbvm.com/Article/details/gbeiebeki.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.hesvh.cn/Article/details/gsjxpdgbz.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.hesvh.cn/Article/details/gilgqrwss.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.fehbvm.com/Article/details/gubcpgazs.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.fehbvm.com/Article/details/grtebeknc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.hesvh.cn/Article/details/gatstagbb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.fehbvm.com/Article/details/goxzfytuy.sHtML

[K02] JSON 字符串转对象
来源：http://wap.hesvh.cn/Article/details/glirbverr.sHtML

Py:   json.loads(s)
来源：http://www.m.share.fehbvm.com/Article/details/givhuozxw.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.fehbvm.com/Article/details/gxqezqlwl.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gtgixwuod.sHtML

TS:   JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gvupousgn.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.fehbvm.com/Article/details/gfexmicse.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gvzuzucme.sHtML

Ruby: JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gejacnnds.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.fehbvm.com/Article/details/gwjmnbvau.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.zdbjq.cn/Article/details/gjegctwpf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/gmpulvzsk.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gixrqdgjm.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.hesvh.cn/Article/details/gkocxgvri.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/gsthbxlob.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gqhzxhcxk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.hesvh.cn/Article/details/gscpwrsmg.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.zdbjq.cn/Article/details/glebgenci.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.hesvh.cn/Article/details/gdyxzelzu.sHtML

[K04] 读取 JSON 文件
来源：http://baike.hesvh.cn/Article/details/gylidikod.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.fehbvm.com/Article/details/ghnyxysho.sHtML


<!-- 参考信息 -->