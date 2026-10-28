代发 wailian999

[H03] 主动抛出异常
来源：http://hz.hammf.cn/gttebnwvhh.html

Py:   raise ValueError("错误信息")
来源：http://hz.xinyue.icu/gtztdokhjf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.c1oappe.top/gtganjokta.html

JS:   throw new Error("错误信息");
来源：http://hz.haohaochexian.top/gttlvtdgou.html

TS:   throw new Error("错误信息");
来源：http://hz.smart0.xyz/gtzmxzhcbv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.gotoacloud.top/gtnqhruvad.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.dashuyun.cn/gtwkuhtekz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xuetiantiany.cn/gtixazvwnt.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.pycfn.com/gtplrxaljt.html

[H04] 自定义异常类型
来源：http://hz.xingfuxueyuan.xyz/gtgxfddyyx.html

Py:   class MyError(Exception): pass
来源：http://hz.shzxlz.cn/gtjofhkvvd.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hongshengwenyu.top/gtjhvrpwdg.html

JS:   class MyError extends Error {}
来源：http://hz.aibaodan.cn/gtkxtardve.html

TS:   class MyError extends Error {}
来源：http://hz.xingfuxueyuan.xyz/gthqosnfbz.html

Java: class MyException extends RuntimeException {}
来源：http://hz.shuidangran.top/gtwblnqlfh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.xuanzx.com/gthvqggqkz.html

Ruby: class MyError < StandardError; end
来源：http://hz.xuanzx.com/gtxbfkvzdi.html

C#:   class MyException : Exception {}
来源：http://hz.hfpthk.cn/gtxoeaemai.html

[H05] 捕获特定类型
来源：http://hz.xuetiantiany.cn/gtdrmzhogw.html

Py:   except ValueError as e:
来源：http://hz.ydzc1.top/gtrglvhrvj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.chenzaomai.com/gtpglboiny.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ehwqpu.com/gtdastegct.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.gaohongyu789.top/gtgdsnjoqu.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.fengsongda.top/gtlublaujl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.snrcjt.cn/gtrtmwujjn.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhongyouzk.top/gtcnfdhtyg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.gogol.net.cn/gtxmrogrbr.html

[H06] 可选值 / 空值安全访问
来源：http://hz.mhx1999.top/gtlcafmtar.html

Py:   value = d.get("k") or default
来源：http://hz.andypj.xyz/gtyctzakgl.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.aibaodan.cn/gtqhoowfxp.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.chenlongwang.top/gtycpewvcb.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jinghuilouyu.cn/gtwiuuqlrp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhengqikj.top/gtjyejgnpx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.pycfn.com/gtwaprsada.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zycfv.cn/gtlalwurqu.html

C#:   obj?.A?.B ?? default
来源：http://hz.sufxvd.cn/gtgbpjamhc.html

[H07] 断言
来源：http://hz.shanyushiyangkeji.top/gtdgjbvkkn.html

Py:   assert x > 0, "必须为正"
来源：http://hz.shzxlz.cn/gtacibuwoi.html

PHP:  assert($x > 0);
来源：http://hz.fengsongda.top/gtsqkzsjyr.html

JS:   console.assert(x > 0);
来源：http://hz.52xcode.cn/gtttlidqih.html

TS:   console.assert(x > 0);
来源：http://hz.zycfv.cn/gtbooqftsf.html

Java: assert x > 0 : "必须为正";
来源：http://hz.hnxiangtu.top/gtjmbkxzua.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.shanyushiyangtech.top/gthghdfpzn.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ppjwa.cn/gtwvllwwjb.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhiwuduotai.top/gtkdzmnodw.html

[H08] 获取错误信息与堆栈
来源：http://hz.jianghu66.top/gtghcejbug.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jyoumei.cn/gtshqkymvo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zycfv.cn/gtckbetkya.html

JS:   e.message;  e.stack
来源：http://hz.hysaishi.cn/gtaafmmgut.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jiagoushi.top/gttwilfmnr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.0kj1m.cn/gtnrowixtu.html

Go:   err.Error()
来源：http://hz.zhengqikj.top/gtvbsuufqp.html

Ruby: e.message;  e.backtrace
来源：http://hz.jqgufenzy.top/gtpsywbwls.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhoulong.xyz/gttycaydxb.html

[H09] 带错误码的异常
来源：http://hz.quarkkingdee.top/gtxknaggqh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.ehwqpu.com/gtmztstpun.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yueranfly.top/gtblixvvix.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.bjfxy.top/gtlxpbxckj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhongyouzk.top/gtwucatthj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.chenzaomai.com/gtqkxcsvbi.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.haohaochexian.top/gtykdfxike.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhixingplan.top/gtxknfhhpi.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhixingplan.top/gtjadbfhvz.html

[H10] 资源自动释放
来源：http://hz.shzxlz.cn/gtelawqqvo.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.smart0.xyz/gtybttxste.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yj202588.top/gthjxicrmp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinqigufen.top/gtoobkgjlt.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gaohongyu789.top/gtrepznhxl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ppjwa.cn/gtasxdgoho.html

Go:   defer f.Close()
来源：http://hz.hammf.cn/gtcpvqdqkt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.9152youxi.cn/gtmhfsjgko.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hnxiangtu.top/gtukkpykag.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtrjpjmrwv.html

I. 正则表达式
来源：http://hz.redwolf501.top/gtkpfzvaib.html

================================================================================
来源：http://hz.hammf.cn/gtmqggskvg.html

[I01] 判断是否匹配
来源：http://hz.gzhubu.top/gtauxglshd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.smart0.xyz/gtrtwmhvvr.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.nanxinkj.top/gtyflkjnqo.html

JS:   /\d+/.test(s)
来源：http://hz.wangdashe.top/gtlbznrahz.html

TS:   /\d+/.test(s)
来源：http://hz.chenlongwang.top/gtyickylzf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.kuanghao11.cn/gtykslvkya.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hysaishi.cn/gtyhzwszra.html

Ruby: s.match?(/\d+/)
来源：http://hz.quarkkingdee.top/gtezfdghsm.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.sweek.top/gtfcojlgnd.html

[I02] 提取所有匹配
来源：http://hz.daxiang520.top/gtrxctefok.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ydzc1.top/gtscfcgflg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xziqi.cn/gtyacnisvm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.wangshuangyany.cn/gteidbqohd.html

TS:   s.match(/\d+/g)
来源：http://hz.yuxming.cn/gtxddfclmb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.daxiang520.top/gtgqjksypd.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.tianlin.xyz/gtfjaupvon.html

Ruby: s.scan(/\d+/)
来源：http://hz.yonumen.top/gtxmvnlnsq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.dashuyun.cn/gtnaoteliu.html

[I03] 提取捕获分组
来源：http://hz.meibo888.top/gteacziuiz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.52xcode.cn/gtknfgpljn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.gaohongyu789.top/gtxpsydgyc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.pengpengdd.cyou/gttuiuigyq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.sysykeji.top/gtsapgqpan.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.ydzc1.top/gtgpimntta.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.nanxinkj.top/gtctgsqzzj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hnqzz.top/gtswcjfaye.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.birdmap.top/gtauqfysjs.html

[I04] 正则替换
来源：http://hz.shangyingyoupin.top/gtlnpesplf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.tian-w.cn/gtvtnfiiuq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jyoumei.cn/gtrkdcfgko.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.pengpengdd.cyou/gtcfxksfth.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.cucudq.cn/gtnvpigijy.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhixingplan.top/gtcqnktnme.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.wangdashe.top/gtgajyfcze.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.nwbrower.top/gtnteqtlsn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.pycfn.com/gtkjozgbqe.html

[I05] 按正则拆分
来源：http://hz.vqdsnc.cn/gtfeugeleh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.gotoacloud.top/gtmehxqguo.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jlsjyb.cn/gteintnrua.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.bjfxy.top/gtdyztdypk.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.gogol.net.cn/gteysaugwr.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jianghu66.top/gtmgdpcgyg.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.shanyushiyangtech.top/gttnjsobcu.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.pengpengdd.cyou/gtscksppzz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhiwuduotai.top/gtjfatschq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.gzhubu.top/gtswrjbzju.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yueranfly.top/gtdflzmjxq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.nwbrower.top/gtujjvzevk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gotoacloud.top/gtuicpmvix.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yj20258888.top/gtcklhuyme.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.wangshuangyany.cn/gtmbgldkjj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hongshengwenyu.top/gtcfrdppti.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.daria6918.cn/gtoklwgwkv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.316326.xyz/gtjwuwwybk.html

[I07] 忽略大小写与多行模式
来源：http://hz.yuxming.cn/gtupofvwjw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ybcxt.top/gtjffoninq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.chenlongwang.top/gtqhyhaoca.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhaomingkeji.xyz/gtdcwnpkqx.html

TS:   /error/gim
来源：http://hz.cqqwz.cn/gtqpzrifja.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.haohaochexian.top/gtddlkxhrs.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhengqikj.top/gtskbtzrti.html

Ruby: s.scan(/error/i)
来源：http://hz.birdmap.top/gtckdbdzhn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ivvv.top/gthkdrhcur.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.haohaochexian.top/gtqnchzeue.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yanxiufei.cn/gttldyneab.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cqqwz.cn/gtjjrsrrxg.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.chenlongwang.top/gtdvvzxjyi.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yonumen.top/gttmeyfjja.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.guannengcc.top/gtabepheon.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.daxiang520.top/gtkrhbrxpi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.xylfe.cn/gtwwtttwqh.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.gogol.net.cn/gtztpjzfnh.html

================================================================================
来源：http://hz.yongpay.top/gtdmhljikq.html

J. 日期与时间
来源：http://hz.yongpay.top/gtcrklpmwx.html

================================================================================
来源：http://hz.aibaodan.cn/gtvirlqpwy.html

[J01] 获取当前时间
来源：http://hz.gzhubu.top/gtnntzqqyy.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.haohaochexian.top/gtexwqwmei.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.shangyingyoupin.top/gtedqjcfso.html

JS:   new Date();  Date.now()
来源：http://hz.quarkkingdee.top/gtogzlglbs.html

TS:   new Date();  Date.now()
来源：http://hz.sysykeji.top/gtbkfvhczh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.nanxinkj.top/gtorogoqyv.html

Go:   time.Now()
来源：http://hz.guannengcc.top/gtfqnxnuig.html

Ruby: Time.now
来源：http://hz.yuxming.cn/gtesfvnzvo.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.tian-w.cn/gtoxjgeegw.html

[J02] 格式化输出
来源：http://hz.zhoulong.xyz/gtyknfecnz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sufxvd.cn/gtwtrxdugr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.316326.xyz/gtzveorcsn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yueranfly.top/gtvwicgage.html

TS:   d.toISOString()
来源：http://hz.9152youxi.cn/gtrtpcccou.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhoulong.xyz/gtbybfzfto.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jinghuilouyu.cn/gtysflbamw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.dianchejie.cn/gtkqbwdtih.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yuanzhike.top/gtxhanslks.html

[J03] 字符串解析为日期
来源：http://hz.xinyue.icu/gtpgzzknsa.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yongpay.top/gtialccyzj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.gzhubu.top/gtvilkhhdn.html

JS:   new Date("2024-01-02")
来源：http://hz.meibo888.top/gtqprnrtys.html

TS:   new Date("2024-01-02")
来源：http://hz.birdmap.top/gtaudrrtue.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.nanxuanxn.top/gtctgueedz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yanxiufei.cn/gtlpnogkbe.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ybcxt.top/gtrcgaxqkc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jqgufenzy.top/gtlacjunfg.html

[J04] 时间戳与日期互转
来源：http://hz.shuidangran.top/gtukhdiuyp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.dashuyun.cn/gtzduqlszf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.tianlin.xyz/gtcrxkgzjb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.xziqi.cn/gtjhxokucd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.nanxinkj.top/gtzfqhajvd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.smart0.xyz/gtxkzdpsvn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.ehwqpu.com/gtfojzbmst.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.sysykeji.top/gtyastfbbb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.wangshuangyany.cn/gtfutyingl.html

[J05] 时间加减（加 7 天）
来源：http://hz.svipenyu.cn/gtbmrjopic.html

Py:   now + timedelta(days=7)
来源：http://hz.cqqwz.cn/gtmiusldsx.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shuidangran.top/gtmprpsayt.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shuidangran.top/gtwlhzrudk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sufxvd.cn/gtobdwcrgc.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.shuidangran.top/gtklndknmj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xuanzx.com/gtowryqqti.html

Ruby: Time.now + 7 * 86400
来源：http://hz.daria6918.cn/gtlldaiyyv.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.tian-w.cn/gtzfppesru.html

[J06] 计算两时间之差
来源：http://hz.zhoulong.xyz/gtchjmudou.html

Py:   (end - start).total_seconds()
来源：http://hz.ivvv.top/gtrfpiahsl.html

PHP:  $end->diff($start)->days;
来源：http://hz.chenzaomai.com/gtpiyiqlpu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.sxryk.cn/gtmczcefeb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.daria6918.cn/gtgjvipmbo.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ppjwa.cn/gteirzfehw.html

Go:   end.Sub(start).Hours()
来源：http://hz.iojbl.cn/gtkslutboq.html

Ruby: end - start                 # 返回秒数
来源：http://hz.dashuyun.cn/gtymwwutou.html

C#:   (end - start).TotalSeconds
来源：http://hz.jqgfzy.top/gtgisyitdj.html

[J07] 比较两个日期
来源：http://hz.hywenlv.cn/gtorpldopp.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.sufxvd.cn/gtydecifxx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hfpthk.cn/gtsvbrrxhe.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.iojbl.cn/gtstbsaxuo.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yueranfly.top/gtarjbrwyk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hongshengwenyu.top/gtiphihbcv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.shangyingyoupin.top/gtlwqvhgcq.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.meibo888.top/gtfqahbxmr.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.guannengcc.top/gtefelmbha.html

[J08] 提取年月日与星期
来源：http://hz.52xcode.cn/gtmxwjdqzj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.shzxlz.cn/gtyrhvyehj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yangfankeji.com/gtuwbubfmh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shzxlz.cn/gtaebnonlp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.sufxvd.cn/gtydblxlol.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.52xcode.cn/gtsjpktlbk.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yongpay.top/gtuhvorica.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cdnleiting.top/gtoffgpooe.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.mhx1999.top/gtuckzvvcz.html

[J09] 时区处理
来源：http://hz.guannengcc.top/gtszamownz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shanyushiyangkeji.top/gtyhgxbnai.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.c1oappe.top/gtbohvyfvj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.aibaodan.cn/gtgqagxmnl.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinqigfzy.top/gtfjrlohmz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hysaishi.cn/gtltznokgv.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.nanxuanxn.top/gtxozywlga.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hammf.cn/gtrernqngk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shuidangran.top/gtdmlbzanc.html

[J10] 取今天 / 本月第一天
来源：http://hz.ydzc1.top/gtachychdn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.tanke756.top/gtbtfzoluy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.shangyingyoupin.top/gtcxwwjzns.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.chenlongwang.top/gtkhxwetbm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cucudq.cn/gtyaceodmc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.svipenyu.cn/gtagnjyzyy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yueranfly.top/gtfqqrcffm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yj20258888.top/gttqylegwx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.iojbl.cn/gtdhpbqyvd.html

================================================================================
来源：http://hz.jyoumei.cn/gtuenybqyw.html

K. JSON 与序列化
来源：http://hz.mhx1999.top/gtjnqqayme.html

================================================================================
来源：http://hz.redwolf501.top/gtqogvndrp.html

[K01] 对象转 JSON 字符串
来源：http://hz.bjfxy.top/gtenbgoeed.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zhengqikj.top/gtpexamyqu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.chenjidiqi.icu/gtgcxjnafh.html

JS:   JSON.stringify(obj)
来源：http://hz.cdnleiting.top/gtslfzkwxn.html

TS:   JSON.stringify(obj)
来源：http://hz.sufxvd.cn/gtrjxgnros.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.gotoacloud.top/gtfmlnmidy.html

Go:   json.Marshal(obj)
来源：http://hz.zycfv.cn/gtrnislrlk.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yonumen.top/gtafiiyedu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.quarkkingdee.top/gttsvxbgwm.html

[K02] JSON 字符串转对象
来源：http://hz.redwolf501.top/gtsnhoofky.html

Py:   json.loads(s)
来源：http://hz.wangshuangyany.cn/gtbyadnkfr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.tian-w.cn/gtrwgqtlix.html

JS:   JSON.parse(s)
来源：http://hz.cqqwz.cn/gtfthptoce.html

TS:   JSON.parse(s)
来源：http://hz.vqdsnc.cn/gtaadihnyg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.9152youxi.cn/gtohttefwb.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ybcxt.top/gtpnuwdysc.html

Ruby: JSON.parse(s)
来源：http://hz.jqgfzy.top/gttbphctst.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.smart0.xyz/gtepobpgwf.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ybcxt.top/gtpqublkkj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jyoumei.cn/gtjyerqvlw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yangfankeji.com/gtucobpepb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.gzhubu.top/gtckxolcsa.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xinyue.icu/gthxnfjlpy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yj20258.top/gthpmnsaxb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.gogol.net.cn/gtuqzezuhc.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.gogol.net.cn/gtedswewsm.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.redwolf501.top/gtushxakup.html

[K04] 读取 JSON 文件
来源：http://hz.yongpay.top/gtxmmdlgiu.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.svipenyu.cn/gtcnpogbqm.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.svipenyu.cn/gtfekicjed.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.nanxinkj.top/gtblzezpxk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhoulong.xyz/gtopucuxzt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.cheryme.top/gtwywkjwly.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.quarkkingdee.top/gtmggbqmyi.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yj20258888.top/gtahiwfwyy.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.pengpengdd.cyou/gtclwwtilx.html

[K05] 深拷贝对象
来源：http://hz.ivvv.top/gtgwvyrlkc.html

Py:   copy.deepcopy(obj)
来源：http://hz.gotoacloud.top/gtcjnawxnj.html

PHP:  unserialize(serialize($obj));
来源：http://hz.shangyingyoupin.top/gtgvwbzohl.html

JS:   structuredClone(obj)
来源：http://hz.vqdsnc.cn/gtctrvjvfk.html

TS:   structuredClone(obj)
来源：http://hz.cashguo.top/gtkcbvxznd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.haohaochexian.top/gtrljgoeec.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xylfe.cn/gtxxsukqrw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.guowangkeji.top/gtskffdqgb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.gogol.net.cn/gtbfuppnzq.html

[K06] 解析 URL 查询串
来源：http://hz.quarkkingdee.top/gthfgdxppp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.tanke756.top/gtodnuqxbw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.dianchejie.cn/gtcfgrgrzp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nanxuanxn.top/gtlqxzkzdi.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.redwolf501.top/gtulnqnpro.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yongpay.top/gtwrgmvxrk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.dashuyun.cn/gtzhdnhwxj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.andypj.xyz/gtkfgsxlog.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jinqigufen.top/gtgaxovzgv.html

[K07] 进制转换
来源：http://hz.nwbrower.top/gtgbpkatkd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.quarkkingdee.top/gtlvrkuazk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhijiandao.cn/gtvfhhlpcs.html


<!-- 参考信息 -->