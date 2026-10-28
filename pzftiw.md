代发 wailian999

JS:   class MyError extends Error {}
来源：http://hz.316326.xyz/gtjwbooolt.html

TS:   class MyError extends Error {}
来源：http://hz.ehwqpu.com/gtqzdegmez.html

Java: class MyException extends RuntimeException {}
来源：http://hz.sweek.top/gtnftkxaob.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.feifeiyinyue.top/gtnseohksu.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhixingplan.top/gtiuoipytv.html

C#:   class MyException : Exception {}
来源：http://hz.smart0.xyz/gtintrrnyz.html

[H05] 捕获特定类型
来源：http://hz.andypj.xyz/gtzugynhye.html

Py:   except ValueError as e:
来源：http://hz.jinghuilouyu.cn/gtnztrhbhf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hywenlv.cn/gtcwvdarxc.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.shanyushiyangtech.top/gtnbwbdsfc.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.fengsongda.top/gtdpryraij.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhaomingkeji.xyz/gtmvjihmwm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.fzhhl.top/gtrcocnaxh.html

Ruby: rescue ArgumentError => e
来源：http://hz.hongshengwenyu.top/gtxayehgoq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jianghu66.top/gtrasisxlo.html

[H06] 可选值 / 空值安全访问
来源：http://hz.9152youxi.cn/gtdfcyvkbr.html

Py:   value = d.get("k") or default
来源：http://hz.yj202588.top/gthixpripl.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.52xcode.cn/gtmxvwyskz.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yvedp.cn/gtjbcdshgm.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jinqigfzy.top/gtjxmowewz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hywenlv.cn/gtknxgardb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jinghuilouyu.cn/gtcueqzmtd.html

Ruby: d&.dig(:a, :b)
来源：http://hz.pycfn.com/gtxajvhmbt.html

C#:   obj?.A?.B ?? default
来源：http://hz.jlsjyb.cn/gthlipzgrc.html

[H07] 断言
来源：http://hz.wangshuangyany.cn/gtkrygzkud.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jiagoushi.top/gtkmedxxny.html

PHP:  assert($x > 0);
来源：http://hz.xuetiantiany.cn/gtkltjwwdj.html

JS:   console.assert(x > 0);
来源：http://hz.gzhubu.top/gtcfjhzpsl.html

TS:   console.assert(x > 0);
来源：http://hz.zdqjudy.top/gtmaozexsz.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yj20258888.top/gtitzhuxiy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.cqqwz.cn/gtipotdikg.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yanxiufei.cn/gtgqaahlal.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jinyuanbaomall.cn/gtuynhxdqh.html

[H08] 获取错误信息与堆栈
来源：http://hz.havefunace.top/gtdkszlvmf.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jqgfzy.top/gttbkzkvmn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ehwqpu.com/gtrfcmthie.html

JS:   e.message;  e.stack
来源：http://hz.zdqjudy.top/gtdafvlzbc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yj202588.top/gtqjzzakxr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yanxiufei.cn/gtiqatddvc.html

Go:   err.Error()
来源：http://hz.ivvv.top/gtdiwndsei.html

Ruby: e.message;  e.backtrace
来源：http://hz.shangyingyoupin.top/gtghceajqy.html

C#:   e.Message;  e.StackTrace
来源：http://hz.daria6918.cn/gtgsmqcwmj.html

[H09] 带错误码的异常
来源：http://hz.redwolf501.top/gtjflbzydy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.sysykeji.top/gtoweyqxwt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jyoumei.cn/gtwsavdnbc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.mhx1999.top/gtfzrocyfa.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jinghuilouyu.cn/gtwsnadica.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jyoumei.cn/gtcqagdwsw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hongshengwenyu.top/gtkdwxathv.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.daxiang520.top/gtmrrtlgzc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yj20258.top/gtglmivmgm.html

[H10] 资源自动释放
来源：http://hz.jinqigfzy.top/gtllvbalja.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.mhx1999.top/gtksyjkzns.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.guannengcc.top/gtecwvxahj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.quarkkingdee.top/gtmmvzebkv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ppjwa.cn/gtzqtqqimz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jlsjyb.cn/gtsbguqlws.html

Go:   defer f.Close()
来源：http://hz.cdnleiting.top/gtdrearqrh.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.tanke756.top/gthkgqasja.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yongpay.top/gtixgkcqgy.html

================================================================================
来源：http://hz.jinqigfzy.top/gtsovlxmea.html

I. 正则表达式
来源：http://hz.svipenyu.cn/gtbyjyovyn.html

================================================================================
来源：http://hz.yonumen.top/gtloemgytz.html

[I01] 判断是否匹配
来源：http://hz.hywenlv.cn/gtedkciaip.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xylfe.cn/gttdlcbbmt.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.sysykeji.top/gtosqdqaxe.html

JS:   /\d+/.test(s)
来源：http://hz.hnqzz.top/gttuhyxami.html

TS:   /\d+/.test(s)
来源：http://hz.zhijiandao.cn/gtlmvybqsu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhengqikj.top/gtvfiasrnf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.daxiang520.top/gtrwzecszc.html

Ruby: s.match?(/\d+/)
来源：http://hz.xingfuxueyuan.xyz/gtlcngvwcd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.nanxuanxn.top/gtnpejnwrq.html

[I02] 提取所有匹配
来源：http://hz.zhiwuduotai.top/gtnsfqsswy.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ywan-chungtsiang.top/gtxdteuupt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yj202588.top/gtcnkltikj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.ppjwa.cn/gtzhaiyeko.html

TS:   s.match(/\d+/g)
来源：http://hz.nanxinkj.top/gtxsbrelqk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.havefunace.top/gtqndchwak.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xziqi.cn/gtjfcvcdli.html

Ruby: s.scan(/\d+/)
来源：http://hz.xylfe.cn/gtugfgqhzb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.dashuyun.cn/gtwejryvab.html

[I03] 提取捕获分组
来源：http://hz.cucudq.cn/gtwwghfekw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.daria6918.cn/gthmlduaed.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hysaishi.cn/gtyvsjlaep.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.vqdsnc.cn/gttkwblbcu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.sufxvd.cn/gtjnpcdwxs.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.snrcjt.cn/gthgieivhy.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhaomingkeji.xyz/gtfhsfcvwy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.sysykeji.top/gtmgyfpnys.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhixingplan.top/gtroogdqui.html

[I04] 正则替换
来源：http://hz.yj20258888.top/gtqypczijn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jianghu66.top/gtquukgxxj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.dianchejie.cn/gtlfsacfwc.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.andypj.xyz/gtqhjthdgx.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xuanzx.com/gtzbrehdae.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.shzxlz.cn/gtvffhkgwa.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jlsjyb.cn/gtukwalnbw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.dianchejie.cn/gtjrvzbwua.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.xuanzx.com/gtgzzitnrf.html

[I05] 按正则拆分
来源：http://hz.52xcode.cn/gtaksuakle.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.0kj1m.cn/gtwyktthpm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.cqqwz.cn/gtxjgklpca.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.sxryk.cn/gthxjlsjyq.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.daxiang520.top/gtgsmantna.html

Java: s.split("\\s*,\\s*")
来源：http://hz.iojbl.cn/gtkmrcictq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ivvv.top/gtklfrbelq.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhengqikj.top/gtgvflhebt.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.cashguo.top/gteqtzzyrt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xinyue.icu/gtmsfobsmy.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.guowangkeji.top/gtvrwrtgjr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jlsjyb.cn/gtzpmkeakp.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ydjk.org.cn/gtksdkillt.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zdqjudy.top/gtdhfbnfqu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zdqjudy.top/gtepttknda.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ydzc1.top/gtyyqujkcb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.snrcjt.cn/gtehnwxdjb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.dashuyun.cn/gtqrwdstpd.html

[I07] 忽略大小写与多行模式
来源：http://hz.jinyuanbaomall.cn/gtesvjtyyj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.haohaochexian.top/gtuwgyvjiq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.sufxvd.cn/gtivrnkkrt.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.aibaodan.cn/gtmvisetso.html

TS:   /error/gim
来源：http://hz.shangyingyoupin.top/gtkskvozxx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.iojbl.cn/gtcnkwocdo.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yj202588.top/gtuxftraee.html

Ruby: s.scan(/error/i)
来源：http://hz.shanyushiyangkeji.top/gtjoycieud.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xuanzx.com/gthklpmhnc.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hysaishi.cn/gtvymevofc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ydzc1.top/gtdnhyavdc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yanxiufei.cn/gtqoteackz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.pengpengdd.cyou/gtaukhelie.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.guannengcc.top/gtageblvlv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jinyuanbaomall.cn/gtrxegqgxv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xingfuxueyuan.xyz/gttmmhrnap.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hammf.cn/gtdjzawgus.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.fengsongda.top/gtxiibucmw.html

================================================================================
来源：http://hz.xylfe.cn/gttkklfvrt.html

J. 日期与时间
来源：http://hz.aibaodan.cn/gtquztzqbm.html

================================================================================
来源：http://hz.quarkkingdee.top/gtgkkrfgml.html

[J01] 获取当前时间
来源：http://hz.0kj1m.cn/gttzpdnmvk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.chenjidiqi.icu/gtisyvooet.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.aizwys.cn/gtfrxvxyau.html

JS:   new Date();  Date.now()
来源：http://hz.zhengqikj.top/gtmcbdiivf.html

TS:   new Date();  Date.now()
来源：http://hz.svipenyu.cn/gtipfgldwy.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ppjwa.cn/gtsueocvsg.html

Go:   time.Now()
来源：http://hz.snrcjt.cn/gtoeohyfvf.html

Ruby: Time.now
来源：http://hz.cheryme.top/gtrltfpjbr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.chenzaomai.com/gtqrynwtfv.html

[J02] 格式化输出
来源：http://hz.ywan-chungtsiang.top/gtqkvvgldq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cheryme.top/gtqcksvjau.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.sxryk.cn/gtbhuwhnhp.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.wangshuangyany.cn/gtcmiukggk.html

TS:   d.toISOString()
来源：http://hz.snrcjt.cn/gtijmurlsd.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.feifeiyinyue.top/gtftjwflhh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.xingfuxueyuan.xyz/gtzkxogffn.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nanxinkj.top/gtgzlvsyei.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.ivvv.top/gtfuepixfx.html

[J03] 字符串解析为日期
来源：http://hz.hywenlv.cn/gtrgevqslh.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yj202588.top/gtrwjrbkmo.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.sufxvd.cn/gtonbbhjdo.html

JS:   new Date("2024-01-02")
来源：http://hz.jqgfzy.top/gtzqjuryki.html

TS:   new Date("2024-01-02")
来源：http://hz.jinqigufen.top/gtaydvsexx.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yvedp.cn/gtkafpnpkr.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hnqzz.top/gtdurhjrqm.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhoulong.xyz/gtuyagkqrl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.nwbrower.top/gtiigvgefg.html

[J04] 时间戳与日期互转
来源：http://hz.meibo888.top/gtuicwnfdu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.gzhubu.top/gtxjhqbexu.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xziqi.cn/gtatfwylga.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ywan-chungtsiang.top/gtxragysfu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.nwbrower.top/gtwojfnuza.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ydzc1.top/gtkfiqqzlz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yj20258888.top/gtvimritgy.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jinqigufen.top/gthjduqcho.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.guannengcc.top/gtbjsttzbd.html

[J05] 时间加减（加 7 天）
来源：http://hz.hysaishi.cn/gtsndzhqrt.html

Py:   now + timedelta(days=7)
来源：http://hz.9152youxi.cn/gtfjvvcwsh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zhixingplan.top/gtibrbneum.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sysykeji.top/gtyzlilxeg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.iojbl.cn/gtvxkqwkue.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.shanyushiyangkeji.top/gtdzczblri.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.aibaodan.cn/gtbsrmruha.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jinqigufen.top/gtxtzokrte.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.meibo888.top/gteemssgxz.html

[J06] 计算两时间之差
来源：http://hz.nanxinkj.top/gtavntsvcd.html

Py:   (end - start).total_seconds()
来源：http://hz.nanxinkj.top/gtbedspuiv.html

PHP:  $end->diff($start)->days;
来源：http://hz.wangdashe.top/gtepafumqn.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.quarkkingdee.top/gtovinxyku.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.cheryme.top/gtdardytug.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.gaohongyu789.top/gtxghvxqsp.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhaomingkeji.xyz/gtcuamjtgf.html

Ruby: end - start                 # 返回秒数
来源：http://hz.cheryme.top/gtbcmmajzi.html

C#:   (end - start).TotalSeconds
来源：http://hz.snrcjt.cn/gthpzfsmpm.html

[J07] 比较两个日期
来源：http://hz.kuanghao11.cn/gtxuhlfrep.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.fengsongda.top/gtznmgwzcf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ybcxt.top/gtlentbcou.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yj202588.top/gtzhnliwsj.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jinghuilouyu.cn/gtxenclwiy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.dashuyun.cn/gtaiqejkkd.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.dashuyun.cn/gtlzfmvzov.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yj20258.top/gtlgnljyag.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.c1oappe.top/gtxxirdbie.html

[J08] 提取年月日与星期
来源：http://hz.hammf.cn/gtkuoiebkg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ywan-chungtsiang.top/gttvmqgxej.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.shanyushiyangtech.top/gtgvzemmfv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yuxming.cn/gtiffrsroi.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jlsjyb.cn/gtonbbijui.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhixingplan.top/gtcbxwvpas.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ehwqpu.com/gtsquomhwe.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.havefunace.top/gtnsscadtf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.shangyingyoupin.top/gtcpnphgod.html

[J09] 时区处理
来源：http://hz.andypj.xyz/gtbvoruoor.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yangfankeji.com/gtcelywnnb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jqgufenzy.top/gtxabdipjs.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.aizwys.cn/gthewbxoza.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinghuilouyu.cn/gtwadnyznw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hywenlv.cn/gtbksxvlmo.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.gzhubu.top/gtrulleqld.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jianghu66.top/gtmnyggnzd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.bjfxy.top/gtsuxrgzdp.html

[J10] 取今天 / 本月第一天
来源：http://hz.yuxming.cn/gtcusvhnxy.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.daria6918.cn/gtfdslolap.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xingfuxueyuan.xyz/gtmsnvodeg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.pycfn.com/gthmzueeas.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.shangyingyoupin.top/gtnvingcdq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.fzhhl.top/gtbejfgfwz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.feifeiyinyue.top/gtnobegknp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhaomingkeji.xyz/gtfhvyioqi.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.shanyushiyangtech.top/gtazcxqulp.html

================================================================================
来源：http://hz.dianchejie.cn/gtlvbxhyam.html

K. JSON 与序列化
来源：http://hz.guowangkeji.top/gtcccxgthh.html

================================================================================
来源：http://hz.aibaodan.cn/gtsofrbviy.html

[K01] 对象转 JSON 字符串
来源：http://hz.andypj.xyz/gtfhqlwqsz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jyoumei.cn/gtpllinvzt.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.daxiang520.top/gtkjjvwwfj.html

JS:   JSON.stringify(obj)
来源：http://hz.sysykeji.top/gtxgdhzouw.html

TS:   JSON.stringify(obj)
来源：http://hz.yangfankeji.com/gtgbzjszja.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hfpthk.cn/gtzvdeukdl.html

Go:   json.Marshal(obj)
来源：http://hz.52xcode.cn/gtyxnqgocm.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yanxiufei.cn/gtbomtsoit.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jinyuanbaomall.cn/gtswvbbyug.html

[K02] JSON 字符串转对象
来源：http://hz.ywan-chungtsiang.top/gtspaojpcx.html

Py:   json.loads(s)
来源：http://hz.wangdashe.top/gtaxayktpc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.havefunace.top/gtyqizhvtd.html

JS:   JSON.parse(s)
来源：http://hz.zhoulong.xyz/gtcpziufcp.html

TS:   JSON.parse(s)
来源：http://hz.birdmap.top/gtcxznaxcf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.cqqwz.cn/gtflfrztwg.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jinqigufen.top/gtakuvondr.html

Ruby: JSON.parse(s)
来源：http://hz.hysaishi.cn/gtouoqtrxo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.tian-w.cn/gtlpvwttkp.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.bjfxy.top/gtmbbgplbu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yvedp.cn/gttyxbxpzs.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ybcxt.top/gtbjdanlcm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shanyushiyangkeji.top/gtwefhgonf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.9152youxi.cn/gtsrlgdngc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.havefunace.top/gtizvgmrkc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ppjwa.cn/gtcvoolvjb.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.nanxinkj.top/gtjivmfctc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yangfankeji.com/gtialozffq.html

[K04] 读取 JSON 文件
来源：http://hz.hnqzz.top/gtupbtgcmz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xinyue.icu/gtbndhewqu.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cheryme.top/gtwsxtzrzu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xylfe.cn/gtiasxiqdn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.guowangkeji.top/gttmoftmws.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.pycfn.com/gttpkdmvgw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.chenlongwang.top/gtcpxmemzi.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.shangyingyoupin.top/gtcojbjpfy.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.gzhubu.top/gtdektoghl.html

[K05] 深拷贝对象
来源：http://hz.cucudq.cn/gtirelpger.html

Py:   copy.deepcopy(obj)
来源：http://hz.ivvv.top/gtswhtjpxx.html

PHP:  unserialize(serialize($obj));
来源：http://hz.fzhhl.top/gtzvfgcbze.html

JS:   structuredClone(obj)
来源：http://hz.yueranfly.top/gtjbzytpnx.html

TS:   structuredClone(obj)
来源：http://hz.shzxlz.cn/gtjgxpysjr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.shanyushiyangkeji.top/gtojbzgsey.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.dashuyun.cn/gtxmwyxpeh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jqgufenzy.top/gtsxuoqqeh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.fengsongda.top/gtkkleiiaw.html

[K06] 解析 URL 查询串
来源：http://hz.cqqwz.cn/gtkiwjfoju.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.chenzaomai.com/gthjcfslsc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.quarkkingdee.top/gtidxxfats.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shanyushiyangtech.top/gtovicqmyv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinqigufen.top/gtnhxndgeg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.xinyue.icu/gtbdjvhyvx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zdqjudy.top/gtxlrxstpj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yvedp.cn/gtsvjrpisb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.shuidangran.top/gtgmjqnbmh.html

[K07] 进制转换
来源：http://hz.zhongyouzk.top/gtgalcklem.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hnxiangtu.top/gtmixfrnpq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.andypj.xyz/gtrxemnesx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jianghu66.top/gtoaqgpcho.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.mhx1999.top/gtilixaxlw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xinyue.icu/gtmrxihsoz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.tian-w.cn/gtepvhhkao.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.quarkkingdee.top/gtcjhybqat.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jyoumei.cn/gtzrlaqwrx.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.cashguo.top/gtsiqromgp.html

Py:   pickle.dumps(obj)
来源：http://hz.jinqigfzy.top/gtgdcvbmhh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.pycfn.com/gtecrsbjgh.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.gaohongyu789.top/gtafeklsya.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.9152youxi.cn/gtiounftlt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.0kj1m.cn/gtpzutduwb.html


<!-- 参考信息 -->