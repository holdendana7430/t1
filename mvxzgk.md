代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jqgfzy.top/gtdotoeuxb.html

[H04] 自定义异常类型
来源：http://hz.yanxiufei.cn/gttkgqyjlm.html

Py:   class MyError(Exception): pass
来源：http://hz.shangyingyoupin.top/gtyhbtiqvb.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhaomingkeji.xyz/gtkpblqmmk.html

JS:   class MyError extends Error {}
来源：http://hz.jinqigfzy.top/gtxqtvhvto.html

TS:   class MyError extends Error {}
来源：http://hz.wangshuangyany.cn/gtsrhwhezc.html

Java: class MyException extends RuntimeException {}
来源：http://hz.nwbrower.top/gtewkogqeh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.iojbl.cn/gtcccsrxnu.html

Ruby: class MyError < StandardError; end
来源：http://hz.feifeiyinyue.top/gtjcruoyks.html

C#:   class MyException : Exception {}
来源：http://hz.tanke756.top/gtxsppthwk.html

[H05] 捕获特定类型
来源：http://hz.quarkkingdee.top/gtkwdfwynz.html

Py:   except ValueError as e:
来源：http://hz.kuanghao11.cn/gtzlijczxx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yj20258888.top/gtezxgoxhl.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.shanyushiyangtech.top/gtgvosfeez.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zycfv.cn/gtsdepqhmu.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yanxiufei.cn/gteikcvvtr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.chenjidiqi.icu/gtfxyqiitz.html

Ruby: rescue ArgumentError => e
来源：http://hz.xingfuxueyuan.xyz/gtfazbawzo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.svipenyu.cn/gtrwlutupf.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zdqjudy.top/gtcoleposs.html

Py:   value = d.get("k") or default
来源：http://hz.fengsongda.top/gtmtkvxrss.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zdqjudy.top/gtcfuebujo.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.cdnleiting.top/gtiafrswmc.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.tianlin.xyz/gtyeejpecz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yj202588.top/gtqppdgjyg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.0kj1m.cn/gtutusvkpr.html

Ruby: d&.dig(:a, :b)
来源：http://hz.c1oappe.top/gtdgjkjgcj.html

C#:   obj?.A?.B ?? default
来源：http://hz.yuanzhike.top/gtmiruopsy.html

[H07] 断言
来源：http://hz.jyoumei.cn/gtwozeqsaw.html

Py:   assert x > 0, "必须为正"
来源：http://hz.shanyushiyangkeji.top/gtxyycsdtp.html

PHP:  assert($x > 0);
来源：http://hz.hammf.cn/gtclffcqyr.html

JS:   console.assert(x > 0);
来源：http://hz.hongshengwenyu.top/gthmwmnviz.html

TS:   console.assert(x > 0);
来源：http://hz.xuanzx.com/gtuaabzmel.html

Java: assert x > 0 : "必须为正";
来源：http://hz.sweek.top/gtcdpyvlcg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.guowangkeji.top/gtqxpiclsg.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.bjfxy.top/gtiqkldcpg.html

C#:   Debug.Assert(x > 0);
来源：http://hz.sxryk.cn/gtrmmhosis.html

[H08] 获取错误信息与堆栈
来源：http://hz.hfpthk.cn/gtiervcaid.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.cucudq.cn/gtfdqgrzlf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.gogol.net.cn/gtyimnkhiq.html

JS:   e.message;  e.stack
来源：http://hz.jyoumei.cn/gttjfnhubg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.daxiang520.top/gtlhokqyih.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.52xcode.cn/gthtjyxtdq.html

Go:   err.Error()
来源：http://hz.cucudq.cn/gtpiuvdarc.html

Ruby: e.message;  e.backtrace
来源：http://hz.snrcjt.cn/gtuqojeuct.html

C#:   e.Message;  e.StackTrace
来源：http://hz.tian-w.cn/gtmaqfnyjq.html

[H09] 带错误码的异常
来源：http://hz.chenlongwang.top/gtwouxucng.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xylfe.cn/gtdubnmvqb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.daxiang520.top/gtkhrxwvid.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.gotoacloud.top/gthnocfkky.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.shuidangran.top/gttalsujdp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yongpay.top/gtcpqoujpk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.smart0.xyz/gttqxtujjp.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhixingplan.top/gtrkhbvtea.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.cucudq.cn/gttdvdlxku.html

[H10] 资源自动释放
来源：http://hz.hnxiangtu.top/gtaytelkgq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.nwbrower.top/gtpklsvdys.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ydzc1.top/gtlngelngr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ppjwa.cn/gtxexddfoy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj20258888.top/gtrthtslqo.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.feifeiyinyue.top/gtgdchhbmu.html

Go:   defer f.Close()
来源：http://hz.hysaishi.cn/gtjkihjhbx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.tanke756.top/gtddwjwtgy.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jinqigufen.top/gtgowvjztr.html

================================================================================
来源：http://hz.daxiang520.top/gtsbdyxhrr.html

I. 正则表达式
来源：http://hz.xingfuxueyuan.xyz/gtncxmfusk.html

================================================================================
来源：http://hz.sufxvd.cn/gtmlmdhvuf.html

[I01] 判断是否匹配
来源：http://hz.zhixingplan.top/gtltflmboc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hnqzz.top/gtmalfyyme.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.cashguo.top/gtvkgudvqu.html

JS:   /\d+/.test(s)
来源：http://hz.hfpthk.cn/gtuiqwbkbm.html

TS:   /\d+/.test(s)
来源：http://hz.ivvv.top/gtcbcwplmg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ywan-chungtsiang.top/gtoyytzqcy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.meibo888.top/gtxkeosyzs.html

Ruby: s.match?(/\d+/)
来源：http://hz.sufxvd.cn/gthalfmvon.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.mhx1999.top/gtbsqfiotb.html

[I02] 提取所有匹配
来源：http://hz.daxiang520.top/gtlrqnkxin.html

Py:   re.findall(r"\d+", s)
来源：http://hz.xuanzx.com/gtwtoccost.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hfpthk.cn/gtchykrubp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yongpay.top/gtzfrbylux.html

TS:   s.match(/\d+/g)
来源：http://hz.mhx1999.top/gtlwiegsva.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.kuanghao11.cn/gthlztxwnk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.birdmap.top/gtzkshfllp.html

Ruby: s.scan(/\d+/)
来源：http://hz.nanxuanxn.top/gtauvaoong.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ybcxt.top/gtipfxpwxk.html

[I03] 提取捕获分组
来源：http://hz.jinqigufen.top/gtvikmcfbx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.wangdashe.top/gtnmhgouzs.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.guowangkeji.top/gtchmvheed.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yangfankeji.com/gtnobketzo.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.sxryk.cn/gtqtiiknzx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.fzhhl.top/gtvcemxiaq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.9152youxi.cn/gtzdtgtclc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jinyuanbaomall.cn/gtfmolwprb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.fengsongda.top/gtwkbyzeli.html

[I04] 正则替换
来源：http://hz.sufxvd.cn/gttdevkaeb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.mhx1999.top/gtuhjbejvz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.shanyushiyangtech.top/gtuytomfmm.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ybcxt.top/gtezlrfseo.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yangfankeji.com/gtlpbrrbzf.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhongyouzk.top/gtnmpchiih.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.sxryk.cn/gtokdznlpg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.smart0.xyz/gtteetuwve.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.gotoacloud.top/gtfkspuiqg.html

[I05] 按正则拆分
来源：http://hz.cashguo.top/gtvbhluhhx.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.tian-w.cn/gtverpjois.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xinyue.icu/gtyzxwdikw.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ehwqpu.com/gtoaohehqb.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhiwuduotai.top/gtjvsrctug.html

Java: s.split("\\s*,\\s*")
来源：http://hz.gogol.net.cn/gtdualbjta.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yvedp.cn/gtvqlkpafr.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jinqigufen.top/gtbipgqdss.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.shzxlz.cn/gtackdwsgz.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.fengsongda.top/gtibizkduk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.chenjidiqi.icu/gtfcirfjht.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.fzhhl.top/gtntzromop.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.chenjidiqi.icu/gtqdvwsrdb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.smart0.xyz/gtofdclboq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.dianchejie.cn/gtkknffzjt.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.guannengcc.top/gthmuiuzbz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hfpthk.cn/gtyknjnvms.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hongshengwenyu.top/gttmqymzqe.html

[I07] 忽略大小写与多行模式
来源：http://hz.xziqi.cn/gtvukdahwg.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.meibo888.top/gtghqpkpgt.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.aizwys.cn/gtxgwwctds.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ppjwa.cn/gtsyrljvsi.html

TS:   /error/gim
来源：http://hz.yvedp.cn/gtktxqnpio.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jlsjyb.cn/gtsidlxwfs.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhiwuduotai.top/gttqgdvmmn.html

Ruby: s.scan(/error/i)
来源：http://hz.hfpthk.cn/gtzfvxrftm.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jqgfzy.top/gtlevliuof.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.pengpengdd.cyou/gtpsnbaawl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.c1oappe.top/gtfdnylaix.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.havefunace.top/gtujibiatv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.quarkkingdee.top/gtznewgnau.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.daxiang520.top/gtjpnxljmn.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.chenjidiqi.icu/gthrtxejuo.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jiagoushi.top/gtvqgfcrdz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.sysykeji.top/gtsdwqtzkc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.nanxinkj.top/gtmwvfllaf.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtlkkvaflk.html

J. 日期与时间
来源：http://hz.ivvv.top/gtxrzqevpp.html

================================================================================
来源：http://hz.jqgufenzy.top/gtphberhtz.html

[J01] 获取当前时间
来源：http://hz.redwolf501.top/gtbiqoxtyt.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ydjk.org.cn/gtnmvqxhlt.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jyoumei.cn/gtckksbmxk.html

JS:   new Date();  Date.now()
来源：http://hz.jinqigufen.top/gtezwlennw.html

TS:   new Date();  Date.now()
来源：http://hz.yuanzhike.top/gtoukyhsbc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.gogol.net.cn/gtqlqwcnxp.html

Go:   time.Now()
来源：http://hz.chenjidiqi.icu/gtbchaeset.html

Ruby: Time.now
来源：http://hz.yangfankeji.com/gttvpkyyqn.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.andypj.xyz/gtrwqoozho.html

[J02] 格式化输出
来源：http://hz.tianlin.xyz/gtafmnyicu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gogol.net.cn/gtxvenhuxd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.cqqwz.cn/gtgrwoamnu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ybcxt.top/gttvmjdggu.html

TS:   d.toISOString()
来源：http://hz.nanxuanxn.top/gtqftqhdls.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.316326.xyz/gtrnijezcs.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.shuidangran.top/gtnhyafrvq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj20258.top/gtqltfklpe.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhoulong.xyz/gtvgizhxer.html

[J03] 字符串解析为日期
来源：http://hz.ywan-chungtsiang.top/gtjszpecnt.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhijiandao.cn/gtxvebcxyt.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.chenlongwang.top/gtlcchvayi.html

JS:   new Date("2024-01-02")
来源：http://hz.chenjidiqi.icu/gtrsomyilg.html

TS:   new Date("2024-01-02")
来源：http://hz.jianghu66.top/gtwnpsukup.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.shangyingyoupin.top/gtntvjjypg.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jinyuanbaomall.cn/gtliqppxql.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.shanyushiyangtech.top/gtqmmakzry.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yonumen.top/gtpwrgrffq.html

[J04] 时间戳与日期互转
来源：http://hz.ydzc1.top/gtxdrcsoku.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.shuidangran.top/gtwmfvzydx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hysaishi.cn/gtvjctbtjd.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hywenlv.cn/gtcyeecpdy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.cashguo.top/gtfqyqryvl.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.daria6918.cn/gtzszgydhp.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.daria6918.cn/gtyndzvjbd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hongshengwenyu.top/gtqwkavlhh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.tanke756.top/gttwcypfzd.html

[J05] 时间加减（加 7 天）
来源：http://hz.hammf.cn/gtcrotfpgi.html

Py:   now + timedelta(days=7)
来源：http://hz.dashuyun.cn/gtoxyxccwx.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yj20258888.top/gtpzvihdpo.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.fzhhl.top/gtyuhwagbt.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shuidangran.top/gtxxvxeang.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.dashuyun.cn/gtbektxbpy.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zdqjudy.top/gtgwxvkode.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yueranfly.top/gtknwubvwi.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.shanyushiyangkeji.top/gtfnhqrrqv.html

[J06] 计算两时间之差
来源：http://hz.zhaomingkeji.xyz/gtzcgmtgub.html

Py:   (end - start).total_seconds()
来源：http://hz.xuetiantiany.cn/gtflxvgdzx.html

PHP:  $end->diff($start)->days;
来源：http://hz.hammf.cn/gtyvtvnqci.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhijiandao.cn/gtsxjfgbmt.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.dashuyun.cn/gtsolbqxbe.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.sxryk.cn/gtmuryunne.html

Go:   end.Sub(start).Hours()
来源：http://hz.ywan-chungtsiang.top/gtkxzdnlum.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jqgufenzy.top/gtywpadqfi.html

C#:   (end - start).TotalSeconds
来源：http://hz.haohaochexian.top/gtizoupowg.html

[J07] 比较两个日期
来源：http://hz.gzhubu.top/gtjisyjgex.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xylfe.cn/gtucwltoog.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhixingplan.top/gtrlcvayks.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258888.top/gtweolibib.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shanyushiyangkeji.top/gtcusgarzm.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.shzxlz.cn/gtkaqtvdxc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.daxiang520.top/gtejuuyjkw.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.fzhhl.top/gtstzclymi.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jinqigfzy.top/gtlcubrcef.html

[J08] 提取年月日与星期
来源：http://hz.bjfxy.top/gtsmwsqnmc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhixingplan.top/gtgffdzrzb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.shuidangran.top/gtcqxyoman.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.c1oappe.top/gtplsrogrg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hnxiangtu.top/gtorpglssq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ehwqpu.com/gtjbhvbnnr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.xuanzx.com/gtpqabwuod.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.iojbl.cn/gtlloqzbjk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.gotoacloud.top/gtjavibanc.html

[J09] 时区处理
来源：http://hz.svipenyu.cn/gticyqtgnv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zhengqikj.top/gtyhckkrmi.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yongpay.top/gtmwtbgqoe.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.vqdsnc.cn/gtxjsudxmi.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yvedp.cn/gtyzwbikpi.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.dianchejie.cn/gtufxinitk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.shanyushiyangtech.top/gtwjpczhxc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.chenlongwang.top/gtqwhcgcvz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.smart0.xyz/gtaglhjynz.html

[J10] 取今天 / 本月第一天
来源：http://hz.jinqigufen.top/gtdvzlsxsg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhiwuduotai.top/gthwxvsjcc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.meibo888.top/gtlhdbdbnj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.shanyushiyangtech.top/gtpxgslklk.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.sufxvd.cn/gtkrdgqolm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yueranfly.top/gtbhffvpvw.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.9152youxi.cn/gtgvyzoxyo.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhixingplan.top/gtbsomsbng.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.svipenyu.cn/gtsjmovvca.html

================================================================================
来源：http://hz.zhijiandao.cn/gtknckpmzv.html

K. JSON 与序列化
来源：http://hz.gotoacloud.top/gtrrfczacf.html

================================================================================
来源：http://hz.tanke756.top/gthmfxtbdk.html

[K01] 对象转 JSON 字符串
来源：http://hz.redwolf501.top/gtxebknuvn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jinqigufen.top/gtgrqwmhbu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.fzhhl.top/gtmxgxkfsq.html

JS:   JSON.stringify(obj)
来源：http://hz.ivvv.top/gtfpppkwdf.html

TS:   JSON.stringify(obj)
来源：http://hz.iojbl.cn/gtnvgufamn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.birdmap.top/gtmtvfbiwu.html

Go:   json.Marshal(obj)
来源：http://hz.shuidangran.top/gtdoswoeyi.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.quarkkingdee.top/gtvzonrohg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.fengsongda.top/gtydztdfps.html

[K02] JSON 字符串转对象
来源：http://hz.xziqi.cn/gtfgzdnnyx.html

Py:   json.loads(s)
来源：http://hz.ehwqpu.com/gtzmhqwyxy.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jiagoushi.top/gtvxcndwlv.html

JS:   JSON.parse(s)
来源：http://hz.meibo888.top/gtqtrlzcww.html

TS:   JSON.parse(s)
来源：http://hz.cashguo.top/gtfgtxulxh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jinqigfzy.top/gteioilcbo.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.c1oappe.top/gtsgiglsya.html

Ruby: JSON.parse(s)
来源：http://hz.yj202588.top/gthwvjfmyp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhijiandao.cn/gtrigbvtvx.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhoulong.xyz/gtdbmoalbn.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zdqjudy.top/gtgdirnlsv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yueranfly.top/gttimxsike.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shanyushiyangkeji.top/gtxunsuvsx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.gotoacloud.top/gtliaocgib.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yanxiufei.cn/gtlqudernp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hongshengwenyu.top/gtnlhgzkcy.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.gzhubu.top/gtyqaavvgf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jinqigfzy.top/gtmkjuclei.html

[K04] 读取 JSON 文件
来源：http://hz.jyoumei.cn/gtxeseamix.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.kuanghao11.cn/gtpokrvoqj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jiagoushi.top/gtxzzpfhnc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinqigfzy.top/gtvhqcwbwn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cqqwz.cn/gtrsjfajfw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ybcxt.top/gtzpxlihuv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.cqqwz.cn/gtdhvykmqm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhengqikj.top/gtkbcmarin.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.cheryme.top/gtbwznknes.html

[K05] 深拷贝对象
来源：http://hz.gzhubu.top/gtnkilmlzq.html

Py:   copy.deepcopy(obj)
来源：http://hz.nwbrower.top/gtldjyrcfb.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yj20258888.top/gtgakxhvoy.html

JS:   structuredClone(obj)
来源：http://hz.yj202588.top/gtmnpopksn.html

TS:   structuredClone(obj)
来源：http://hz.yangfankeji.com/gtpjjqmqaa.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jqgfzy.top/gtucltexqu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.52xcode.cn/gturfzzbod.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.sysykeji.top/gtxpokxapn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.dianchejie.cn/gtnmyvjzvy.html

[K06] 解析 URL 查询串
来源：http://hz.iojbl.cn/gtyldviixf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yuanzhike.top/gtvgtmnvhj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.mhx1999.top/gteurlowkf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.haohaochexian.top/gthchectfe.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.birdmap.top/gtdekuuret.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.xingfuxueyuan.xyz/gteajvonex.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhixingplan.top/gtfapkeqql.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.cdnleiting.top/gtgsrmgyyj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cqqwz.cn/gtqjaocwqf.html

[K07] 进制转换
来源：http://hz.jinqigfzy.top/gtmgfrivxu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.chenzaomai.com/gttnffblpz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.shuidangran.top/gtsshkiawa.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zdqjudy.top/gtuoxdnrwr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.dashuyun.cn/gtjjcroslu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jyoumei.cn/gtxmieppds.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.kuanghao11.cn/gtavntjnqq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.sxryk.cn/gtucwbsfaa.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yueranfly.top/gtxureacfg.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.hongshengwenyu.top/gtfbuwimuo.html

Py:   pickle.dumps(obj)
来源：http://hz.daria6918.cn/gtpttuzuib.html


<!-- 参考信息 -->