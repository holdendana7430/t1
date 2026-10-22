代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2qzifcdbe.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2aisuguhg.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2rcjdcype.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2dwakydxd.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2unrngdzq.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rmlxbdbn.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2aafkpmyl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2mrkcuiry.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2txentzml.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2loqzsbxm.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2wmdqehhb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ldvusgvd.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2xibxtazl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oqrebblt.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2tzdqrzuj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2gobsgxfc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xropsloj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2xkncrpzk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2cfgzhwfi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2dqdxtegp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2gdkyaesl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2ffvqorkr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2fwsfehly.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2wsgutxxg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2qndeqesy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uugrykqf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gkjxmfit.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hirwkkjc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2djdsmjgc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2vexrscrq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2meczkkct.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gndsmkfw.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2lsiwbprg.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2fufmauzp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gkngwogu.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hdhaahjc.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ysmbanoj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2sgmltkmp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2skfrhocv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2gxzepmzj.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2oomhlvee.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2jpesiskd.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2sovcigwc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2zyvfrpqg.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2hlyrqdvw.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2hrgdrlox.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2feidsuhf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2wijsohhu.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2dmomxtwc.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2nnvqnnvq.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2atphniem.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2yznsrhrq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2wiakheag.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ajnohyky.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ihdcrxml.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ullkvxel.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2ltuyfpei.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2jjeahkwc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2tosvwoei.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2ztwdavta.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2jgkmeotn.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2jkekqrru.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2vbxektmr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2boklpque.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2qozfgpsi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2nsidhweb.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2puhirhgh.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2pyuljaqc.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2tpbytqjo.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2aliavygt.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2trxepzmf.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sfaqrzbn.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2chfmjjur.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2mwyponvt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2cimzqbwv.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2sxkuncwc.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2gcyxwuhy.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2zglmlbdt.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2krysywxh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2uqrwaybo.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2lcinazba.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2rigclplt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2fahydxzc.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2ykcqvdcz.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2zvcokekp.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2zljffrzx.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2bmrvgdmo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2eyakgrgc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2fvwzqehd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2kgpiqmam.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2niidonxa.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2pkxrqkgf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2vgjmjmtm.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2qqygjsxf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2esskvbzf.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2yrtzcjun.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2shvyqfnc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2hopcbhkd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2vhwghooz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2fvwzvegn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2rycbpeij.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2hdracnis.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2ystvlvgn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2greptdnk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qtabrvnx.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2dwpxpurf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ssictnsw.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2scxiwoxn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2yvftvysw.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2nvlbutls.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2cejrbjyt.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2rskfzqad.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2uuxuffcq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2ggfxagvv.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2bpndkhyc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2pyyaorqb.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kltppvno.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rponnyqh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2yiihalmv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2wmznigpo.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2wfclsfrx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2rycgqkqh.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ligjvomt.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2arvdxmje.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hkmtlwqt.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2lrjravkr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ijxkufqk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2idkhqwqq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2wbxoptvc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2yscdyfnl.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2couhteaf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2sgemwxvv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2jlrdtzri.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2bpsqucle.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2fscyhbvj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2mupmkzfg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2fvmnkbdn.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2jgcgekfd.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2uslgpkwv.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2dpffhguw.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2ydmvdlni.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2idilcnhu.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2yximjktq.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2jdknnkxn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2zgnvekyf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2momrzhrn.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2tmcswpfd.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2lqqcgqov.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2qzfpcore.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2vrhgdupf.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2gscwkrmm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2gstsybjj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2hhmwayst.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2iemsqjku.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2dtrzcmjd.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2jqogphuz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2mrzykdrg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2rztpocpm.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2bwifhlna.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2nchepfzc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2wgzkizes.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2jgwzulja.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2kuugmwql.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2uvcctycj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2ksfubqxt.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2hoaibwaw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2fitqejlc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2efwagsju.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2qkoziznb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2tvmeyoem.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dqatydcv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2gmuucmcz.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2qlzdhytb.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2xjghtemv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2drfxnhsy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2wnxsurub.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2nxwcrjme.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2ofhaaeoq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2ijudylmk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nxwgahil.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2eytpxsud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ujjekpcc.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2pjnoaxap.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2aoovcryt.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2trlqjfvk.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2lovcpyvu.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ucvcmvyh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2cprpaimi.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2zorztxet.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2wdrvqpoo.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2pfbkcixn.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2sifsaqxq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2piasacoj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2gifzcbkt.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2yrwppsge.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2vwsotvmu.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2djupxgxs.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2frnfaimv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2xenlaabu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2spsswzhe.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2mkjkkubz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2gjinkyup.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2yxwlgljk.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2qnigufcj.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2vaoaxjnz.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ecgcqxfv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2embyefoo.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2iliqrhuk.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2wsvwfrdk.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2tmtkplvt.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2eilqpzxd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2laorqebr.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2kkutftrq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2gtopegmt.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2qlhrhfdg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yrnqiprb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2gvjhwije.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2qpcdoywm.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2wlemlcej.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2ozbswkky.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2mwknvnbe.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2bxtsusjf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2zjhwbiem.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2domlbion.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2seohjefh.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2nixttnqn.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2izgolxei.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2vqzcauac.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2ugweldjm.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2wanvxcnb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2uysskbqa.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2nwccshku.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2llnlsgxc.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2vmttsuqr.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2vubcsyvq.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2jueaiefu.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2yuzsrali.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2zwiazgkd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2ojazhbzb.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2upfmxpdq.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2lnarjmsx.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2rjywthot.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2igvlsgfz.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2mmxnvtuu.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2agoujweg.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2cisvfcmr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2uhzgqsqh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2ccmnjyqg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2hbaerxii.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2ssvvttkl.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2liaxjbya.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2tqxnwvtr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2mlsiwyqg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2rydwnxkc.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2owjftknu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2xtuyznle.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2zpoudajz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2drzzyxhd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2jzhurnty.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2paxbmguf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2hqblemox.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2itmrafiw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2mvmyanxo.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2fiofedwz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2dazxbmrh.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2jmlauyfo.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2waggtaoj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dxzuizum.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2fdurtphl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2gmainvmp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2axttfpft.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xunpbevo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rqoxfxqr.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2zgmowxtd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jlkajwvb.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gamvcxdi.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2zwftdwfn.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2fjxvabdn.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2ntgeqfnd.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2twpkbgco.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2kwuzizys.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nnyqhagx.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2sajjhshe.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ksnvsimu.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2jvzakfnr.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xlyrazgv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2pmkatuhy.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ogcljuyw.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hpligvuy.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2oljamwjr.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ioaphhne.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2pmfjzkrd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dwmbcekn.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2kdwztjit.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2yquyywtr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2lfxcjcrv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2idxjkdvo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zebcmdac.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2ubghwkfa.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2wqhpcvxv.html


<!-- 参考信息 -->