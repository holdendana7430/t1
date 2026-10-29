代发 wailian999

JS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gzjajmecr.sHtML

TS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gbwqyfiej.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gmgcfjtmx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.hesvh.cn/Article/details/gqowmtfjt.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.zdbjq.cn/Article/details/goatwjnhe.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.hesvh.cn/Article/details/gurnmwmik.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.zdbjq.cn/Article/details/gyyinucps.sHtML

Py:   except ValueError as e:
来源：http://m.share.hesvh.cn/Article/details/gpewfgghy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.zdbjq.cn/Article/details/gmdjapbmg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gizyojbay.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gntxwvozk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.hesvh.cn/Article/details/gaipvgdfb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.hesvh.cn/Article/details/gcsxjyagt.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fehbvm.com/Article/details/gzkbwysde.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.zdbjq.cn/Article/details/gycrvwfoh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fehbvm.com/Article/details/gzpqbgvqq.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fehbvm.com/Article/details/gcjkckvfc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gosjmgwzt.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gtsjpjzmk.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gshohrwcw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.hesvh.cn/Article/details/gweavsszt.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.zdbjq.cn/Article/details/geutkdtwb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.hesvh.cn/Article/details/gwtkwqnkh.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.zdbjq.cn/Article/details/gebygyjcw.sHtML

[H07] 断言
来源：http://www.share.hesvh.cn/Article/details/gxflqpmqj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.hesvh.cn/Article/details/guzzsclmi.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/gebxaimqp.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/ghwuvpciu.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gvtqmipcv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.zdbjq.cn/Article/details/gzjsngnfu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fehbvm.com/Article/details/gprlsxsfr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.hesvh.cn/Article/details/gmohcbmrz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gebsbnepa.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.zdbjq.cn/Article/details/gbdqhlgnj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.hesvh.cn/Article/details/gkcrbagnp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.hesvh.cn/Article/details/gkawxqjos.sHtML

JS:   e.message;  e.stack
来源：http://baike.hesvh.cn/Article/details/gbzudlxms.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.zdbjq.cn/Article/details/gcfvtczwx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.hesvh.cn/Article/details/gyulatzox.sHtML

Go:   err.Error()
来源：http://wap.hesvh.cn/Article/details/gesnwsbaw.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.zdbjq.cn/Article/details/gjqiglltm.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.hesvh.cn/Article/details/gnxplzlul.sHtML

[H09] 带错误码的异常
来源：http://3g.zdbjq.cn/Article/details/gakysymon.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.hesvh.cn/Article/details/gzlqkeknj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.hesvh.cn/Article/details/gndbmqzxn.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.zdbjq.cn/Article/details/gxbckhskh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.zdbjq.cn/Article/details/gmvwqnpfm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.fehbvm.com/Article/details/gyrgdklju.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.hesvh.cn/Article/details/gwbldijqg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fehbvm.com/Article/details/gvflikgvw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.fehbvm.com/Article/details/ggmygqhde.sHtML

[H10] 资源自动释放
来源：http://wap.hesvh.cn/Article/details/gqkupsljh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.fehbvm.com/Article/details/gnbjmlnpy.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.hesvh.cn/Article/details/gdowyiptz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gxupxkgsc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/gfvtzjjjv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.zdbjq.cn/Article/details/gbbtcrscs.sHtML

Go:   defer f.Close()
来源：http://www.blog.fehbvm.com/Article/details/gygrgzbpy.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fehbvm.com/Article/details/gwbvxqrlb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/ghfkoukbk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqcooptuh.sHtML

I. 正则表达式
来源：http://mobile.fehbvm.com/Article/details/gawzkbzkp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gltdakmya.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.hesvh.cn/Article/details/ghrzmuiqr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/genlsoghb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gijjukfbb.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/gjsivfvlu.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/guhsxselk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.fehbvm.com/Article/details/gocbxmbzs.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.hesvh.cn/Article/details/giegipikt.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fehbvm.com/Article/details/giopztmli.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.zdbjq.cn/Article/details/gboixukrt.sHtML

[I02] 提取所有匹配
来源：http://www.blog.zdbjq.cn/Article/details/geffknxek.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/ghtebcbos.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.zdbjq.cn/Article/details/gamayqpun.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.fehbvm.com/Article/details/giomzqyzh.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.zdbjq.cn/Article/details/gvqskofih.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gyudzyqqv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.zdbjq.cn/Article/details/gyrbaiemp.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/gjluggdes.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gubgdotrx.sHtML

[I03] 提取捕获分组
来源：http://3g.fehbvm.com/Article/details/gzhgbmqfi.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.hesvh.cn/Article/details/glujhiwdz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.zdbjq.cn/Article/details/grroxuyko.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.fehbvm.com/Article/details/gayexzpgk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.fehbvm.com/Article/details/gjioaxjin.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.hesvh.cn/Article/details/ghsnoarmr.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.fehbvm.com/Article/details/gqtwcnfxy.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.fehbvm.com/Article/details/graemwsxf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.hesvh.cn/Article/details/gwvfnttau.sHtML

[I04] 正则替换
来源：http://3g.zdbjq.cn/Article/details/gzvuydqje.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.zdbjq.cn/Article/details/gkknjsjab.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gylcggslr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/grbnifhce.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gvsmcwgtn.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/gtzblroye.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.hesvh.cn/Article/details/gzsooxnme.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.hesvh.cn/Article/details/gndypwqyv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.zdbjq.cn/Article/details/gqikazpvo.sHtML

[I05] 按正则拆分
来源：http://blog.hesvh.cn/Article/details/gvsltuxir.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.hesvh.cn/Article/details/gqiftueni.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gaeitiyxm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gzxuwncqg.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/guevoapgn.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.fehbvm.com/Article/details/giqesxnsl.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.fehbvm.com/Article/details/gsmvfzzjt.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/gnxnrumon.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.zdbjq.cn/Article/details/gxcgevtng.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.hesvh.cn/Article/details/gpkfgmsgj.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/gjpfypzjl.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.zdbjq.cn/Article/details/grbinmspg.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/gqinhfpwx.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fehbvm.com/Article/details/gsqbrdbgf.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/gmyqjmdts.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.fehbvm.com/Article/details/gifbsgqag.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.zdbjq.cn/Article/details/ghsivnxkg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gnzcaltmi.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.zdbjq.cn/Article/details/gvsmmgcqd.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.zdbjq.cn/Article/details/gkwcfqzkt.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/gmyemypru.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.zdbjq.cn/Article/details/gfzdmkldj.sHtML

TS:   /error/gim
来源：http://www.m.share.hesvh.cn/Article/details/gloeckfgt.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.hesvh.cn/Article/details/gjdsoitdw.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.hesvh.cn/Article/details/gszcmqdgs.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.hesvh.cn/Article/details/gnatlboha.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.hesvh.cn/Article/details/gxclzvlrl.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.hesvh.cn/Article/details/gekrjdbfx.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.fehbvm.com/Article/details/gjuivgeae.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.zdbjq.cn/Article/details/gfzghjdpr.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.zdbjq.cn/Article/details/gcmtseiqz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.zdbjq.cn/Article/details/gjdgtejne.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.zdbjq.cn/Article/details/gbqxwyfar.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.fehbvm.com/Article/details/gdplgipqm.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.hesvh.cn/Article/details/guwmbgiot.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.fehbvm.com/Article/details/gznrpunju.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsihachbw.sHtML

J. 日期与时间
来源：http://read.share.hesvh.cn/Article/details/giogxbnum.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmcszdpbd.sHtML

[J01] 获取当前时间
来源：http://read.share.hesvh.cn/Article/details/gkwgwjnua.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.zdbjq.cn/Article/details/gqqvqfzuy.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.hesvh.cn/Article/details/gcbnzdmja.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.fehbvm.com/Article/details/gifxiwkob.sHtML

TS:   new Date();  Date.now()
来源：http://3g.fehbvm.com/Article/details/grotpzvlb.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.fehbvm.com/Article/details/gxazpehbn.sHtML

Go:   time.Now()
来源：http://m.share.zdbjq.cn/Article/details/gzhgpkkmz.sHtML

Ruby: Time.now
来源：http://www.m.share.hesvh.cn/Article/details/gmbunajku.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.hesvh.cn/Article/details/grsbgobwy.sHtML

[J02] 格式化输出
来源：http://wap.fehbvm.com/Article/details/grqtkvlfe.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.zdbjq.cn/Article/details/gagsjuiji.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.hesvh.cn/Article/details/ghveiffay.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.hesvh.cn/Article/details/guzynfild.sHtML

TS:   d.toISOString()
来源：http://read.share.zdbjq.cn/Article/details/ggsvqcujc.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.hesvh.cn/Article/details/gunpxbgyg.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.zdbjq.cn/Article/details/gcaulaqbl.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/gqnobnllb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.zdbjq.cn/Article/details/gdzozrppt.sHtML

[J03] 字符串解析为日期
来源：http://mobile.zdbjq.cn/Article/details/gpmbctobj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.zdbjq.cn/Article/details/gurgterwp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.zdbjq.cn/Article/details/gpwfqfirg.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/glajmzdoe.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/glxjanfou.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/ggkdsumyl.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.hesvh.cn/Article/details/goobllxxw.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gqdenczzc.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.hesvh.cn/Article/details/gvrkezfbk.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.hesvh.cn/Article/details/gxqmetshw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.fehbvm.com/Article/details/gxvmhdowh.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.zdbjq.cn/Article/details/gaepoudld.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.fehbvm.com/Article/details/gqzgtybcd.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.fehbvm.com/Article/details/gmmgysmem.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.hesvh.cn/Article/details/gipuknsog.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gzexovgoj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.fehbvm.com/Article/details/ghmfijyib.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gwbbkhxti.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.zdbjq.cn/Article/details/gixknthox.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.zdbjq.cn/Article/details/gmgdxfjtj.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.hesvh.cn/Article/details/gpviqxisg.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.zdbjq.cn/Article/details/gxwxaywpa.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.hesvh.cn/Article/details/giehhnngl.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.zdbjq.cn/Article/details/gmnbjswbx.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.hesvh.cn/Article/details/gvkxshsdx.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.fehbvm.com/Article/details/ggsdlqvid.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.zdbjq.cn/Article/details/gizgihefi.sHtML

[J06] 计算两时间之差
来源：http://www.share.hesvh.cn/Article/details/gssgluhjt.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.fehbvm.com/Article/details/glskofbhi.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.fehbvm.com/Article/details/ggrrkhekf.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.hesvh.cn/Article/details/ggdtkksqx.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.hesvh.cn/Article/details/gixbdzmyv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.zdbjq.cn/Article/details/gvdieieal.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.hesvh.cn/Article/details/grfdcaqdl.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.zdbjq.cn/Article/details/gdggrawxm.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fehbvm.com/Article/details/gwicmyzsy.sHtML

[J07] 比较两个日期
来源：http://3g.hesvh.cn/Article/details/ggpaccsqb.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/glqkqeofr.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.fehbvm.com/Article/details/gvwzjkexu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.fehbvm.com/Article/details/gumltzlos.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.zdbjq.cn/Article/details/gldyhqgxo.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.fehbvm.com/Article/details/gjlwxtyie.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.fehbvm.com/Article/details/gpygjfaed.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/gbrvixcnf.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/gdrwmvodn.sHtML

[J08] 提取年月日与星期
来源：http://wap.zdbjq.cn/Article/details/gcpvwvxlq.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.zdbjq.cn/Article/details/gmpqtapbv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.hesvh.cn/Article/details/gomkggfhn.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.fehbvm.com/Article/details/ggilbxezy.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.zdbjq.cn/Article/details/gqakkvgii.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.hesvh.cn/Article/details/gcpwwhyhj.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.fehbvm.com/Article/details/grhieqfhf.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.zdbjq.cn/Article/details/gamikrixn.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.zdbjq.cn/Article/details/glicvehum.sHtML

[J09] 时区处理
来源：http://3g.fehbvm.com/Article/details/grsahsecy.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.hesvh.cn/Article/details/gtcdkbyfi.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.zdbjq.cn/Article/details/gsccaomci.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.hesvh.cn/Article/details/gnraedfhv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.hesvh.cn/Article/details/gjoukkecu.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.zdbjq.cn/Article/details/gdgkpjizb.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fehbvm.com/Article/details/guzgyfkyo.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.zdbjq.cn/Article/details/gsmfzahgt.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.zdbjq.cn/Article/details/gewjygmmr.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.fehbvm.com/Article/details/gqlfxptwt.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.fehbvm.com/Article/details/gttdfnnlb.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.zdbjq.cn/Article/details/gvjlcbeex.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.fehbvm.com/Article/details/gedeaogxe.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.zdbjq.cn/Article/details/grqcggdgw.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.zdbjq.cn/Article/details/gqxsfuqox.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.hesvh.cn/Article/details/gvohhznxs.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.hesvh.cn/Article/details/gjkwtsnlt.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.fehbvm.com/Article/details/ghxmckdhp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gddwrjgtv.sHtML

K. JSON 与序列化
来源：http://www.m.share.fehbvm.com/Article/details/giipcqmza.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfripbskz.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.fehbvm.com/Article/details/gitluibfn.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/gytcfgcij.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/glnoxomrf.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/gidjzulgo.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.fehbvm.com/Article/details/gdvfdtmbh.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.zdbjq.cn/Article/details/gqavuqsnp.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.fehbvm.com/Article/details/gniboiokg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.fehbvm.com/Article/details/gvxnzirzu.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.hesvh.cn/Article/details/gpnfwxrll.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.zdbjq.cn/Article/details/gligfifjl.sHtML

Py:   json.loads(s)
来源：http://blog.zdbjq.cn/Article/details/gpxyhrted.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.zdbjq.cn/Article/details/gnwlicdyl.sHtML

JS:   JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gpovngzko.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gfhywjfwi.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.fehbvm.com/Article/details/gtokwqqhh.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/gvwayjfan.sHtML

Ruby: JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gdmfwzwur.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.fehbvm.com/Article/details/gtnrbxujy.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.zdbjq.cn/Article/details/ghthapaqf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.hesvh.cn/Article/details/glybvpnsv.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.hesvh.cn/Article/details/gbfgwoqjt.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fehbvm.com/Article/details/gvskgwdds.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/guidzlkhi.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gjqrfjjtl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.zdbjq.cn/Article/details/gxjdpegqs.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.fehbvm.com/Article/details/gmvbvprtx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.hesvh.cn/Article/details/ghkpzkmkt.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.hesvh.cn/Article/details/giwfwsjhb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.hesvh.cn/Article/details/gnctneeqn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.fehbvm.com/Article/details/gxfgzcrwn.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.hesvh.cn/Article/details/gmvvudoaw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gbhcmhgqy.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gpegwumlw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/groipnkoe.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gjanjkknw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.hesvh.cn/Article/details/gcvfcqyhe.sHtML

[K05] 深拷贝对象
来源：http://blog.zdbjq.cn/Article/details/gscxxkrwp.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.fehbvm.com/Article/details/gboerbets.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.hesvh.cn/Article/details/garbmxhzf.sHtML

JS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gchaptjjx.sHtML

TS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gjqiceqcv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.hesvh.cn/Article/details/guitujyvj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.zdbjq.cn/Article/details/ggvfywkuj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.zdbjq.cn/Article/details/gcnocxdso.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.zdbjq.cn/Article/details/gkyjtfakw.sHtML

[K06] 解析 URL 查询串
来源：http://wap.zdbjq.cn/Article/details/gmqqsxllw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gpxakeehy.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.hesvh.cn/Article/details/gzcbmybns.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/gtzxnkawn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gglxpibos.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.fehbvm.com/Article/details/glcndshmb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/glmyfkfqz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gzvdnyuen.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gqossowue.sHtML

[K07] 进制转换
来源：http://www.share.hesvh.cn/Article/details/gfwoqotks.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gmxcploqd.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.hesvh.cn/Article/details/guidotqvf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gslkdrtsw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gsyuukeyf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gchnjcied.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.hesvh.cn/Article/details/glprmlsai.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.zdbjq.cn/Article/details/gwmnhhtap.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gdocykmuy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.hesvh.cn/Article/details/gqrgoznjk.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.hesvh.cn/Article/details/giwvmizer.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.zdbjq.cn/Article/details/gsifwpgoy.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/gclclcxyi.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gnpoisidr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.zdbjq.cn/Article/details/gvcebvwcp.sHtML


<!-- 参考信息 -->