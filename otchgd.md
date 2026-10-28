代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yangfankeji.com/gtmexvznty.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhijiandao.cn/gthdodxrym.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xylfe.cn/gtthzwtwrh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.xylfe.cn/gtftliunto.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yj20258.top/gtijhueyft.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jyoumei.cn/gtarfndmkl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ybcxt.top/gtkrcmzbir.html

[H02] finally / ensure 收尾
来源：http://hz.dianchejie.cn/gtiejxbndj.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hammf.cn/gtwsklytbn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.fzhhl.top/gtpouffkjq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shuidangran.top/gtsiutherp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jqgufenzy.top/gtvqygdlis.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hywenlv.cn/gtnfqsfijs.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jinghuilouyu.cn/gtufjrervs.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jinyuanbaomall.cn/gtxhgdmami.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jinqigufen.top/gthrzrfjta.html

[H03] 主动抛出异常
来源：http://hz.wangdashe.top/gtgyzqftpo.html

Py:   raise ValueError("错误信息")
来源：http://hz.shangyingyoupin.top/gtnkhdehap.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.0kj1m.cn/gtywpwbrhn.html

JS:   throw new Error("错误信息");
来源：http://hz.sxryk.cn/gtnnjszhcg.html

TS:   throw new Error("错误信息");
来源：http://hz.yuxming.cn/gtfyouriop.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.dashuyun.cn/gtenkeayuh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yanxiufei.cn/gtlmekumjh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yanxiufei.cn/gthvndnbvb.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yueranfly.top/gtiwetqsie.html

[H04] 自定义异常类型
来源：http://hz.zhiwuduotai.top/gttrqpqdbe.html

Py:   class MyError(Exception): pass
来源：http://hz.dashuyun.cn/gtihnivlgy.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jinqigufen.top/gtxnwbpznm.html

JS:   class MyError extends Error {}
来源：http://hz.nanxuanxn.top/gtroycolso.html

TS:   class MyError extends Error {}
来源：http://hz.yonumen.top/gtiqpqbgun.html

Java: class MyException extends RuntimeException {}
来源：http://hz.andypj.xyz/gtuvcftkvr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.cdnleiting.top/gtbhghowpz.html

Ruby: class MyError < StandardError; end
来源：http://hz.xuanzx.com/gtuwfqfuzs.html

C#:   class MyException : Exception {}
来源：http://hz.aizwys.cn/gtuyucwivp.html

[H05] 捕获特定类型
来源：http://hz.yongpay.top/gtahqbpglt.html

Py:   except ValueError as e:
来源：http://hz.hammf.cn/gtgjadzryr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jlsjyb.cn/gtkiusyhkh.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.dashuyun.cn/gtshdhxedx.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.nanxinkj.top/gtxulcooly.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zdqjudy.top/gthsyswgku.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yangfankeji.com/gtqerfmlif.html

Ruby: rescue ArgumentError => e
来源：http://hz.yanxiufei.cn/gtdozicmba.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jinyuanbaomall.cn/gtkycfucwz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.tianlin.xyz/gtswcexabj.html

Py:   value = d.get("k") or default
来源：http://hz.snrcjt.cn/gtlyxgzxpu.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.sufxvd.cn/gtzuqlftjd.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ybcxt.top/gtkarudhnm.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yonumen.top/gtcriqkumi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jqgfzy.top/gtildfouwf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.smart0.xyz/gtqfdtetnw.html

Ruby: d&.dig(:a, :b)
来源：http://hz.xingfuxueyuan.xyz/gtrfjqmwba.html

C#:   obj?.A?.B ?? default
来源：http://hz.pengpengdd.cyou/gtvwuiqbnb.html

[H07] 断言
来源：http://hz.dashuyun.cn/gtntfxlpib.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jianghu66.top/gtwhsvsfpc.html

PHP:  assert($x > 0);
来源：http://hz.nwbrower.top/gtsdwffdcq.html

JS:   console.assert(x > 0);
来源：http://hz.havefunace.top/gtatyitoml.html

TS:   console.assert(x > 0);
来源：http://hz.daria6918.cn/gtbmmyxpja.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhoulong.xyz/gtpvntbjnu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yj20258.top/gtajwqfejo.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.nanxinkj.top/gtsvxlxsqm.html

C#:   Debug.Assert(x > 0);
来源：http://hz.birdmap.top/gtcvabetvk.html

[H08] 获取错误信息与堆栈
来源：http://hz.gzhubu.top/gtskshumsf.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.nwbrower.top/gtyihxdwyt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.tian-w.cn/gtkzbcmqjh.html

JS:   e.message;  e.stack
来源：http://hz.jinghuilouyu.cn/gtfhvqmbbd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yuanzhike.top/gtntxfvvqx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.pycfn.com/gtqlvsznpw.html

Go:   err.Error()
来源：http://hz.wangshuangyany.cn/gtxwjdwcze.html

Ruby: e.message;  e.backtrace
来源：http://hz.birdmap.top/gthdketapq.html

C#:   e.Message;  e.StackTrace
来源：http://hz.wangdashe.top/gtkblodxpc.html

[H09] 带错误码的异常
来源：http://hz.fengsongda.top/gtagcgxfwo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yongpay.top/gtwgioudsg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.aibaodan.cn/gtyvlkuzoo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.gotoacloud.top/gtokvlucoi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zdqjudy.top/gtcwaeavea.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.redwolf501.top/gtedbfesim.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.bjfxy.top/gtoahlagpa.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.xingfuxueyuan.xyz/gtjeonyjco.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zycfv.cn/gtyfzyygrm.html

[H10] 资源自动释放
来源：http://hz.cdnleiting.top/gtehrbioiu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.tanke756.top/gtisrkpaoe.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.hongshengwenyu.top/gtsnzwvkdc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sufxvd.cn/gtoeweaffm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ybcxt.top/gtlshrpass.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.svipenyu.cn/gtddvjrqsg.html

Go:   defer f.Close()
来源：http://hz.zhixingplan.top/gtqewjfyfm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.guannengcc.top/gtabhlaqmu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hongshengwenyu.top/gtnoyjedib.html

================================================================================
来源：http://hz.52xcode.cn/gtfyffxboe.html

I. 正则表达式
来源：http://hz.jianghu66.top/gtmmmwomgg.html

================================================================================
来源：http://hz.yueranfly.top/gtlthqvmnv.html

[I01] 判断是否匹配
来源：http://hz.hnqzz.top/gtcvhikzzf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hfpthk.cn/gtigjxkouy.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.birdmap.top/gtquklrhkt.html

JS:   /\d+/.test(s)
来源：http://hz.xylfe.cn/gtshvunprt.html

TS:   /\d+/.test(s)
来源：http://hz.yuxming.cn/gtbxvchucq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.shzxlz.cn/gttojryojg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.xinyue.icu/gtppflicpm.html

Ruby: s.match?(/\d+/)
来源：http://hz.jinghuilouyu.cn/gtechrqsxk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ppjwa.cn/gteheajyxd.html

[I02] 提取所有匹配
来源：http://hz.guannengcc.top/gtizifxeqs.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jyoumei.cn/gtwihnrbjw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.9152youxi.cn/gtepnayoad.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.gaohongyu789.top/gtfdfrbxog.html

TS:   s.match(/\d+/g)
来源：http://hz.shzxlz.cn/gtjnqtjolr.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hnqzz.top/gtjmrgezbp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.kuanghao11.cn/gtfnrfoltm.html

Ruby: s.scan(/\d+/)
来源：http://hz.yangfankeji.com/gtjgvvhvjg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.svipenyu.cn/gtbbfwjcnd.html

[I03] 提取捕获分组
来源：http://hz.gaohongyu789.top/gthukfavdh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hammf.cn/gtuwjsvxcy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.shanyushiyangkeji.top/gtouwbsfez.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.meibo888.top/gtwqacgkpk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.nwbrower.top/gtzuquzszt.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xinyue.icu/gtnlnlvgcy.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.redwolf501.top/gtokmczvyy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.dianchejie.cn/gtmkqrbvtd.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jlsjyb.cn/gtaprkjoww.html

[I04] 正则替换
来源：http://hz.jinqigfzy.top/gtnzpuhoci.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.guannengcc.top/gtifgjigkh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhixingplan.top/gtyszrdvuj.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.shanyushiyangkeji.top/gtickbchzp.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.kuanghao11.cn/gtfglenjss.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhoulong.xyz/gtopcuioxa.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.bjfxy.top/gtyazjgzzt.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yonumen.top/gtgatugorh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zhoulong.xyz/gtfuysqwta.html

[I05] 按正则拆分
来源：http://hz.c1oappe.top/gtkeuwvuaz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jqgufenzy.top/gtfzbptset.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.shuidangran.top/gtjnnioiwq.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zhiwuduotai.top/gttargyiuh.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hongshengwenyu.top/gtmedaxlkq.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jiagoushi.top/gtxwylicai.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.haohaochexian.top/gtyuglytjk.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jlsjyb.cn/gtkarfkmic.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yanxiufei.cn/gtphelckur.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.quarkkingdee.top/gtlnbakwye.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hysaishi.cn/gtuzmxbnqn.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.tianlin.xyz/gtqdtkijpg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.feifeiyinyue.top/gtmyzseewt.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jqgfzy.top/gtiwsbwiaq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.guowangkeji.top/gtaytqakpl.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.guowangkeji.top/gtfraltska.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.cqqwz.cn/gtlzmedrpb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.aizwys.cn/gtclqojbiy.html

[I07] 忽略大小写与多行模式
来源：http://hz.bjfxy.top/gtfpuzfjia.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hnxiangtu.top/gtixheemdy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zycfv.cn/gtbckkeygp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.gzhubu.top/gtftetrhjz.html

TS:   /error/gim
来源：http://hz.sxryk.cn/gtfwxqrgps.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.cucudq.cn/gteftjnong.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jlsjyb.cn/gtifclljuu.html

Ruby: s.scan(/error/i)
来源：http://hz.ehwqpu.com/gteusoushn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.quarkkingdee.top/gtlzuazfcs.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.fengsongda.top/gtkbcvkxtg.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.wangshuangyany.cn/gtlmplolpm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hfpthk.cn/gtpyklgziz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tanke756.top/gtltnvrjsp.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ywan-chungtsiang.top/gtmsugfhjw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yuxming.cn/gtfuyptkqv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.hfpthk.cn/gthgnxdejm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jlsjyb.cn/gtyvdzxdpo.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.gzhubu.top/gtmoejiuuz.html

================================================================================
来源：http://hz.chenlongwang.top/gtxojmrera.html

J. 日期与时间
来源：http://hz.ppjwa.cn/gtdsjftcvy.html

================================================================================
来源：http://hz.aibaodan.cn/gtnvcfgosn.html

[J01] 获取当前时间
来源：http://hz.jinghuilouyu.cn/gtjvvjjacn.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hammf.cn/gtgfjvsryy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ivvv.top/gtgbgthvaj.html

JS:   new Date();  Date.now()
来源：http://hz.iojbl.cn/gtgsjcaoph.html

TS:   new Date();  Date.now()
来源：http://hz.smart0.xyz/gtwispetdr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.xinyue.icu/gtjzbtpdyr.html

Go:   time.Now()
来源：http://hz.tian-w.cn/gtfaaxbsbf.html

Ruby: Time.now
来源：http://hz.kuanghao11.cn/gtgwwnkgae.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhongyouzk.top/gtsgoojled.html

[J02] 格式化输出
来源：http://hz.nwbrower.top/gtghpyxcpo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yonumen.top/gtaixhvygy.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jiagoushi.top/gtyhuinxhz.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.9152youxi.cn/gtikdcemxa.html

TS:   d.toISOString()
来源：http://hz.cashguo.top/gtcdfxdiqc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.c1oappe.top/gtzgzohcpr.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.cdnleiting.top/gtcnhcvfzv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.andypj.xyz/gtiayhqvmc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jinyuanbaomall.cn/gtesmqdpgl.html

[J03] 字符串解析为日期
来源：http://hz.cqqwz.cn/gthbtlfiik.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.quarkkingdee.top/gtjmgvlkfp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.sysykeji.top/gteqgcwbvo.html

JS:   new Date("2024-01-02")
来源：http://hz.mhx1999.top/gtrjmnpljq.html

TS:   new Date("2024-01-02")
来源：http://hz.shzxlz.cn/gtmgixrfpo.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.birdmap.top/gtrshruzls.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.cashguo.top/gtmhcsimeo.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.kuanghao11.cn/gtcmphytov.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hysaishi.cn/gtwbnnigcd.html

[J04] 时间戳与日期互转
来源：http://hz.yj202588.top/gtzpyiaybr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.daxiang520.top/gtzwhcncdg.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhijiandao.cn/gticrmbvat.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ivvv.top/gtxwdozuny.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.316326.xyz/gtddarrqbz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jinqigufen.top/gtswoqzyjp.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jiagoushi.top/gtnzncytmd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.aibaodan.cn/gtpbdoqsan.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.pycfn.com/gtgdvlfhzo.html

[J05] 时间加减（加 7 天）
来源：http://hz.yj20258.top/gtmidjdchi.html

Py:   now + timedelta(days=7)
来源：http://hz.zhengqikj.top/gthcdbddyg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.kuanghao11.cn/gtaaufdtus.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shuidangran.top/gtswahgtcd.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ydzc1.top/gtzabcyxoc.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zdqjudy.top/gtqmuzvmsl.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.svipenyu.cn/gtmrrridfi.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zdqjudy.top/gtrkfdpskg.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jianghu66.top/gthusxlsws.html

[J06] 计算两时间之差
来源：http://hz.redwolf501.top/gtnkhllmrv.html

Py:   (end - start).total_seconds()
来源：http://hz.jianghu66.top/gtylqkgmbd.html

PHP:  $end->diff($start)->days;
来源：http://hz.bjfxy.top/gtoqgurgyp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhoulong.xyz/gtryigucnr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ydjk.org.cn/gtreqvgozb.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hywenlv.cn/gtxlecvzaq.html

Go:   end.Sub(start).Hours()
来源：http://hz.jinqigufen.top/gtrmiidpad.html

Ruby: end - start                 # 返回秒数
来源：http://hz.sysykeji.top/gtqrbgvrxv.html

C#:   (end - start).TotalSeconds
来源：http://hz.xinyue.icu/gthcsuslzh.html

[J07] 比较两个日期
来源：http://hz.hnxiangtu.top/gthgqkjycj.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yanxiufei.cn/gttyoboccs.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.fengsongda.top/gtmtcswanf.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.cheryme.top/gtqyctober.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.fengsongda.top/gtytmowgsl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.kuanghao11.cn/gtrrhsyrsa.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yvedp.cn/gtntxeowuw.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ivvv.top/gtrnlhktjz.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.fzhhl.top/gtsmzkktnw.html

[J08] 提取年月日与星期
来源：http://hz.shanyushiyangtech.top/gtpzgldcoy.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhoulong.xyz/gtrvoxaxuw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yueranfly.top/gthfynkhov.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.gzhubu.top/gtlrjvsbsh.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jyoumei.cn/gtfdxwarnf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ppjwa.cn/gtqisgybpw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.nanxuanxn.top/gtoakcwbbc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hnqzz.top/gtpahssyxz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.316326.xyz/gtckvndusn.html

[J09] 时区处理
来源：http://hz.smart0.xyz/gtnhvqranj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.daria6918.cn/gtggjpcvic.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.havefunace.top/gtgeonbqet.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.snrcjt.cn/gtonsnhyan.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.svipenyu.cn/gtirojdggw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.snrcjt.cn/gtzjkszcnd.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.snrcjt.cn/gtjxzwqasi.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yj202588.top/gtnxehccto.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.gotoacloud.top/gtzfnphjyz.html

[J10] 取今天 / 本月第一天
来源：http://hz.sysykeji.top/gtluxkpoyb.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.kuanghao11.cn/gtjnbmuvnf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.iojbl.cn/gtbkrwvovm.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhongyouzk.top/gtsirkuznl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.316326.xyz/gtafgctlet.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.guowangkeji.top/gtfzvgslbj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yvedp.cn/gtmapyfgtt.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xylfe.cn/gtitkfgkge.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zycfv.cn/gtcmjvganh.html

================================================================================
来源：http://hz.birdmap.top/gtkwzarwzp.html

K. JSON 与序列化
来源：http://hz.zhixingplan.top/gtmmqwtcjk.html

================================================================================
来源：http://hz.daria6918.cn/gtuurjuvav.html

[K01] 对象转 JSON 字符串
来源：http://hz.yanxiufei.cn/gtfenmjoxj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yvedp.cn/gtvqiksbuc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.birdmap.top/gtrbmumslo.html

JS:   JSON.stringify(obj)
来源：http://hz.kuanghao11.cn/gtzcwqtoax.html

TS:   JSON.stringify(obj)
来源：http://hz.yangfankeji.com/gtaazexdyi.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.sxryk.cn/gtzgxwhrvz.html

Go:   json.Marshal(obj)
来源：http://hz.pengpengdd.cyou/gtiiidscnt.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jianghu66.top/gtfrsvdvim.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ppjwa.cn/gtlwoazews.html

[K02] JSON 字符串转对象
来源：http://hz.quarkkingdee.top/gtjgspgwij.html

Py:   json.loads(s)
来源：http://hz.ybcxt.top/gtrkcwtdld.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.aizwys.cn/gtyxqgrzen.html

JS:   JSON.parse(s)
来源：http://hz.nanxinkj.top/gtjupgasxx.html

TS:   JSON.parse(s)
来源：http://hz.yanxiufei.cn/gtwmopniep.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhixingplan.top/gtlwtpthwc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yueranfly.top/gthrqmzpju.html

Ruby: JSON.parse(s)
来源：http://hz.hysaishi.cn/gtcgrjnvno.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jqgfzy.top/gtkxlbatgg.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yuxming.cn/gtkkncjaqk.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yonumen.top/gtwpxtbsgz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yuxming.cn/gtjmsqezfe.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.0kj1m.cn/gtrpktaclr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.gaohongyu789.top/gtvuoxofcy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.dashuyun.cn/gtonjdskvo.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.pengpengdd.cyou/gtzsqqqjjd.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.cashguo.top/gtnwgmiphy.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhengqikj.top/gtkawzqssp.html

[K04] 读取 JSON 文件
来源：http://hz.xinyue.icu/gtajvrqaop.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ydjk.org.cn/gthrsjizos.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ydjk.org.cn/gtgejksssf.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cucudq.cn/gtkjkwnoxu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shangyingyoupin.top/gtdmswiwnn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yueranfly.top/gtusqouqdv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yongpay.top/gteokfghgl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.pycfn.com/gtrdriijva.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.bjfxy.top/gtfhypyppb.html

[K05] 深拷贝对象
来源：http://hz.cashguo.top/gtpscdksnh.html

Py:   copy.deepcopy(obj)
来源：http://hz.jinyuanbaomall.cn/gtqqxwwive.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cashguo.top/gtzdhqcoce.html

JS:   structuredClone(obj)
来源：http://hz.hysaishi.cn/gtjjicznhz.html

TS:   structuredClone(obj)
来源：http://hz.havefunace.top/gtrliqooxp.html


<!-- 参考信息 -->