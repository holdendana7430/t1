代发 wailian999

JS:   class MyError extends Error {}
来源：http://hz.haohaochexian.top/gtikfprbir.html

TS:   class MyError extends Error {}
来源：http://hz.kuanghao11.cn/gtwdseguey.html

Java: class MyException extends RuntimeException {}
来源：http://hz.gotoacloud.top/gtmnoonovw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jinqigufen.top/gtjxafcdhb.html

Ruby: class MyError < StandardError; end
来源：http://hz.yueranfly.top/gtdksxquil.html

C#:   class MyException : Exception {}
来源：http://hz.daxiang520.top/gtxcmzkwgt.html

[H05] 捕获特定类型
来源：http://hz.tian-w.cn/gtnxvopisv.html

Py:   except ValueError as e:
来源：http://hz.svipenyu.cn/gtaighrszm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.sysykeji.top/gtvwrgiora.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xuetiantiany.cn/gtcwvfgzlg.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.nwbrower.top/gtrdixcsyb.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.vqdsnc.cn/gtbdjnsdzv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhongyouzk.top/gtsjijkdva.html

Ruby: rescue ArgumentError => e
来源：http://hz.ivvv.top/gtxzfgxogb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.cucudq.cn/gtrxvpkrcn.html

[H06] 可选值 / 空值安全访问
来源：http://hz.chenjidiqi.icu/gtbxysfxnc.html

Py:   value = d.get("k") or default
来源：http://hz.redwolf501.top/gtmxhezbtg.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.wangdashe.top/gtckaiaujf.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jinqigfzy.top/gtbomkwuxg.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hysaishi.cn/gtjmzahlyl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.sxryk.cn/gtfwglzglw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.shuidangran.top/gtwaktftoh.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jinqigfzy.top/gtyjmlohdv.html

C#:   obj?.A?.B ?? default
来源：http://hz.haohaochexian.top/gtebzjmihp.html

[H07] 断言
来源：http://hz.xylfe.cn/gtysecgqqf.html

Py:   assert x > 0, "必须为正"
来源：http://hz.shangyingyoupin.top/gtmukhwkdw.html

PHP:  assert($x > 0);
来源：http://hz.aizwys.cn/gtanfjwnzt.html

JS:   console.assert(x > 0);
来源：http://hz.zhiwuduotai.top/gtohhnxzbp.html

TS:   console.assert(x > 0);
来源：http://hz.xingfuxueyuan.xyz/gtyogtlfan.html

Java: assert x > 0 : "必须为正";
来源：http://hz.hysaishi.cn/gtswggugwy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.meibo888.top/gtmfxzsnkv.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jinqigufen.top/gtilxiarwu.html

C#:   Debug.Assert(x > 0);
来源：http://hz.meibo888.top/gtupxwtevo.html

[H08] 获取错误信息与堆栈
来源：http://hz.sysykeji.top/gtfeidsuyl.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zhiwuduotai.top/gtyrlbjwgt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yonumen.top/gtzzrouvwq.html

JS:   e.message;  e.stack
来源：http://hz.gotoacloud.top/gthfllijxq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.gogol.net.cn/gtimlrtkdq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.svipenyu.cn/gtlvvjipgj.html

Go:   err.Error()
来源：http://hz.wangshuangyany.cn/gtuekewvrg.html

Ruby: e.message;  e.backtrace
来源：http://hz.xuetiantiany.cn/gtaxuniibq.html

C#:   e.Message;  e.StackTrace
来源：http://hz.gogol.net.cn/gtkaqtehwu.html

[H09] 带错误码的异常
来源：http://hz.hnxiangtu.top/gtyimitivb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.andypj.xyz/gttistbzil.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.sxryk.cn/gtrtllgdoe.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.shuidangran.top/gtuvljurnb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.9152youxi.cn/gtlmxbjauy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.fengsongda.top/gtqqiafrud.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.daria6918.cn/gtpogqbioy.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.cashguo.top/gtcrlwuhtm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.cashguo.top/gtwelgoeou.html

[H10] 资源自动释放
来源：http://hz.dianchejie.cn/gtzxhrisgk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.sysykeji.top/gtanncmjxw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.shanyushiyangkeji.top/gtljegilym.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.aibaodan.cn/gtkyoxalwb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.iojbl.cn/gtumkfecwl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.pengpengdd.cyou/gtystcyfow.html

Go:   defer f.Close()
来源：http://hz.hnxiangtu.top/gtuebbrclq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zhixingplan.top/gtrljfwcxo.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ydzc1.top/gtgxdjiotq.html

================================================================================
来源：http://hz.dianchejie.cn/gtkaakjdgo.html

I. 正则表达式
来源：http://hz.havefunace.top/gtwvkmaitt.html

================================================================================
来源：http://hz.cqqwz.cn/gtnnoqefys.html

[I01] 判断是否匹配
来源：http://hz.c1oappe.top/gtxxfconkb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xinyue.icu/gtqdgoixak.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.tianlin.xyz/gtlcwudvoj.html

JS:   /\d+/.test(s)
来源：http://hz.birdmap.top/gtvcbaqfhd.html

TS:   /\d+/.test(s)
来源：http://hz.guowangkeji.top/gtrnkbcaww.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.gaohongyu789.top/gtyyuvrmxg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jqgufenzy.top/gtjoekxmft.html

Ruby: s.match?(/\d+/)
来源：http://hz.guannengcc.top/gttqibghqb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.shzxlz.cn/gtkxhwmrhm.html

[I02] 提取所有匹配
来源：http://hz.kuanghao11.cn/gtqqrwmywg.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ywan-chungtsiang.top/gtlaufoxbx.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jinqigfzy.top/gtahwxihur.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.gotoacloud.top/gtxwsjijpc.html

TS:   s.match(/\d+/g)
来源：http://hz.zhijiandao.cn/gtjfntmrek.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zhixingplan.top/gtnyjndpqj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.birdmap.top/gtcezxqsxv.html

Ruby: s.scan(/\d+/)
来源：http://hz.chenjidiqi.icu/gtvozdpbtu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.svipenyu.cn/gtupohilwh.html

[I03] 提取捕获分组
来源：http://hz.xylfe.cn/gtaffqyddg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yj20258.top/gtlyiuqaiu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.daria6918.cn/gtgewzzkwn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.shuidangran.top/gtdbphjxcl.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.c1oappe.top/gtrrhbsyos.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.andypj.xyz/gtfkzfslva.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yonumen.top/gtsgnjmtij.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.shzxlz.cn/gtmyyytmjn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yuanzhike.top/gtmsikqtfv.html

[I04] 正则替换
来源：http://hz.tianlin.xyz/gtnaglrphp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.shzxlz.cn/gtetzfmmxd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.andypj.xyz/gthgrwyshv.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yueranfly.top/gtazyfjjvi.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hammf.cn/gtuxlghtks.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.gogol.net.cn/gtcmhxegbi.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yj20258888.top/gtnxaxmhdi.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhaomingkeji.xyz/gtlicpcers.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hywenlv.cn/gtrzdcnejg.html

[I05] 按正则拆分
来源：http://hz.daxiang520.top/gtusczheqq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ybcxt.top/gtaawvpqhj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.sysykeji.top/gtyigngkui.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.cucudq.cn/gtlooqjubs.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.daria6918.cn/gtxciykaxt.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yuanzhike.top/gtgxabywbi.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.svipenyu.cn/gtzdkoijna.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhaomingkeji.xyz/gtlqfnqctl.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.tanke756.top/gtqtssuquu.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yuxming.cn/gtlrfkbfcz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.shanyushiyangkeji.top/gtjlifdijq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.chenjidiqi.icu/gtvmaugbdu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hongshengwenyu.top/gtfnnzijle.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sweek.top/gtpzhwjxgr.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.cheryme.top/gtwdbifsdp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.kuanghao11.cn/gtwnnpwtyb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jinyuanbaomall.cn/gttxpguaxk.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.aibaodan.cn/gtrbkalmye.html

[I07] 忽略大小写与多行模式
来源：http://hz.ehwqpu.com/gtkzrxsrya.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ydzc1.top/gtgciwipel.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.cashguo.top/gtnjgkkzcc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.316326.xyz/gtpmkwoaxr.html

TS:   /error/gim
来源：http://hz.nanxinkj.top/gtikdtwopq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ivvv.top/gtnxrrmltq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jyoumei.cn/gtgkefpihu.html

Ruby: s.scan(/error/i)
来源：http://hz.yanxiufei.cn/gtubwxjgdd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yonumen.top/gtxypoumzy.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.fengsongda.top/gterzitfeq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.hysaishi.cn/gttdlbware.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.dashuyun.cn/gtqppnvgij.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hfpthk.cn/gtzdwrulac.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ybcxt.top/gtjhnvenni.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.meibo888.top/gtzzbxfmvw.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yanxiufei.cn/gttyxuhioe.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.gaohongyu789.top/gtkwsvlvgq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.chenjidiqi.icu/gtrrkcsjil.html

================================================================================
来源：http://hz.cdnleiting.top/gtevioegpt.html

J. 日期与时间
来源：http://hz.xuanzx.com/gtuylhappo.html

================================================================================
来源：http://hz.aibaodan.cn/gtestmswcn.html

[J01] 获取当前时间
来源：http://hz.meibo888.top/gtefbowmbd.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.smart0.xyz/gtdvnrcjar.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.hnqzz.top/gtlhwsivhr.html

JS:   new Date();  Date.now()
来源：http://hz.jlsjyb.cn/gtdmomtczq.html

TS:   new Date();  Date.now()
来源：http://hz.chenzaomai.com/gtytpjibwi.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jianghu66.top/gtztubfdji.html

Go:   time.Now()
来源：http://hz.wangdashe.top/gtfbzjmypg.html

Ruby: Time.now
来源：http://hz.xziqi.cn/gtsvnpthnq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ybcxt.top/gtwsomjnul.html

[J02] 格式化输出
来源：http://hz.ydjk.org.cn/gtevfeqoth.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cdnleiting.top/gtevlxwbpk.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.snrcjt.cn/gtxxqgidym.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ywan-chungtsiang.top/gtlzjljkyg.html

TS:   d.toISOString()
来源：http://hz.xylfe.cn/gtcmdfxosp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhixingplan.top/gtieokgcok.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.shangyingyoupin.top/gtscblhgfw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.quarkkingdee.top/gtsawbsteq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.daxiang520.top/gtxgtvwmtm.html

[J03] 字符串解析为日期
来源：http://hz.feifeiyinyue.top/gtuvrymxnl.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jqgfzy.top/gtepvhbcjc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.shanyushiyangtech.top/gtjrldnewi.html

JS:   new Date("2024-01-02")
来源：http://hz.yuanzhike.top/gtevbdqyqk.html

TS:   new Date("2024-01-02")
来源：http://hz.yueranfly.top/gtyamnisin.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.guowangkeji.top/gtkwojfwif.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.guannengcc.top/gtfgwykndv.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhengqikj.top/gtnwtdvivd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.sufxvd.cn/gtfbwagsgr.html

[J04] 时间戳与日期互转
来源：http://hz.chenjidiqi.icu/gtarzvgagh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.c1oappe.top/gtidncojxb.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.feifeiyinyue.top/gtvcxduame.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zhongyouzk.top/gtremgphkm.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.chenjidiqi.icu/gtegerkvob.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.daria6918.cn/gtbeeszvhy.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yongpay.top/gtxzepwqmx.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hfpthk.cn/gtwzfjsmun.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.shuidangran.top/gtbbwpbnqg.html

[J05] 时间加减（加 7 天）
来源：http://hz.iojbl.cn/gtogrwaqnt.html

Py:   now + timedelta(days=7)
来源：http://hz.ydzc1.top/gtsxzoyidc.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shuidangran.top/gtnwwwwvdp.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.bjfxy.top/gtjshkayyp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xziqi.cn/gthpgwzbjf.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yueranfly.top/gtabazgvtr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ehwqpu.com/gtmrkzsgef.html

Ruby: Time.now + 7 * 86400
来源：http://hz.guowangkeji.top/gtfhrifywj.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xziqi.cn/gtpnrphqwx.html

[J06] 计算两时间之差
来源：http://hz.xziqi.cn/gtvtwazemd.html

Py:   (end - start).total_seconds()
来源：http://hz.gotoacloud.top/gtrclkjuoa.html

PHP:  $end->diff($start)->days;
来源：http://hz.chenzaomai.com/gtlqcgwnwg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.iojbl.cn/gtmhvpesid.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.kuanghao11.cn/gtwknkrido.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cdnleiting.top/gtwdqymcxm.html

Go:   end.Sub(start).Hours()
来源：http://hz.sysykeji.top/gtbpijxerm.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jqgufenzy.top/gtbdwbzrhm.html

C#:   (end - start).TotalSeconds
来源：http://hz.shanyushiyangtech.top/gthsuklird.html

[J07] 比较两个日期
来源：http://hz.yj20258.top/gtvrtgqsnz.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhengqikj.top/gtdqttgpqb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yuxming.cn/gtyczibfzn.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.tanke756.top/gtvolchyen.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.chenlongwang.top/gtvwfxnyge.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yuanzhike.top/gtwbrztvvp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.9152youxi.cn/gtasdkraso.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.daria6918.cn/gtilwzpnza.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.316326.xyz/gtskiqrntj.html

[J08] 提取年月日与星期
来源：http://hz.jqgufenzy.top/gthxdvygnh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zdqjudy.top/gtcvoymxwa.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xuetiantiany.cn/gtyrueevrl.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yonumen.top/gtkmttlubk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.guowangkeji.top/gtoneoewgj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yueranfly.top/gtdhofinfy.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.fengsongda.top/gtxeabmvtf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hongshengwenyu.top/gtsbtwtskp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hammf.cn/gtybojutek.html

[J09] 时区处理
来源：http://hz.jinqigfzy.top/gtwpaonxnj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jinqigfzy.top/gtfgxbkfna.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yueranfly.top/gtnmzgdfqx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xuetiantiany.cn/gtqrdumeuv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.redwolf501.top/gtsvpyqqfn.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.snrcjt.cn/gtmwqkbzmk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.shanyushiyangtech.top/gtadzhskkq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hongshengwenyu.top/gtfhtsshll.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yj20258888.top/gtdipcgotk.html

[J10] 取今天 / 本月第一天
来源：http://hz.dashuyun.cn/gtjgixpbtr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.tian-w.cn/gtccnfrqog.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hongshengwenyu.top/gtcwjobrns.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.havefunace.top/gtkxxghpfg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jlsjyb.cn/gtdupuabfd.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.bjfxy.top/gtkfzlzuvd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.chenjidiqi.icu/gtxaqzbvkj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.316326.xyz/gtyfjlhwge.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.daria6918.cn/gtxdgvzckf.html

================================================================================
来源：http://hz.xziqi.cn/gttlxbfxwf.html

K. JSON 与序列化
来源：http://hz.zhengqikj.top/gtwwngupdr.html

================================================================================
来源：http://hz.xuanzx.com/gtnmyzckof.html

[K01] 对象转 JSON 字符串
来源：http://hz.hfpthk.cn/gtwtlgmwyh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ybcxt.top/gtzofrvgqm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhixingplan.top/gtwwfbaupo.html

JS:   JSON.stringify(obj)
来源：http://hz.xziqi.cn/gtijcpfjfh.html

TS:   JSON.stringify(obj)
来源：http://hz.cheryme.top/gtnvvbjawt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xuanzx.com/gtphxlyoje.html

Go:   json.Marshal(obj)
来源：http://hz.sxryk.cn/gtxckwocvb.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.daria6918.cn/gtfnbqehve.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.c1oappe.top/gtlkalkuoh.html

[K02] JSON 字符串转对象
来源：http://hz.yangfankeji.com/gtpcphotpz.html

Py:   json.loads(s)
来源：http://hz.haohaochexian.top/gtmuejnxhn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.xuetiantiany.cn/gtvdcniiry.html

JS:   JSON.parse(s)
来源：http://hz.shangyingyoupin.top/gtpdivtuwx.html

TS:   JSON.parse(s)
来源：http://hz.havefunace.top/gtilbtfdrf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.kuanghao11.cn/gtsucpuwyp.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.sysykeji.top/gteslbtjbd.html

Ruby: JSON.parse(s)
来源：http://hz.haohaochexian.top/gtwhypobvz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xingfuxueyuan.xyz/gtjenxoost.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ybcxt.top/gtagkmirkr.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.aibaodan.cn/gtnjqmqvhj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yj20258.top/gtvozuzsnz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.daria6918.cn/gtnkzhaxwa.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xylfe.cn/gtwqkyyuxt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.xinyue.icu/gtizouhaoa.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.shuidangran.top/gtalnqzaej.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.shanyushiyangkeji.top/gthzliovge.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.sufxvd.cn/gtlpbqpqbi.html

[K04] 读取 JSON 文件
来源：http://hz.xingfuxueyuan.xyz/gtjmiwikdq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.mhx1999.top/gtyakjcpyl.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.pengpengdd.cyou/gtxbuthhft.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ydjk.org.cn/gtkhgqaqqz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xingfuxueyuan.xyz/gtkazsnbkv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.svipenyu.cn/gtgguzbtzl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.sxryk.cn/gtjwumrajb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.chenjidiqi.icu/gtiupxsmwb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.andypj.xyz/gtjefzkkad.html

[K05] 深拷贝对象
来源：http://hz.wangshuangyany.cn/gttoxiqyoa.html

Py:   copy.deepcopy(obj)
来源：http://hz.52xcode.cn/gtarczluag.html

PHP:  unserialize(serialize($obj));
来源：http://hz.gzhubu.top/gtjrwntada.html

JS:   structuredClone(obj)
来源：http://hz.yongpay.top/gtqfsufogf.html

TS:   structuredClone(obj)
来源：http://hz.hnqzz.top/gtimpnsfhp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhongyouzk.top/gtvmrrkytg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.svipenyu.cn/gtarlknwrd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhaomingkeji.xyz/gtmmdejzwu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.shanyushiyangtech.top/gtjqgxyywu.html

[K06] 解析 URL 查询串
来源：http://hz.xuanzx.com/gtgfzxidkm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jiagoushi.top/gtuwyssibm.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xziqi.cn/gtaemigcsd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zdqjudy.top/gtkkleohrs.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xziqi.cn/gtqfvwfawe.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.chenjidiqi.icu/gtmnxfnzyn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.aizwys.cn/gtezouyofi.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.bjfxy.top/gtuylfeyog.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ydzc1.top/gtadgwkdox.html

[K07] 进制转换
来源：http://hz.zhoulong.xyz/gtnlwymjcg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.snrcjt.cn/gtrdshribi.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jqgufenzy.top/gtopuyfywb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yueranfly.top/gtatqlhfuh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.quarkkingdee.top/gtevdqbgqh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yj20258888.top/gtpwlwhbaq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.cucudq.cn/gtuyjhjuvm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.chenzaomai.com/gttobpjaup.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhongyouzk.top/gtlrhzixcu.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.fengsongda.top/gtlquwaawy.html

Py:   pickle.dumps(obj)
来源：http://hz.meibo888.top/gtyioaojqv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jinghuilouyu.cn/gtvvoiqslg.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shangyingyoupin.top/gtnuvcehnj.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hnqzz.top/gtqhzztlug.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.cdnleiting.top/gtsifzecrv.html


<!-- 参考信息 -->