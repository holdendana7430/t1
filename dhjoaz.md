代发 wailian999

JS:   class MyError extends Error {}
来源：http://hz.snrcjt.cn/gtonuuziom.html

TS:   class MyError extends Error {}
来源：http://hz.shanyushiyangkeji.top/gttxybxbad.html

Java: class MyException extends RuntimeException {}
来源：http://hz.wangdashe.top/gtbakgkhsb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.hammf.cn/gtwozxdckx.html

Ruby: class MyError < StandardError; end
来源：http://hz.hongshengwenyu.top/gtjmpdbccf.html

C#:   class MyException : Exception {}
来源：http://hz.jiagoushi.top/gtafzkbaps.html

[H05] 捕获特定类型
来源：http://hz.redwolf501.top/gtrotqyokp.html

Py:   except ValueError as e:
来源：http://hz.hongshengwenyu.top/gtghkpmpwz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.aizwys.cn/gtdrndgikg.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.aizwys.cn/gtskhbdric.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.cheryme.top/gtqmmwivmx.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.cqqwz.cn/gtwjqoncam.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.sxryk.cn/gtjrpecdyt.html

Ruby: rescue ArgumentError => e
来源：http://hz.xziqi.cn/gtmrybfmkn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yuxming.cn/gtufzpnvak.html

[H06] 可选值 / 空值安全访问
来源：http://hz.chenzaomai.com/gticnrcsdm.html

Py:   value = d.get("k") or default
来源：http://hz.redwolf501.top/gtfccgetko.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.birdmap.top/gtmcaqyvxi.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.cashguo.top/gtpsggohiv.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhoulong.xyz/gtnddnzvad.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.daria6918.cn/gtkwrxfxfk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.mhx1999.top/gtvmuvtffv.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhiwuduotai.top/gtdrvqylnh.html

C#:   obj?.A?.B ?? default
来源：http://hz.svipenyu.cn/gtsylqoxdt.html

[H07] 断言
来源：http://hz.hammf.cn/gtsanjqgzc.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jyoumei.cn/gtcunmrukz.html

PHP:  assert($x > 0);
来源：http://hz.gaohongyu789.top/gtzlsrlgjh.html

JS:   console.assert(x > 0);
来源：http://hz.wangshuangyany.cn/gtusrxsmir.html

TS:   console.assert(x > 0);
来源：http://hz.chenzaomai.com/gtpmoafmtz.html

Java: assert x > 0 : "必须为正";
来源：http://hz.xingfuxueyuan.xyz/gtrmpfyzti.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jinqigufen.top/gtlmryixuc.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.xuanzx.com/gtgfbgepdi.html

C#:   Debug.Assert(x > 0);
来源：http://hz.redwolf501.top/gtucqprbsc.html

[H08] 获取错误信息与堆栈
来源：http://hz.hammf.cn/gtlusaoknd.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.cashguo.top/gtyobpgpqb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.svipenyu.cn/gteuwstkww.html

JS:   e.message;  e.stack
来源：http://hz.wangdashe.top/gtrgiqhhwr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.52xcode.cn/gtqsmsqint.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.cashguo.top/gtzdwrvpzc.html

Go:   err.Error()
来源：http://hz.c1oappe.top/gttydtmjro.html

Ruby: e.message;  e.backtrace
来源：http://hz.tian-w.cn/gtajtrmehp.html

C#:   e.Message;  e.StackTrace
来源：http://hz.xinyue.icu/gtzhxqvrlw.html

[H09] 带错误码的异常
来源：http://hz.sysykeji.top/gtpkfhnbtn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.aizwys.cn/gtkxjxokci.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.mhx1999.top/gtkdlpmrln.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.0kj1m.cn/gtgwyczxlr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.cheryme.top/gtqvqervxa.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhoulong.xyz/gtjancnmac.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.sufxvd.cn/gtiylxmmel.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.vqdsnc.cn/gtroxtizay.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jiagoushi.top/gtcfsipygf.html

[H10] 资源自动释放
来源：http://hz.xingfuxueyuan.xyz/gtnpoggxus.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shangyingyoupin.top/gtlpwgutcp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.andypj.xyz/gtofinknfi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yvedp.cn/gtsvytreom.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.iojbl.cn/gtadbwyypu.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ywan-chungtsiang.top/gtojbimwxc.html

Go:   defer f.Close()
来源：http://hz.cashguo.top/gtfulivpdp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.shangyingyoupin.top/gtlozfizsp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zhaomingkeji.xyz/gtsspqysiz.html

================================================================================
来源：http://hz.cashguo.top/gtncadalpx.html

I. 正则表达式
来源：http://hz.hnxiangtu.top/gtbcjpybyr.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gteacfurvc.html

[I01] 判断是否匹配
来源：http://hz.shangyingyoupin.top/gticisblio.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.tian-w.cn/gtkqznaaha.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hnxiangtu.top/gtpbyrbcsq.html

JS:   /\d+/.test(s)
来源：http://hz.dashuyun.cn/gtisuevuim.html

TS:   /\d+/.test(s)
来源：http://hz.gotoacloud.top/gtviktnhtr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.guowangkeji.top/gtsudtikfi.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.vqdsnc.cn/gtmymplgdu.html

Ruby: s.match?(/\d+/)
来源：http://hz.haohaochexian.top/gtgvnhqgll.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.cqqwz.cn/gtljlcsynz.html

[I02] 提取所有匹配
来源：http://hz.ivvv.top/gtlswvrsfy.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zdqjudy.top/gthfhhynaf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.0kj1m.cn/gtbrhbcjqv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.redwolf501.top/gtstimtdzc.html

TS:   s.match(/\d+/g)
来源：http://hz.jiagoushi.top/gtalwshdeu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jqgufenzy.top/gtiexbvldd.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.aibaodan.cn/gtgvtuuugs.html

Ruby: s.scan(/\d+/)
来源：http://hz.yvedp.cn/gtxrviiglt.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.chenzaomai.com/gtfkydnrol.html

[I03] 提取捕获分组
来源：http://hz.hammf.cn/gtwpbhxths.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zdqjudy.top/gtuhkbucrn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yonumen.top/gthpotivre.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.cucudq.cn/gtjzxqoxyu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhongyouzk.top/gterwbebfb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.aizwys.cn/gtipcvgwpd.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.pycfn.com/gtaroifocw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.snrcjt.cn/gtlyrkftsu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.nanxinkj.top/gttexbxvtx.html

[I04] 正则替换
来源：http://hz.bjfxy.top/gttkwrhlhk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.svipenyu.cn/gtpicxggxk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.haohaochexian.top/gtuuyowwft.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.52xcode.cn/gtnkwpdznu.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yongpay.top/gtiaqwcvdm.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.nwbrower.top/gtiddoeaao.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.mhx1999.top/gtlogihuie.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ybcxt.top/gtryhspzhz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.cheryme.top/gtxjurgicv.html

[I05] 按正则拆分
来源：http://hz.jlsjyb.cn/gtgysldtpw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.smart0.xyz/gtmyzktomw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ydjk.org.cn/gtqovuxmyq.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zycfv.cn/gtdfakokbd.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhongyouzk.top/gtwotdvtby.html

Java: s.split("\\s*,\\s*")
来源：http://hz.bjfxy.top/gtfnwglwzz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jinqigufen.top/gtfjxxqptb.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xziqi.cn/gtquxbazgu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.wangshuangyany.cn/gtgvrmazyy.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhaomingkeji.xyz/gtrpqcwzvs.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jiagoushi.top/gtbcvneole.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yuanzhike.top/gtcznqjjeb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ppjwa.cn/gtsqsmleac.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhongyouzk.top/gtldhpygdl.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jinqigfzy.top/gtydokfsei.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.shanyushiyangtech.top/gtdiugyvpf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.wangshuangyany.cn/gtfdwzvqaf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yonumen.top/gthmeftdru.html

[I07] 忽略大小写与多行模式
来源：http://hz.guowangkeji.top/gtkgnvewsl.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yj20258888.top/gtrsjyqumd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yuanzhike.top/gtbepudfux.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.nwbrower.top/gtnikdizgt.html

TS:   /error/gim
来源：http://hz.ydjk.org.cn/gteygfuwoa.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jianghu66.top/gtlguewwxm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.cheryme.top/gtoslbvkot.html

Ruby: s.scan(/error/i)
来源：http://hz.wangshuangyany.cn/gtvmukqzkr.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.wangdashe.top/gtlmegqzlh.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.gzhubu.top/gtltunsvjm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.gzhubu.top/gtaccsxzuu.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.guannengcc.top/gtvsreynno.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.pengpengdd.cyou/gtywxgqapa.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yonumen.top/gtdkvoqgzm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hywenlv.cn/gtmssdynzb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.fengsongda.top/gtpneksneb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hnxiangtu.top/gtlycdppdr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhoulong.xyz/gtefategcn.html

================================================================================
来源：http://hz.daria6918.cn/gthfxjyscw.html

J. 日期与时间
来源：http://hz.ivvv.top/gtjansyryv.html

================================================================================
来源：http://hz.yuxming.cn/gteiyarcpj.html

[J01] 获取当前时间
来源：http://hz.xuanzx.com/gtzqgaeqjj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.cheryme.top/gtzizegbyx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ppjwa.cn/gtuokxchlg.html

JS:   new Date();  Date.now()
来源：http://hz.sysykeji.top/gtnfgizspl.html

TS:   new Date();  Date.now()
来源：http://hz.xylfe.cn/gtokrevoke.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jlsjyb.cn/gtwkmawjzu.html

Go:   time.Now()
来源：http://hz.tian-w.cn/gtcqymxzst.html

Ruby: Time.now
来源：http://hz.sxryk.cn/gttjtspktp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.daria6918.cn/gtolwoxxfa.html

[J02] 格式化输出
来源：http://hz.zhoulong.xyz/gtwnkrqrrw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hywenlv.cn/gtbebgwwjg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhiwuduotai.top/gtuckusyzh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.tianlin.xyz/gtbudvlqhg.html

TS:   d.toISOString()
来源：http://hz.ydzc1.top/gtfuznupwl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jinyuanbaomall.cn/gthgncyart.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.gzhubu.top/gtulqlvajq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tanke756.top/gtuiyvahqp.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.sxryk.cn/gtszwjbggk.html

[J03] 字符串解析为日期
来源：http://hz.birdmap.top/gtqedyhvyv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.cucudq.cn/gtepmvmrhh.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yuxming.cn/gtclogxatk.html

JS:   new Date("2024-01-02")
来源：http://hz.yangfankeji.com/gttakteupz.html

TS:   new Date("2024-01-02")
来源：http://hz.yuxming.cn/gtmsqifqfv.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhoulong.xyz/gtmknjgrda.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.9152youxi.cn/gtylyetqbg.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.tanke756.top/gtugoqlbhw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.shzxlz.cn/gtnzokdmej.html

[J04] 时间戳与日期互转
来源：http://hz.nwbrower.top/gtmicsfzjb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hammf.cn/gtgqjhkbbw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xuetiantiany.cn/gtykcazaqi.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yuxming.cn/gthijrxlbq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hammf.cn/gtekfpixmu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.nanxinkj.top/gtyncrkkci.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhengqikj.top/gtbokfdgyi.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.iojbl.cn/gtaeinombp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ydjk.org.cn/gtgooykbbo.html

[J05] 时间加减（加 7 天）
来源：http://hz.nwbrower.top/gtqaalfmvl.html

Py:   now + timedelta(days=7)
来源：http://hz.yj20258888.top/gtpfwjubpo.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.smart0.xyz/gtnrcjgjge.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jiagoushi.top/gtzbuavzwd.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.haohaochexian.top/gtvwizwesc.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.shzxlz.cn/gtgjlwopia.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.chenlongwang.top/gtogccsbiv.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yj202588.top/gtfslwpmwm.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.iojbl.cn/gtowkdhyoj.html

[J06] 计算两时间之差
来源：http://hz.wangdashe.top/gtxntezubo.html

Py:   (end - start).total_seconds()
来源：http://hz.smart0.xyz/gtsukbaoam.html

PHP:  $end->diff($start)->days;
来源：http://hz.yj20258.top/gtdgqrwcun.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.cqqwz.cn/gtpjtekcny.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.guowangkeji.top/gtdnfkwzzf.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ydjk.org.cn/gtxaazcbdn.html

Go:   end.Sub(start).Hours()
来源：http://hz.9152youxi.cn/gtumualmlu.html

Ruby: end - start                 # 返回秒数
来源：http://hz.tianlin.xyz/gtlphurxek.html

C#:   (end - start).TotalSeconds
来源：http://hz.aibaodan.cn/gtndsrvmfu.html

[J07] 比较两个日期
来源：http://hz.redwolf501.top/gtqbodkukb.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.smart0.xyz/gtdbjbfddi.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.daxiang520.top/gtlpfuzyvn.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.birdmap.top/gtgiczszrz.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.pycfn.com/gtvhfwxppf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xziqi.cn/gtkzccetgd.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hfpthk.cn/gtggrgrjlt.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.316326.xyz/gtlsaxwwvr.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jinqigufen.top/gtcttvafzj.html

[J08] 提取年月日与星期
来源：http://hz.gotoacloud.top/gtpektvoel.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.xuetiantiany.cn/gtsydtlnbh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.pengpengdd.cyou/gtjoeomrok.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.xziqi.cn/gtjaixqobf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yanxiufei.cn/gtvfuoywdj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.vqdsnc.cn/gtoqywbqvs.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.chenjidiqi.icu/gtbzjykosp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.fengsongda.top/gtbgbomubg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jinyuanbaomall.cn/gtpjmqlnsq.html

[J09] 时区处理
来源：http://hz.wangshuangyany.cn/gtptysruhg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.guowangkeji.top/gtdpynbtzt.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jinghuilouyu.cn/gtzrjoycbc.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhixingplan.top/gtgmkkxtor.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhaomingkeji.xyz/gthfpccjth.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yuanzhike.top/gtjthkiprv.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.birdmap.top/gtovkzuudr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.xuetiantiany.cn/gtwqvsvuto.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.dashuyun.cn/gtwsmxwglu.html

[J10] 取今天 / 本月第一天
来源：http://hz.xziqi.cn/gtkxilezqq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jianghu66.top/gtmsbudprg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hnxiangtu.top/gtjoecflcj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ehwqpu.com/gtpgyqwtlm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.sysykeji.top/gtvicgzxum.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhongyouzk.top/gtfsqtkmtc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ywan-chungtsiang.top/gtyqjzdbsg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yongpay.top/gtiiteynin.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.tian-w.cn/gtwulnjycg.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtuzniweqy.html

K. JSON 与序列化
来源：http://hz.zdqjudy.top/gtzqizsvfv.html

================================================================================
来源：http://hz.chenlongwang.top/gtvaelgogw.html

[K01] 对象转 JSON 字符串
来源：http://hz.hongshengwenyu.top/gtftsumjbp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.haohaochexian.top/gtknyqfybj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.wangdashe.top/gtpromnzln.html

JS:   JSON.stringify(obj)
来源：http://hz.zhoulong.xyz/gtamftczeu.html

TS:   JSON.stringify(obj)
来源：http://hz.jinqigufen.top/gtwutdywzm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.daria6918.cn/gtebnakpjo.html

Go:   json.Marshal(obj)
来源：http://hz.zdqjudy.top/gthgqjaoht.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhixingplan.top/gtutvbdzec.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jyoumei.cn/gtaqwowcxn.html

[K02] JSON 字符串转对象
来源：http://hz.sweek.top/gtqvxtylzm.html

Py:   json.loads(s)
来源：http://hz.hnqzz.top/gtvklzfoyq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.c1oappe.top/gtvftblibx.html

JS:   JSON.parse(s)
来源：http://hz.quarkkingdee.top/gtxtjebbfk.html

TS:   JSON.parse(s)
来源：http://hz.xylfe.cn/gtfrbdtetb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.gogol.net.cn/gtberkmeqy.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.316326.xyz/gtttipiyaz.html

Ruby: JSON.parse(s)
来源：http://hz.gzhubu.top/gtblekpynj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.gaohongyu789.top/gtnhodhcyl.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hywenlv.cn/gtwlcsedeh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ybcxt.top/gtwijrxsfv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ywan-chungtsiang.top/gtetbruzzu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.cheryme.top/gtngkufxke.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.ydzc1.top/gthcwxhfwv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.pycfn.com/gthfkdvkil.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.52xcode.cn/gtklvfuzan.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.cdnleiting.top/gtrpqudqqa.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.gotoacloud.top/gtjsvdeyfi.html

[K04] 读取 JSON 文件
来源：http://hz.jlsjyb.cn/gtjvqxcbvz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ywan-chungtsiang.top/gtymbuprqk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ywan-chungtsiang.top/gtksntpmxh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jlsjyb.cn/gtqxejahnz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cdnleiting.top/gtfumboaiy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.gaohongyu789.top/gtxrxrbkjc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.wangdashe.top/gtdsgukvdj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.chenlongwang.top/gtvtmsxbne.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.0kj1m.cn/gtecfcdcdc.html

[K05] 深拷贝对象
来源：http://hz.jlsjyb.cn/gtkzigxjyr.html

Py:   copy.deepcopy(obj)
来源：http://hz.yj202588.top/gtvjqrujwt.html

PHP:  unserialize(serialize($obj));
来源：http://hz.guowangkeji.top/gtnwbpnanl.html

JS:   structuredClone(obj)
来源：http://hz.tianlin.xyz/gtpsinbnpz.html

TS:   structuredClone(obj)
来源：http://hz.bjfxy.top/gtwrdsdfuj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jqgufenzy.top/gtintjfkir.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yj20258.top/gtrjhbthbo.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xylfe.cn/gtegfxxpwj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ydzc1.top/gtaovifhff.html

[K06] 解析 URL 查询串
来源：http://hz.daxiang520.top/gtkkmmlxgv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.bjfxy.top/gtxmakntua.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.sxryk.cn/gtdtrazsrj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.dianchejie.cn/gtqaylgcmo.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.redwolf501.top/gtrzuqivey.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.sufxvd.cn/gttzrepofm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yuxming.cn/gtjpmqnpvf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.iojbl.cn/gtffqgeplh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.fzhhl.top/gtamivkbvg.html

[K07] 进制转换
来源：http://hz.fengsongda.top/gteicfydub.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.havefunace.top/gtgvvbpifz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jqgufenzy.top/gttbmuhbin.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yuxming.cn/gtqqyhwbcl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.vqdsnc.cn/gtaphiuffq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yangfankeji.com/gtynqptnld.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.shanyushiyangtech.top/gtvnmtqflu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yueranfly.top/gtayqpolvu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hywenlv.cn/gtxtqgshie.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.sweek.top/gttpesutjm.html

Py:   pickle.dumps(obj)
来源：http://hz.nanxuanxn.top/gtdsffplya.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.snrcjt.cn/gtrmutfzit.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hongshengwenyu.top/gtasrfnfez.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jinghuilouyu.cn/gtjvvaazkr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yj20258.top/gtnarbekci.html


<!-- 参考信息 -->