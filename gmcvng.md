代发 wailian999

Py:   value = d.get("k") or default
来源：http://hz.xziqi.cn/gtbweburxk.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.havefunace.top/gtmoliocji.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yj202588.top/gtydujicdp.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.chenzaomai.com/gtgqyogcra.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jinyuanbaomall.cn/gtxwxsubkz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jqgfzy.top/gtlbfyvtnk.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yvedp.cn/gtbreojfxv.html

C#:   obj?.A?.B ?? default
来源：http://hz.cashguo.top/gtngunqgkx.html

[H07] 断言
来源：http://hz.316326.xyz/gtzdpwkyzj.html

Py:   assert x > 0, "必须为正"
来源：http://hz.xylfe.cn/gtqfcogxdj.html

PHP:  assert($x > 0);
来源：http://hz.shanyushiyangtech.top/gtarduxadt.html

JS:   console.assert(x > 0);
来源：http://hz.pycfn.com/gtysvomkay.html

TS:   console.assert(x > 0);
来源：http://hz.andypj.xyz/gtpyesngpf.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yuanzhike.top/gtnyxmkjnt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.snrcjt.cn/gttwttxeui.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.dianchejie.cn/gtwcrbaknu.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhoulong.xyz/gtgqytkcce.html

[H08] 获取错误信息与堆栈
来源：http://hz.52xcode.cn/gtmhbtfcri.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.cdnleiting.top/gttzxuwfty.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zycfv.cn/gtzdzfmiuw.html

JS:   e.message;  e.stack
来源：http://hz.kuanghao11.cn/gtavmdjrcv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yuxming.cn/gtqlyodujw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.52xcode.cn/gtxbfumlgf.html

Go:   err.Error()
来源：http://hz.redwolf501.top/gtugiuhhti.html

Ruby: e.message;  e.backtrace
来源：http://hz.tian-w.cn/gtofsxvoyd.html

C#:   e.Message;  e.StackTrace
来源：http://hz.gaohongyu789.top/gtkwontjjt.html

[H09] 带错误码的异常
来源：http://hz.bjfxy.top/gtofcsivwc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xylfe.cn/gtoqtixpva.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.iojbl.cn/gtlacpgbyb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.guannengcc.top/gtppjjthyp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.sufxvd.cn/gtztfbajkl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yj20258888.top/gtiezlefjj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.snrcjt.cn/gtofraulon.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhixingplan.top/gtrurepczc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.meibo888.top/gtnwzmsbaq.html

[H10] 资源自动释放
来源：http://hz.xinyue.icu/gtwsrqwphh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.smart0.xyz/gtlyaclcqn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.dianchejie.cn/gtdxdobebx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sysykeji.top/gtupfhqwtr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.feifeiyinyue.top/gtccvufnyj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.pycfn.com/gtwoyyuwly.html

Go:   defer f.Close()
来源：http://hz.gaohongyu789.top/gtmrkfwfjl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xingfuxueyuan.xyz/gtlxrpzlyj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.0kj1m.cn/gtllhbtvwv.html

================================================================================
来源：http://hz.xylfe.cn/gtbkelcglf.html

I. 正则表达式
来源：http://hz.tian-w.cn/gtkqcijpcq.html

================================================================================
来源：http://hz.xinyue.icu/gtjisntjqu.html

[I01] 判断是否匹配
来源：http://hz.guannengcc.top/gtzrqevchr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hnxiangtu.top/gtjkkoyabw.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.feifeiyinyue.top/gtheaqckmp.html

JS:   /\d+/.test(s)
来源：http://hz.aizwys.cn/gtuwkyfvtm.html

TS:   /\d+/.test(s)
来源：http://hz.xingfuxueyuan.xyz/gtaqkaoxrj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhixingplan.top/gtoacghsta.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.cheryme.top/gtsuavufts.html

Ruby: s.match?(/\d+/)
来源：http://hz.fengsongda.top/gtgoxuegwk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.svipenyu.cn/gtskwmtlyc.html

[I02] 提取所有匹配
来源：http://hz.cashguo.top/gtpmqlivvd.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hammf.cn/gtdtmqkrmh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hfpthk.cn/gtjgxoujcn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.wangshuangyany.cn/gtukawxrjr.html

TS:   s.match(/\d+/g)
来源：http://hz.birdmap.top/gtskikbytv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yj20258.top/gtzpklkcfq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhixingplan.top/gtossoemev.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhoulong.xyz/gtfzksxyqb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zhiwuduotai.top/gtgpqrdykn.html

[I03] 提取捕获分组
来源：http://hz.sysykeji.top/gtdonlhldn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.chenjidiqi.icu/gtsgknjspi.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.chenlongwang.top/gtrvpvlfta.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.tian-w.cn/gtmullogkx.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhiwuduotai.top/gtekkackkm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zdqjudy.top/gtkjvlmrsw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hysaishi.cn/gtlxrmsxew.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.cucudq.cn/gtobauctgn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yueranfly.top/gtendfvffc.html

[I04] 正则替换
来源：http://hz.snrcjt.cn/gtloqwvzqp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hfpthk.cn/gtozkesivi.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jlsjyb.cn/gtgqxmbalw.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yj20258.top/gtwncqalbg.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.ywan-chungtsiang.top/gtpiyygtkf.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yonumen.top/gtjrvosrvf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.guannengcc.top/gtfavvpgke.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.xuetiantiany.cn/gtrflcsseh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.sxryk.cn/gtoyxkzgaa.html

[I05] 按正则拆分
来源：http://hz.zhiwuduotai.top/gtytbhrmvm.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hnqzz.top/gtfzmxaokp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.chenlongwang.top/gtcpwwncul.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zhoulong.xyz/gtotufiwnc.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.iojbl.cn/gtahknefky.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jqgufenzy.top/gtkpcxsfzf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ywan-chungtsiang.top/gtfuanioyl.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jinqigfzy.top/gthysmxcov.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.daxiang520.top/gthckgmdwa.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.aizwys.cn/gthoxxnbus.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.cdnleiting.top/gtsmvcknbh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.cucudq.cn/gtjwgqqgrp.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.snrcjt.cn/gtajeuzxss.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cqqwz.cn/gtosmgmxvt.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yongpay.top/gthzqfiavv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jqgufenzy.top/gtonsvcyqc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.gogol.net.cn/gtsoqcvovb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yongpay.top/gtlxwuczyn.html

[I07] 忽略大小写与多行模式
来源：http://hz.hfpthk.cn/gtvvwxvxfc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zhoulong.xyz/gtkjnrfxpk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhengqikj.top/gtdpqurmkg.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.quarkkingdee.top/gtjjeumxdk.html

TS:   /error/gim
来源：http://hz.cashguo.top/gtvhtrxlqh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.vqdsnc.cn/gtmhplbpni.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hfpthk.cn/gtqsjtfpee.html

Ruby: s.scan(/error/i)
来源：http://hz.nanxinkj.top/gtemcukkdw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.52xcode.cn/gtdlnyadim.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.chenjidiqi.icu/gtkxynfzns.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yj20258888.top/gtzcubkmzg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jinqigfzy.top/gtnrnnlrxw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ybcxt.top/gteqseyqnu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xinyue.icu/gtatgofsiy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hysaishi.cn/gtrgtjxhhz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.havefunace.top/gtwgcfbgug.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.dashuyun.cn/gtvswgucki.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.cucudq.cn/gtdwroxwpi.html

================================================================================
来源：http://hz.jiagoushi.top/gtcvbiaevo.html

J. 日期与时间
来源：http://hz.jianghu66.top/gtxogprvxr.html

================================================================================
来源：http://hz.tian-w.cn/gtnvdqhtil.html

[J01] 获取当前时间
来源：http://hz.jyoumei.cn/gtpmrdedaa.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.tian-w.cn/gtdzzhymqj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.sweek.top/gtvcecwsrg.html

JS:   new Date();  Date.now()
来源：http://hz.ybcxt.top/gtgdbfoyyx.html

TS:   new Date();  Date.now()
来源：http://hz.fengsongda.top/gtegxoqiez.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.guowangkeji.top/gtvrtdwlag.html

Go:   time.Now()
来源：http://hz.yuxming.cn/gtcdykjonm.html

Ruby: Time.now
来源：http://hz.svipenyu.cn/gtccryszhj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.daxiang520.top/gtmlccpqoo.html

[J02] 格式化输出
来源：http://hz.ywan-chungtsiang.top/gtioedsjwo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.aibaodan.cn/gtzqnteyhp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.chenlongwang.top/gtcwskjrux.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xuetiantiany.cn/gtcdgliifp.html

TS:   d.toISOString()
来源：http://hz.tanke756.top/gtizoauhhr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jqgufenzy.top/gtwdjeyite.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhongyouzk.top/gtvhhkiulf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.snrcjt.cn/gtvrxlifsr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.daria6918.cn/gtqtxellon.html

[J03] 字符串解析为日期
来源：http://hz.smart0.xyz/gtbquecykc.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.fengsongda.top/gtvtmsigto.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.nanxuanxn.top/gtmnxrxqkw.html

JS:   new Date("2024-01-02")
来源：http://hz.zdqjudy.top/gtgsittoal.html

TS:   new Date("2024-01-02")
来源：http://hz.shangyingyoupin.top/gtzijjuovv.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hammf.cn/gtofodpqqf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yj20258888.top/gtbzuhdxlk.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jiagoushi.top/gtchtpfdpk.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jqgfzy.top/gtppwyjwcx.html

[J04] 时间戳与日期互转
来源：http://hz.shanyushiyangkeji.top/gtjdqfdmlh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.ydjk.org.cn/gtiorvfizb.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.havefunace.top/gtchaunwxj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.daxiang520.top/gtwsvtlqid.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.shanyushiyangkeji.top/gtyjmjpskd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.sxryk.cn/gturrflkpz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhixingplan.top/gtoyojrmjc.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.wangshuangyany.cn/gtlmrhbnpj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.dashuyun.cn/gthkkutjvl.html

[J05] 时间加减（加 7 天）
来源：http://hz.ydjk.org.cn/gtdndyrldr.html

Py:   now + timedelta(days=7)
来源：http://hz.ydjk.org.cn/gtiedhiiuc.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.wangshuangyany.cn/gtdruszpss.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinqigufen.top/gtduusmewk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hnxiangtu.top/gtejvrlpvd.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.wangshuangyany.cn/gtmocsggcz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xuanzx.com/gtmkepvhdo.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jyoumei.cn/gthctxicoh.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.c1oappe.top/gtlkflfwwg.html

[J06] 计算两时间之差
来源：http://hz.cashguo.top/gtsbjpbvfm.html

Py:   (end - start).total_seconds()
来源：http://hz.ivvv.top/gtsmflauyd.html

PHP:  $end->diff($start)->days;
来源：http://hz.pengpengdd.cyou/gtqrwtpgco.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ydjk.org.cn/gtddocihds.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.guowangkeji.top/gtbosvupcb.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jlsjyb.cn/gtpaepbobe.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhijiandao.cn/gtwzgnlejb.html

Ruby: end - start                 # 返回秒数
来源：http://hz.daxiang520.top/gtarzvcljk.html

C#:   (end - start).TotalSeconds
来源：http://hz.dianchejie.cn/gtmryzvpoi.html

[J07] 比较两个日期
来源：http://hz.zhengqikj.top/gtfpiqjwvp.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.meibo888.top/gtqmjfxfdl.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.sweek.top/gttewpmfjv.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yongpay.top/gtonfoppua.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhengqikj.top/gtkuysdqcj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yvedp.cn/gtcilfklqe.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.daria6918.cn/gtpxhsgyna.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.sysykeji.top/gtyiyqpaqd.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.pengpengdd.cyou/gtvihwjgsr.html

[J08] 提取年月日与星期
来源：http://hz.snrcjt.cn/gtzpzpqqap.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.sxryk.cn/gtvgggeyqz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hnqzz.top/gtdqzuolxv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.cucudq.cn/gtgwqwjnys.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.gogol.net.cn/gtzcqjfici.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.quarkkingdee.top/gtfpwsikab.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.tanke756.top/gtrsipjtlw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.feifeiyinyue.top/gtozgrutuw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.shuidangran.top/gtkwwpjlow.html

[J09] 时区处理
来源：http://hz.meibo888.top/gttsytureg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shanyushiyangtech.top/gtzifdxxup.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.gaohongyu789.top/gtbcjtxgoz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yonumen.top/gtlrqrkeof.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ehwqpu.com/gtretxwqjl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.iojbl.cn/gthhvdphgn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hnqzz.top/gtnegsunzm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.shuidangran.top/gtbpbanmnw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yuxming.cn/gtolayinkt.html

[J10] 取今天 / 本月第一天
来源：http://hz.jiagoushi.top/gtzvouqlsc.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.xingfuxueyuan.xyz/gtyxqztvmu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jqgufenzy.top/gtbjjpewcl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.dashuyun.cn/gtgedmdjul.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.pycfn.com/gtbidlyckm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jinqigufen.top/gtmitlskiy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hysaishi.cn/gtxltlibcm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ybcxt.top/gtmjoqbeik.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.nanxinkj.top/gtbtgxwssv.html

================================================================================
来源：http://hz.snrcjt.cn/gtgwtwachu.html

K. JSON 与序列化
来源：http://hz.jinghuilouyu.cn/gthcukkfzs.html

================================================================================
来源：http://hz.chenzaomai.com/gtnxxogzpg.html

[K01] 对象转 JSON 字符串
来源：http://hz.nanxuanxn.top/gtymruamir.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zycfv.cn/gtmbyupzqr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xuetiantiany.cn/gtybpjidoj.html

JS:   JSON.stringify(obj)
来源：http://hz.shanyushiyangkeji.top/gtepxewsmh.html

TS:   JSON.stringify(obj)
来源：http://hz.zhiwuduotai.top/gtrqyvmsia.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hammf.cn/gtnfweozvm.html

Go:   json.Marshal(obj)
来源：http://hz.yj20258.top/gtsipxuzux.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jqgfzy.top/gtxuikyyhi.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yangfankeji.com/gtzfjtjgkw.html

[K02] JSON 字符串转对象
来源：http://hz.dashuyun.cn/gtsgkvckqz.html

Py:   json.loads(s)
来源：http://hz.nanxinkj.top/gtrcyimtgz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.snrcjt.cn/gtodzksuqq.html

JS:   JSON.parse(s)
来源：http://hz.hongshengwenyu.top/gtakmxolaz.html

TS:   JSON.parse(s)
来源：http://hz.gogol.net.cn/gtjpiwfrfj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.guowangkeji.top/gtjujaixgn.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhixingplan.top/gtvglfzwah.html

Ruby: JSON.parse(s)
来源：http://hz.quarkkingdee.top/gtdzixrjxo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.aibaodan.cn/gtbtjafcoj.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.tian-w.cn/gtfujitqtf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhaomingkeji.xyz/gtzalghebz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhixingplan.top/gteetrdgsb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jiagoushi.top/gtenfalswi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.chenzaomai.com/gtfqswjbhw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.xingfuxueyuan.xyz/gtuyjmphfu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.nanxuanxn.top/gtgfdiwvax.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yangfankeji.com/gtplivbaqi.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ywan-chungtsiang.top/gtszsrneoy.html

[K04] 读取 JSON 文件
来源：http://hz.hnxiangtu.top/gthouscohj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xuanzx.com/gtnfsbrqfo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jinqigufen.top/gtozfmddwc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gotoacloud.top/gtvvpehnce.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cashguo.top/gtxguxjhdz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.chenzaomai.com/gtbndndpld.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.pengpengdd.cyou/gtibdqxqxg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.c1oappe.top/gtmwefrazt.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.gotoacloud.top/gtbgixcaan.html

[K05] 深拷贝对象
来源：http://hz.tanke756.top/gtamosenpg.html

Py:   copy.deepcopy(obj)
来源：http://hz.jinghuilouyu.cn/gtswipacvi.html

PHP:  unserialize(serialize($obj));
来源：http://hz.shanyushiyangkeji.top/gtinafslxk.html

JS:   structuredClone(obj)
来源：http://hz.tanke756.top/gtxyagtxtk.html

TS:   structuredClone(obj)
来源：http://hz.jqgufenzy.top/gtaydsatht.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jinghuilouyu.cn/gtrlinmvdu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yongpay.top/gtrizhniju.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.tian-w.cn/gtxczqmidp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.sysykeji.top/gtlfaqufli.html

[K06] 解析 URL 查询串
来源：http://hz.tian-w.cn/gtluknwfnc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.fengsongda.top/gtnlurpqji.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yj20258.top/gtlyfwwigq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.daxiang520.top/gtsylknknx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cdnleiting.top/gtedznntpm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yueranfly.top/gtvxdkezdp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.wangshuangyany.cn/gtquttqwlc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.redwolf501.top/gtmnvwsjdl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yanxiufei.cn/gtfglfyvef.html

[K07] 进制转换
来源：http://hz.wangshuangyany.cn/gtgubmritt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.c1oappe.top/gtjygbhjuw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jianghu66.top/gtpsnevipb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.gaohongyu789.top/gtdggqxxas.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.dianchejie.cn/gtlshqvudz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.quarkkingdee.top/gtpzobutha.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.52xcode.cn/gtemzkpcts.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yonumen.top/gtmnegygji.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.gogol.net.cn/gtwolyotdu.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.xuetiantiany.cn/gtyueoksij.html

Py:   pickle.dumps(obj)
来源：http://hz.shuidangran.top/gtnbwnfirf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.gaohongyu789.top/gtkhixafrx.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hywenlv.cn/gtgwzizwqk.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.havefunace.top/gtrtgsjumu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.chenzaomai.com/gtbprrwlsg.html

Go:   encoding/gob
来源：http://hz.hnxiangtu.top/gtxvveerda.html

Ruby: Marshal.dump(obj)
来源：http://hz.ivvv.top/gtmfdjnhda.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.fengsongda.top/gtohiuvnqv.html

================================================================================
来源：http://hz.fengsongda.top/gtbvhxfjhn.html

L. 网络请求
来源：http://hz.snrcjt.cn/gtxfkqjqcq.html

================================================================================
来源：http://hz.bjfxy.top/gtpbtubhxy.html

[L01] 发送 GET 请求
来源：http://hz.shangyingyoupin.top/gtgupiwcyy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.chenzaomai.com/gtdjvrxvby.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jiagoushi.top/gtcycietdu.html

JS:   await fetch(url)
来源：http://hz.0kj1m.cn/gtnuellsmq.html

TS:   await fetch(url)
来源：http://hz.hnxiangtu.top/gtsbhufbpe.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.nanxuanxn.top/gthatbwncu.html

Go:   resp, err := http.Get(url)
来源：http://hz.jinyuanbaomall.cn/gtmvnckmos.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.daria6918.cn/gtcbfzeihz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yvedp.cn/gtktdpxroh.html

[L02] 发送 POST JSON
来源：http://hz.chenzaomai.com/gtqrkkljsi.html


<!-- 参考信息 -->