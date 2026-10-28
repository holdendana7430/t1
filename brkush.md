代发 wailian999

TS:   throw new Error("错误信息");
来源：http://hz.gaohongyu789.top/gtgddrdafi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jqgfzy.top/gtbebmgpqb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.guowangkeji.top/gtjgtbjnte.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.shzxlz.cn/gtwilsngyb.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.redwolf501.top/gtfxycurjq.html

[H04] 自定义异常类型
来源：http://hz.cucudq.cn/gtpypsqsey.html

Py:   class MyError(Exception): pass
来源：http://hz.zhixingplan.top/gtspyhtqoq.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.aizwys.cn/gtigvfkxqy.html

JS:   class MyError extends Error {}
来源：http://hz.dashuyun.cn/gtcqcudchl.html

TS:   class MyError extends Error {}
来源：http://hz.zhongyouzk.top/gtgmmivpjn.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhijiandao.cn/gthjdbtzyc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.xinyue.icu/gtrwkxzgiv.html

Ruby: class MyError < StandardError; end
来源：http://hz.daxiang520.top/gtrwseqnkk.html

C#:   class MyException : Exception {}
来源：http://hz.hfpthk.cn/gtgqgfxxjr.html

[H05] 捕获特定类型
来源：http://hz.316326.xyz/gtbotphziq.html

Py:   except ValueError as e:
来源：http://hz.xinyue.icu/gtpfvcjzxy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hysaishi.cn/gttrkahato.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ivvv.top/gtzdmbzkrz.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.xinyue.icu/gtyhtonqsu.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jinghuilouyu.cn/gtjrxtydou.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hnxiangtu.top/gtfrwlsqiw.html

Ruby: rescue ArgumentError => e
来源：http://hz.xziqi.cn/gtcqzkszgh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.0kj1m.cn/gtpnidemuk.html

[H06] 可选值 / 空值安全访问
来源：http://hz.svipenyu.cn/gtdeikqrov.html

Py:   value = d.get("k") or default
来源：http://hz.meibo888.top/gtddfciues.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hfpthk.cn/gtopbsvuhf.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.nwbrower.top/gtgqumrsau.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jlsjyb.cn/gtkwnnzxkv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ehwqpu.com/gtnzagsgki.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.havefunace.top/gtffzvccbd.html

Ruby: d&.dig(:a, :b)
来源：http://hz.mhx1999.top/gtsdjrariz.html

C#:   obj?.A?.B ?? default
来源：http://hz.svipenyu.cn/gtdyyvqrbe.html

[H07] 断言
来源：http://hz.yueranfly.top/gtuwplqowz.html

Py:   assert x > 0, "必须为正"
来源：http://hz.kuanghao11.cn/gtzjbmgyjr.html

PHP:  assert($x > 0);
来源：http://hz.jqgufenzy.top/gtoszdpxol.html

JS:   console.assert(x > 0);
来源：http://hz.bjfxy.top/gtnhbhrbkz.html

TS:   console.assert(x > 0);
来源：http://hz.jqgfzy.top/gtyhtnkumf.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yonumen.top/gttecduncn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.snrcjt.cn/gtktapvvit.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.nanxinkj.top/gtpfdrvtfu.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jqgfzy.top/gtnohifdhc.html

[H08] 获取错误信息与堆栈
来源：http://hz.quarkkingdee.top/gthuqaxxiv.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.iojbl.cn/gtpvlhzvsr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.cdnleiting.top/gtqyeemdfh.html

JS:   e.message;  e.stack
来源：http://hz.haohaochexian.top/gtpksniupl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hysaishi.cn/gtrnzdkcuv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.cucudq.cn/gtvhoisopp.html

Go:   err.Error()
来源：http://hz.zhixingplan.top/gthqyooxri.html

Ruby: e.message;  e.backtrace
来源：http://hz.hnqzz.top/gtkdwscixb.html

C#:   e.Message;  e.StackTrace
来源：http://hz.tianlin.xyz/gtituqcztp.html

[H09] 带错误码的异常
来源：http://hz.jinqigfzy.top/gtdlzzmqbu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jianghu66.top/gtkietfkcu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.fzhhl.top/gtfdiivcnn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.svipenyu.cn/gtyzjreauj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhixingplan.top/gtnspiinym.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.cdnleiting.top/gtfqawvhmc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.snrcjt.cn/gtjtgoeejm.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jyoumei.cn/gtctjzktdn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.gotoacloud.top/gtbymowvpz.html

[H10] 资源自动释放
来源：http://hz.smart0.xyz/gtuyumldcn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ywan-chungtsiang.top/gtwewtqpyt.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.redwolf501.top/gttliphoay.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yueranfly.top/gtzilsznqx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ydjk.org.cn/gtxodxdelr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.wangdashe.top/gthfxdwvng.html

Go:   defer f.Close()
来源：http://hz.cqqwz.cn/gtqfvbuewp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xuetiantiany.cn/gtffyrxtpw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shangyingyoupin.top/gtpqqizwye.html

================================================================================
来源：http://hz.svipenyu.cn/gtuqnhqhdq.html

I. 正则表达式
来源：http://hz.chenzaomai.com/gtqphuakrb.html

================================================================================
来源：http://hz.ivvv.top/gtirbuvosn.html

[I01] 判断是否匹配
来源：http://hz.fzhhl.top/gtwrfwomel.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.chenlongwang.top/gtxgzuieyw.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yvedp.cn/gtaswocmev.html

JS:   /\d+/.test(s)
来源：http://hz.haohaochexian.top/gtwsdojsaq.html

TS:   /\d+/.test(s)
来源：http://hz.xuetiantiany.cn/gtvelrscey.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.wangdashe.top/gtabwwmngn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.meibo888.top/gttaijzbew.html

Ruby: s.match?(/\d+/)
来源：http://hz.feifeiyinyue.top/gtvfgjbnxe.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ybcxt.top/gtmcgtbljk.html

[I02] 提取所有匹配
来源：http://hz.haohaochexian.top/gtbxkregbl.html

Py:   re.findall(r"\d+", s)
来源：http://hz.xziqi.cn/gtuckvmzzd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.pengpengdd.cyou/gtcjfgqpdc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hysaishi.cn/gtmcmnfcld.html

TS:   s.match(/\d+/g)
来源：http://hz.gaohongyu789.top/gtuljppbnd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.tanke756.top/gtkkjtjkbe.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.cqqwz.cn/gtpzgkkpxs.html

Ruby: s.scan(/\d+/)
来源：http://hz.dashuyun.cn/gtqgivxcty.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.haohaochexian.top/gttfjlibkp.html

[I03] 提取捕获分组
来源：http://hz.zycfv.cn/gtpnjbktjf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.pycfn.com/gtfvbixqlv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.shuidangran.top/gthgwmecpf.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zdqjudy.top/gtjcdelhlp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.redwolf501.top/gtnseaaloi.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jinqigfzy.top/gtbnnpsapu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hywenlv.cn/gtqljrmrmj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhoulong.xyz/gteadzelko.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.tanke756.top/gtgyowyhve.html

[I04] 正则替换
来源：http://hz.guowangkeji.top/gtuvxycjhm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.nanxuanxn.top/gtttjmigfk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.feifeiyinyue.top/gtyjypiowh.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.daxiang520.top/gtmhkgzbip.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.shanyushiyangkeji.top/gtlrduvkax.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.nwbrower.top/gtznqbkcbz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.chenjidiqi.icu/gtvgwapyhi.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ywan-chungtsiang.top/gtxwfakuvm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zhiwuduotai.top/gtbvlndkfa.html

[I05] 按正则拆分
来源：http://hz.zdqjudy.top/gtnbibduzd.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.birdmap.top/gtiezsdppc.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xziqi.cn/gtdocjbvdz.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.shuidangran.top/gtizomwouc.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.daria6918.cn/gtiljignwi.html

Java: s.split("\\s*,\\s*")
来源：http://hz.wangdashe.top/gtcaexfvtl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hysaishi.cn/gtkjhgwnum.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yongpay.top/gtaqtvsrti.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zycfv.cn/gtijcmrgrh.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.quarkkingdee.top/gtlfkdfusl.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.pengpengdd.cyou/gtpibzidst.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.svipenyu.cn/gtutvcwfyw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhiwuduotai.top/gtcycpzqpx.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.aibaodan.cn/gtwhnlmomh.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.tian-w.cn/gtjfurnfzf.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ppjwa.cn/gteussgpxf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.shangyingyoupin.top/gtwqqdzrbm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yj20258888.top/gtiaycwwck.html

[I07] 忽略大小写与多行模式
来源：http://hz.ydzc1.top/gtiibvlaaf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yj20258888.top/gtswijctzn.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jqgufenzy.top/gtwgymnvnm.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.gzhubu.top/gtzxdjcnrc.html

TS:   /error/gim
来源：http://hz.tianlin.xyz/gtphqztjom.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.redwolf501.top/gtacjofike.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.mhx1999.top/gtbteowfac.html

Ruby: s.scan(/error/i)
来源：http://hz.mhx1999.top/gtjpmiitjv.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ydzc1.top/gtfpkkvzfe.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jinghuilouyu.cn/gtbawgfnah.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhengqikj.top/gttvshtejm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ydjk.org.cn/gtfemfdowc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.fzhhl.top/gtnhbhlqoy.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tanke756.top/gtnkudqpti.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.sufxvd.cn/gtlsuluuys.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.ybcxt.top/gtxtmsuckc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ybcxt.top/gtmfbsvytr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.hnqzz.top/gtmsqmnpsp.html

================================================================================
来源：http://hz.52xcode.cn/gtyyupbcjo.html

J. 日期与时间
来源：http://hz.gaohongyu789.top/gtyntowqsm.html

================================================================================
来源：http://hz.yj20258888.top/gtmfbsbgel.html

[J01] 获取当前时间
来源：http://hz.yongpay.top/gtecdmntkh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.nwbrower.top/gtnpdupbgh.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yuxming.cn/gtwfwavxss.html

JS:   new Date();  Date.now()
来源：http://hz.sweek.top/gtasrfibvv.html

TS:   new Date();  Date.now()
来源：http://hz.c1oappe.top/gtksfftegn.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.haohaochexian.top/gtdtqyudhr.html

Go:   time.Now()
来源：http://hz.pengpengdd.cyou/gtabgtztqg.html

Ruby: Time.now
来源：http://hz.tanke756.top/gtzbssgeqq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhaomingkeji.xyz/gtrgerohyq.html

[J02] 格式化输出
来源：http://hz.wangshuangyany.cn/gthvtfznmz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hywenlv.cn/gtwlinavrx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.feifeiyinyue.top/gtqqnikgfx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hysaishi.cn/gtvvzprzdg.html

TS:   d.toISOString()
来源：http://hz.jiagoushi.top/gtfiinslzr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yj20258.top/gthislbhhb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.tanke756.top/gtjjpqywai.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.316326.xyz/gtnjepunuc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.0kj1m.cn/gtdlfzmokt.html

[J03] 字符串解析为日期
来源：http://hz.tianlin.xyz/gtsihasuuu.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yj20258888.top/gtqywjdelz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.shanyushiyangtech.top/gtmvmfsdou.html

JS:   new Date("2024-01-02")
来源：http://hz.c1oappe.top/gtzekqlzgn.html

TS:   new Date("2024-01-02")
来源：http://hz.daxiang520.top/gtziqfjfru.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.nwbrower.top/gtfqhmozed.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yuxming.cn/gtjnkdmbxg.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.tanke756.top/gtdelrqsvc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.bjfxy.top/gtrahunoea.html

[J04] 时间戳与日期互转
来源：http://hz.guowangkeji.top/gtreszyssk.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.cashguo.top/gtrqidmbsy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jinqigfzy.top/gtjilpxrtt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ppjwa.cn/gtpguzknow.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.nanxuanxn.top/gtcntnelxq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yj20258888.top/gtscwaxnni.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jqgfzy.top/gtmgvfkygs.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.gogol.net.cn/gtzwlgythz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.gzhubu.top/gtskclvzgs.html

[J05] 时间加减（加 7 天）
来源：http://hz.wangdashe.top/gtlgtwhaut.html

Py:   now + timedelta(days=7)
来源：http://hz.shanyushiyangkeji.top/gtpmeicfww.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hysaishi.cn/gtlwododvy.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xinyue.icu/gtktxxevsf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinyuanbaomall.cn/gtigbectsu.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.chenjidiqi.icu/gtbappqupe.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cheryme.top/gtdupzokcb.html

Ruby: Time.now + 7 * 86400
来源：http://hz.shuidangran.top/gtxgbaqyxy.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.gogol.net.cn/gtanyzsfvx.html

[J06] 计算两时间之差
来源：http://hz.xziqi.cn/gtfaeuywmk.html

Py:   (end - start).total_seconds()
来源：http://hz.cashguo.top/gtewzsrxmm.html

PHP:  $end->diff($start)->days;
来源：http://hz.9152youxi.cn/gtarygzapp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.aizwys.cn/gtzhwsjhjr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.kuanghao11.cn/gtbgylftvz.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.aizwys.cn/gtkqhrzrpa.html

Go:   end.Sub(start).Hours()
来源：http://hz.jlsjyb.cn/gtmrmovtvo.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ydzc1.top/gtjkvdvmuj.html

C#:   (end - start).TotalSeconds
来源：http://hz.nanxinkj.top/gtptufnudp.html

[J07] 比较两个日期
来源：http://hz.hammf.cn/gtomkvyfoq.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.cqqwz.cn/gtiagxdqio.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.meibo888.top/gtnlkencha.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yueranfly.top/gtnbrsntid.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yvedp.cn/gtmvognrmi.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jqgufenzy.top/gtqbqgbujd.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jqgfzy.top/gtbjwcfgeh.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jinghuilouyu.cn/gtjyyicpfq.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hysaishi.cn/gtklqffbxh.html

[J08] 提取年月日与星期
来源：http://hz.9152youxi.cn/gtlsjikzov.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.aibaodan.cn/gtxwzavflu.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.daria6918.cn/gtpvnufsnx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.gzhubu.top/gternzaciy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhiwuduotai.top/gtiwlkljca.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.sysykeji.top/gtqoibvoeo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.fengsongda.top/gtgkdjzygq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jqgufenzy.top/gtgaqubdap.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jqgufenzy.top/gtfdvbnjdj.html

[J09] 时区处理
来源：http://hz.andypj.xyz/gtoqrmygwc.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yj20258888.top/gtpsqwwbuc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yonumen.top/gtenuwyvap.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhijiandao.cn/gttuybkrop.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.fzhhl.top/gtkrjhjzts.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.wangshuangyany.cn/gtmjwxinvn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.fzhhl.top/gttvoppgsz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.iojbl.cn/gtmalucxgk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.redwolf501.top/gtzlzncumj.html

[J10] 取今天 / 本月第一天
来源：http://hz.vqdsnc.cn/gthvunobce.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jqgufenzy.top/gtnycjgtcc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yj202588.top/gtobuqaclh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.quarkkingdee.top/gtxfetmkwc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.havefunace.top/gtjnpxoqav.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.ybcxt.top/gtvwjpzbfs.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jianghu66.top/gthwnbvchv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.gaohongyu789.top/gttvdrszcb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xinyue.icu/gtlngrktpg.html

================================================================================
来源：http://hz.fzhhl.top/gtknimaooi.html

K. JSON 与序列化
来源：http://hz.nwbrower.top/gtncwgkyfj.html

================================================================================
来源：http://hz.tian-w.cn/gtxwflpdpn.html

[K01] 对象转 JSON 字符串
来源：http://hz.jinqigufen.top/gtycfjqdcp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.xziqi.cn/gtcgigpqjk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.andypj.xyz/gtnvgnoabl.html

JS:   JSON.stringify(obj)
来源：http://hz.sweek.top/gtlkrjcngw.html

TS:   JSON.stringify(obj)
来源：http://hz.sxryk.cn/gtmyfzljia.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhengqikj.top/gtjmxtiiry.html

Go:   json.Marshal(obj)
来源：http://hz.ivvv.top/gtlltrxvjf.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.c1oappe.top/gtfolanwpv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.shzxlz.cn/gthqvwvmqo.html

[K02] JSON 字符串转对象
来源：http://hz.ydzc1.top/gtvypsrrfs.html

Py:   json.loads(s)
来源：http://hz.hysaishi.cn/gtzptkihmv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.dashuyun.cn/gtdnkppcaz.html

JS:   JSON.parse(s)
来源：http://hz.kuanghao11.cn/gtjwafgzpt.html

TS:   JSON.parse(s)
来源：http://hz.gotoacloud.top/gtyumvyvot.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.shanyushiyangtech.top/gtpshdgdxj.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.fengsongda.top/gtlbnedjrd.html

Ruby: JSON.parse(s)
来源：http://hz.cucudq.cn/gtpgyprcjt.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xylfe.cn/gtbakgcmjy.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.daria6918.cn/gtkyzsswdw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.aizwys.cn/gtnouatsbn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hnqzz.top/gtnqkosepl.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.sweek.top/gtcgfxptpv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.sysykeji.top/gtdddfimta.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.svipenyu.cn/gtqobvaxpe.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.meibo888.top/gttsxexbbp.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ydzc1.top/gtkegsbiwl.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hfpthk.cn/gtcllgdbtc.html

[K04] 读取 JSON 文件
来源：http://hz.0kj1m.cn/gtiesdwheg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.52xcode.cn/gtuthhqrst.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cdnleiting.top/gtvqaerfvn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.c1oappe.top/gthgagyogz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yuanzhike.top/gtjekqxdcd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hnqzz.top/gtmokgmefn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hfpthk.cn/gtzoruxqwb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.haohaochexian.top/gtwardvqla.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.cdnleiting.top/gtdifwrsys.html

[K05] 深拷贝对象
来源：http://hz.quarkkingdee.top/gtrlxydnsg.html

Py:   copy.deepcopy(obj)
来源：http://hz.sufxvd.cn/gtsvekzffj.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yangfankeji.com/gtijuixfko.html

JS:   structuredClone(obj)
来源：http://hz.sxryk.cn/gtzeukxcnb.html

TS:   structuredClone(obj)
来源：http://hz.ywan-chungtsiang.top/gtpsprfvpv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.wangshuangyany.cn/gtpfepdjzn.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.chenzaomai.com/gtglaczfpk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.quarkkingdee.top/gtklmumima.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.feifeiyinyue.top/gtrldvopry.html

[K06] 解析 URL 查询串
来源：http://hz.hywenlv.cn/gtwxdxhkoh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yuanzhike.top/gtfaohnbht.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.shanyushiyangtech.top/gtxansbvgi.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yuxming.cn/gtthnsmvqc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xingfuxueyuan.xyz/gtbsojxpzu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yj202588.top/gtjcsucqbi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.tianlin.xyz/gtsxbpbkjy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jinyuanbaomall.cn/gtchhgixmv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yj202588.top/gtrelnsacg.html

[K07] 进制转换
来源：http://hz.shanyushiyangtech.top/gtevfaupaa.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ehwqpu.com/gtptqatinf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.fengsongda.top/gtjtlsfknz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hongshengwenyu.top/gtenosnwyx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.dashuyun.cn/gtyaabbrsd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.bjfxy.top/gtksqzskjk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yongpay.top/gtdwhpkshl.html


<!-- 参考信息 -->