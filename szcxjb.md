代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.chenjidiqi.icu/gtruajsecb.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.tian-w.cn/gtyetmymtw.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhengqikj.top/gtfvjjyoqk.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhengqikj.top/gtslbcveov.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ivvv.top/gtgacwharq.html

Ruby: rescue ArgumentError => e
来源：http://hz.chenjidiqi.icu/gtmidgtuab.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hongshengwenyu.top/gtfqfwxafo.html

[H06] 可选值 / 空值安全访问
来源：http://hz.shzxlz.cn/gtjhufdmfe.html

Py:   value = d.get("k") or default
来源：http://hz.guowangkeji.top/gttdqvvvnl.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ivvv.top/gtasflavqs.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ydzc1.top/gtxfcdnqcj.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jqgufenzy.top/gtmbbpehev.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhoulong.xyz/gtunxtmjwc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jinqigufen.top/gtfucylxmy.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jinyuanbaomall.cn/gtsdcmadov.html

C#:   obj?.A?.B ?? default
来源：http://hz.hnqzz.top/gtovviomqc.html

[H07] 断言
来源：http://hz.zhaomingkeji.xyz/gtxiqjiazc.html

Py:   assert x > 0, "必须为正"
来源：http://hz.nanxinkj.top/gtkjqoohcz.html

PHP:  assert($x > 0);
来源：http://hz.fzhhl.top/gthwnhygqx.html

JS:   console.assert(x > 0);
来源：http://hz.cheryme.top/gtbzgsrqok.html

TS:   console.assert(x > 0);
来源：http://hz.gotoacloud.top/gtgcvjfgzb.html

Java: assert x > 0 : "必须为正";
来源：http://hz.mhx1999.top/gthyttkvbl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jyoumei.cn/gtllkyckek.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.chenzaomai.com/gtmdgmspbc.html

C#:   Debug.Assert(x > 0);
来源：http://hz.hnxiangtu.top/gtlhybndiy.html

[H08] 获取错误信息与堆栈
来源：http://hz.xinyue.icu/gtyjesynja.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.aizwys.cn/gtiuvpvgtd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.cheryme.top/gtnstskruk.html

JS:   e.message;  e.stack
来源：http://hz.chenzaomai.com/gtoxhfcaoj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cucudq.cn/gtmmryslvz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.nanxinkj.top/gtmphwislz.html

Go:   err.Error()
来源：http://hz.ydzc1.top/gtxmyscgbk.html

Ruby: e.message;  e.backtrace
来源：http://hz.hnqzz.top/gtuywcaqaz.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yongpay.top/gtuqppbrra.html

[H09] 带错误码的异常
来源：http://hz.zhiwuduotai.top/gtcbsbgpbo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xylfe.cn/gtoasrhvbb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.cdnleiting.top/gtrtednkmq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jqgfzy.top/gtbzjcxskm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.dianchejie.cn/gtwgbzvvty.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hysaishi.cn/gthdralogn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.shuidangran.top/gtzeacvczj.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.shanyushiyangtech.top/gtmzmewuzb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shuidangran.top/gtavswvxrb.html

[H10] 资源自动释放
来源：http://hz.yuxming.cn/gtjqdmekvx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhixingplan.top/gtzdycxmdw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.pycfn.com/gtiecwsatf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jqgufenzy.top/gtjllbzuaj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenlongwang.top/gtrzvjsvmg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hongshengwenyu.top/gtprjdhpky.html

Go:   defer f.Close()
来源：http://hz.gzhubu.top/gtuvrtqyre.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.smart0.xyz/gtkytitobw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.gzhubu.top/gtervedwtq.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtoiavuczn.html

I. 正则表达式
来源：http://hz.nanxuanxn.top/gtalwxswoo.html

================================================================================
来源：http://hz.chenzaomai.com/gtqzluucer.html

[I01] 判断是否匹配
来源：http://hz.sweek.top/gtmtouonzo.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhixingplan.top/gtvklsfose.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jlsjyb.cn/gtasxogdkh.html

JS:   /\d+/.test(s)
来源：http://hz.xuanzx.com/gtcnihkgkw.html

TS:   /\d+/.test(s)
来源：http://hz.yongpay.top/gtbjonkycn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.bjfxy.top/gtivhedqsj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ydjk.org.cn/gtesyxdzav.html

Ruby: s.match?(/\d+/)
来源：http://hz.jlsjyb.cn/gtpxihkvsa.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.316326.xyz/gtjyqvvmav.html

[I02] 提取所有匹配
来源：http://hz.guannengcc.top/gtoohtvgwk.html

Py:   re.findall(r"\d+", s)
来源：http://hz.quarkkingdee.top/gtlbvgotcp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shuidangran.top/gtsfsxstza.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xinyue.icu/gtdlxzysza.html

TS:   s.match(/\d+/g)
来源：http://hz.haohaochexian.top/gthtgtyfnf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.xinyue.icu/gtxqqhqjjg.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.cqqwz.cn/gtgoabbosv.html

Ruby: s.scan(/\d+/)
来源：http://hz.sysykeji.top/gtnlqgoudu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.birdmap.top/gtbyrwnrtq.html

[I03] 提取捕获分组
来源：http://hz.nanxinkj.top/gtsibzslrj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.aizwys.cn/gtsxqpzvgz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hfpthk.cn/gtiyydeoei.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yj20258888.top/gtwjroduvp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.sysykeji.top/gtpeyebygl.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.tianlin.xyz/gtigcmnrcm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.shanyushiyangkeji.top/gtoiagekcs.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jqgfzy.top/gtburtikrx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jlsjyb.cn/gtylmfwphg.html

[I04] 正则替换
来源：http://hz.yonumen.top/gtwqednfnf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.redwolf501.top/gtysczztbs.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hywenlv.cn/gthbcouuco.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hfpthk.cn/gtrarkzhsw.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.cqqwz.cn/gtlaluovrh.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.xylfe.cn/gtgcqcaorz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.aibaodan.cn/gtnpgokxab.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jinghuilouyu.cn/gtzdkusdui.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.mhx1999.top/gtmdxajaet.html

[I05] 按正则拆分
来源：http://hz.hammf.cn/gtgbvfenmg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.mhx1999.top/gtecpogpap.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.dashuyun.cn/gtbcsvdpok.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.cdnleiting.top/gtvjteibeh.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.sufxvd.cn/gtscyhfbnx.html

Java: s.split("\\s*,\\s*")
来源：http://hz.aizwys.cn/gtxxdvwydk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.guowangkeji.top/gtmzbmucej.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xinyue.icu/gtvivrnklw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.daria6918.cn/gtvofsgycm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.haohaochexian.top/gtefwnmfxf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jinqigufen.top/gtqngmyrwa.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.nwbrower.top/gtspnawnuj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.snrcjt.cn/gtlywpccmm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cheryme.top/gtjdoxkvln.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhoulong.xyz/gtprnewriy.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ppjwa.cn/gtumnyqori.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.snrcjt.cn/gtjotzkzqi.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yongpay.top/gtanuqazdh.html

[I07] 忽略大小写与多行模式
来源：http://hz.bjfxy.top/gtzskgzuqp.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.tian-w.cn/gtdczbdsxw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xinyue.icu/gtxakcurbn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.wangshuangyany.cn/gtydhpfaba.html

TS:   /error/gim
来源：http://hz.ivvv.top/gtwxjydnoj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.havefunace.top/gtjwfhpwba.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.aizwys.cn/gtyluktshf.html

Ruby: s.scan(/error/i)
来源：http://hz.guowangkeji.top/gtcibksngo.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ivvv.top/gtwnqkqglm.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zdqjudy.top/gtzasosdkm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.shanyushiyangkeji.top/gtrtaiyjlw.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.sweek.top/gtsosfexjr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.aizwys.cn/gtvixkrbsn.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhengqikj.top/gtmpfnrmxh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jyoumei.cn/gtmufyllqe.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.hywenlv.cn/gtimnosyml.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zhoulong.xyz/gthejdtdsy.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.nanxuanxn.top/gtydywmvjw.html

================================================================================
来源：http://hz.sysykeji.top/gtkpspkwie.html

J. 日期与时间
来源：http://hz.sufxvd.cn/gtbbwtjjeo.html

================================================================================
来源：http://hz.ppjwa.cn/gtghbxnajl.html

[J01] 获取当前时间
来源：http://hz.pengpengdd.cyou/gthfhnrknn.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.svipenyu.cn/gtxckfonzy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.cheryme.top/gtzbjafhbw.html

JS:   new Date();  Date.now()
来源：http://hz.redwolf501.top/gtnzyyrzbo.html

TS:   new Date();  Date.now()
来源：http://hz.yvedp.cn/gtlmqzaswx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.xziqi.cn/gtjqijnxxs.html

Go:   time.Now()
来源：http://hz.cdnleiting.top/gtzypgmmyk.html

Ruby: Time.now
来源：http://hz.yonumen.top/gtwuthwsxh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hnxiangtu.top/gtcvpasaen.html

[J02] 格式化输出
来源：http://hz.sweek.top/gtszpcfisd.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shzxlz.cn/gtxzrchhrr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yueranfly.top/gtxwfxszow.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xziqi.cn/gtvvwcwzej.html

TS:   d.toISOString()
来源：http://hz.yongpay.top/gtcewagcot.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.meibo888.top/gtbhsqgotf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.gaohongyu789.top/gtpjctlsak.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xylfe.cn/gtzvxextnd.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.52xcode.cn/gtggophgdi.html

[J03] 字符串解析为日期
来源：http://hz.sysykeji.top/gtsnxlmlxy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hnqzz.top/gttuvvljik.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhengqikj.top/gtsafglfjv.html

JS:   new Date("2024-01-02")
来源：http://hz.snrcjt.cn/gtrtmgurth.html

TS:   new Date("2024-01-02")
来源：http://hz.yanxiufei.cn/gtldsrpwbd.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.feifeiyinyue.top/gtllukkolt.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.tian-w.cn/gtqkktyyzs.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.dianchejie.cn/gtpmufzwvl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.dianchejie.cn/gtcbwbssjt.html

[J04] 时间戳与日期互转
来源：http://hz.cashguo.top/gtclczmede.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.gogol.net.cn/gtgyxtqmok.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.sufxvd.cn/gtvsneozic.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zhongyouzk.top/gtmcuvqgxx.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.52xcode.cn/gtgzswhjdw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.smart0.xyz/gtxnladcms.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.fzhhl.top/gtaqnjsqqq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yuxming.cn/gtrddjqvab.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.xuetiantiany.cn/gtpnyyfqhu.html

[J05] 时间加减（加 7 天）
来源：http://hz.zycfv.cn/gtharkmlkv.html

Py:   now + timedelta(days=7)
来源：http://hz.9152youxi.cn/gtloklosrg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ivvv.top/gthnyhboot.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.chenlongwang.top/gtfrijwryy.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ydjk.org.cn/gtflxidlbs.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yuanzhike.top/gtiwtdgxja.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.haohaochexian.top/gtfbufzxsu.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jiagoushi.top/gtskeeoydr.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jinyuanbaomall.cn/gtbqgggwek.html

[J06] 计算两时间之差
来源：http://hz.aibaodan.cn/gtzkiptjsd.html

Py:   (end - start).total_seconds()
来源：http://hz.9152youxi.cn/gttzuxmvyu.html

PHP:  $end->diff($start)->days;
来源：http://hz.nwbrower.top/gtxtqotxoe.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jinghuilouyu.cn/gtjfowxigz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.chenjidiqi.icu/gtwhkzkgql.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cheryme.top/gtvfbmxbka.html

Go:   end.Sub(start).Hours()
来源：http://hz.zdqjudy.top/gtzwsxhaja.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ydzc1.top/gtekbwwatm.html

C#:   (end - start).TotalSeconds
来源：http://hz.gaohongyu789.top/gtcysvhsyk.html

[J07] 比较两个日期
来源：http://hz.snrcjt.cn/gtzrnigpwk.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.tian-w.cn/gtdlvvkjxb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jiagoushi.top/gtconbtvzm.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ywan-chungtsiang.top/gtymeikaer.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.0kj1m.cn/gtbpipiwqd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ppjwa.cn/gthtcfebve.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.aizwys.cn/gtfxfxqiny.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.sweek.top/gtbcuwdpsp.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.sxryk.cn/gtmxslegio.html

[J08] 提取年月日与星期
来源：http://hz.ivvv.top/gthonddmil.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.pycfn.com/gtvypyjwfh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jlsjyb.cn/gtinihqsqf.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.aibaodan.cn/gtvpuwccql.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhijiandao.cn/gtzavstgcz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yuxming.cn/gtnjltgaek.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhixingplan.top/gtlvywqudh.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.aizwys.cn/gtlpfneezu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jinqigufen.top/gtcrfultbg.html

[J09] 时区处理
来源：http://hz.hysaishi.cn/gtnzvrxkdw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.fengsongda.top/gtwpkmgmgz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jqgufenzy.top/gtbzipktmy.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sufxvd.cn/gtxugzjszg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.chenlongwang.top/gtecugxqyw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hongshengwenyu.top/gtmlysygjk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.daria6918.cn/gtzbwfubwd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.fengsongda.top/gtjcjqgfll.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jinqigfzy.top/gtgffnwuqa.html

[J10] 取今天 / 本月第一天
来源：http://hz.xuanzx.com/gtaaomwfxv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.sufxvd.cn/gtaidhaeje.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.fengsongda.top/gtbypjzzwo.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xingfuxueyuan.xyz/gtqysjlzxm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zycfv.cn/gthucnpsru.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.ydjk.org.cn/gtjqpisivv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yonumen.top/gtqwwvstuz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jinqigfzy.top/gtictqtexc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jinghuilouyu.cn/gtlwiqvlcj.html

================================================================================
来源：http://hz.hammf.cn/gtrcsecaga.html

K. JSON 与序列化
来源：http://hz.c1oappe.top/gtfxazagrg.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtqdkvpfti.html

[K01] 对象转 JSON 字符串
来源：http://hz.dianchejie.cn/gtnbpdsfzw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.0kj1m.cn/gtznbxcyxy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ybcxt.top/gtgriydhqo.html

JS:   JSON.stringify(obj)
来源：http://hz.tian-w.cn/gtlhkgkfvp.html

TS:   JSON.stringify(obj)
来源：http://hz.cheryme.top/gtdwfazkok.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.chenzaomai.com/gtnvwvrnip.html

Go:   json.Marshal(obj)
来源：http://hz.ywan-chungtsiang.top/gtwxdwufvq.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hnxiangtu.top/gtkenewroy.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.9152youxi.cn/gtkbbtwqch.html

[K02] JSON 字符串转对象
来源：http://hz.zycfv.cn/gtzauzdbqs.html

Py:   json.loads(s)
来源：http://hz.bjfxy.top/gtimjyselp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.gaohongyu789.top/gtkhpwlagm.html

JS:   JSON.parse(s)
来源：http://hz.bjfxy.top/gtnupewype.html

TS:   JSON.parse(s)
来源：http://hz.nwbrower.top/gtvxqqzylk.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.mhx1999.top/gtlymetmse.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.aibaodan.cn/gtescilwmo.html

Ruby: JSON.parse(s)
来源：http://hz.cdnleiting.top/gtnnhknwbf.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.aizwys.cn/gtaozijjzq.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.andypj.xyz/gtlsfxmpxm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yongpay.top/gtcfhcqrvi.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jianghu66.top/gtyebrmyng.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.pengpengdd.cyou/gtntunaotz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.bjfxy.top/gtuezbamja.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zhoulong.xyz/gtsjxzyrum.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.wangdashe.top/gtnjferoob.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jlsjyb.cn/gtqefqpguj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhengqikj.top/gtnulpkwia.html

[K04] 读取 JSON 文件
来源：http://hz.bjfxy.top/gtdouqwymk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.c1oappe.top/gtqjklntph.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cdnleiting.top/gtcrndbmtb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yj20258888.top/gtwwnouefq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jyoumei.cn/gtyidvoibx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.meibo888.top/gtlzamfyto.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.meibo888.top/gtscxamxys.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.cashguo.top/gtcfyftvmy.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.xuanzx.com/gtrtzixvki.html

[K05] 深拷贝对象
来源：http://hz.jinyuanbaomall.cn/gtklpvtrtk.html

Py:   copy.deepcopy(obj)
来源：http://hz.52xcode.cn/gtcnumqiua.html

PHP:  unserialize(serialize($obj));
来源：http://hz.meibo888.top/gtfmzhjbjs.html

JS:   structuredClone(obj)
来源：http://hz.sufxvd.cn/gtqjywemlj.html

TS:   structuredClone(obj)
来源：http://hz.xziqi.cn/gttndziwjq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhaomingkeji.xyz/gtdpcvvfeb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.quarkkingdee.top/gtudroyqoy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yongpay.top/gtfsufqdyi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.gzhubu.top/gtpgseramt.html

[K06] 解析 URL 查询串
来源：http://hz.fengsongda.top/gtynugyove.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.svipenyu.cn/gthujdlhui.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhengqikj.top/gtnfmhvqag.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gotoacloud.top/gtahrwulqx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cqqwz.cn/gtvfoktrkc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yj20258.top/gtvlsnfpyl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.sxryk.cn/gtukooqilz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jqgfzy.top/gtdhyaskcv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jyoumei.cn/gtohojltju.html

[K07] 进制转换
来源：http://hz.tanke756.top/gtkmnyxpnf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yangfankeji.com/gtcxlfjtxj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhiwuduotai.top/gtyshemjwq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.redwolf501.top/gtleuwyjeo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.cucudq.cn/gtydmrvgfe.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.nanxuanxn.top/gtzhlyywgc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.gaohongyu789.top/gttubfmnhh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.nwbrower.top/gtelptjynw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.0kj1m.cn/gthlihqmgd.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.xuanzx.com/gtmjofmogv.html

Py:   pickle.dumps(obj)
来源：http://hz.c1oappe.top/gtnikzagmw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yj202588.top/gtpkmyuukw.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.feifeiyinyue.top/gtmnuhlyvr.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.c1oappe.top/gtlhnujusk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.shzxlz.cn/gtmcqlgkkc.html

Go:   encoding/gob
来源：http://hz.xziqi.cn/gtmvyihajg.html

Ruby: Marshal.dump(obj)
来源：http://hz.zycfv.cn/gtnswuvnmb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.svipenyu.cn/gtprzfnrhd.html

================================================================================
来源：http://hz.yj20258888.top/gtfkylzqxs.html

L. 网络请求
来源：http://hz.zhaomingkeji.xyz/gtzigxlhqv.html

================================================================================
来源：http://hz.cdnleiting.top/gtxkjaipph.html

[L01] 发送 GET 请求
来源：http://hz.shuidangran.top/gtxsfznqqi.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yj20258.top/gtctmocbmj.html


<!-- 参考信息 -->