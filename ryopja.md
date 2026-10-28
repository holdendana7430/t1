代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.cheryme.top/gtscarfjam.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.svipenyu.cn/gteeyoqrcc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.nanxuanxn.top/gtctmnfuvq.html

[H02] finally / ensure 收尾
来源：http://hz.cashguo.top/gtyyyfazbk.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.iojbl.cn/gttmqbwxbl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jinghuilouyu.cn/gtfjocpycw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.0kj1m.cn/gticxjojoi.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.gzhubu.top/gtschqcvaf.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.ppjwa.cn/gtyoanngak.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ydzc1.top/gtewtgmziw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.316326.xyz/gtrxqqdehz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yanxiufei.cn/gtfagatepo.html

[H03] 主动抛出异常
来源：http://hz.yj20258888.top/gthqonkumg.html

Py:   raise ValueError("错误信息")
来源：http://hz.yuanzhike.top/gtlmnaykiv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jinqigufen.top/gtyixvjjsd.html

JS:   throw new Error("错误信息");
来源：http://hz.guannengcc.top/gtqrdbbnpl.html

TS:   throw new Error("错误信息");
来源：http://hz.jianghu66.top/gtlmzoutzm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.quarkkingdee.top/gtgvzdnpwx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.chenjidiqi.icu/gtltcwdplm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.redwolf501.top/gtfmkyejdf.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.cqqwz.cn/gtfftjugvc.html

[H04] 自定义异常类型
来源：http://hz.cdnleiting.top/gtyxhvsluc.html

Py:   class MyError(Exception): pass
来源：http://hz.jianghu66.top/gtbvpmwflm.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.0kj1m.cn/gtyhgchesc.html

JS:   class MyError extends Error {}
来源：http://hz.yj20258888.top/gtosebqmub.html

TS:   class MyError extends Error {}
来源：http://hz.sufxvd.cn/gtjrgaxonv.html

Java: class MyException extends RuntimeException {}
来源：http://hz.fzhhl.top/gtjtbjbdjh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.sufxvd.cn/gtikwdbcin.html

Ruby: class MyError < StandardError; end
来源：http://hz.fzhhl.top/gtfrsmhomp.html

C#:   class MyException : Exception {}
来源：http://hz.hnqzz.top/gtsjimlhyl.html

[H05] 捕获特定类型
来源：http://hz.sysykeji.top/gtfrqyccmf.html

Py:   except ValueError as e:
来源：http://hz.shanyushiyangkeji.top/gtabcewwlm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.smart0.xyz/gtrqmqmczm.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.pycfn.com/gtstcorzpf.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.gogol.net.cn/gtxprbksvj.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.gotoacloud.top/gtjugghquu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.smart0.xyz/gtgdfgjoco.html

Ruby: rescue ArgumentError => e
来源：http://hz.shzxlz.cn/gtreagoqia.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.feifeiyinyue.top/gtscqmifsq.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hnxiangtu.top/gtflgkqtgi.html

Py:   value = d.get("k") or default
来源：http://hz.yueranfly.top/gtvwfpqmcn.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.aibaodan.cn/gtsqsdtzaa.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.daria6918.cn/gtvvthpawn.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yangfankeji.com/gtosfhgule.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.pengpengdd.cyou/gtlxrjavey.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.nanxuanxn.top/gtcxbohotv.html

Ruby: d&.dig(:a, :b)
来源：http://hz.cashguo.top/gtbobzdcln.html

C#:   obj?.A?.B ?? default
来源：http://hz.dashuyun.cn/gtryjxemyr.html

[H07] 断言
来源：http://hz.xingfuxueyuan.xyz/gtevyxokrs.html

Py:   assert x > 0, "必须为正"
来源：http://hz.chenlongwang.top/gtjrdcmmei.html

PHP:  assert($x > 0);
来源：http://hz.zhaomingkeji.xyz/gtmvkjvirq.html

JS:   console.assert(x > 0);
来源：http://hz.yueranfly.top/gtbnovazop.html

TS:   console.assert(x > 0);
来源：http://hz.ppjwa.cn/gtapggiabw.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ppjwa.cn/gtfdvbwyom.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.daria6918.cn/gtchrqhjtv.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.xylfe.cn/gtmaunuifg.html

C#:   Debug.Assert(x > 0);
来源：http://hz.andypj.xyz/gtarvsveii.html

[H08] 获取错误信息与堆栈
来源：http://hz.shanyushiyangtech.top/gtmlkztsqf.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jqgfzy.top/gtlccmpnev.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.aizwys.cn/gtjrhkbeqs.html

JS:   e.message;  e.stack
来源：http://hz.aizwys.cn/gtegjxmnah.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.wangshuangyany.cn/gtupodfwwe.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.316326.xyz/gtvqepxlij.html

Go:   err.Error()
来源：http://hz.hammf.cn/gttnhihadu.html

Ruby: e.message;  e.backtrace
来源：http://hz.wangdashe.top/gtbqsjyqps.html

C#:   e.Message;  e.StackTrace
来源：http://hz.pycfn.com/gtebjprybk.html

[H09] 带错误码的异常
来源：http://hz.cashguo.top/gtlttpmcqp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.cashguo.top/gtebelupcv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yanxiufei.cn/gtzfsmmqak.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhiwuduotai.top/gtkrnjbimx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yj20258.top/gtydunhlwb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.dianchejie.cn/gtnbmtrkqr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.tanke756.top/gttrqyqvmj.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jianghu66.top/gtgjkcrocb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.aizwys.cn/gthypzalxa.html

[H10] 资源自动释放
来源：http://hz.redwolf501.top/gtgsmdjtea.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.iojbl.cn/gtgzhpvdzk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.wangdashe.top/gtbjyarzlj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xuanzx.com/gtkpqqflib.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yongpay.top/gtembvzstn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.havefunace.top/gtymztxgjn.html

Go:   defer f.Close()
来源：http://hz.aibaodan.cn/gtrwxzndyf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.tian-w.cn/gtcxputhin.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zycfv.cn/gtmzeuhbxg.html

================================================================================
来源：http://hz.xinyue.icu/gtrttrqivy.html

I. 正则表达式
来源：http://hz.hnxiangtu.top/gtpfxbzymv.html

================================================================================
来源：http://hz.pycfn.com/gtsmkneqvv.html

[I01] 判断是否匹配
来源：http://hz.yuanzhike.top/gtyzcpjgql.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ydjk.org.cn/gtqyoyrszh.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.aizwys.cn/gtpjaqbudj.html

JS:   /\d+/.test(s)
来源：http://hz.hongshengwenyu.top/gtllxxgegf.html

TS:   /\d+/.test(s)
来源：http://hz.ppjwa.cn/gtggguxfid.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.sufxvd.cn/gtwmuaccfu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.sxryk.cn/gtgkicobwj.html

Ruby: s.match?(/\d+/)
来源：http://hz.yanxiufei.cn/gtejtskzye.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.shuidangran.top/gttoiehzvm.html

[I02] 提取所有匹配
来源：http://hz.xinyue.icu/gtioyoxjgc.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hammf.cn/gtyfskujwk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.birdmap.top/gtmygjyqdj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.pycfn.com/gtklpyokkg.html

TS:   s.match(/\d+/g)
来源：http://hz.xuanzx.com/gtixhfotdc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hnqzz.top/gtokjphnjz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.bjfxy.top/gtcubdddqe.html

Ruby: s.scan(/\d+/)
来源：http://hz.yj202588.top/gtgdlkmgva.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hysaishi.cn/gtzarfjpza.html

[I03] 提取捕获分组
来源：http://hz.yongpay.top/gtcrvtijcv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ivvv.top/gteljvwuer.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jqgufenzy.top/gtrikwpkhg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jinqigufen.top/gtomlpbwgh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hnxiangtu.top/gtnfwjxdhm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.aizwys.cn/gtqzbplyyo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yuxming.cn/gtscwobevq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhongyouzk.top/gtrveelgxc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yangfankeji.com/gtbebaoajp.html

[I04] 正则替换
来源：http://hz.chenjidiqi.icu/gtjncpimqm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.52xcode.cn/gtnpsfdbdy.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.cqqwz.cn/gtcgiknegn.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.sweek.top/gtcoqemhwx.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.nanxinkj.top/gtbwflduso.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hnqzz.top/gtdhfudssg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hysaishi.cn/gtxpucmeym.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.birdmap.top/gtpejmnszj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.tanke756.top/gtkyvdfsjh.html

[I05] 按正则拆分
来源：http://hz.xinyue.icu/gttrssawje.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.tian-w.cn/gtskrroxvc.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.aibaodan.cn/gtaypoqtdu.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.wangshuangyany.cn/gtwsrvxtlj.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.shangyingyoupin.top/gttpjjzkmv.html

Java: s.split("\\s*,\\s*")
来源：http://hz.cucudq.cn/gtiidqsiln.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jinyuanbaomall.cn/gtpyytwzam.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yj20258888.top/gtcwhivfwx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yanxiufei.cn/gtvglsxecx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.chenzaomai.com/gtqezvowvb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.iojbl.cn/gtuelrhzlx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jlsjyb.cn/gtkxgayztt.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tian-w.cn/gtsjrxmytk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinqigfzy.top/gtlsmoqydt.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.ybcxt.top/gtkdfgsvme.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.chenlongwang.top/gtgdmislpg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.cqqwz.cn/gtdoakjddd.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.c1oappe.top/gtzdrfmwoo.html

[I07] 忽略大小写与多行模式
来源：http://hz.shuidangran.top/gtpovewepa.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.xingfuxueyuan.xyz/gtlvowiwfa.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hongshengwenyu.top/gtpwhygcks.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.chenlongwang.top/gthqubkskz.html

TS:   /error/gim
来源：http://hz.0kj1m.cn/gtgnbyzfiw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jiagoushi.top/gtwxpnazww.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ywan-chungtsiang.top/gtjexulurp.html

Ruby: s.scan(/error/i)
来源：http://hz.chenjidiqi.icu/gtnasvlsub.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jiagoushi.top/gtvlfsygea.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jinqigfzy.top/gtmzkmbwsx.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ybcxt.top/gtaixonrzd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.smart0.xyz/gtzlcqhjsa.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shuidangran.top/gtvjsvevik.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nanxinkj.top/gtwfeeljuq.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhaomingkeji.xyz/gtfwpmajum.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zycfv.cn/gtblvxrdsj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.gaohongyu789.top/gttmpcmxwq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ehwqpu.com/gtwhvkidsx.html

================================================================================
来源：http://hz.vqdsnc.cn/gtgfmmavmn.html

J. 日期与时间
来源：http://hz.jinqigfzy.top/gtgacwvjla.html

================================================================================
来源：http://hz.haohaochexian.top/gtardnhpbp.html

[J01] 获取当前时间
来源：http://hz.wangshuangyany.cn/gteitolqoj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shanyushiyangkeji.top/gtyffpdhxt.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.shanyushiyangtech.top/gthuvscomi.html

JS:   new Date();  Date.now()
来源：http://hz.tanke756.top/gtlplfkrxz.html

TS:   new Date();  Date.now()
来源：http://hz.dashuyun.cn/gtmmecxkap.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.xingfuxueyuan.xyz/gtgwvhtshn.html

Go:   time.Now()
来源：http://hz.meibo888.top/gtyuqxuthl.html

Ruby: Time.now
来源：http://hz.feifeiyinyue.top/gtgwuvrzug.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xuetiantiany.cn/gtlwfnsdly.html

[J02] 格式化输出
来源：http://hz.yanxiufei.cn/gtxkrjuhim.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.dianchejie.cn/gtzzmfnhzw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.shuidangran.top/gtdretbiii.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.fzhhl.top/gtfzthffqx.html

TS:   d.toISOString()
来源：http://hz.hfpthk.cn/gtlmepolzd.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.shanyushiyangkeji.top/gtftyszbye.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.cdnleiting.top/gtkfjyswju.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.aizwys.cn/gtzrlrrwtk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.sweek.top/gtrvyncsne.html

[J03] 字符串解析为日期
来源：http://hz.guowangkeji.top/gtlmbtfnux.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ppjwa.cn/gtmmcxliga.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.shanyushiyangkeji.top/gtbmmxkfxq.html

JS:   new Date("2024-01-02")
来源：http://hz.cdnleiting.top/gtbxxhqrsm.html

TS:   new Date("2024-01-02")
来源：http://hz.ydzc1.top/gtybgfttto.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.svipenyu.cn/gtmaxvogcz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yuxming.cn/gtgaumstmy.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.hongshengwenyu.top/gtayjvmqan.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.sysykeji.top/gtfjaoxrmo.html

[J04] 时间戳与日期互转
来源：http://hz.pengpengdd.cyou/gtcpatizqt.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jinghuilouyu.cn/gtsrjflnil.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.cucudq.cn/gtmsjmncrz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zhoulong.xyz/gtmbulhhnu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hywenlv.cn/gtzhrplsde.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.nwbrower.top/gtckuselrk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jyoumei.cn/gtrjnogjyb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.nwbrower.top/gtwtpbkswh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.0kj1m.cn/gtukzhmxgw.html

[J05] 时间加减（加 7 天）
来源：http://hz.nwbrower.top/gtibvdwdil.html

Py:   now + timedelta(days=7)
来源：http://hz.tanke756.top/gtfuksmxvm.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hongshengwenyu.top/gtlwuomefb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.daria6918.cn/gtjrzjlgnx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ivvv.top/gtgnydyqvk.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yj20258.top/gtsdbknpgc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hnqzz.top/gtgisfyiee.html

Ruby: Time.now + 7 * 86400
来源：http://hz.tanke756.top/gtmqhmwwjj.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xingfuxueyuan.xyz/gtbfbkxhba.html

[J06] 计算两时间之差
来源：http://hz.hywenlv.cn/gttksniwxr.html

Py:   (end - start).total_seconds()
来源：http://hz.fzhhl.top/gthpqabzxt.html

PHP:  $end->diff($start)->days;
来源：http://hz.jqgfzy.top/gthbbwmanf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.bjfxy.top/gtrttczzwm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hnxiangtu.top/gtwlqqdrjk.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.redwolf501.top/gtwrughxrm.html

Go:   end.Sub(start).Hours()
来源：http://hz.hysaishi.cn/gtynayplxy.html

Ruby: end - start                 # 返回秒数
来源：http://hz.cqqwz.cn/gtyoajppby.html

C#:   (end - start).TotalSeconds
来源：http://hz.xuanzx.com/gtyqdcvwub.html

[J07] 比较两个日期
来源：http://hz.mhx1999.top/gtaerbtebo.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yj202588.top/gtploizlgg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.gzhubu.top/gtpqjmdiql.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhijiandao.cn/gtbjnjvwvz.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258888.top/gtmkkedpvi.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jianghu66.top/gtvoplblbj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.0kj1m.cn/gtgjsmudng.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yanxiufei.cn/gtllicnvab.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.nwbrower.top/gtmksehxlx.html

[J08] 提取年月日与星期
来源：http://hz.fzhhl.top/gtoelgcweg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jinqigfzy.top/gtcnwimgis.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zdqjudy.top/gtrsmqqikg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.sufxvd.cn/gtrqjgqhll.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.52xcode.cn/gtrlootksm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.chenjidiqi.icu/gtueefuloa.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhiwuduotai.top/gtzlerovsb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.svipenyu.cn/gtzhmumrzk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhoulong.xyz/gtmaowaghg.html

[J09] 时区处理
来源：http://hz.jinghuilouyu.cn/gtjknibkgk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.haohaochexian.top/gtsxcqydak.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.feifeiyinyue.top/gtbpkpncut.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hnxiangtu.top/gtmxqopoat.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hfpthk.cn/gtzjxauopv.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.havefunace.top/gtavrpxyei.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yongpay.top/gtrfavupwi.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jinyuanbaomall.cn/gtimgvsotk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhongyouzk.top/gtoqpuwdux.html

[J10] 取今天 / 本月第一天
来源：http://hz.guowangkeji.top/gtwhlrnkbu.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yuanzhike.top/gtoeciglbc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yanxiufei.cn/gtcfsndgbc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hywenlv.cn/gtiidmakgd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.xylfe.cn/gtwoltmsuv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.xuetiantiany.cn/gtogmmqbzo.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yongpay.top/gtnpyiolrd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.pycfn.com/gtjmcxicgf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.wangshuangyany.cn/gtwnzbajhw.html

================================================================================
来源：http://hz.yj20258888.top/gtpmiahgjw.html

K. JSON 与序列化
来源：http://hz.nanxuanxn.top/gtgvbjtmgi.html

================================================================================
来源：http://hz.fzhhl.top/gtcmccuazz.html

[K01] 对象转 JSON 字符串
来源：http://hz.cheryme.top/gtjcdudaxq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zhoulong.xyz/gtitjjtffg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hnqzz.top/gtcqarqrnh.html

JS:   JSON.stringify(obj)
来源：http://hz.bjfxy.top/gtflamflaq.html

TS:   JSON.stringify(obj)
来源：http://hz.sufxvd.cn/gtttallfud.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.cdnleiting.top/gtvwhjswop.html

Go:   json.Marshal(obj)
来源：http://hz.yj202588.top/gtjmqlbstz.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.sweek.top/gtorqzdpop.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.feifeiyinyue.top/gtikwgfpzt.html

[K02] JSON 字符串转对象
来源：http://hz.9152youxi.cn/gtdlbwfnxv.html

Py:   json.loads(s)
来源：http://hz.daria6918.cn/gtowzhcwbd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.0kj1m.cn/gtahlmzcjn.html

JS:   JSON.parse(s)
来源：http://hz.xingfuxueyuan.xyz/gtymhbkysc.html

TS:   JSON.parse(s)
来源：http://hz.zycfv.cn/gtdzfuhrws.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.nanxuanxn.top/gtifikiuep.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhongyouzk.top/gtakaljyxf.html

Ruby: JSON.parse(s)
来源：http://hz.yuxming.cn/gthmwtbhlr.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.mhx1999.top/gtnqbaqbxl.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yj202588.top/gtyfpljflz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.0kj1m.cn/gtflfxjbkp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.wangshuangyany.cn/gtsewoslqo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.dashuyun.cn/gtkbwzebte.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hywenlv.cn/gtyrdiqeet.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jqgfzy.top/gtsalpgilx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yuanzhike.top/gtdblrpnom.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.feifeiyinyue.top/gtozxvsmwg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yanxiufei.cn/gtyduteecp.html

[K04] 读取 JSON 文件
来源：http://hz.hammf.cn/gtseojzypy.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.vqdsnc.cn/gtkzzwcegc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ybcxt.top/gtnhduqquj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhaomingkeji.xyz/gtfcadyhov.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.smart0.xyz/gtynoxulgf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yangfankeji.com/gtknfhgebt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhijiandao.cn/gtbxongdzf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhiwuduotai.top/gtdmbbhjcn.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.andypj.xyz/gtobmqglrt.html

[K05] 深拷贝对象
来源：http://hz.cheryme.top/gtfuviknic.html

Py:   copy.deepcopy(obj)
来源：http://hz.wangshuangyany.cn/gtrlunbfaz.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jyoumei.cn/gtvpmierix.html

JS:   structuredClone(obj)
来源：http://hz.fzhhl.top/gttccknknk.html

TS:   structuredClone(obj)
来源：http://hz.jyoumei.cn/gtmbkrguvk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yangfankeji.com/gtcnkopmrc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yonumen.top/gtwijcjgao.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zdqjudy.top/gtxcybzgmh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yvedp.cn/gtrshuvrps.html


<!-- 参考信息 -->