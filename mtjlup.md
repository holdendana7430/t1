代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zhengqikj.top/gtonjaxhwa.html

[H04] 自定义异常类型
来源：http://hz.gotoacloud.top/gtruedgoiv.html

Py:   class MyError(Exception): pass
来源：http://hz.yueranfly.top/gtqjobcjpf.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yueranfly.top/gttcydjlom.html

JS:   class MyError extends Error {}
来源：http://hz.jqgfzy.top/gtiqvmgrgg.html

TS:   class MyError extends Error {}
来源：http://hz.zhiwuduotai.top/gtgvaibbdh.html

Java: class MyException extends RuntimeException {}
来源：http://hz.fengsongda.top/gtyqltoxwm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.havefunace.top/gthafqglgj.html

Ruby: class MyError < StandardError; end
来源：http://hz.feifeiyinyue.top/gtallkbhsd.html

C#:   class MyException : Exception {}
来源：http://hz.zhongyouzk.top/gtsjtswtma.html

[H05] 捕获特定类型
来源：http://hz.fzhhl.top/gttmnkhmhh.html

Py:   except ValueError as e:
来源：http://hz.jyoumei.cn/gtraxmluih.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yanxiufei.cn/gttomfwspr.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yj20258888.top/gtzbziablw.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.gogol.net.cn/gtrcjsbzpi.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.ppjwa.cn/gtgivjvukn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.shzxlz.cn/gttjmudarr.html

Ruby: rescue ArgumentError => e
来源：http://hz.yueranfly.top/gtuinmchjt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.bjfxy.top/gtgxigtgxz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yj20258888.top/gtzhkloehb.html

Py:   value = d.get("k") or default
来源：http://hz.tanke756.top/gtlwcbgdxy.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.aibaodan.cn/gtkxnjzlfx.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.guowangkeji.top/gtckdbdwee.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.gogol.net.cn/gtzjhgccxc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.nwbrower.top/gtyelvprpi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.52xcode.cn/gtfmypxhmy.html

Ruby: d&.dig(:a, :b)
来源：http://hz.aizwys.cn/gtzqbgngjd.html

C#:   obj?.A?.B ?? default
来源：http://hz.feifeiyinyue.top/gtgujmsgfb.html

[H07] 断言
来源：http://hz.shanyushiyangtech.top/gtiwaavdlc.html

Py:   assert x > 0, "必须为正"
来源：http://hz.guowangkeji.top/gtgkuzlbao.html

PHP:  assert($x > 0);
来源：http://hz.cheryme.top/gtcgwkhrji.html

JS:   console.assert(x > 0);
来源：http://hz.jinqigfzy.top/gtwwxjyljk.html

TS:   console.assert(x > 0);
来源：http://hz.fzhhl.top/gtsfhaezwi.html

Java: assert x > 0 : "必须为正";
来源：http://hz.wangshuangyany.cn/gtlrmacofu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.wangdashe.top/gttoymrlcu.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhixingplan.top/gtcasmkvvy.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhaomingkeji.xyz/gtahbhyhcx.html

[H08] 获取错误信息与堆栈
来源：http://hz.nanxinkj.top/gtodvznvti.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jyoumei.cn/gthrmjxzkr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.chenjidiqi.icu/gtxivomopp.html

JS:   e.message;  e.stack
来源：http://hz.wangdashe.top/gtjmgrmyhl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.daxiang520.top/gtpiatssgn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yanxiufei.cn/gtnuwhqqsc.html

Go:   err.Error()
来源：http://hz.jinyuanbaomall.cn/gtjqwvbeux.html

Ruby: e.message;  e.backtrace
来源：http://hz.sufxvd.cn/gtjhoivgga.html

C#:   e.Message;  e.StackTrace
来源：http://hz.gotoacloud.top/gtgmzsmmih.html

[H09] 带错误码的异常
来源：http://hz.xingfuxueyuan.xyz/gtwsksmaww.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.cqqwz.cn/gteijpipiw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhiwuduotai.top/gtsdpbdjvs.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ppjwa.cn/gtlfbdmmwn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.nanxinkj.top/gtdrpwvsvl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.guowangkeji.top/gtrvjtnqab.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.xingfuxueyuan.xyz/gtdlzwdweq.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhiwuduotai.top/gtyztdoffy.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhaomingkeji.xyz/gtmtkfdxxr.html

[H10] 资源自动释放
来源：http://hz.yj20258888.top/gtpnepapdc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yj20258.top/gtifrzzjlu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.gzhubu.top/gtlcevznhy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.vqdsnc.cn/gtmrzjjmbd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.pengpengdd.cyou/gtvpxuzpij.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yj20258888.top/gtzwcpobyx.html

Go:   defer f.Close()
来源：http://hz.jinyuanbaomall.cn/gteddumspm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.cdnleiting.top/gtepygdlvl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hnxiangtu.top/gtqxibrnfb.html

================================================================================
来源：http://hz.mhx1999.top/gtwoymlpdv.html

I. 正则表达式
来源：http://hz.andypj.xyz/gtvvicfhjv.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtfqqdoykk.html

[I01] 判断是否匹配
来源：http://hz.jlsjyb.cn/gtfrcukwgd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hywenlv.cn/gtmkswzogk.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.nanxuanxn.top/gtblyhuywa.html

JS:   /\d+/.test(s)
来源：http://hz.jqgfzy.top/gtcnscofuj.html

TS:   /\d+/.test(s)
来源：http://hz.nwbrower.top/gtabtltjvn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.shuidangran.top/gtwteocprv.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.andypj.xyz/gtdckbpoil.html

Ruby: s.match?(/\d+/)
来源：http://hz.xuetiantiany.cn/gtlubsacpv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.gogol.net.cn/gtlnmgeiqr.html

[I02] 提取所有匹配
来源：http://hz.jinqigufen.top/gtnruzxics.html

Py:   re.findall(r"\d+", s)
来源：http://hz.sxryk.cn/gtdjidzdyp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zycfv.cn/gtdellbcol.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.snrcjt.cn/gtcuslkppj.html

TS:   s.match(/\d+/g)
来源：http://hz.fengsongda.top/gtssgvpyyi.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zycfv.cn/gtnnrtbmih.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.shuidangran.top/gtgzjdzbym.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhongyouzk.top/gtjzivirfh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.kuanghao11.cn/gtildveezu.html

[I03] 提取捕获分组
来源：http://hz.gotoacloud.top/gtzekezqke.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yj20258888.top/gtxdpmlwkf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.gzhubu.top/gtqxezomfc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.quarkkingdee.top/gtjrcfsdbw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.birdmap.top/gtxzmjpbve.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.pengpengdd.cyou/gtxmwmgjtr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.kuanghao11.cn/gtfehylxpz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xuetiantiany.cn/gtribmounx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yj20258.top/gtieeisgvd.html

[I04] 正则替换
来源：http://hz.jinghuilouyu.cn/gtaxliygnh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.dashuyun.cn/gtnhxfkgoq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.meibo888.top/gtindjdnrc.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ywan-chungtsiang.top/gtpjflvubo.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.pycfn.com/gtfuaytexb.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.svipenyu.cn/gtjrlcqini.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhiwuduotai.top/gttgjydoli.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.iojbl.cn/gtnxworuvy.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jinqigfzy.top/gtzczygykf.html

[I05] 按正则拆分
来源：http://hz.ivvv.top/gtzinnvext.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.birdmap.top/gtuhnapbfh.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.daria6918.cn/gtwzmidijn.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.shuidangran.top/gtpfyhviyl.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhaomingkeji.xyz/gtvsqtfhun.html

Java: s.split("\\s*,\\s*")
来源：http://hz.hammf.cn/gtdkinzlac.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.52xcode.cn/gtkrfugnrv.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.9152youxi.cn/gtbiwgouzz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.gogol.net.cn/gtxpboqpbq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhijiandao.cn/gttsnitgfx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.wangshuangyany.cn/gtksbrbqnp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.c1oappe.top/gtokqaghey.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yj20258.top/gtqmbaavul.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tianlin.xyz/gtplesmvrc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.cucudq.cn/gtnujnqeav.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.sufxvd.cn/gtqsiidcma.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.gaohongyu789.top/gtvxmkijjs.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yonumen.top/gtgyjthxkk.html

[I07] 忽略大小写与多行模式
来源：http://hz.jinqigufen.top/gtrylhjybo.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.svipenyu.cn/gtkjbcizhv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.smart0.xyz/gthrhesgqr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.52xcode.cn/gtmghmiarg.html

TS:   /error/gim
来源：http://hz.zhijiandao.cn/gtraeulgww.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jlsjyb.cn/gtonpqylbe.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.0kj1m.cn/gtfwvilhyw.html

Ruby: s.scan(/error/i)
来源：http://hz.jiagoushi.top/gtpckuwokq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.c1oappe.top/gtwyyqijye.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ywan-chungtsiang.top/gtixvodpbp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.havefunace.top/gtpzssgvnp.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jqgufenzy.top/gtjychjveo.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shanyushiyangkeji.top/gtcpqqyzpr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xuanzx.com/gtyaxodxdz.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.andypj.xyz/gtlnxjqxhw.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.andypj.xyz/gtcpgcaiex.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zhijiandao.cn/gtshukkpir.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.cdnleiting.top/gtqksngnhh.html

================================================================================
来源：http://hz.jlsjyb.cn/gtborjlekr.html

J. 日期与时间
来源：http://hz.shanyushiyangtech.top/gtqfhnbhjz.html

================================================================================
来源：http://hz.nanxuanxn.top/gtdobuxmdj.html

[J01] 获取当前时间
来源：http://hz.hysaishi.cn/gtljxelmpl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jlsjyb.cn/gtysdmjcqj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.dianchejie.cn/gtkxnuruqr.html

JS:   new Date();  Date.now()
来源：http://hz.jinqigfzy.top/gtxyjjcddr.html

TS:   new Date();  Date.now()
来源：http://hz.snrcjt.cn/gtshdombmr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.nwbrower.top/gtwicclcsj.html

Go:   time.Now()
来源：http://hz.daxiang520.top/gtdzitgzwi.html

Ruby: Time.now
来源：http://hz.daxiang520.top/gtgzjoidks.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.bjfxy.top/gtjvyhwrkb.html

[J02] 格式化输出
来源：http://hz.jyoumei.cn/gtieagqrvz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.52xcode.cn/gtytchjgwg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.gzhubu.top/gtnxynakgw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.meibo888.top/gtkpgqalvo.html

TS:   d.toISOString()
来源：http://hz.aibaodan.cn/gtswpvxtwq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.shangyingyoupin.top/gtvzkvxcxf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ydzc1.top/gteneircut.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhaomingkeji.xyz/gtzwetoixr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.andypj.xyz/gtcnonjmpb.html

[J03] 字符串解析为日期
来源：http://hz.kuanghao11.cn/gtyqkazrzc.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.haohaochexian.top/gtluijfeqb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cdnleiting.top/gtrbbpzowc.html

JS:   new Date("2024-01-02")
来源：http://hz.yangfankeji.com/gtpzsvuqnj.html

TS:   new Date("2024-01-02")
来源：http://hz.smart0.xyz/gtccivdcxy.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hnxiangtu.top/gtaqgcruko.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jqgfzy.top/gtgwazxjnm.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jinqigufen.top/gtobniidbv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hywenlv.cn/gtqpoocsle.html

[J04] 时间戳与日期互转
来源：http://hz.hongshengwenyu.top/gtjizfsock.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.cqqwz.cn/gtmgsfocjz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.gzhubu.top/gtvozlplub.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.bjfxy.top/gtknkmxing.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hongshengwenyu.top/gtxehkypps.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.gotoacloud.top/gtmsfvkngj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.xuanzx.com/gtptuqvtpu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.316326.xyz/gtbkiltcec.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.sxryk.cn/gthhdgcoab.html

[J05] 时间加减（加 7 天）
来源：http://hz.vqdsnc.cn/gtximnpacn.html

Py:   now + timedelta(days=7)
来源：http://hz.yangfankeji.com/gtcfxvonhf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.smart0.xyz/gttlbtfhhi.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.dianchejie.cn/gtkpmcbhqy.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.guannengcc.top/gthknstjra.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jinqigfzy.top/gtizzjzbuq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.daria6918.cn/gthxoksuxc.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zycfv.cn/gtzowyxvjo.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jlsjyb.cn/gtfzrmldbq.html

[J06] 计算两时间之差
来源：http://hz.hnqzz.top/gtptylmzos.html

Py:   (end - start).total_seconds()
来源：http://hz.chenlongwang.top/gtfomymeig.html

PHP:  $end->diff($start)->days;
来源：http://hz.haohaochexian.top/gtithwhugc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jiagoushi.top/gtvgmfpxcv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.pycfn.com/gtkkxddede.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.0kj1m.cn/gtwdjbcvah.html

Go:   end.Sub(start).Hours()
来源：http://hz.ybcxt.top/gtzkwbljax.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jiagoushi.top/gtcznrtcfb.html

C#:   (end - start).TotalSeconds
来源：http://hz.xuanzx.com/gtlhvkaqyc.html

[J07] 比较两个日期
来源：http://hz.havefunace.top/gtjoccrluc.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.andypj.xyz/gtuvcgijax.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.shanyushiyangkeji.top/gtrhtaggft.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.cdnleiting.top/gtxjcebylp.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xinyue.icu/gtdvjbfgkv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jinyuanbaomall.cn/gtyzbcwehw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zdqjudy.top/gtvzeqbpzg.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hammf.cn/gtqbvfdecv.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jqgfzy.top/gtmwuyroxz.html

[J08] 提取年月日与星期
来源：http://hz.guannengcc.top/gtqqxjhgzp.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.chenlongwang.top/gtnupbcwlg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhongyouzk.top/gtazcfrhwc.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.ybcxt.top/gtpwpmqrxs.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.xinyue.icu/gtmbpqgzis.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.cqqwz.cn/gtlkdafijo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.cucudq.cn/gtzwesayzh.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.dashuyun.cn/gtbdpunrmy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.cashguo.top/gtigqvbcle.html

[J09] 时区处理
来源：http://hz.yuanzhike.top/gtmbielbsr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cdnleiting.top/gtmtbdghii.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jiagoushi.top/gtgzohfnea.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cheryme.top/gtmeodnzxu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sufxvd.cn/gticfqprij.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.nanxuanxn.top/gthexaiabr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.iojbl.cn/gtnmjdgcvj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yvedp.cn/gtobgybboj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ywan-chungtsiang.top/gtfiedtjlq.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhaomingkeji.xyz/gtjwpxfnlo.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.nanxuanxn.top/gthvsazlpm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jiagoushi.top/gtcrvvfuzh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.havefunace.top/gtirepswln.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ppjwa.cn/gtycikhxtb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.9152youxi.cn/gtammrtpdg.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xingfuxueyuan.xyz/gtqxigjjuq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.quarkkingdee.top/gtsqjnhauz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.bjfxy.top/gtffnsyypo.html

================================================================================
来源：http://hz.yuxming.cn/gtipmjsozj.html

K. JSON 与序列化
来源：http://hz.havefunace.top/gtgmokvykz.html

================================================================================
来源：http://hz.xuanzx.com/gtzvosnkus.html

[K01] 对象转 JSON 字符串
来源：http://hz.cqqwz.cn/gtatevjydi.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.cheryme.top/gtyusdblac.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhongyouzk.top/gtfdqvuyxd.html

JS:   JSON.stringify(obj)
来源：http://hz.cqqwz.cn/gtfqhfskub.html

TS:   JSON.stringify(obj)
来源：http://hz.zhongyouzk.top/gtoeevpunk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yuanzhike.top/gtftmufyzj.html

Go:   json.Marshal(obj)
来源：http://hz.cashguo.top/gtolahjkoc.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.havefunace.top/gtmfkmoqqw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yongpay.top/gtqyvsvkut.html

[K02] JSON 字符串转对象
来源：http://hz.zhiwuduotai.top/gtmglkvrya.html

Py:   json.loads(s)
来源：http://hz.aibaodan.cn/gtuddknpue.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yanxiufei.cn/gtoydrvsdi.html

JS:   JSON.parse(s)
来源：http://hz.svipenyu.cn/gtpejclvzm.html

TS:   JSON.parse(s)
来源：http://hz.zhixingplan.top/gtydxfkryp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.havefunace.top/gtruotqrxc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.9152youxi.cn/gtbxymlfyk.html

Ruby: JSON.parse(s)
来源：http://hz.zhiwuduotai.top/gtgdrpanwh.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.gotoacloud.top/gtsruyliwf.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.guowangkeji.top/gtxlamwakn.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.tian-w.cn/gtnsuxqnfc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.aizwys.cn/gtxcghebhw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.cheryme.top/gttfglhbgw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cucudq.cn/gtdmzlqcpz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jinqigfzy.top/gtatiwtwcb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hnqzz.top/gtjpwjcjto.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yuxming.cn/gtzuidurjb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yuanzhike.top/gthzaybpaf.html

[K04] 读取 JSON 文件
来源：http://hz.yanxiufei.cn/gtjlycecnh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hysaishi.cn/gtygeqstco.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yonumen.top/gtakroekwf.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sxryk.cn/gtcvwvqztc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cucudq.cn/gteiuvscsr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.guowangkeji.top/gtcoppqhdp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhoulong.xyz/gtfqsqlrvw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.kuanghao11.cn/gtkfnpqxay.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ehwqpu.com/gtyimrfxez.html

[K05] 深拷贝对象
来源：http://hz.yangfankeji.com/gttzfcchjq.html

Py:   copy.deepcopy(obj)
来源：http://hz.316326.xyz/gthnrrerov.html

PHP:  unserialize(serialize($obj));
来源：http://hz.daria6918.cn/gtclsapbkt.html

JS:   structuredClone(obj)
来源：http://hz.andypj.xyz/gtuvyeikct.html

TS:   structuredClone(obj)
来源：http://hz.wangshuangyany.cn/gthecktjnr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hywenlv.cn/gtcvcgmufr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.pycfn.com/gtguvdeyvf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ywan-chungtsiang.top/gtzdkrgphl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhijiandao.cn/gtsxhkhicu.html

[K06] 解析 URL 查询串
来源：http://hz.yj202588.top/gtrdacdowr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.birdmap.top/gtwabuguur.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.svipenyu.cn/gtkwmetnjg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.dianchejie.cn/gtffhijbmv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.dashuyun.cn/gtypovrjau.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jinqigufen.top/gtqrccnarg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jinghuilouyu.cn/gteogasdxh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.havefunace.top/gtfclsjpmq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.nwbrower.top/gtdyusykkj.html

[K07] 进制转换
来源：http://hz.zhaomingkeji.xyz/gtaydjztjk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.dashuyun.cn/gtrjaekyou.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.52xcode.cn/gtbvdqkaoa.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.dianchejie.cn/gtozfzocrv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yonumen.top/gtjjhezlth.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cucudq.cn/gtgwkrgljq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.sxryk.cn/gtqreawdgk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xinyue.icu/gtymnvhudu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jlsjyb.cn/gtrlitlxxd.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhiwuduotai.top/gtcgvdwjie.html

Py:   pickle.dumps(obj)
来源：http://hz.dashuyun.cn/gtjkfpwfid.html


<!-- 参考信息 -->