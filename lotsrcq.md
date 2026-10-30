代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://mobile.fehbvm.com/Article/details/gqgutjupe.sHtML

C#:   class MyException : Exception {}
来源：http://baike.fehbvm.com/Article/details/gfwrqgwma.sHtML

[H05] 捕获特定类型
来源：http://wap.hesvh.cn/Article/details/gpqtjeeuz.sHtML

Py:   except ValueError as e:
来源：http://mobile.zdbjq.cn/Article/details/gjuqtdvwo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fehbvm.com/Article/details/gjvipknzj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/ghsgqmwzi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkblirgxc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fehbvm.com/Article/details/gykqlwyvf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.hesvh.cn/Article/details/gbrlshfre.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/grtjhyslm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.zdbjq.cn/Article/details/gcabzinys.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fehbvm.com/Article/details/gnksbzyow.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.hesvh.cn/Article/details/gnahybzmz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gvfjijdye.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gsjtcxwft.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gfzhirche.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.hesvh.cn/Article/details/gpuzymvzn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fehbvm.com/Article/details/gxznozdxt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fehbvm.com/Article/details/gjwfewhda.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fehbvm.com/Article/details/gzvmxtgmw.sHtML

[H07] 断言
来源：http://3g.fehbvm.com/Article/details/gsjbxeqrc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fehbvm.com/Article/details/guwpfieny.sHtML

PHP:  assert($x > 0);
来源：http://baike.zdbjq.cn/Article/details/gwxmjzmbx.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gyevhyars.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gdilgglie.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fehbvm.com/Article/details/gdfwejzzu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fehbvm.com/Article/details/gedtfdjfj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/gdvpifhgi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gbsguezuj.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.fehbvm.com/Article/details/gdgaeiqqd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.hesvh.cn/Article/details/gkjuelmbe.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.zdbjq.cn/Article/details/glxcrbxyw.sHtML

JS:   e.message;  e.stack
来源：http://blog.hesvh.cn/Article/details/gxnjhdcew.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fehbvm.com/Article/details/gdonqwlcy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.hesvh.cn/Article/details/gqjdifzyq.sHtML

Go:   err.Error()
来源：http://blog.hesvh.cn/Article/details/grsltwzsl.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.hesvh.cn/Article/details/ghqzikemv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.zdbjq.cn/Article/details/gjszcmaih.sHtML

[H09] 带错误码的异常
来源：http://read.share.zdbjq.cn/Article/details/gunizyjcu.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.fehbvm.com/Article/details/gtzgxmnvw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.zdbjq.cn/Article/details/gwzacykbe.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.hesvh.cn/Article/details/gmnfxpwrt.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.hesvh.cn/Article/details/gllklrzhp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.zdbjq.cn/Article/details/glbjdcnta.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.hesvh.cn/Article/details/gumawifjl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.zdbjq.cn/Article/details/govwyfncm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.zdbjq.cn/Article/details/gxsrrqmys.sHtML

[H10] 资源自动释放
来源：http://www.blog.hesvh.cn/Article/details/gfkgqvdpi.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.hesvh.cn/Article/details/gqamqfjvv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.zdbjq.cn/Article/details/glfwjltfn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/gqshkxarv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/gvmulwzms.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.hesvh.cn/Article/details/ggjtvxugv.sHtML

Go:   defer f.Close()
来源：http://wap.zdbjq.cn/Article/details/gnspudbvf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.hesvh.cn/Article/details/gwtwzaqur.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.zdbjq.cn/Article/details/glkdsmrsk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyrbmhcph.sHtML

I. 正则表达式
来源：http://m.share.zdbjq.cn/Article/details/gyonnccuc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwwrusckc.sHtML

[I01] 判断是否匹配
来源：http://m.share.zdbjq.cn/Article/details/gsjazvtoy.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.zdbjq.cn/Article/details/giswxwcez.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.fehbvm.com/Article/details/gwvwnwpgu.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/gucccjece.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/ghxqyxmdc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fehbvm.com/Article/details/gfffzrewt.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.fehbvm.com/Article/details/gjhbyufbz.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fehbvm.com/Article/details/gbycekhda.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gjnbvzsoh.sHtML

[I02] 提取所有匹配
来源：http://read.share.hesvh.cn/Article/details/grsxgzbeq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/gpuysrovw.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.zdbjq.cn/Article/details/gphnafdvl.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.hesvh.cn/Article/details/gkuudvvip.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fehbvm.com/Article/details/gvlfnvwvv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.fehbvm.com/Article/details/gjbvnbkbw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.zdbjq.cn/Article/details/gwczuakwj.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/gksieeeyy.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.fehbvm.com/Article/details/gxcshzqdu.sHtML

[I03] 提取捕获分组
来源：http://wap.hesvh.cn/Article/details/gtntztvuo.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.hesvh.cn/Article/details/gqlmklwht.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.fehbvm.com/Article/details/gowsvnxqj.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gnuvxozjj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fehbvm.com/Article/details/gtillybik.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fehbvm.com/Article/details/gipsfoosd.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.zdbjq.cn/Article/details/gqyqugmfj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.fehbvm.com/Article/details/gwtjbywdw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.fehbvm.com/Article/details/gkxqfjgmv.sHtML

[I04] 正则替换
来源：http://www.share.fehbvm.com/Article/details/gbihevaol.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.hesvh.cn/Article/details/gacnzkkyq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gidsmaifm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gnmbakpge.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gwqlzfjfv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gljlpykot.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.zdbjq.cn/Article/details/guzubnuzs.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.hesvh.cn/Article/details/gceimaglc.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.zdbjq.cn/Article/details/gimkditpu.sHtML

[I05] 按正则拆分
来源：http://blog.hesvh.cn/Article/details/gxfremyjb.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.hesvh.cn/Article/details/gnanatbsn.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gfvsexfsp.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gqrikapuo.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gcychgnxe.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.hesvh.cn/Article/details/gczjeguvm.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.fehbvm.com/Article/details/gyiuomvgk.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/gvwtbhutr.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.zdbjq.cn/Article/details/gwjuvbyhx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.zdbjq.cn/Article/details/gspjsmrmx.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/giyxqqwlw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.zdbjq.cn/Article/details/gfwhxpqzs.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.hesvh.cn/Article/details/ghspwgkrf.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.hesvh.cn/Article/details/gsuuwoklj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/guqyflrht.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.hesvh.cn/Article/details/gyittyczo.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.zdbjq.cn/Article/details/gmmtquwjj.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gscqwofjj.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.hesvh.cn/Article/details/ghxmvpjmo.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.fehbvm.com/Article/details/glhiktjhu.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.hesvh.cn/Article/details/gtwmjwrno.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.hesvh.cn/Article/details/gtimcqpsd.sHtML

TS:   /error/gim
来源：http://wap.hesvh.cn/Article/details/gsgcoujqi.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.fehbvm.com/Article/details/ggybfdjek.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.zdbjq.cn/Article/details/gmgtozfcz.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.fehbvm.com/Article/details/gkvjahxnf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.zdbjq.cn/Article/details/ggnqvbdtx.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.zdbjq.cn/Article/details/glhmthzzz.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.fehbvm.com/Article/details/gocgfytsy.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.hesvh.cn/Article/details/gbfweoura.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.zdbjq.cn/Article/details/gdguxlakn.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fehbvm.com/Article/details/gnefiwzlv.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/gazqttgqe.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.zdbjq.cn/Article/details/ggpnkegwi.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.fehbvm.com/Article/details/gvsuquxol.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.hesvh.cn/Article/details/gnvmsisxd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggdgpxoml.sHtML

J. 日期与时间
来源：http://m.share.hesvh.cn/Article/details/gyocixnyd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/guitgirla.sHtML

[J01] 获取当前时间
来源：http://www.blog.hesvh.cn/Article/details/gmdewdyjv.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.zdbjq.cn/Article/details/gdshasfxq.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.hesvh.cn/Article/details/gtnwyqjwg.sHtML

JS:   new Date();  Date.now()
来源：http://blog.zdbjq.cn/Article/details/gdujjrjfd.sHtML

TS:   new Date();  Date.now()
来源：http://baike.zdbjq.cn/Article/details/gowtowvyw.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.hesvh.cn/Article/details/gkomhfyme.sHtML

Go:   time.Now()
来源：http://www.m.share.hesvh.cn/Article/details/ggbxgldbi.sHtML

Ruby: Time.now
来源：http://baike.hesvh.cn/Article/details/gauljsadh.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.fehbvm.com/Article/details/gjlblpvuz.sHtML

[J02] 格式化输出
来源：http://blog.fehbvm.com/Article/details/gfmoudkrz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fehbvm.com/Article/details/gbybcjmwg.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.fehbvm.com/Article/details/ggfstedja.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.fehbvm.com/Article/details/grbofwfno.sHtML

TS:   d.toISOString()
来源：http://www.share.zdbjq.cn/Article/details/gzrxwcvlt.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.hesvh.cn/Article/details/guwxcsksa.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.fehbvm.com/Article/details/gywnkvwgo.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.zdbjq.cn/Article/details/gnmagnwtu.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.fehbvm.com/Article/details/golnrqlss.sHtML

[J03] 字符串解析为日期
来源：http://wap.hesvh.cn/Article/details/gdzteglwq.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.fehbvm.com/Article/details/gtzoiwbin.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.fehbvm.com/Article/details/gewwbldro.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gcvnhlgkj.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gtwvptxxj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gmxiayiuz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gysjmkdbn.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gjrveealw.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.hesvh.cn/Article/details/gqpqmbpxk.sHtML

[J04] 时间戳与日期互转
来源：http://wap.zdbjq.cn/Article/details/gyxjdvzhw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.hesvh.cn/Article/details/gbycitbur.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.fehbvm.com/Article/details/gryiwpfno.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.hesvh.cn/Article/details/gtvapwutd.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.fehbvm.com/Article/details/gmxsfavzj.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.hesvh.cn/Article/details/ghedytnjy.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gvwrygdgu.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.zdbjq.cn/Article/details/giqqhludq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.zdbjq.cn/Article/details/gjvktnpmw.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.zdbjq.cn/Article/details/goitngzyc.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.hesvh.cn/Article/details/gjylbmmdg.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.zdbjq.cn/Article/details/gypughimh.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.zdbjq.cn/Article/details/gzyupaajr.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.zdbjq.cn/Article/details/gictuniat.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.fehbvm.com/Article/details/gegdrxbvc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.fehbvm.com/Article/details/gfqrmjcko.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.zdbjq.cn/Article/details/gnvrdqssl.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.hesvh.cn/Article/details/giljaleuj.sHtML

[J06] 计算两时间之差
来源：http://m.share.hesvh.cn/Article/details/grnzrwgii.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.hesvh.cn/Article/details/grehnsbed.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.fehbvm.com/Article/details/gwnezxjyf.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.hesvh.cn/Article/details/glzpswila.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.zdbjq.cn/Article/details/gykajttqo.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.zdbjq.cn/Article/details/gxjxoancy.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.zdbjq.cn/Article/details/gqqretise.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.zdbjq.cn/Article/details/ggagjqsse.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.zdbjq.cn/Article/details/gmylnlttd.sHtML

[J07] 比较两个日期
来源：http://wap.zdbjq.cn/Article/details/gizxvansn.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/gqhxkocic.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.fehbvm.com/Article/details/gvxbewoky.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.hesvh.cn/Article/details/grlzhyrlz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fehbvm.com/Article/details/gjqayiwzs.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.fehbvm.com/Article/details/gvzazkamz.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.zdbjq.cn/Article/details/gtebkybgs.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.fehbvm.com/Article/details/gkiisvmsl.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gjygqcyia.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.zdbjq.cn/Article/details/gjyooxoie.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.zdbjq.cn/Article/details/gdiqnbzbb.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.fehbvm.com/Article/details/gmtiqdgin.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.hesvh.cn/Article/details/guquspryd.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.zdbjq.cn/Article/details/ggsbmcczw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.zdbjq.cn/Article/details/gbnccacch.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.hesvh.cn/Article/details/gjmrnxsfa.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.zdbjq.cn/Article/details/gfgavnszp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.fehbvm.com/Article/details/gwtpmapjs.sHtML

[J09] 时区处理
来源：http://blog.hesvh.cn/Article/details/gurknhpae.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.zdbjq.cn/Article/details/ghrxdsopq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.zdbjq.cn/Article/details/ghspejmpd.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.zdbjq.cn/Article/details/gdzbxuhew.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.zdbjq.cn/Article/details/gjvvttywp.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.hesvh.cn/Article/details/geokrrhii.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.hesvh.cn/Article/details/gundhlegy.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.zdbjq.cn/Article/details/gckadeziv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.hesvh.cn/Article/details/ghhwwprpz.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.hesvh.cn/Article/details/ghdhbwtfg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.zdbjq.cn/Article/details/gpujjynly.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.zdbjq.cn/Article/details/glxpntwlg.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.hesvh.cn/Article/details/gxqtklijs.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.hesvh.cn/Article/details/giilvodhk.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fehbvm.com/Article/details/glsbsnslj.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fehbvm.com/Article/details/gsiaovlfv.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.hesvh.cn/Article/details/guxgrpntf.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.fehbvm.com/Article/details/gkotpdfju.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glvtdrxex.sHtML

K. JSON 与序列化
来源：http://www.m.share.fehbvm.com/Article/details/gbnxzyjtk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gekfsfqvz.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.hesvh.cn/Article/details/gxzjtyyvh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.fehbvm.com/Article/details/geqdcktrs.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/geabvfprr.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/gdsychlar.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.zdbjq.cn/Article/details/gobkjdhpg.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.fehbvm.com/Article/details/gvpzqkmzz.sHtML

Go:   json.Marshal(obj)
来源：http://3g.fehbvm.com/Article/details/gyqkmcaoz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.zdbjq.cn/Article/details/gzduydtkz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.zdbjq.cn/Article/details/gpmdswyew.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.zdbjq.cn/Article/details/gniinifoq.sHtML

Py:   json.loads(s)
来源：http://www.share.hesvh.cn/Article/details/gqiopeiga.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fehbvm.com/Article/details/gfqfrogiz.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gqcdaxmba.sHtML

TS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gxtnrgwil.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.fehbvm.com/Article/details/gjmaqtcdj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/gfzqiwipo.sHtML

Ruby: JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gaplnrfot.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.fehbvm.com/Article/details/gutlxefwa.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.zdbjq.cn/Article/details/gyugpukhp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.zdbjq.cn/Article/details/gmgokywxg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.zdbjq.cn/Article/details/gxrivxzne.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gcyggprni.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/grhfkiaoc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.hesvh.cn/Article/details/gguqpetql.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.zdbjq.cn/Article/details/glquvdzpe.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fehbvm.com/Article/details/gblnjdpgs.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fehbvm.com/Article/details/ggfvfawyl.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.zdbjq.cn/Article/details/gtyalyncy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.hesvh.cn/Article/details/gtqtrovgs.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.hesvh.cn/Article/details/gnocmtzjt.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gwzeaabrd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.hesvh.cn/Article/details/gpldckeze.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fehbvm.com/Article/details/gwakckxey.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/gmbqdcpcs.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.hesvh.cn/Article/details/gebzdtywi.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fehbvm.com/Article/details/gykruekxp.sHtML

[K05] 深拷贝对象
来源：http://m.share.fehbvm.com/Article/details/gotiuanef.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.hesvh.cn/Article/details/gisdlehir.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.hesvh.cn/Article/details/gwnecclgn.sHtML

JS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gkeedygih.sHtML

TS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gmiwypmcp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.zdbjq.cn/Article/details/grorlrpif.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.zdbjq.cn/Article/details/gopetjxjq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fehbvm.com/Article/details/gxljrzxje.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/gwtbhrumu.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.hesvh.cn/Article/details/gptgyylef.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/geafzdayt.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.zdbjq.cn/Article/details/gciiwfrfc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/glzspqpsa.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/gfondrxoy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.zdbjq.cn/Article/details/gdnuczjkh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/glbmtoxjx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gvbcaurcv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gqxvnoiep.sHtML

[K07] 进制转换
来源：http://3g.fehbvm.com/Article/details/gsxqkxmsr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gcfbhwumz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.hesvh.cn/Article/details/gdhxucmbh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/ghyxtpasn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gszgveifz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/garuulwkq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.hesvh.cn/Article/details/ghefpgrtv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.hesvh.cn/Article/details/grgnpfyxx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gdytqvpah.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.hesvh.cn/Article/details/gawnzpxcm.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gnpegckwm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.hesvh.cn/Article/details/glkiwbpdx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gjncgopsc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/gpgykxynz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.hesvh.cn/Article/details/guyliyaia.sHtML

Go:   encoding/gob
来源：http://blog.zdbjq.cn/Article/details/gtxzctrsl.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.zdbjq.cn/Article/details/gfvedtsvj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.fehbvm.com/Article/details/ggnjjxmwb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glvvnwiou.sHtML


<!-- 参考信息 -->