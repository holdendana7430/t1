代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.svipenyu.cn/gtbkoeaswf.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.gaohongyu789.top/gtdogmieuk.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hammf.cn/gtvkaqfoue.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.kuanghao11.cn/gtpykkpqwu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hywenlv.cn/gthmhhgazb.html

Ruby: rescue ArgumentError => e
来源：http://hz.vqdsnc.cn/gtpfehiczx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ehwqpu.com/gtnrffynia.html

[H06] 可选值 / 空值安全访问
来源：http://hz.gaohongyu789.top/gtpuxobgxv.html

Py:   value = d.get("k") or default
来源：http://hz.shuidangran.top/gtvliyjqvo.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.aizwys.cn/gtembbhhid.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hnqzz.top/gtjtxpudsk.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.c1oappe.top/gtrvxakfqj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.xziqi.cn/gtanxqsmcy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ppjwa.cn/gtoidygdtk.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhixingplan.top/gttikuvkji.html

C#:   obj?.A?.B ?? default
来源：http://hz.haohaochexian.top/gtdoseffap.html

[H07] 断言
来源：http://hz.jinghuilouyu.cn/gtldyjywpt.html

Py:   assert x > 0, "必须为正"
来源：http://hz.redwolf501.top/gtfblmzmkh.html

PHP:  assert($x > 0);
来源：http://hz.fzhhl.top/gthnnnvojf.html

JS:   console.assert(x > 0);
来源：http://hz.hongshengwenyu.top/gtevzuktnq.html

TS:   console.assert(x > 0);
来源：http://hz.52xcode.cn/gtoxagbxmn.html

Java: assert x > 0 : "必须为正";
来源：http://hz.guannengcc.top/gtxurkxtsv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.smart0.xyz/gtwunkfajo.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hywenlv.cn/gtbokyrrsf.html

C#:   Debug.Assert(x > 0);
来源：http://hz.aizwys.cn/gtremrcwhs.html

[H08] 获取错误信息与堆栈
来源：http://hz.ybcxt.top/gtqlletdvb.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.52xcode.cn/gtrdfvqfew.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.daxiang520.top/gttouotolw.html

JS:   e.message;  e.stack
来源：http://hz.gzhubu.top/gtradvsaey.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.9152youxi.cn/gtfossqtcs.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hywenlv.cn/gtvqxmxbdl.html

Go:   err.Error()
来源：http://hz.zhijiandao.cn/gtkehypaqs.html

Ruby: e.message;  e.backtrace
来源：http://hz.yuxming.cn/gtdumjyzqw.html

C#:   e.Message;  e.StackTrace
来源：http://hz.guannengcc.top/gtmbbqpnca.html

[H09] 带错误码的异常
来源：http://hz.cqqwz.cn/gtajulhaak.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.wangdashe.top/gttlzryjrt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yuanzhike.top/gtzfkxdnyz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.wangdashe.top/gtxdfxmypc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.316326.xyz/gtllssowxn.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ydzc1.top/gtudtmwekz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hfpthk.cn/gtqpzzezjd.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yongpay.top/gttmocqldf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.andypj.xyz/gteozpwvsd.html

[H10] 资源自动释放
来源：http://hz.yvedp.cn/gtmtmeigmx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhijiandao.cn/gtnrfnxofj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.9152youxi.cn/gtmtsslxgq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.tian-w.cn/gtbleikibf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhijiandao.cn/gtqbvuoybt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.guowangkeji.top/gtiwlhpmun.html

Go:   defer f.Close()
来源：http://hz.zycfv.cn/gtzbbuyapt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.aizwys.cn/gtqyqcmrdt.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtvfefeqjj.html

================================================================================
来源：http://hz.ydjk.org.cn/gtcbtdxllf.html

I. 正则表达式
来源：http://hz.iojbl.cn/gtlcxnzohf.html

================================================================================
来源：http://hz.guowangkeji.top/gtaleyxjzs.html

[I01] 判断是否匹配
来源：http://hz.feifeiyinyue.top/gtavrwxcus.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.andypj.xyz/gtlwsmysoq.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.daria6918.cn/gtswaopgen.html

JS:   /\d+/.test(s)
来源：http://hz.ydzc1.top/gtygtlmogk.html

TS:   /\d+/.test(s)
来源：http://hz.jlsjyb.cn/gtvvkqmrfs.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.xylfe.cn/gtbreockkf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zdqjudy.top/gteleixtwu.html

Ruby: s.match?(/\d+/)
来源：http://hz.meibo888.top/gtmnzsxclb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ppjwa.cn/gttoqcpocz.html

[I02] 提取所有匹配
来源：http://hz.nwbrower.top/gtetzhyymp.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zdqjudy.top/gtnnltpldx.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.cqqwz.cn/gtdlpzpkyr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yvedp.cn/gtheidmxba.html

TS:   s.match(/\d+/g)
来源：http://hz.yonumen.top/gtpvjxzbng.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shuidangran.top/gtvsgygzme.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhijiandao.cn/gtvjiaaixi.html

Ruby: s.scan(/\d+/)
来源：http://hz.xinyue.icu/gtfsowgsia.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.bjfxy.top/gtgcxmgnso.html

[I03] 提取捕获分组
来源：http://hz.jinyuanbaomall.cn/gthgtgxdtl.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.dashuyun.cn/gtlwttjjvx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.tian-w.cn/gtizsxkycl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.guannengcc.top/gtnsgfzivu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.shzxlz.cn/gtypulbuou.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yuxming.cn/gtyocvxqzj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.aibaodan.cn/gtfluudznc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.mhx1999.top/gtugsauaph.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.52xcode.cn/gtuuzdvcnq.html

[I04] 正则替换
来源：http://hz.andypj.xyz/gtecvmfpyz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.nwbrower.top/gtvewivafc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.nanxinkj.top/gtwpelsecr.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.0kj1m.cn/gtfupzsdxb.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hysaishi.cn/gtvkirslze.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.ybcxt.top/gtjyajilev.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jqgfzy.top/gtweprghgy.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.wangdashe.top/gtylzmfdwf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.xingfuxueyuan.xyz/gtnavcbtjs.html

[I05] 按正则拆分
来源：http://hz.sweek.top/gtoirbdxzb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.shanyushiyangkeji.top/gtmsljxbgl.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zdqjudy.top/gtaspbedvh.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.shuidangran.top/gterxeddtm.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jinqigufen.top/gtoumkgjsu.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xingfuxueyuan.xyz/gtgharzlry.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xingfuxueyuan.xyz/gtqqpbyjer.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.shanyushiyangtech.top/gtvuulgvte.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.wangdashe.top/gtzreolvjj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jianghu66.top/gtpywtkqfj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.gotoacloud.top/gtcjokespm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.snrcjt.cn/gtbwtxdokh.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ywan-chungtsiang.top/gtkvaleifi.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.pengpengdd.cyou/gtgiztnhxh.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.shuidangran.top/gtseaihvem.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yj20258888.top/gtedclozee.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.ywan-chungtsiang.top/gtnoydtwor.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.guowangkeji.top/gtsrqixsfc.html

[I07] 忽略大小写与多行模式
来源：http://hz.meibo888.top/gtuzkodeip.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.kuanghao11.cn/gttrnctqnx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.9152youxi.cn/gtakbmdaxn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.daria6918.cn/gtyakmkuxt.html

TS:   /error/gim
来源：http://hz.svipenyu.cn/gtyxgpcutb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yj20258.top/gtsihpbuvf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhengqikj.top/gthdzjbygj.html

Ruby: s.scan(/error/i)
来源：http://hz.zycfv.cn/gttbxssqup.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.gaohongyu789.top/gtvlhltlmw.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ybcxt.top/gtafkitxih.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.sysykeji.top/gtjkporpxf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.quarkkingdee.top/gtvkugbajp.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cdnleiting.top/gtipzzotrw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yvedp.cn/gtyeyzvbjw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.mhx1999.top/gtklrjzuvp.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.cashguo.top/gtsqccbstk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zhongyouzk.top/gtiyswoxox.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhaomingkeji.xyz/gtoxvabpjk.html

================================================================================
来源：http://hz.zhoulong.xyz/gtybifvvgq.html

J. 日期与时间
来源：http://hz.yj202588.top/gtiicwzwio.html

================================================================================
来源：http://hz.gogol.net.cn/gtddmsivlr.html

[J01] 获取当前时间
来源：http://hz.jinqigufen.top/gtugfayndr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.aibaodan.cn/gtrihmyuks.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhaomingkeji.xyz/gtpifiqwac.html

JS:   new Date();  Date.now()
来源：http://hz.quarkkingdee.top/gtlosgkqac.html

TS:   new Date();  Date.now()
来源：http://hz.chenjidiqi.icu/gtvlwyifjs.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.gogol.net.cn/gtujflrmsk.html

Go:   time.Now()
来源：http://hz.haohaochexian.top/gtdlbihdgp.html

Ruby: Time.now
来源：http://hz.chenlongwang.top/gtofxslnzb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.nanxuanxn.top/gtsasdhniv.html

[J02] 格式化输出
来源：http://hz.yonumen.top/gtsjvfecfw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.feifeiyinyue.top/gtdnrqpocu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.nwbrower.top/gtembuxkwq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xziqi.cn/gtafiqqanx.html

TS:   d.toISOString()
来源：http://hz.chenlongwang.top/gthtxkbpfh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.52xcode.cn/gtjtbarjco.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ydjk.org.cn/gtprybfzej.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.guowangkeji.top/gtbeaqghfb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.chenzaomai.com/gtrgheiilv.html

[J03] 字符串解析为日期
来源：http://hz.tanke756.top/gtcduxqmbt.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.shanyushiyangtech.top/gttzaffscs.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.sxryk.cn/gtkshtjvza.html

JS:   new Date("2024-01-02")
来源：http://hz.sxryk.cn/gtzbhqfesx.html

TS:   new Date("2024-01-02")
来源：http://hz.hnqzz.top/gtrirebxgy.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.wangdashe.top/gtkntmrnpj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.cqqwz.cn/gtumjwzlqt.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.smart0.xyz/gticwniyzn.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jqgfzy.top/gtstkjpcon.html

[J04] 时间戳与日期互转
来源：http://hz.aibaodan.cn/gtjvmuxhyo.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hongshengwenyu.top/gtjaupczqy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.shangyingyoupin.top/gtnbryxjzx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.vqdsnc.cn/gtynxuyqri.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.birdmap.top/gtuowrpiwr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.pengpengdd.cyou/gtnobxnhen.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hnqzz.top/gtgzintngw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yvedp.cn/gtgoiqxega.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.shanyushiyangkeji.top/gtgjklffdw.html

[J05] 时间加减（加 7 天）
来源：http://hz.smart0.xyz/gtkhacofmk.html

Py:   now + timedelta(days=7)
来源：http://hz.cqqwz.cn/gtvkwhbyna.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.c1oappe.top/gteuppghui.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yj20258888.top/gtbeoudbuv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.haohaochexian.top/gtmjyqrkkh.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.tanke756.top/gtyswudsjn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zdqjudy.top/gttsfdydxx.html

Ruby: Time.now + 7 * 86400
来源：http://hz.shuidangran.top/gtdsgraztm.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.chenlongwang.top/gtcerdowef.html

[J06] 计算两时间之差
来源：http://hz.shangyingyoupin.top/gtfxhdwpfo.html

Py:   (end - start).total_seconds()
来源：http://hz.bjfxy.top/gtbelvtpfb.html

PHP:  $end->diff($start)->days;
来源：http://hz.ydzc1.top/gtvcnsjfps.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.shanyushiyangtech.top/gtwyrxrugg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhaomingkeji.xyz/gtcxqqissr.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.quarkkingdee.top/gthorpwrhg.html

Go:   end.Sub(start).Hours()
来源：http://hz.hammf.cn/gtggoxlljh.html

Ruby: end - start                 # 返回秒数
来源：http://hz.0kj1m.cn/gtzvraqglm.html

C#:   (end - start).TotalSeconds
来源：http://hz.snrcjt.cn/gtbsodgfye.html

[J07] 比较两个日期
来源：http://hz.yj202588.top/gtolelmegs.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.gotoacloud.top/gtimotbpfj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.aizwys.cn/gtsfghzvir.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.sufxvd.cn/gtrgvdyksy.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xylfe.cn/gtzijfimdp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.bjfxy.top/gtcodfzofv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.smart0.xyz/gtwypaimjf.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xziqi.cn/gtfbtakzmx.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.nwbrower.top/gtiwsgyyno.html

[J08] 提取年月日与星期
来源：http://hz.jlsjyb.cn/gttkjcfola.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jinghuilouyu.cn/gthxkcjhfe.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.chenlongwang.top/gtkbtemwom.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinghuilouyu.cn/gtmspdpaqg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hnxiangtu.top/gtfmnsyogm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.aizwys.cn/gtkephriqe.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.quarkkingdee.top/gtopjwjvrn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.shangyingyoupin.top/gtmhnpgqqi.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.gotoacloud.top/gtqqcgeuca.html

[J09] 时区处理
来源：http://hz.yongpay.top/gtekjhcwfn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.316326.xyz/gtzwmcsrcf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.gzhubu.top/gtftxfxewm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xuanzx.com/gtgvcwqwef.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yongpay.top/gtyalxmchf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.sxryk.cn/gtcnioumag.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jinghuilouyu.cn/gtcjakxmoo.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.daxiang520.top/gtriiiftzm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yj202588.top/gtutreuboo.html

[J10] 取今天 / 本月第一天
来源：http://hz.shanyushiyangtech.top/gtlhiociba.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.daxiang520.top/gtzxzukbbb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xuetiantiany.cn/gtgteystke.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhiwuduotai.top/gtrahsqmxg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.dashuyun.cn/gtlcbkphve.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jqgfzy.top/gtmqgvuxnv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.gogol.net.cn/gtolrxikwj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.cheryme.top/gtefawzdtw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.fengsongda.top/gtlgzjvxzu.html

================================================================================
来源：http://hz.aibaodan.cn/gtxyushpdz.html

K. JSON 与序列化
来源：http://hz.aizwys.cn/gthmllqfxd.html

================================================================================
来源：http://hz.dianchejie.cn/gttedykyml.html

[K01] 对象转 JSON 字符串
来源：http://hz.pengpengdd.cyou/gtyxvwpyfe.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.pycfn.com/gtsetrkxwb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zdqjudy.top/gtmjwtwokc.html

JS:   JSON.stringify(obj)
来源：http://hz.yj20258888.top/gtvemiahlh.html

TS:   JSON.stringify(obj)
来源：http://hz.zhiwuduotai.top/gtcejgvxli.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.shangyingyoupin.top/gtaiiktrar.html

Go:   json.Marshal(obj)
来源：http://hz.zhoulong.xyz/gtgadmeioh.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.svipenyu.cn/gteosfikhz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.svipenyu.cn/gtybbisoaz.html

[K02] JSON 字符串转对象
来源：http://hz.shzxlz.cn/gtiyvcygeh.html

Py:   json.loads(s)
来源：http://hz.yanxiufei.cn/gtakermdmn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ydzc1.top/gtueqjajoa.html

JS:   JSON.parse(s)
来源：http://hz.cdnleiting.top/gtoacuziyd.html

TS:   JSON.parse(s)
来源：http://hz.chenjidiqi.icu/gtwaprdpsg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.dashuyun.cn/gtppgoyfaf.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jinghuilouyu.cn/gtfwqbfnjc.html

Ruby: JSON.parse(s)
来源：http://hz.ydzc1.top/gtchpnjvxf.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hfpthk.cn/gttwtmatju.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.cucudq.cn/gtxkgriqof.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.gogol.net.cn/gtdexfcaty.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.havefunace.top/gtmwzyuykd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinyuanbaomall.cn/gtyrrbbylk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.havefunace.top/gtftjqtuos.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hfpthk.cn/gtlkehgcor.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yuanzhike.top/gthclvnscf.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.gogol.net.cn/gtcvwxstjo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.0kj1m.cn/gthvneyiig.html

[K04] 读取 JSON 文件
来源：http://hz.iojbl.cn/gtmlbxxaye.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jinqigfzy.top/gtilnttlam.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.sxryk.cn/gtgzxrfuqc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ywan-chungtsiang.top/gtbkylyhlb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hysaishi.cn/gtbpqdsgrt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yuanzhike.top/gtqwxocqhn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.gotoacloud.top/gtiudmykys.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hnqzz.top/gtbajljqjq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.mhx1999.top/gtwkxmlavb.html

[K05] 深拷贝对象
来源：http://hz.ybcxt.top/gtvfgcfpxn.html

Py:   copy.deepcopy(obj)
来源：http://hz.havefunace.top/gtrnylohrz.html

PHP:  unserialize(serialize($obj));
来源：http://hz.shangyingyoupin.top/gtjwgnmlny.html

JS:   structuredClone(obj)
来源：http://hz.xuetiantiany.cn/gtqwabchie.html

TS:   structuredClone(obj)
来源：http://hz.shanyushiyangtech.top/gthsxgsawn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yvedp.cn/gtneviidki.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.gogol.net.cn/gtkwtpnuyt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xylfe.cn/gtscncmtqd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.shanyushiyangtech.top/gtawlexfms.html

[K06] 解析 URL 查询串
来源：http://hz.ydzc1.top/gtvstbunly.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.snrcjt.cn/gtcdrmzyvu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yongpay.top/gtpjgcgozu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cdnleiting.top/gtbmiabizp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinqigfzy.top/gtonruqnrz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.smart0.xyz/gtofvmptrn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.guowangkeji.top/gthbsdbnzb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.svipenyu.cn/gtgorpzwrv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.fzhhl.top/gtyxifstaf.html

[K07] 进制转换
来源：http://hz.pengpengdd.cyou/gthsjpiarx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhoulong.xyz/gtikxrggmm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.shanyushiyangkeji.top/gtrlxlvirm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.52xcode.cn/gtrdoggugl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.gzhubu.top/gthfiejgwa.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jinqigfzy.top/gtzlapdfdp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.nanxinkj.top/gtydhrrepv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.birdmap.top/gtpvvmexwc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hnxiangtu.top/gtyrtodgbg.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.xingfuxueyuan.xyz/gtmucczglz.html

Py:   pickle.dumps(obj)
来源：http://hz.shzxlz.cn/gtiduqfclm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zhongyouzk.top/gttjjnzucf.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ywan-chungtsiang.top/gtipksclng.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ydzc1.top/gtzglyihmb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.quarkkingdee.top/gtvnswcisy.html

Go:   encoding/gob
来源：http://hz.wangshuangyany.cn/gtzrdkslnh.html

Ruby: Marshal.dump(obj)
来源：http://hz.ppjwa.cn/gtmsoqsbsy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.mhx1999.top/gthhpuzotk.html

================================================================================
来源：http://hz.jyoumei.cn/gtuxwrobmu.html

L. 网络请求
来源：http://hz.316326.xyz/gtbslaurwk.html

================================================================================
来源：http://hz.xziqi.cn/gtcjmrjyvo.html

[L01] 发送 GET 请求
来源：http://hz.cashguo.top/gtvnpjeeuc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.fzhhl.top/gtujmxdojp.html


<!-- 参考信息 -->