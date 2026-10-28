代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://hz.nanxinkj.top/gthdkfwjvf.html

[H04] 自定义异常类型
来源：http://hz.daxiang520.top/gtucijfxiq.html

Py:   class MyError(Exception): pass
来源：http://hz.sysykeji.top/gtlkrapozt.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.9152youxi.cn/gtmetxnigw.html

JS:   class MyError extends Error {}
来源：http://hz.zycfv.cn/gthyopxloj.html

TS:   class MyError extends Error {}
来源：http://hz.havefunace.top/gthpgspfqx.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jiagoushi.top/gtgisxiyji.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.sxryk.cn/gttavdjjvw.html

Ruby: class MyError < StandardError; end
来源：http://hz.wangdashe.top/gtwxgpkyjj.html

C#:   class MyException : Exception {}
来源：http://hz.ywan-chungtsiang.top/gtsgyzqhlq.html

[H05] 捕获特定类型
来源：http://hz.mhx1999.top/gtvalrwwya.html

Py:   except ValueError as e:
来源：http://hz.fzhhl.top/gtvoliboxa.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhaomingkeji.xyz/gtxiybvdjg.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhongyouzk.top/gtbtcxlpno.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hnqzz.top/gtdsepptij.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhixingplan.top/gtjytglqjk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.cheryme.top/gtkefdmclk.html

Ruby: rescue ArgumentError => e
来源：http://hz.yuxming.cn/gtfoelanqr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yanxiufei.cn/gtmyctrycf.html

[H06] 可选值 / 空值安全访问
来源：http://hz.gaohongyu789.top/gtynbnlkwi.html

Py:   value = d.get("k") or default
来源：http://hz.sufxvd.cn/gtxuqyhsfk.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.wangshuangyany.cn/gtktxvnusg.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.snrcjt.cn/gtkkvumqzm.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.fengsongda.top/gttyayslpb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jqgufenzy.top/gtpnsswmot.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.hfpthk.cn/gtwjyxfxoy.html

Ruby: d&.dig(:a, :b)
来源：http://hz.chenlongwang.top/gtigszxhfx.html

C#:   obj?.A?.B ?? default
来源：http://hz.pengpengdd.cyou/gtnqtbhtca.html

[H07] 断言
来源：http://hz.andypj.xyz/gtkkuriqfm.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jianghu66.top/gtoredulvg.html

PHP:  assert($x > 0);
来源：http://hz.jqgfzy.top/gtujbetage.html

JS:   console.assert(x > 0);
来源：http://hz.chenlongwang.top/gtviwdjoiy.html

TS:   console.assert(x > 0);
来源：http://hz.yongpay.top/gtrdwrvbkr.html

Java: assert x > 0 : "必须为正";
来源：http://hz.nanxuanxn.top/gthelqzsoj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhixingplan.top/gtlsctaemj.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ppjwa.cn/gtnnuxgpll.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jqgufenzy.top/gtalphuiea.html

[H08] 获取错误信息与堆栈
来源：http://hz.ppjwa.cn/gtryfcogam.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.redwolf501.top/gtoftnqtug.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jqgfzy.top/gtbeupjkkl.html

JS:   e.message;  e.stack
来源：http://hz.zhengqikj.top/gtwpitgbor.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.fengsongda.top/gtdqlrntdr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xinyue.icu/gtihvuhnvg.html

Go:   err.Error()
来源：http://hz.hywenlv.cn/gtdjqhiajw.html

Ruby: e.message;  e.backtrace
来源：http://hz.yj20258888.top/gtwvsjeddm.html

C#:   e.Message;  e.StackTrace
来源：http://hz.xinyue.icu/gtwqrdunmi.html

[H09] 带错误码的异常
来源：http://hz.redwolf501.top/gtbuwiytyq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.316326.xyz/gtkswhjupe.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.pycfn.com/gtjrcsnmej.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.tianlin.xyz/gtkpfdzinf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xylfe.cn/gtekrxydfk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.tianlin.xyz/gtgarehele.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.shanyushiyangtech.top/gtwavzjvlv.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.xziqi.cn/gtiwebdxhp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.nanxinkj.top/gtxdjwtlue.html

[H10] 资源自动释放
来源：http://hz.andypj.xyz/gtbomanmsa.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jlsjyb.cn/gtadjuuurt.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yvedp.cn/gtjjbykcoa.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenzaomai.com/gtcsvdlfkq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.c1oappe.top/gtaasfauch.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.sxryk.cn/gtrwbfpskl.html

Go:   defer f.Close()
来源：http://hz.xziqi.cn/gtmrawfkhm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.pengpengdd.cyou/gtbpliltse.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jqgufenzy.top/gtlwryihln.html

================================================================================
来源：http://hz.sufxvd.cn/gtvkgfthku.html

I. 正则表达式
来源：http://hz.yvedp.cn/gtpylgyaaw.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtphxooyio.html

[I01] 判断是否匹配
来源：http://hz.sweek.top/gtfwltlalq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.gogol.net.cn/gtmnznaxkp.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.bjfxy.top/gtftayqjeo.html

JS:   /\d+/.test(s)
来源：http://hz.tian-w.cn/gtcxppivbt.html

TS:   /\d+/.test(s)
来源：http://hz.0kj1m.cn/gtyyfplvnu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yueranfly.top/gtznnkwxeu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.shanyushiyangtech.top/gtioewnkij.html

Ruby: s.match?(/\d+/)
来源：http://hz.yuanzhike.top/gtxvncelbz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.iojbl.cn/gtzhsovwbz.html

[I02] 提取所有匹配
来源：http://hz.tian-w.cn/gtgohhuonl.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ybcxt.top/gtslmpuwgs.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hnxiangtu.top/gtprytymbm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hongshengwenyu.top/gtqjeynxra.html

TS:   s.match(/\d+/g)
来源：http://hz.ywan-chungtsiang.top/gtthiuwsia.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ywan-chungtsiang.top/gtvgrrurku.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hysaishi.cn/gtmlkngcvu.html

Ruby: s.scan(/\d+/)
来源：http://hz.ehwqpu.com/gtaoxhcoxi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.sxryk.cn/gtbavmfaut.html

[I03] 提取捕获分组
来源：http://hz.yj20258.top/gtbumtznbu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.birdmap.top/gtcvaikitf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ivvv.top/gtfwamayzd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhixingplan.top/gthlwphkea.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.shuidangran.top/gtzujibgdv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.cucudq.cn/gtllhdpdsp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.xinyue.icu/gtwpacjhpe.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yvedp.cn/gtsqktlcxe.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.xuetiantiany.cn/gtqtfogydn.html

[I04] 正则替换
来源：http://hz.cqqwz.cn/gttwzhqcxd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yvedp.cn/gtwbbgguie.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.gaohongyu789.top/gtkfemtxqi.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.havefunace.top/gtoqzweapb.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xuetiantiany.cn/gttnfjhdke.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.52xcode.cn/gtauicwyod.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ywan-chungtsiang.top/gtchfgersw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jqgfzy.top/gthrnzxuhx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zycfv.cn/gticyqyxnj.html

[I05] 按正则拆分
来源：http://hz.sufxvd.cn/gtogosmzbn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hammf.cn/gtqfjtcrty.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ehwqpu.com/gthnesqoym.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hongshengwenyu.top/gtlrlenqyz.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhaomingkeji.xyz/gtryvhiodx.html

Java: s.split("\\s*,\\s*")
来源：http://hz.hongshengwenyu.top/gtmfqjclnz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.0kj1m.cn/gtzovqffmx.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.feifeiyinyue.top/gtowwmvscg.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ehwqpu.com/gtevroorbq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.shanyushiyangkeji.top/gtmdiexybr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.chenzaomai.com/gttdogcjie.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ywan-chungtsiang.top/gterqekqnp.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.nwbrower.top/gtacwvtbmc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xingfuxueyuan.xyz/gtffcylrba.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.haohaochexian.top/gtvvxmglep.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.guowangkeji.top/gtfqnxtkpv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hysaishi.cn/gtbrpbjkrr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.gzhubu.top/gtyksxsegs.html

[I07] 忽略大小写与多行模式
来源：http://hz.wangdashe.top/gtobdmgbpm.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hysaishi.cn/gtsiadpnfp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yanxiufei.cn/gtiplkuimn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yueranfly.top/gtsehqsdnj.html

TS:   /error/gim
来源：http://hz.jyoumei.cn/gtxqdxwrty.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.mhx1999.top/gtdtzcowtr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hywenlv.cn/gtlonjvjrf.html

Ruby: s.scan(/error/i)
来源：http://hz.sufxvd.cn/gtqopilfrb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.feifeiyinyue.top/gtrekczttk.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhiwuduotai.top/gtsljnmlsd.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yvedp.cn/gtvcqjcopq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.wangdashe.top/gtnisqtfwi.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinghuilouyu.cn/gtpwhsbelw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cheryme.top/gtlkmzfnuc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.shuidangran.top/gtedrowmti.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.dianchejie.cn/gtumzmyymz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yj202588.top/gtfkbbcdro.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.0kj1m.cn/gtqzrnxcim.html

================================================================================
来源：http://hz.yongpay.top/gtubeorcgi.html

J. 日期与时间
来源：http://hz.316326.xyz/gtnmiarzft.html

================================================================================
来源：http://hz.aizwys.cn/gtigtwejhi.html

[J01] 获取当前时间
来源：http://hz.cucudq.cn/gtpkrudamw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.chenjidiqi.icu/gtyehbdtjf.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.sweek.top/gtgkdwkjpm.html

JS:   new Date();  Date.now()
来源：http://hz.ehwqpu.com/gtelhduatd.html

TS:   new Date();  Date.now()
来源：http://hz.zhijiandao.cn/gttoqadhou.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.tanke756.top/gttttbznmj.html

Go:   time.Now()
来源：http://hz.sxryk.cn/gtsxengicd.html

Ruby: Time.now
来源：http://hz.hnqzz.top/gthuxqkhus.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.shanyushiyangkeji.top/gtdunsbmev.html

[J02] 格式化输出
来源：http://hz.xziqi.cn/gtcnxlgqup.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ydzc1.top/gtbecwjemi.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ybcxt.top/gtphbubnif.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.shangyingyoupin.top/gtpmfwwqal.html

TS:   d.toISOString()
来源：http://hz.tanke756.top/gteouftsqc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yj202588.top/gtckxbntnc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.iojbl.cn/gtgcelkvjx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj20258.top/gtcjfkxjlg.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.pycfn.com/gtwzzedcip.html

[J03] 字符串解析为日期
来源：http://hz.smart0.xyz/gtcjtodhjo.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.0kj1m.cn/gttytxeyix.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.shzxlz.cn/gtgmyhthhp.html

JS:   new Date("2024-01-02")
来源：http://hz.iojbl.cn/gtfhqkexsu.html

TS:   new Date("2024-01-02")
来源：http://hz.meibo888.top/gtoorpwvmj.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.52xcode.cn/gtvwnyadcs.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.chenjidiqi.icu/gtdiqjxfrj.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ppjwa.cn/gthwkiscgg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.sweek.top/gtkicwjsup.html

[J04] 时间戳与日期互转
来源：http://hz.yuanzhike.top/gtahngykgi.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.xuetiantiany.cn/gtnotkvbzp.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.nwbrower.top/gttmtburvo.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yueranfly.top/gttjtnsgzd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.havefunace.top/gtgzfnqeno.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.vqdsnc.cn/gtjxkjifau.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.fengsongda.top/gtsnxtebkx.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.pengpengdd.cyou/gtpqqvliww.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.quarkkingdee.top/gtgyowqfrl.html

[J05] 时间加减（加 7 天）
来源：http://hz.andypj.xyz/gtlvrzxnlu.html

Py:   now + timedelta(days=7)
来源：http://hz.xuetiantiany.cn/gtpbcrtznq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.wangdashe.top/gtmmuhizoz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhaomingkeji.xyz/gtgetpclmh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.guowangkeji.top/gtoghhgklc.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.aizwys.cn/gtijcdinxy.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yangfankeji.com/gtjzlkoxgp.html

Ruby: Time.now + 7 * 86400
来源：http://hz.tian-w.cn/gtplxlvpvy.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.hfpthk.cn/gtrdqgqqoa.html

[J06] 计算两时间之差
来源：http://hz.jlsjyb.cn/gtafcunbvv.html

Py:   (end - start).total_seconds()
来源：http://hz.sysykeji.top/gtnagoxwtq.html

PHP:  $end->diff($start)->days;
来源：http://hz.c1oappe.top/gtuzxlccsv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ydzc1.top/gtglaigbch.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.mhx1999.top/gtuwdidvfb.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cqqwz.cn/gtpqjrwfkm.html

Go:   end.Sub(start).Hours()
来源：http://hz.svipenyu.cn/gtirxvcpew.html

Ruby: end - start                 # 返回秒数
来源：http://hz.52xcode.cn/gtjecytxzt.html

C#:   (end - start).TotalSeconds
来源：http://hz.aizwys.cn/gtnakmozbx.html

[J07] 比较两个日期
来源：http://hz.gogol.net.cn/gtuublhdnm.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yvedp.cn/gtzzzrljin.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.316326.xyz/gtgflhrinj.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.xingfuxueyuan.xyz/gtcinkvqdl.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shuidangran.top/gtenvsdfbu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.sysykeji.top/gtbjflaujn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.shanyushiyangtech.top/gtmpbixvmm.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hfpthk.cn/gtlljyrdld.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhijiandao.cn/gtdjbneamj.html

[J08] 提取年月日与星期
来源：http://hz.kuanghao11.cn/gtmhyhmypn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zycfv.cn/gtutjhzmvs.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.daxiang520.top/gtpdhkejxz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.xylfe.cn/gtxscqjlfl.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.9152youxi.cn/gtefdxjstj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.sufxvd.cn/gtgdjlxgki.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ehwqpu.com/gtsymsvqiy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.gogol.net.cn/gtggmcamtc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xingfuxueyuan.xyz/gttsuzgngx.html

[J09] 时区处理
来源：http://hz.fengsongda.top/gtdpwzydcp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.sufxvd.cn/gtvskfrqlr.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.shuidangran.top/gtzsjkvxyn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.birdmap.top/gthjimnkav.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.c1oappe.top/gtkwfgsdsv.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jinqigfzy.top/gtueqbachm.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhongyouzk.top/gtcnlvefez.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yuxming.cn/gtgfpblebn.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yuxming.cn/gtkgnkikdp.html

[J10] 取今天 / 本月第一天
来源：http://hz.sxryk.cn/gtrdvdrxzu.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.sufxvd.cn/gttqpitxnw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.mhx1999.top/gtptylywcl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.dianchejie.cn/gtwdpwdcqz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.9152youxi.cn/gtqxcikbau.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.chenjidiqi.icu/gtwudjfoac.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.pycfn.com/gtxygzqyln.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhoulong.xyz/gtaunmhfex.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.nanxuanxn.top/gtjpfcmyqx.html

================================================================================
来源：http://hz.yvedp.cn/gtqrynyrqr.html

K. JSON 与序列化
来源：http://hz.xziqi.cn/gtmifoaxmx.html

================================================================================
来源：http://hz.yj20258.top/gtjcsozosh.html

[K01] 对象转 JSON 字符串
来源：http://hz.xuanzx.com/gtqzwcmaey.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.xuetiantiany.cn/gtkqnvywtm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yongpay.top/gtzkdmhook.html

JS:   JSON.stringify(obj)
来源：http://hz.nanxuanxn.top/gtrhkghnnv.html

TS:   JSON.stringify(obj)
来源：http://hz.svipenyu.cn/gtpcoelzlr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.smart0.xyz/gtwyefvmum.html

Go:   json.Marshal(obj)
来源：http://hz.hfpthk.cn/gtvvcclkhv.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.feifeiyinyue.top/gtqnxqxqhg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yangfankeji.com/gtnpmetjer.html

[K02] JSON 字符串转对象
来源：http://hz.c1oappe.top/gtshxssydk.html

Py:   json.loads(s)
来源：http://hz.havefunace.top/gtaqeaxzss.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.iojbl.cn/gtesemxfeo.html

JS:   JSON.parse(s)
来源：http://hz.guannengcc.top/gtvykqrabj.html

TS:   JSON.parse(s)
来源：http://hz.316326.xyz/gtyfpiigpd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.daria6918.cn/gtkioxjoox.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jinghuilouyu.cn/gtsrlncutd.html

Ruby: JSON.parse(s)
来源：http://hz.xinyue.icu/gtfdxfsvdf.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hysaishi.cn/gtsoedbaig.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.xingfuxueyuan.xyz/gtfdwpxwvz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.haohaochexian.top/gtddpzzjop.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hfpthk.cn/gtwepcpeix.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hywenlv.cn/gtofpgqmum.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.havefunace.top/gtqbqkmdxd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zhiwuduotai.top/gtojfcwybn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.daxiang520.top/gtvzofmncz.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.snrcjt.cn/gtvnkmxakw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ydzc1.top/gtkxbwxybw.html

[K04] 读取 JSON 文件
来源：http://hz.yanxiufei.cn/gtoljpwmbq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.chenzaomai.com/gtgwtqmhek.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhiwuduotai.top/gtojoxvmqn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.kuanghao11.cn/gtewolwqcc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.tian-w.cn/gtxpsfqddx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.xylfe.cn/gttiuirktl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ydjk.org.cn/gtddttulkw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.birdmap.top/gttsinbssp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.gotoacloud.top/gtgaeqcafg.html

[K05] 深拷贝对象
来源：http://hz.yangfankeji.com/gtnnlhdywm.html

Py:   copy.deepcopy(obj)
来源：http://hz.hysaishi.cn/gtjzgejggq.html

PHP:  unserialize(serialize($obj));
来源：http://hz.birdmap.top/gtwtafgrfr.html

JS:   structuredClone(obj)
来源：http://hz.zdqjudy.top/gtmumsjvps.html

TS:   structuredClone(obj)
来源：http://hz.chenlongwang.top/gtsxberpla.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hongshengwenyu.top/gtbfxqlvix.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hammf.cn/gtylxnegfy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhengqikj.top/gtmkkblljh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.nanxuanxn.top/gtidegrotg.html

[K06] 解析 URL 查询串
来源：http://hz.c1oappe.top/gtypavxgln.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.sxryk.cn/gtzrdduuyf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jqgufenzy.top/gtyqpvdyhi.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.snrcjt.cn/gtsnrvmcay.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xziqi.cn/gttoypozgp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.52xcode.cn/gtacrervlf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.316326.xyz/gtmmjxipfe.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.wangdashe.top/gtowfgpoew.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yj20258.top/gtejkuqsdh.html

[K07] 进制转换
来源：http://hz.shangyingyoupin.top/gtbeujfodt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jinyuanbaomall.cn/gtjbhjmccm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.gotoacloud.top/gtwuzofetp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.aizwys.cn/gtnozmyobw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jqgfzy.top/gtqagaehgo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xuanzx.com/gtdetqajqd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.bjfxy.top/gtrorazfab.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.gogol.net.cn/gtmsscweoj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.9152youxi.cn/gtrrzspduw.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jiagoushi.top/gtutqfwdfc.html

Py:   pickle.dumps(obj)
来源：http://hz.xuanzx.com/gtxytnsjxh.html


<!-- 参考信息 -->