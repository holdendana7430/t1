代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hysaishi.cn/gtabmwkrfb.html

[H04] 自定义异常类型
来源：http://hz.svipenyu.cn/gtyklmfkow.html

Py:   class MyError(Exception): pass
来源：http://hz.yj20258.top/gtmitimfco.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.52xcode.cn/gttpvnmjxs.html

JS:   class MyError extends Error {}
来源：http://hz.cucudq.cn/gtrmorlrai.html

TS:   class MyError extends Error {}
来源：http://hz.chenlongwang.top/gtafivfspy.html

Java: class MyException extends RuntimeException {}
来源：http://hz.nanxuanxn.top/gtthjrjwyg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yj20258.top/gttchwmngf.html

Ruby: class MyError < StandardError; end
来源：http://hz.zdqjudy.top/gtqmiicnpw.html

C#:   class MyException : Exception {}
来源：http://hz.aizwys.cn/gtolrdotzo.html

[H05] 捕获特定类型
来源：http://hz.jinqigufen.top/gtotpfzubq.html

Py:   except ValueError as e:
来源：http://hz.haohaochexian.top/gtqpbfohkl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.dianchejie.cn/gtntnhmpco.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.pengpengdd.cyou/gthntbkfum.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.tian-w.cn/gthgkiilmh.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hnxiangtu.top/gtuaxlyywt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xingfuxueyuan.xyz/gtepipvxux.html

Ruby: rescue ArgumentError => e
来源：http://hz.yanxiufei.cn/gtytnqkdzv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.52xcode.cn/gthmqlctvr.html

[H06] 可选值 / 空值安全访问
来源：http://hz.daxiang520.top/gtadjlrduz.html

Py:   value = d.get("k") or default
来源：http://hz.cheryme.top/gtvfnayius.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.havefunace.top/gtifygbwjb.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.nanxinkj.top/gtqenzkyhc.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.chenjidiqi.icu/gtouhvdjcp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.sufxvd.cn/gtvfxkvjho.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.sxryk.cn/gtpeshuigv.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yangfankeji.com/gtkveqyzqh.html

C#:   obj?.A?.B ?? default
来源：http://hz.xingfuxueyuan.xyz/gtzilqayug.html

[H07] 断言
来源：http://hz.sufxvd.cn/gtdmbankgs.html

Py:   assert x > 0, "必须为正"
来源：http://hz.9152youxi.cn/gtkbvsqdka.html

PHP:  assert($x > 0);
来源：http://hz.nwbrower.top/gtgcwklhcx.html

JS:   console.assert(x > 0);
来源：http://hz.cucudq.cn/gtnpijnhmk.html

TS:   console.assert(x > 0);
来源：http://hz.jinqigufen.top/gtlrswhvfk.html

Java: assert x > 0 : "必须为正";
来源：http://hz.0kj1m.cn/gtbbmcrdqp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yongpay.top/gtqqkjdlww.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.chenlongwang.top/gtybzjpsxo.html

C#:   Debug.Assert(x > 0);
来源：http://hz.aibaodan.cn/gtgubtqcrq.html

[H08] 获取错误信息与堆栈
来源：http://hz.jyoumei.cn/gtbaxkaubd.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ywan-chungtsiang.top/gtyovpabgx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ydjk.org.cn/gtzpkeoqjs.html

JS:   e.message;  e.stack
来源：http://hz.cheryme.top/gtsrnwvyht.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.xuanzx.com/gtqmpgzxjv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.dashuyun.cn/gtmtzxnvlh.html

Go:   err.Error()
来源：http://hz.feifeiyinyue.top/gtafhakjla.html

Ruby: e.message;  e.backtrace
来源：http://hz.guannengcc.top/gtpefzhbvz.html

C#:   e.Message;  e.StackTrace
来源：http://hz.daria6918.cn/gtaajnrowi.html

[H09] 带错误码的异常
来源：http://hz.guowangkeji.top/gtcearaszs.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jqgufenzy.top/gtvphwnwel.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zycfv.cn/gtgdvpjkxi.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.svipenyu.cn/gtihdiiery.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhijiandao.cn/gtzbgcmksc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.pycfn.com/gthvybxevk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ydzc1.top/gtmekcucnn.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yonumen.top/gtpyodpbrg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.cucudq.cn/gtspotmsxn.html

[H10] 资源自动释放
来源：http://hz.ydzc1.top/gtwvkwzday.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.guannengcc.top/gthhmqdmun.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.sxryk.cn/gtmcxxmbut.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.andypj.xyz/gtrpqbfgch.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sxryk.cn/gtwxydfeln.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.kuanghao11.cn/gtelqwrrps.html

Go:   defer f.Close()
来源：http://hz.guannengcc.top/gtkukgcjhd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.redwolf501.top/gtgaouzcpm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.daxiang520.top/gthwaloghj.html

================================================================================
来源：http://hz.yanxiufei.cn/gtqdjelhfd.html

I. 正则表达式
来源：http://hz.jiagoushi.top/gtyhsknnjs.html

================================================================================
来源：http://hz.ivvv.top/gtpykotgos.html

[I01] 判断是否匹配
来源：http://hz.quarkkingdee.top/gtdxzzgcug.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.sweek.top/gtuyskcaoy.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zycfv.cn/gtvmukvasr.html

JS:   /\d+/.test(s)
来源：http://hz.shanyushiyangtech.top/gtsbvjllyp.html

TS:   /\d+/.test(s)
来源：http://hz.ivvv.top/gtngterhxz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.gotoacloud.top/gtphfkvkod.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.chenzaomai.com/gtixpyalql.html

Ruby: s.match?(/\d+/)
来源：http://hz.fengsongda.top/gtxrkbltow.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.shuidangran.top/gtkryztrfu.html

[I02] 提取所有匹配
来源：http://hz.pycfn.com/gtxpqwxfip.html

Py:   re.findall(r"\d+", s)
来源：http://hz.tianlin.xyz/gtdydyhqer.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.quarkkingdee.top/gtgbhgdpih.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.316326.xyz/gttftkntij.html

TS:   s.match(/\d+/g)
来源：http://hz.zhongyouzk.top/gtqjxlprog.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jyoumei.cn/gtddndlfaa.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.sysykeji.top/gtozwyoowy.html

Ruby: s.scan(/\d+/)
来源：http://hz.ydzc1.top/gtdbilnsfz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.tian-w.cn/gtmahblwet.html

[I03] 提取捕获分组
来源：http://hz.hywenlv.cn/gtkhiuvvzu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.chenzaomai.com/gtlkykggwc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.tianlin.xyz/gtzcvojhvh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.dianchejie.cn/gtmjamykhv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.tanke756.top/gtacpvztsm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.meibo888.top/gtkvmzchwe.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhaomingkeji.xyz/gtyngqxjfb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.guannengcc.top/gtaqkdnpwi.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.daxiang520.top/gtnwciamww.html

[I04] 正则替换
来源：http://hz.cucudq.cn/gtyqxxcige.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhongyouzk.top/gtxxkfkuhn.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.52xcode.cn/gtpavigamv.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yanxiufei.cn/gtljxpsyrz.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xinyue.icu/gtnkzvbufl.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.ivvv.top/gtorsjkhpk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yj202588.top/gtddhxxohk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.andypj.xyz/gtyhbmanyc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zhiwuduotai.top/gtwiayroeg.html

[I05] 按正则拆分
来源：http://hz.chenjidiqi.icu/gtfgitgahs.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.316326.xyz/gtecxqecqr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yj20258888.top/gtrdttlcqe.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.sxryk.cn/gtkwhzrybp.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.feifeiyinyue.top/gtttpekwmp.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jinghuilouyu.cn/gticymbcji.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.dianchejie.cn/gtitygeacs.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.sufxvd.cn/gtbvembnrt.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.vqdsnc.cn/gtgaojvxnl.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.smart0.xyz/gthzrqztrj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.smart0.xyz/gtoakvktjx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.sxryk.cn/gtgwoaxwjq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.wangshuangyany.cn/gtnmlmuish.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cdnleiting.top/gteeefsdgi.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.guannengcc.top/gtbigmamfc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yonumen.top/gtugbydadn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.aibaodan.cn/gtajyfbjer.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yj202588.top/gtejihcbxh.html

[I07] 忽略大小写与多行模式
来源：http://hz.yangfankeji.com/gtooiqgbei.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.aibaodan.cn/gtidopwtdp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.chenzaomai.com/gtvswsgafp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.shanyushiyangkeji.top/gtybsitmvt.html

TS:   /error/gim
来源：http://hz.andypj.xyz/gtoarnqcxh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.316326.xyz/gtiwepropt.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.iojbl.cn/gtxkuiiasv.html

Ruby: s.scan(/error/i)
来源：http://hz.nanxuanxn.top/gtcjehpqaa.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jinyuanbaomall.cn/gtouqyemax.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhongyouzk.top/gtyynzisfh.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.gotoacloud.top/gtmtlvexmb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.daxiang520.top/gtejbkixji.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yuanzhike.top/gtfygwigqm.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shuidangran.top/gttzsjmpsp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.xuanzx.com/gtbglcgquk.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.sufxvd.cn/gtyrenyzdy.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.aibaodan.cn/gtanatlmdr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.316326.xyz/gtrsoaxkzi.html

================================================================================
来源：http://hz.kuanghao11.cn/gtfrvkwnag.html

J. 日期与时间
来源：http://hz.svipenyu.cn/gtdfstsofv.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtagbgmlrm.html

[J01] 获取当前时间
来源：http://hz.quarkkingdee.top/gtzzetymvf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.xingfuxueyuan.xyz/gtipdjynxv.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ydzc1.top/gtnlqwdtji.html

JS:   new Date();  Date.now()
来源：http://hz.sysykeji.top/gtraeluoln.html

TS:   new Date();  Date.now()
来源：http://hz.wangdashe.top/gtxbgorfij.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jinqigfzy.top/gttohpvjfs.html

Go:   time.Now()
来源：http://hz.gaohongyu789.top/gtaykoofjj.html

Ruby: Time.now
来源：http://hz.ehwqpu.com/gtpwalbydn.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yanxiufei.cn/gtyophylqj.html

[J02] 格式化输出
来源：http://hz.chenlongwang.top/gtmaoawvlw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jqgfzy.top/gtduhrubvx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhongyouzk.top/gtgsvyftak.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhoulong.xyz/gtdxmuyrno.html

TS:   d.toISOString()
来源：http://hz.dashuyun.cn/gtngrquctr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yueranfly.top/gtcnunxvnp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hnxiangtu.top/gtduhrleyw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sufxvd.cn/gtibrjzuvj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhongyouzk.top/gtzqlcaiym.html

[J03] 字符串解析为日期
来源：http://hz.zycfv.cn/gtbgfdgidy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.shzxlz.cn/gtlbwbwwht.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.shzxlz.cn/gtbnjpojmo.html

JS:   new Date("2024-01-02")
来源：http://hz.daria6918.cn/gtgyazmwul.html

TS:   new Date("2024-01-02")
来源：http://hz.52xcode.cn/gtslgdigjc.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.shuidangran.top/gtljgxcnqf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yuanzhike.top/gtuyoaqlsz.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.316326.xyz/gtctvqgxvv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jqgufenzy.top/gtstkrhahw.html

[J04] 时间戳与日期互转
来源：http://hz.wangdashe.top/gtvinqvdcn.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.andypj.xyz/gtjtyrqptc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yueranfly.top/gteznnpsjd.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zhijiandao.cn/gtdcgfrjni.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yuanzhike.top/gtajhnwfmz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.svipenyu.cn/gtuyvfxxxw.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.nanxuanxn.top/gtenwzstcq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ehwqpu.com/gtiduqffjj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.cashguo.top/gteohrrarz.html

[J05] 时间加减（加 7 天）
来源：http://hz.jqgfzy.top/gtnexdpzwo.html

Py:   now + timedelta(days=7)
来源：http://hz.fzhhl.top/gtrnhmkons.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.wangdashe.top/gtgjnhaekt.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.aibaodan.cn/gtforssjgq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.wangshuangyany.cn/gtauqvoqwc.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhiwuduotai.top/gtvtiteoon.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yanxiufei.cn/gtfhfvbdrj.html

Ruby: Time.now + 7 * 86400
来源：http://hz.dashuyun.cn/gtzowqqwel.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.dashuyun.cn/gtgeiclido.html

[J06] 计算两时间之差
来源：http://hz.aizwys.cn/gtmnytoejt.html

Py:   (end - start).total_seconds()
来源：http://hz.jiagoushi.top/gtjdaztwur.html

PHP:  $end->diff($start)->days;
来源：http://hz.cucudq.cn/gtorivaisn.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.dashuyun.cn/gtepofbfen.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ybcxt.top/gtyottdqrn.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.sysykeji.top/gtnxizjonn.html

Go:   end.Sub(start).Hours()
来源：http://hz.daxiang520.top/gtqgcxbkld.html

Ruby: end - start                 # 返回秒数
来源：http://hz.316326.xyz/gtxdefvdxs.html

C#:   (end - start).TotalSeconds
来源：http://hz.fengsongda.top/gtogdfvvog.html

[J07] 比较两个日期
来源：http://hz.kuanghao11.cn/gtrxupdjdi.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.fzhhl.top/gtincjmpoh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.tian-w.cn/gtjrefcwui.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhoulong.xyz/gtkxetmzgd.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yueranfly.top/gtnxkpfzzo.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hongshengwenyu.top/gtqukozssp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.gotoacloud.top/gtbbylsjaq.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yj20258.top/gthocoarwh.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.svipenyu.cn/gtindggazq.html

[J08] 提取年月日与星期
来源：http://hz.zhiwuduotai.top/gtsixiuaqd.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.chenjidiqi.icu/gtafaxxjfp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.smart0.xyz/gtutthiwnm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhiwuduotai.top/gtexhgdvrb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hongshengwenyu.top/gtpjosezkt.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jqgufenzy.top/gtwrabjbtx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.guowangkeji.top/gtaxucslgy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.guowangkeji.top/gtkdcolvvq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.gzhubu.top/gtngivcefe.html

[J09] 时区处理
来源：http://hz.kuanghao11.cn/gtuogsvfhz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cucudq.cn/gtgphsgilv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hysaishi.cn/gtfnqlkugo.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nanxuanxn.top/gtavajfurc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hammf.cn/gtxrawajpu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xziqi.cn/gtxtltqagw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.aibaodan.cn/gtcxcxqrqt.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.chenjidiqi.icu/gtaowybvil.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.smart0.xyz/gtzrhrlstm.html

[J10] 取今天 / 本月第一天
来源：http://hz.xuetiantiany.cn/gtwhjdkzie.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.feifeiyinyue.top/gtyiwdqdda.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhijiandao.cn/gtlgisnryz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.sxryk.cn/gtxrpacson.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhaomingkeji.xyz/gtfoqrrskz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.pycfn.com/gtqbnlfdej.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.fengsongda.top/gtfvihtnqt.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.nwbrower.top/gtxrfwchna.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.chenjidiqi.icu/gtdvvcpwsx.html

================================================================================
来源：http://hz.xuetiantiany.cn/gteamrsgjr.html

K. JSON 与序列化
来源：http://hz.haohaochexian.top/gtydusgsoo.html

================================================================================
来源：http://hz.sufxvd.cn/gtrutzswje.html

[K01] 对象转 JSON 字符串
来源：http://hz.yj20258.top/gtzrkazvnw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ybcxt.top/gtoapyywpw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.gogol.net.cn/gtbotkeagz.html

JS:   JSON.stringify(obj)
来源：http://hz.zycfv.cn/gtfbeajrqd.html

TS:   JSON.stringify(obj)
来源：http://hz.jiagoushi.top/gtnqvbejgx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yangfankeji.com/gtcpkderfm.html

Go:   json.Marshal(obj)
来源：http://hz.zhixingplan.top/gtskwzbwyo.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.sweek.top/gtqhfamshh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.wangshuangyany.cn/gtquozuanh.html

[K02] JSON 字符串转对象
来源：http://hz.yj20258.top/gtvbxotrqv.html

Py:   json.loads(s)
来源：http://hz.jqgufenzy.top/gtunjndcdr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yongpay.top/gtuzgqxbgo.html

JS:   JSON.parse(s)
来源：http://hz.tianlin.xyz/gtkebnvhge.html

TS:   JSON.parse(s)
来源：http://hz.chenjidiqi.icu/gtzalavpoi.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhongyouzk.top/gtrbqenmiv.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.shangyingyoupin.top/gtyemhphgp.html

Ruby: JSON.parse(s)
来源：http://hz.52xcode.cn/gtglnfhzkv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jqgfzy.top/gtqyqmcmhj.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.tian-w.cn/gtbdxjuxoi.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ywan-chungtsiang.top/gtzfggkibp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.cheryme.top/gtupcrwcsq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jqgfzy.top/gtovrodiot.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhengqikj.top/gtnvnryevd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.gaohongyu789.top/gtmxugkawd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.nanxuanxn.top/gtgavteqvh.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhoulong.xyz/gtwxjidmlh.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.fengsongda.top/gtmfclzhqc.html

[K04] 读取 JSON 文件
来源：http://hz.9152youxi.cn/gtaweaawwr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xinyue.icu/gtmoqyzwjn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ivvv.top/gtcbhmuqun.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.guowangkeji.top/gtlybwaoev.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yuanzhike.top/gtujzkfsmg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.sysykeji.top/gtxvmnwxzc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.wangshuangyany.cn/gtodpymgld.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.guowangkeji.top/gtngegggpr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.iojbl.cn/gtcsptulml.html

[K05] 深拷贝对象
来源：http://hz.smart0.xyz/gtbcmtwrcj.html

Py:   copy.deepcopy(obj)
来源：http://hz.jiagoushi.top/gtbovvumey.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jiagoushi.top/gtfnilhqpy.html

JS:   structuredClone(obj)
来源：http://hz.dashuyun.cn/gtbmaaxvfh.html

TS:   structuredClone(obj)
来源：http://hz.daxiang520.top/gtwffcxkse.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.gotoacloud.top/gttzugnric.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xziqi.cn/gtzxdlrcdz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yueranfly.top/gtgdsptnmk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhaomingkeji.xyz/gtcadoovli.html

[K06] 解析 URL 查询串
来源：http://hz.pengpengdd.cyou/gtvyahppxy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.snrcjt.cn/gtcqfgfzdj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.c1oappe.top/gtkofatmto.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhengqikj.top/gtfkahyxfv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.guowangkeji.top/gtqbdtmnzv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.cqqwz.cn/gtcuvojylu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.aibaodan.cn/gtiamwsfxi.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ybcxt.top/gtedkqmjzl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.dianchejie.cn/gttykibcsu.html

[K07] 进制转换
来源：http://hz.yj20258.top/gtdhhipvmc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.daria6918.cn/gtbdfrfmma.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.cdnleiting.top/gtfzrmfraq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.redwolf501.top/gtrrypwdzx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jqgufenzy.top/gtpbaacdme.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.pengpengdd.cyou/gttfhovnrc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.redwolf501.top/gtxvdtoksr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yangfankeji.com/gtsbergzui.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.c1oappe.top/gteebxawjw.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.tianlin.xyz/gtqqsvpkah.html

Py:   pickle.dumps(obj)
来源：http://hz.sweek.top/gtowrjxjvk.html


<!-- 参考信息 -->