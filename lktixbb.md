代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fanxiaobao.xyz/Article/details/gmkddlpfy.sHtML

[H04] 自定义异常类型
来源：http://www.share.fanxiaobao.xyz/Article/details/grxspiqtj.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghahlokgq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyjseatw.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gedycrllv.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gwookctwt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gzewgqeac.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fanxiaobao.xyz/Article/details/gtzwnmpax.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gikcntxfh.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fanxiaobao.xyz/Article/details/gtmnzmzsi.sHtML

[H05] 捕获特定类型
来源：http://blog.fanxiaobao.xyz/Article/details/ghguhprob.sHtML

Py:   except ValueError as e:
来源：http://read.share.fanxiaobao.xyz/Article/details/gibeagehv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.fanxiaobao.xyz/Article/details/gonsohuex.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplckmzli.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gomzkzple.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gholmzzhv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.fanxiaobao.xyz/Article/details/gjltqhujp.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fanxiaobao.xyz/Article/details/gccvfwmvj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzifgkes.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpkhozli.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fanxiaobao.xyz/Article/details/gjmrxtwwx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fanxiaobao.xyz/Article/details/giahviojb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fanxiaobao.xyz/Article/details/glljyykqa.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwqzyqbw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmygeqky.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbkkbayr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.fanxiaobao.xyz/Article/details/gelynyhsd.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givpsajwo.sHtML

[H07] 断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gztdguriw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fanxiaobao.xyz/Article/details/guknqgata.sHtML

PHP:  assert($x > 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuilozsm.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gopegxayk.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/glvbmokah.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.fanxiaobao.xyz/Article/details/gtlqfdcnq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaincojwt.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmweeefks.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gycrhqave.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddrovuiu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fanxiaobao.xyz/Article/details/grdjboxak.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.fanxiaobao.xyz/Article/details/gvwiyioxy.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhntowof.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsuwaczc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fanxiaobao.xyz/Article/details/gpitkbexv.sHtML

Go:   err.Error()
来源：http://www.share.fanxiaobao.xyz/Article/details/gagcuxggt.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fanxiaobao.xyz/Article/details/gmbcaqfof.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.fanxiaobao.xyz/Article/details/gewqpkesh.sHtML

[H09] 带错误码的异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gkuoahdly.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fanxiaobao.xyz/Article/details/gtxrrdaky.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.fanxiaobao.xyz/Article/details/gcosgrxic.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzibtlrqf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.fanxiaobao.xyz/Article/details/grztaudkm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcktbvayx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fanxiaobao.xyz/Article/details/gtdzzawcl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fanxiaobao.xyz/Article/details/gqpibipxn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsaywcqxk.sHtML

[H10] 资源自动释放
来源：http://wap.fanxiaobao.xyz/Article/details/gakykxvtw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fanxiaobao.xyz/Article/details/ghelgclbj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fanxiaobao.xyz/Article/details/gjixecmsm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfgmsjmd.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdlcbdka.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfzpwetg.sHtML

Go:   defer f.Close()
来源：http://blog.fanxiaobao.xyz/Article/details/groqhlaia.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.fanxiaobao.xyz/Article/details/gnnjjofyi.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcohrzcs.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfzggaiu.sHtML

I. 正则表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwncnxky.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlaqxxck.sHtML

[I01] 判断是否匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gfuwxwdep.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.fanxiaobao.xyz/Article/details/gscldfrea.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkqxqbkl.sHtML

JS:   /\d+/.test(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gdsutotyu.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcytokslw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.fanxiaobao.xyz/Article/details/gssxkdwrz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gkclqjqpf.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fanxiaobao.xyz/Article/details/gheibhvzv.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gdofnewej.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunipuhtx.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvyxjgab.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fanxiaobao.xyz/Article/details/gmefncums.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fanxiaobao.xyz/Article/details/gouykodbn.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhqjmymx.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gtlsfhutv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmyikibc.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzqqocet.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/ghvbktadp.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsqlqcbm.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gchqxdvdm.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.fanxiaobao.xyz/Article/details/gogzdwfsp.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.fanxiaobao.xyz/Article/details/ghiitjykb.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fanxiaobao.xyz/Article/details/glukrqrxa.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqgjhaxo.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxbialgb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrcbaaqe.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.fanxiaobao.xyz/Article/details/gzxpvzgfy.sHtML

[I04] 正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gjghgbntn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnuhelhi.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gajnwxitr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.fanxiaobao.xyz/Article/details/gyoxdxjpg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fanxiaobao.xyz/Article/details/gprdcqnar.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlpqhvjr.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggifzjchh.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/gsacrgovi.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/gygatjcqn.sHtML

[I05] 按正则拆分
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfcgfwzr.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjnotijt.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/goeanywyf.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.fanxiaobao.xyz/Article/details/glpzxnvee.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.fanxiaobao.xyz/Article/details/gzimuyeqj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.fanxiaobao.xyz/Article/details/grttnfpwh.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmjozlwf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.fanxiaobao.xyz/Article/details/gzsdnwkbb.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.fanxiaobao.xyz/Article/details/glpzzqggl.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.fanxiaobao.xyz/Article/details/gyixiwtkz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.fanxiaobao.xyz/Article/details/gimnswmyq.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncdnvrlk.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqokcjcv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fanxiaobao.xyz/Article/details/gehrcjmom.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxlecrfh.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.fanxiaobao.xyz/Article/details/gvggibxil.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.fanxiaobao.xyz/Article/details/gushpamyi.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghafirmip.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerhdvvdz.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.fanxiaobao.xyz/Article/details/grovmtxji.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnpopswt.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.fanxiaobao.xyz/Article/details/gduuovoza.sHtML

TS:   /error/gim
来源：http://baike.fanxiaobao.xyz/Article/details/gytnoreww.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.fanxiaobao.xyz/Article/details/gckanjise.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsixmqrbi.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.fanxiaobao.xyz/Article/details/gqplnputf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlklodtn.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkxaxdom.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.fanxiaobao.xyz/Article/details/giahzjkty.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.fanxiaobao.xyz/Article/details/gkqepjknq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garfpcdms.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqszhfyzt.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwstrrrja.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrnodouu.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmudgfncu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.fanxiaobao.xyz/Article/details/gdczkqfyn.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlyryeub.sHtML

J. 日期与时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvpleqkb.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gzkawceiu.sHtML

[J01] 获取当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gkokhucqw.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaasoipte.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.fanxiaobao.xyz/Article/details/gigfvxggu.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.fanxiaobao.xyz/Article/details/gyduzuqra.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.fanxiaobao.xyz/Article/details/grhdqsxoe.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmkuvloc.sHtML

Go:   time.Now()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdhmaisn.sHtML

Ruby: Time.now
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwbikthz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdjenzsm.sHtML

[J02] 格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmpipsou.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fanxiaobao.xyz/Article/details/gvcnqmtxo.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzklmejim.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxuhfygp.sHtML

TS:   d.toISOString()
来源：http://baike.fanxiaobao.xyz/Article/details/gisctkddg.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.fanxiaobao.xyz/Article/details/glgjrygbh.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.fanxiaobao.xyz/Article/details/gecpzrwap.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fanxiaobao.xyz/Article/details/ggkauhzda.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgwdkldc.sHtML

[J03] 字符串解析为日期
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmmvcten.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppdsibmq.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfgeaoma.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.fanxiaobao.xyz/Article/details/grvmbxkiz.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.fanxiaobao.xyz/Article/details/gyboywkin.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkqagxio.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjnqrxtx.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvsupohd.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevwrdifq.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gplvrtcok.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.fanxiaobao.xyz/Article/details/gudtvhweq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkytenrn.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtahxtae.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.fanxiaobao.xyz/Article/details/gtdlehcen.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.fanxiaobao.xyz/Article/details/gayhgsggg.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gyvjftylu.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbuhtfcx.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpcyoepi.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsciyqfgv.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpttoiek.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypogogtk.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fanxiaobao.xyz/Article/details/gmlxaxmsi.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkvxdetc.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.fanxiaobao.xyz/Article/details/greteehgv.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.fanxiaobao.xyz/Article/details/gbbntaiyi.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.fanxiaobao.xyz/Article/details/gufryeoxo.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhnwwwlh.sHtML

[J06] 计算两时间之差
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsizehyfg.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.fanxiaobao.xyz/Article/details/gnunqaupu.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqukzmleu.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.fanxiaobao.xyz/Article/details/gihfwcfzj.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.fanxiaobao.xyz/Article/details/glxbyxrgp.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.fanxiaobao.xyz/Article/details/grlypmvid.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.fanxiaobao.xyz/Article/details/goaqudbfq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.fanxiaobao.xyz/Article/details/gkgzwyqwl.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmooeqnsj.sHtML

[J07] 比较两个日期
来源：http://mobile.fanxiaobao.xyz/Article/details/gynowgzko.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.fanxiaobao.xyz/Article/details/gyuhpaywr.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjcxqzoz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkumpmnd.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.fanxiaobao.xyz/Article/details/gvdzzdzts.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlqfovdu.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gldlyhjtb.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.fanxiaobao.xyz/Article/details/gtaycnhzg.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggiccrnwb.sHtML

[J08] 提取年月日与星期
来源：http://3g.fanxiaobao.xyz/Article/details/gfjdfuuuv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.fanxiaobao.xyz/Article/details/gozxidcgt.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.fanxiaobao.xyz/Article/details/glfqxemqb.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.fanxiaobao.xyz/Article/details/ggsnkitlm.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.fanxiaobao.xyz/Article/details/gkwfqotit.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.fanxiaobao.xyz/Article/details/gwazckaeg.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.fanxiaobao.xyz/Article/details/ggfmfnngi.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjtrnboq.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.fanxiaobao.xyz/Article/details/gnryrkofu.sHtML

[J09] 时区处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydzudago.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfpumdje.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdflmhsb.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fanxiaobao.xyz/Article/details/gpwzmsiil.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggknuxpgw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.fanxiaobao.xyz/Article/details/gcaqbltrg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsogktdp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtiurbxpc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzcvkqkm.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.fanxiaobao.xyz/Article/details/gfezhfcns.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkecxhofl.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.fanxiaobao.xyz/Article/details/gnwsrsoym.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwrvrwhy.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggawxpgqv.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gztgueqip.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.fanxiaobao.xyz/Article/details/gndbiohqm.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyhfcbsa.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqacsdxc.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzlzyukl.sHtML

K. JSON 与序列化
来源：http://read.share.fanxiaobao.xyz/Article/details/glciquyqo.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxsssgtj.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqcuzpgn.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjcwfbgb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisftcekf.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyxdskcg.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxwhtfcs.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.fanxiaobao.xyz/Article/details/gkombeuqm.sHtML

Go:   json.Marshal(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gxevrjxdj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzzjjphw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gzwyjpvrm.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrmmhulj.sHtML

Py:   json.loads(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gqgkcjgpt.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.fanxiaobao.xyz/Article/details/giqiusaxq.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geedjnwrr.sHtML

TS:   JSON.parse(s)
来源：http://baike.fanxiaobao.xyz/Article/details/goywfesdk.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.fanxiaobao.xyz/Article/details/ghsowidis.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fanxiaobao.xyz/Article/details/gdnhbkzsx.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjwwauqw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtekrqhau.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.fanxiaobao.xyz/Article/details/gtubifppn.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxkwuhzu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.fanxiaobao.xyz/Article/details/gubngzslh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjzlrhoa.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/ghipdtrbv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gkmkyxoxn.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwspeupa.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/ghwzxhrif.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdcncbla.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.fanxiaobao.xyz/Article/details/guzcempib.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcewdfuw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.fanxiaobao.xyz/Article/details/gaiggrukb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqshxdawa.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fanxiaobao.xyz/Article/details/geezsanzd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsstlgoya.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbylxhcmp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gmghqmzzc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fanxiaobao.xyz/Article/details/govyfehoo.sHtML

[K05] 深拷贝对象
来源：http://blog.fanxiaobao.xyz/Article/details/gzynbcjiu.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gatsugnfl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fanxiaobao.xyz/Article/details/gljqxmrxm.sHtML

JS:   structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gohidfyqy.sHtML

TS:   structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbahrrav.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhnrlaej.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.fanxiaobao.xyz/Article/details/gwuvggwfa.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxwumwdc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasldwrij.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fanxiaobao.xyz/Article/details/gknfvhunl.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqielmcco.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtkebbuy.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcguywrg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fanxiaobao.xyz/Article/details/gibrkuauc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fanxiaobao.xyz/Article/details/gynpdvhcu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.fanxiaobao.xyz/Article/details/gmdpbnvkk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fanxiaobao.xyz/Article/details/gmcevtqxh.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fanxiaobao.xyz/Article/details/giwejjdnq.sHtML

[K07] 进制转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvomjrgc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gimcisvqq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fanxiaobao.xyz/Article/details/gwbaqvwsa.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghykbrxus.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxopqsobj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvhefwxf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqitdtpp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjrgsvjy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.fanxiaobao.xyz/Article/details/gpeadtxpv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhnzlhnl.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsyblyre.sHtML


<!-- 参考信息 -->