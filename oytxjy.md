代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jrtpdurx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2wonjjtlc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ngsombsd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2qqkzceun.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2vhejqcfw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2zeugswkr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2eeudvsgm.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2lhfznfss.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2aylwxlft.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2oxabatlx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2leiiqile.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cypefibj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ztixftmj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2sdjlgfva.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2ehqplnyq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kjsgjpis.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2xtmogvvu.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2qypctkci.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nflcemnl.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bknsdphj.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2svjyeljg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fibxduki.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2uxrgvdbh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2lzcqmagh.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ffymwomb.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2cfzlifob.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2aczbtepo.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2unjfxggj.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2cszpihkp.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2fuwhplkv.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2qmgbsigq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2fvjfvoii.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2gbvzshxd.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2bshcxghc.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2fprubaij.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2hifydeyj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2spmcciat.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cbspkuis.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2hscfxosa.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2bfehobmi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2lypznomn.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2obzfczhg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2ujlmogkv.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2renkejbo.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2usjwxkxi.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2clwhwclx.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2zpqhvqux.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2wtbjkskf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2mrpambos.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2oguzghzj.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2aykiilcu.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2zzbjhnbw.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2tigqdswn.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2ddkwuzmb.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qiqzxjsd.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vlktcril.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2yzpzdgdu.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2vqkvdcgz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2kbwsbgoj.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2ypmmkkbm.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xyrtjseg.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2bxkaksby.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2usrjewzm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2llosinxn.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2itzrppsj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2guhiqrsm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2zmyvquab.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2elgwaivy.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2asttfpdx.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2qymhqxco.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2hvsancat.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2byukkseh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2zpykscse.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2mshiljgu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2lqadijft.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2hozvfzlw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2efnoqnhr.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2ekclnynn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2qqsrwzkm.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2zmftiagm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2lhfednje.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2bvzeerzf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2yseehodi.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2lanryvci.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2aowbwdcq.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2lxxpqaix.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2wmdbbmza.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yjvuooyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2obxsjkmo.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2testvyes.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zmnbffzz.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2dpaeukcm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2bwrzkcne.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2naohgvje.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2bboxdjue.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wqvxkwvn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2vwbllkmp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2bctjliev.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ztbpnozc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2isiehtlo.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gtxeywaq.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2vwtbqnbe.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2jjbnrwov.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2kalgbyai.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2jtptpkcw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2upzfzrsj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2htknxjfc.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2fcjdbieh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wythbzjq.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2otacbubc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2hvwekdvj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2jjdxdzjl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2qymbmcfx.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2fuvrktmk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2qtbrukqe.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2goqsyxsk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2sqiufymb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2yrvtbhoo.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2bgvdkduf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2iuqyptxx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2jixaopxm.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2avmdfcta.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2dgirmpaz.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2yhtnbepk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2ylbowfht.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2uqfyzjcq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2bygicqvv.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2atagmbwo.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2lrfnnlwp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2oliwezvf.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2mlvjszwk.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2aofneyxc.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2fsoeffyu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2bhudxuww.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2eqoiwxyw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2waetnslr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2zilgqbfa.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2rukofrno.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2cqvzplzx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2aisxxzes.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2twqjqurt.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2xfutwgak.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2ibrazajo.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2dlqidgte.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ihublfjp.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2eqlctdpb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2joaewgqy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2mtozruhk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2owwqwgcl.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2czrlfoor.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2iaujobxc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2cexfrkjv.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2sviccyfm.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2pmjgjywh.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2gigrghrs.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2fdgfwepz.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2qcxnfscx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2pexstogu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2pahilqzg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2uqyuwvlo.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2ibjtqtac.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2mlbzcnjl.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2xifalyxi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lwhiegmi.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2panyvwua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jxrlqtdv.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2cruvfipb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2wwdbbjlh.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2btjfbhoa.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2ldtqwpot.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2fcgrkfzl.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2gtbruhup.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2xytnwvzh.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2dzvbywjt.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2czvqlfnv.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2tnfjovdt.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2lfxznmwd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2jbxzgnun.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2wqybjupq.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2chasdvvr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2udyeauoo.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2biesyopb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2qfllfugw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2spykhdiz.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2mazwwids.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2iiybljrc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2qzqgahsm.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2imdwgrlr.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2quxwdbqu.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2iajavhmo.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2xlobpzng.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2oalbupmr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2bpuxqqwt.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2tcmjeqdx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2bggyxxdm.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2caohdxqs.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2eonizirk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2blhlxocq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2pwbfwhmo.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2vimmxznp.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2uomvpyrw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2nwstldtu.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2bowfxrio.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2yailacue.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2idbiwyha.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2ikhsccbj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2vjmkftmy.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2yatnmnnt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2sfubvjqy.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2kggyctsg.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2oxsxtlsq.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2byfksbtm.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2cvtpkljl.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2dlnauhpf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2lcjnvppk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2urcayxry.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2xofsfxml.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2dgvzhabh.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2uzlbnjea.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2ztqrwjrs.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2omagpovk.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2twuwfcbw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2gmxcmtvv.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2chgknsor.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2ahxiqwvi.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2glqodsqk.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2fjolnmvh.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2nkcfwhwg.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2fxvteugk.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2hduyqbww.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2thkvdzvf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2jxvwjokh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2pnvzlbux.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2ttllstql.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2eiyolzth.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2tiuomxhs.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2ytvvohbg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2gujkbsrd.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2togzvfeg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2zsozwkqk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2tpjjoqvc.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2wwgwhure.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2nurawjjg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2jcijpgad.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2rgttoiry.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2clkmppfj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2eiunrzjc.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2iwcyncdh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2cwkzlelr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2dszmwvnm.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wgcwgvvd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2nshlecap.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2znievlkc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2wouabhds.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2zuyohihp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2lqmlbjpa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yscwyvix.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2jxxwwkgl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vmpnfplb.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2ktdbhgaq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2elyotdav.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2nfuzplza.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2jneulyll.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rlshagnm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2voyhwdlh.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ywijdiie.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2uyuyehfq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hhdjktsl.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2lcwqdyvx.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bjpuricg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2tosnelsv.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2eeazlawe.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2okgaldye.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2yjwyuwae.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2cqpepwpq.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2blikrokx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2iindjmhc.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2nyqktkwh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2vftjblzd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2cmbbpqtv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cdrdjsud.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2kvlpznnd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dmvoefvq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2kdtwokse.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2xgxxthzr.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2sxwyftnq.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2fglqelro.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2jvmtrulu.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2frolsciq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2loabctzs.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2dopamjjh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2tbexekgc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2gxrpbfnj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2mtalxaau.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2wyctblss.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2vnvsdwvu.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2ccjcelgr.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2ghnrkawf.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2hslvqxzc.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2nrvirdpo.html


<!-- 参考信息 -->