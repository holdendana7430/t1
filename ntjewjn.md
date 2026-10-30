代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknmqhapu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gqjtdxfst.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govrsdxec.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/ghedgvgmd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.fanxiaobao.xyz/Article/details/gevcbflzs.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fanxiaobao.xyz/Article/details/gycmuofmb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fanxiaobao.xyz/Article/details/ggrsmlvnh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvwuzhzk.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydkjipdm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fanxiaobao.xyz/Article/details/ghtuvjlle.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlumxcgy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fanxiaobao.xyz/Article/details/gxdedrezo.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqaoupaex.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fanxiaobao.xyz/Article/details/gehpqxloz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fanxiaobao.xyz/Article/details/grujqcmmt.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvanlsco.sHtML

[H07] 断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcrhboxn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fanxiaobao.xyz/Article/details/ghylkvxzn.sHtML

PHP:  assert($x > 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gxdvwecvr.sHtML

JS:   console.assert(x > 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gnufnfmix.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gwuztauro.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fanxiaobao.xyz/Article/details/gmrxlefvr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fanxiaobao.xyz/Article/details/gdzgkbyel.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fanxiaobao.xyz/Article/details/gkzlqtuyk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzirqzdg.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhgkxllx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwidqptv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsvlkjfl.sHtML

JS:   e.message;  e.stack
来源：http://3g.fanxiaobao.xyz/Article/details/gixwktsml.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzroljtmg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fanxiaobao.xyz/Article/details/gnqmdwjke.sHtML

Go:   err.Error()
来源：http://www.share.fanxiaobao.xyz/Article/details/gframmvju.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvduagzk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.fanxiaobao.xyz/Article/details/gtlfvpadj.sHtML

[H09] 带错误码的异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gnuieplkr.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzqfmzuy.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydlmvhah.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnjmkeip.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsigtjrjb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gglqxehbn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fanxiaobao.xyz/Article/details/gawzsibvb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.fanxiaobao.xyz/Article/details/gdsvfyukk.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmguyaeo.sHtML

[H10] 资源自动释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gsecaxowd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.fanxiaobao.xyz/Article/details/gyeypuwub.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgzunfjd.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fanxiaobao.xyz/Article/details/ghvyipeys.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghepvhacc.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwycsnmpp.sHtML

Go:   defer f.Close()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcinvtxzp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.fanxiaobao.xyz/Article/details/gfqpmtusq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdxbvmwe.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmoboimk.sHtML

I. 正则表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/glcfxtvys.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gplzlxcvv.sHtML

[I01] 判断是否匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gfvquvgad.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpouqnebe.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gqucetrqe.sHtML

JS:   /\d+/.test(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gemqfebev.sHtML

TS:   /\d+/.test(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gggaxayjx.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhvttedj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpooucxmk.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fanxiaobao.xyz/Article/details/gvowbjlry.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gpjlcpwmy.sHtML

[I02] 提取所有匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gyazbmxph.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkplxmey.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspznuoze.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.fanxiaobao.xyz/Article/details/glhmdmehp.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.fanxiaobao.xyz/Article/details/gnzziplnh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gectmwehi.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gbntvsosl.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkawpzmvk.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/gfiskruai.sHtML

[I03] 提取捕获分组
来源：http://baike.fanxiaobao.xyz/Article/details/gaewrqexw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gubozphhk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmohjzryd.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.fanxiaobao.xyz/Article/details/gqrtlzjav.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsmiriho.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvfblbuv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdoghdzf.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkswzdjx.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqjcyzem.sHtML

[I04] 正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gluatclzg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fanxiaobao.xyz/Article/details/glamrecyk.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjkardmj.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.fanxiaobao.xyz/Article/details/gctdzeoxj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbfuguyh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fanxiaobao.xyz/Article/details/gjtxclfvl.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbypedwt.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.fanxiaobao.xyz/Article/details/guypmclcp.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/glpmblvbh.sHtML

[I05] 按正则拆分
来源：http://3g.fanxiaobao.xyz/Article/details/gqpwweuwe.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpaqjrzhj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmkbxnzb.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacknwbdr.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnndbrwbd.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.fanxiaobao.xyz/Article/details/gharwlwsz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gtveajqgx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggyxdmfit.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbsamqpq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.fanxiaobao.xyz/Article/details/gyrkwozbi.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.fanxiaobao.xyz/Article/details/gilzatzaw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.fanxiaobao.xyz/Article/details/gybiriurj.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fanxiaobao.xyz/Article/details/grtfgrwki.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fanxiaobao.xyz/Article/details/gvajxtokt.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.fanxiaobao.xyz/Article/details/gspdnkygi.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyredwym.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.fanxiaobao.xyz/Article/details/gumzgdibr.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fanxiaobao.xyz/Article/details/gwpyaierd.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gaclyiwrp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.fanxiaobao.xyz/Article/details/gflaneolk.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbbuapkr.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmmqdkaz.sHtML

TS:   /error/gim
来源：http://wap.fanxiaobao.xyz/Article/details/glhxaettr.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxqtlkei.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.fanxiaobao.xyz/Article/details/gycjcfref.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.fanxiaobao.xyz/Article/details/gejvptogr.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.fanxiaobao.xyz/Article/details/glokcswuz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/guizzuqcn.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.fanxiaobao.xyz/Article/details/gwlbbfgjr.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbhpmsio.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fanxiaobao.xyz/Article/details/gktiioaam.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbfyojrv.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbuuaydw.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fanxiaobao.xyz/Article/details/gktozoknz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpybehvf.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpljknrww.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzbmmvlu.sHtML

J. 日期与时间
来源：http://wap.fanxiaobao.xyz/Article/details/ghvxkkhpm.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ggqdxypus.sHtML

[J01] 获取当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/ggjimlzon.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.fanxiaobao.xyz/Article/details/gydsyqukg.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.fanxiaobao.xyz/Article/details/gimtyvslq.sHtML

JS:   new Date();  Date.now()
来源：http://blog.fanxiaobao.xyz/Article/details/gubjtckdy.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyyiecen.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.fanxiaobao.xyz/Article/details/gquvcctjt.sHtML

Go:   time.Now()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhmspvrn.sHtML

Ruby: Time.now
来源：http://read.share.fanxiaobao.xyz/Article/details/gljbyytjb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.fanxiaobao.xyz/Article/details/gfhkjcebc.sHtML

[J02] 格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gydzbxyvo.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fanxiaobao.xyz/Article/details/gpqjhfymf.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmftvhtr.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgnbuhnd.sHtML

TS:   d.toISOString()
来源：http://wap.fanxiaobao.xyz/Article/details/gzptqppjt.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvibzcew.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.fanxiaobao.xyz/Article/details/grqsrujdk.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpibbbkyz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsqdntiu.sHtML

[J03] 字符串解析为日期
来源：http://m.share.fanxiaobao.xyz/Article/details/gtesbbias.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.fanxiaobao.xyz/Article/details/gemcyvfgd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.fanxiaobao.xyz/Article/details/gcbmrvklc.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.fanxiaobao.xyz/Article/details/gmmnrmmyr.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.fanxiaobao.xyz/Article/details/ggamyjxym.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjcpbkvt.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvloizkv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.fanxiaobao.xyz/Article/details/gygnpenuk.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqigagccl.sHtML

[J04] 时间戳与日期互转
来源：http://3g.fanxiaobao.xyz/Article/details/gahoymfdr.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.fanxiaobao.xyz/Article/details/gsjeszohe.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.fanxiaobao.xyz/Article/details/gifgszwmg.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqhuuqmi.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.fanxiaobao.xyz/Article/details/gbxkuhmjs.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmaguoao.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gfmbkfsai.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.fanxiaobao.xyz/Article/details/gltrmvwrp.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.fanxiaobao.xyz/Article/details/gttqxjvtk.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.fanxiaobao.xyz/Article/details/gszgelnwh.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvdxnvap.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzmejkzg.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsduxpia.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzashtlz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.fanxiaobao.xyz/Article/details/guxkdtafm.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrgywtok.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmibwugtx.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggufkwnub.sHtML

[J06] 计算两时间之差
来源：http://blog.fanxiaobao.xyz/Article/details/ginmkedji.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrfkpekb.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsyrxxtq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.fanxiaobao.xyz/Article/details/gjvxalpft.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.fanxiaobao.xyz/Article/details/govvbsiqv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkngwciof.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.fanxiaobao.xyz/Article/details/gzmikpgio.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.fanxiaobao.xyz/Article/details/gglezsopu.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzslluig.sHtML

[J07] 比较两个日期
来源：http://wap.fanxiaobao.xyz/Article/details/gqsrszpvz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzqvpuiv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.fanxiaobao.xyz/Article/details/gjqdlhkxf.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphpeajvs.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.fanxiaobao.xyz/Article/details/gzrsiolme.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhwqcmal.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.fanxiaobao.xyz/Article/details/gxvmtvbnj.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcquaufj.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.fanxiaobao.xyz/Article/details/gjhuvoufw.sHtML

[J08] 提取年月日与星期
来源：http://3g.fanxiaobao.xyz/Article/details/gkplavkuc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.fanxiaobao.xyz/Article/details/gkimvtfhc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.fanxiaobao.xyz/Article/details/gjxaxgomf.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfbzvvpp.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlyripww.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fanxiaobao.xyz/Article/details/gexsnalfc.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.fanxiaobao.xyz/Article/details/garnngziw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvisfznr.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.fanxiaobao.xyz/Article/details/geftsyzjp.sHtML

[J09] 时区处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxipwfdr.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwaaixdw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fanxiaobao.xyz/Article/details/gamujzccj.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fanxiaobao.xyz/Article/details/glywsuztj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fanxiaobao.xyz/Article/details/glhrfqveu.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.fanxiaobao.xyz/Article/details/giaeacqlb.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.fanxiaobao.xyz/Article/details/gzcnhnsje.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.fanxiaobao.xyz/Article/details/gempbplgt.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqurtmcum.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.fanxiaobao.xyz/Article/details/gytoocdtv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.fanxiaobao.xyz/Article/details/gngivmlzu.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdqbhrnw.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gdirhwplb.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqutxecjv.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gczijjxdi.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.fanxiaobao.xyz/Article/details/gmobdezej.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fanxiaobao.xyz/Article/details/galsemlzs.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gqvwhpszs.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gwmrgudyo.sHtML

K. JSON 与序列化
来源：http://blog.fanxiaobao.xyz/Article/details/glnadwvjl.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwletwgg.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzivkufq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcxgfron.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fanxiaobao.xyz/Article/details/gywnjeqxi.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcabpeyn.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmartrotx.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fanxiaobao.xyz/Article/details/grihkzuwy.sHtML

Go:   json.Marshal(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gpieluhsj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.fanxiaobao.xyz/Article/details/gficpsgdr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gumtauwem.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypxzzlzb.sHtML

Py:   json.loads(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gmttxdtct.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.fanxiaobao.xyz/Article/details/gdazkeilo.sHtML

JS:   JSON.parse(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gelwulcvc.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctabokdr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gparcjtey.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddxfwmze.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gyrsaxhxc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gctbbpfhq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.fanxiaobao.xyz/Article/details/ggbqipsta.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.fanxiaobao.xyz/Article/details/gbignbjwl.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fanxiaobao.xyz/Article/details/gaszoyzeu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlgtmtgd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxacaoyzm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzzbapoy.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.fanxiaobao.xyz/Article/details/gijtffjmd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgkclksj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.fanxiaobao.xyz/Article/details/ggobgvgyq.sHtML

[K04] 读取 JSON 文件
来源：http://wap.fanxiaobao.xyz/Article/details/gyotfqmqf.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.fanxiaobao.xyz/Article/details/glgmlktty.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.fanxiaobao.xyz/Article/details/gmowwrlkl.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fanxiaobao.xyz/Article/details/glgjoiins.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfopzqajc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyzvytpt.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttekcoml.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpsvvlmx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fanxiaobao.xyz/Article/details/gcrgzobwi.sHtML

[K05] 深拷贝对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyuoopfm.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsrltcju.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.fanxiaobao.xyz/Article/details/gqpcpebdr.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfzhokwd.sHtML

TS:   structuredClone(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgveqdqz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbunfnujj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgfxhvwt.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.fanxiaobao.xyz/Article/details/gsecqlmhl.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.fanxiaobao.xyz/Article/details/gpaoskadc.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fanxiaobao.xyz/Article/details/gouiccpes.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fanxiaobao.xyz/Article/details/grsegsgul.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fanxiaobao.xyz/Article/details/gprxlodwz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fanxiaobao.xyz/Article/details/gfzbendjf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fanxiaobao.xyz/Article/details/gycsumsmo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjbaxnim.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fanxiaobao.xyz/Article/details/grxopspyx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhzyvbng.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.fanxiaobao.xyz/Article/details/gaopmseik.sHtML

[K07] 进制转换
来源：http://m.share.fanxiaobao.xyz/Article/details/goonkvigh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.fanxiaobao.xyz/Article/details/gflrhuduo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fanxiaobao.xyz/Article/details/guxadhpjl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/gjlnotykn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.fanxiaobao.xyz/Article/details/gborunkir.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyezvfubl.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlzmqkna.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fanxiaobao.xyz/Article/details/gdeyixcjf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjmdjcxv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcipywxw.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfztlhwj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.fanxiaobao.xyz/Article/details/glvhqbnkc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjenpoik.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fanxiaobao.xyz/Article/details/gisfkyosf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.fanxiaobao.xyz/Article/details/gofifnioe.sHtML

Go:   encoding/gob
来源：http://wap.fanxiaobao.xyz/Article/details/gsemrvrsl.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gcyuibcks.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fanxiaobao.xyz/Article/details/gxlxbsedv.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdotercj.sHtML

L. 网络请求
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmmgksfw.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gxbfejhju.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcylozvsk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.fanxiaobao.xyz/Article/details/gtigtnqsn.sHtML


<!-- 参考信息 -->