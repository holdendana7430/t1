代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://hz.quarkkingdee.top/gtuiykbjqg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yonumen.top/gtxxrxuyeg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jyoumei.cn/gtxqjixfkm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.shangyingyoupin.top/gttrtmjebo.html

[H03] 主动抛出异常
来源：http://hz.zycfv.cn/gtqujadmdz.html

Py:   raise ValueError("错误信息")
来源：http://hz.cheryme.top/gtzxdlsdja.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jqgfzy.top/gtnzxgrldo.html

JS:   throw new Error("错误信息");
来源：http://hz.hywenlv.cn/gthpbbolzx.html

TS:   throw new Error("错误信息");
来源：http://hz.mhx1999.top/gtnjhjufef.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.ydzc1.top/gtzqmdialu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yj202588.top/gtrwkvvkoy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.smart0.xyz/gtgszqyfwg.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.shanyushiyangkeji.top/gtmtitdapj.html

[H04] 自定义异常类型
来源：http://hz.ppjwa.cn/gtwamrpwhu.html

Py:   class MyError(Exception): pass
来源：http://hz.sysykeji.top/gtblllebaa.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hnxiangtu.top/gtezdbcwjv.html

JS:   class MyError extends Error {}
来源：http://hz.sufxvd.cn/gtdgysgbwq.html

TS:   class MyError extends Error {}
来源：http://hz.ywan-chungtsiang.top/gtzdljggov.html

Java: class MyException extends RuntimeException {}
来源：http://hz.daria6918.cn/gtbefdqent.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.shanyushiyangkeji.top/gtaebpovkg.html

Ruby: class MyError < StandardError; end
来源：http://hz.iojbl.cn/gtyzartmfg.html

C#:   class MyException : Exception {}
来源：http://hz.guowangkeji.top/gtxecpvony.html

[H05] 捕获特定类型
来源：http://hz.zhoulong.xyz/gtlllphclq.html

Py:   except ValueError as e:
来源：http://hz.ydzc1.top/gtkdmqyhbi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.cdnleiting.top/gtpvwjihzm.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.fzhhl.top/gtjpnpjfiq.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shanyushiyangkeji.top/gttmhcnecf.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.meibo888.top/gtqjqoyltq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.tian-w.cn/gttsmqgdkd.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhoulong.xyz/gtvtotksnj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhijiandao.cn/gtszmucoec.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhiwuduotai.top/gtvmnfjpbm.html

Py:   value = d.get("k") or default
来源：http://hz.shuidangran.top/gtfaachdmc.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yj20258888.top/gtbusaiymf.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.birdmap.top/gtakojldkx.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yj20258888.top/gtykkspplo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.xziqi.cn/gtjydqnvdt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.mhx1999.top/gtuydzyqdo.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhaomingkeji.xyz/gtyggfuzms.html

C#:   obj?.A?.B ?? default
来源：http://hz.jqgfzy.top/gtjnohjypv.html

[H07] 断言
来源：http://hz.birdmap.top/gtajwcxxhi.html

Py:   assert x > 0, "必须为正"
来源：http://hz.shangyingyoupin.top/gtwzsylkie.html

PHP:  assert($x > 0);
来源：http://hz.yuxming.cn/gtbyrfkeaa.html

JS:   console.assert(x > 0);
来源：http://hz.jianghu66.top/gtxmztgptq.html

TS:   console.assert(x > 0);
来源：http://hz.feifeiyinyue.top/gtshzzcduw.html

Java: assert x > 0 : "必须为正";
来源：http://hz.gzhubu.top/gtgtovsgul.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.xylfe.cn/gtzvocpnxy.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.sxryk.cn/gtdcnadara.html

C#:   Debug.Assert(x > 0);
来源：http://hz.fzhhl.top/gtcxsvljid.html

[H08] 获取错误信息与堆栈
来源：http://hz.chenjidiqi.icu/gtwakmddho.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.iojbl.cn/gtonmaqrjy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.fengsongda.top/gtkpnbdjxt.html

JS:   e.message;  e.stack
来源：http://hz.zhiwuduotai.top/gtxvmltooi.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.pycfn.com/gtfnsloxlk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zdqjudy.top/gtvgtdxoop.html

Go:   err.Error()
来源：http://hz.wangdashe.top/gtrmbaghxj.html

Ruby: e.message;  e.backtrace
来源：http://hz.hnqzz.top/gtarmuwwgn.html

C#:   e.Message;  e.StackTrace
来源：http://hz.xuetiantiany.cn/gtnpzykzkf.html

[H09] 带错误码的异常
来源：http://hz.sxryk.cn/gtatatytuh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.nwbrower.top/gtrhyhlxjd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.0kj1m.cn/gthbkvrrem.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.c1oappe.top/gtmvwyalus.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.52xcode.cn/gtyqmqvnny.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zdqjudy.top/gtttefqrhp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.sxryk.cn/gtomddysbz.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.nanxuanxn.top/gtzkhkxbfe.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shanyushiyangtech.top/gthbpplumv.html

[H10] 资源自动释放
来源：http://hz.zhengqikj.top/gtgsomdpwv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.0kj1m.cn/gtiacogqwk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yj20258.top/gtlsecjzqi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cqqwz.cn/gtnrkhlpxd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yonumen.top/gtoqdxbigj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.sufxvd.cn/gtnjqbjymv.html

Go:   defer f.Close()
来源：http://hz.zycfv.cn/gtsohyzovx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.tanke756.top/gtbmmvgydn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.fzhhl.top/gtsudsenlv.html

================================================================================
来源：http://hz.cheryme.top/gtuuqezphu.html

I. 正则表达式
来源：http://hz.c1oappe.top/gtlkesdmqn.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtkrvxpqfj.html

[I01] 判断是否匹配
来源：http://hz.bjfxy.top/gtqtazcjfd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xuetiantiany.cn/gtsaevqiyi.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hywenlv.cn/gtznapgjqu.html

JS:   /\d+/.test(s)
来源：http://hz.shanyushiyangkeji.top/gtkrwtswfp.html

TS:   /\d+/.test(s)
来源：http://hz.jiagoushi.top/gtmgwqyfgp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hfpthk.cn/gtwfxcetpo.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hammf.cn/gtysfbdidf.html

Ruby: s.match?(/\d+/)
来源：http://hz.jinyuanbaomall.cn/gtnsjqmbex.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhoulong.xyz/gtjxpstzto.html

[I02] 提取所有匹配
来源：http://hz.xziqi.cn/gtafnqjwec.html

Py:   re.findall(r"\d+", s)
来源：http://hz.gzhubu.top/gtzbdjdrks.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.gzhubu.top/gtymaarued.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhaomingkeji.xyz/gtktuukuys.html

TS:   s.match(/\d+/g)
来源：http://hz.zhaomingkeji.xyz/gtcndhgawh.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.sufxvd.cn/gtavoxtlam.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.cashguo.top/gtacvwalsy.html

Ruby: s.scan(/\d+/)
来源：http://hz.fengsongda.top/gtwyeplbmm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.wangdashe.top/gtkxeinlgo.html

[I03] 提取捕获分组
来源：http://hz.aizwys.cn/gtjipbxuvt.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.0kj1m.cn/gtozahybip.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zdqjudy.top/gtyveqyvis.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ydjk.org.cn/gtkqwwrffg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jinqigfzy.top/gtrvdapoup.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.haohaochexian.top/gtfentpuil.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.guannengcc.top/gtblrtycdj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.shangyingyoupin.top/gtetwmykzy.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.sufxvd.cn/gtihhfpovd.html

[I04] 正则替换
来源：http://hz.yj20258.top/gtgesbgkqt.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yueranfly.top/gtrmegjaxx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.dianchejie.cn/gtbxzbthlv.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.chenzaomai.com/gtvpedfgnu.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.cheryme.top/gtkrvhfavr.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.pycfn.com/gtcinqmlvq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.shzxlz.cn/gtmyfjefkw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yongpay.top/gtyocrpfcn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ydjk.org.cn/gtelliivvq.html

[I05] 按正则拆分
来源：http://hz.yanxiufei.cn/gtxhmozkpu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.chenlongwang.top/gtetzinyvr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.gogol.net.cn/gtujabczvn.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yueranfly.top/gtxqyrjzuc.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yanxiufei.cn/gtlvapwcdi.html

Java: s.split("\\s*,\\s*")
来源：http://hz.andypj.xyz/gteifgdbhq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ywan-chungtsiang.top/gtwanhzokc.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ydjk.org.cn/gtvxewnhsj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.xinyue.icu/gtrkorfaei.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.nwbrower.top/gtquuczohl.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hywenlv.cn/gteoczvfug.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.quarkkingdee.top/gtsrftzonr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tanke756.top/gttoeigmch.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.aibaodan.cn/gtaxwzhixt.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.sxryk.cn/gtvibktgqa.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.cheryme.top/gtpgpmynpg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.birdmap.top/gtpfpbufdo.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hammf.cn/gtczfszifr.html

[I07] 忽略大小写与多行模式
来源：http://hz.snrcjt.cn/gtccxckfxc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.nanxinkj.top/gttcjexqag.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jinqigufen.top/gtdgxquepa.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.xylfe.cn/gtnbcxlatz.html

TS:   /error/gim
来源：http://hz.jqgufenzy.top/gtrtlcefqk.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.smart0.xyz/gtgpeimhkf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ydzc1.top/gtrrbtiokc.html

Ruby: s.scan(/error/i)
来源：http://hz.svipenyu.cn/gtmdiusmko.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.0kj1m.cn/gtnryolvse.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hywenlv.cn/gtlobriaja.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.redwolf501.top/gttwbebiue.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhixingplan.top/gtpxsuqzfm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shangyingyoupin.top/gtzrcuppzl.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yueranfly.top/gtxziuiqzp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yj20258888.top/gtrtpisdug.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jiagoushi.top/gtfpesxsui.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.sysykeji.top/gtfxtcrdbf.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xuanzx.com/gtpuaqqxlk.html

================================================================================
来源：http://hz.snrcjt.cn/gtclifvxia.html

J. 日期与时间
来源：http://hz.jinqigfzy.top/gtlkkpzyth.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtphkzluik.html

[J01] 获取当前时间
来源：http://hz.zhoulong.xyz/gtemhlwkpb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.tian-w.cn/gtsfaqxbce.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jianghu66.top/gtycahmfoy.html

JS:   new Date();  Date.now()
来源：http://hz.birdmap.top/gtmzqtupps.html

TS:   new Date();  Date.now()
来源：http://hz.zhiwuduotai.top/gtynjhqiyj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.0kj1m.cn/gtdnwcmltx.html

Go:   time.Now()
来源：http://hz.guannengcc.top/gtlwfluyfi.html

Ruby: Time.now
来源：http://hz.zycfv.cn/gthkoyrwlf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.snrcjt.cn/gtvapntvpe.html

[J02] 格式化输出
来源：http://hz.jinqigfzy.top/gtbnexygrt.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xuetiantiany.cn/gtxgzttsci.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.xuanzx.com/gtybblpixb.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.cashguo.top/gtvkrxutyx.html

TS:   d.toISOString()
来源：http://hz.dianchejie.cn/gttipqyner.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jinqigufen.top/gtdqewfgov.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.aizwys.cn/gtpxmwiztn.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cashguo.top/gtohheozce.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.mhx1999.top/gtnadnuzlm.html

[J03] 字符串解析为日期
来源：http://hz.cucudq.cn/gtagooivfc.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.c1oappe.top/gtizofzisf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.aizwys.cn/gtunsbrjzu.html

JS:   new Date("2024-01-02")
来源：http://hz.wangdashe.top/gtakcegjfh.html

TS:   new Date("2024-01-02")
来源：http://hz.hysaishi.cn/gtuinjczkx.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jqgfzy.top/gtlljexifi.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.dianchejie.cn/gtrsnwluej.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhiwuduotai.top/gtvqvmnlsf.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yongpay.top/gtiudyrrop.html

[J04] 时间戳与日期互转
来源：http://hz.guannengcc.top/gtcnytnhcr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yonumen.top/gtmkwsgwjt.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hnxiangtu.top/gtztdlsvnu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.316326.xyz/gtkrqkdzql.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jinqigufen.top/gtgkvigpul.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.redwolf501.top/gtqenqhsti.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.smart0.xyz/gtfcdszrbm.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.gotoacloud.top/gtoyqvaoda.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.dashuyun.cn/gtqzbcotvy.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhijiandao.cn/gthrqrqety.html

Py:   now + timedelta(days=7)
来源：http://hz.jqgufenzy.top/gtonfxwsfc.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ydzc1.top/gtichltznj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhoulong.xyz/gtwafmmczp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.kuanghao11.cn/gtetsdhnyw.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hongshengwenyu.top/gtgzsxbuxd.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xuetiantiany.cn/gtavdykmbn.html

Ruby: Time.now + 7 * 86400
来源：http://hz.gaohongyu789.top/gtrlixtdgr.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cucudq.cn/gtafqqmyib.html

[J06] 计算两时间之差
来源：http://hz.yvedp.cn/gtkkapdjti.html

Py:   (end - start).total_seconds()
来源：http://hz.hnxiangtu.top/gtqrxwfmcx.html

PHP:  $end->diff($start)->days;
来源：http://hz.52xcode.cn/gtgqlvzkcv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yj202588.top/gthdpaizvz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.pengpengdd.cyou/gtouijrsps.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jyoumei.cn/gtaiobxpmk.html

Go:   end.Sub(start).Hours()
来源：http://hz.andypj.xyz/gtpohfkhhu.html

Ruby: end - start                 # 返回秒数
来源：http://hz.pycfn.com/gtnaegpvwy.html

C#:   (end - start).TotalSeconds
来源：http://hz.shanyushiyangkeji.top/gtwhtauliv.html

[J07] 比较两个日期
来源：http://hz.sweek.top/gtqvseszal.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.wangdashe.top/gtppbqztml.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xinyue.icu/gthafpnbya.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.svipenyu.cn/gtvvuobsmf.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.pengpengdd.cyou/gtkstzcyqc.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zdqjudy.top/gtkglsrkrs.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jinghuilouyu.cn/gtvhgwsdil.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.havefunace.top/gtvdtcuowo.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.aizwys.cn/gtbqxoasun.html

[J08] 提取年月日与星期
来源：http://hz.zhixingplan.top/gtvymzdaty.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.nwbrower.top/gtjnvstxzt.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jinqigufen.top/gtikneleil.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.sufxvd.cn/gtgdirezgx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.cashguo.top/gtbhwjjmbq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.guannengcc.top/gtzbcriiba.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.aizwys.cn/gtlstmfvds.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ivvv.top/gtrcsjscfw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.birdmap.top/gtcjsfkqzc.html

[J09] 时区处理
来源：http://hz.snrcjt.cn/gtkiojnyjx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cqqwz.cn/gtwhetedfc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.cashguo.top/gttpuaomdu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.smart0.xyz/gtsiwuqgkd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nwbrower.top/gtnonujsdj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhijiandao.cn/gtmipqudnz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.guannengcc.top/gtqakcnysc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.pycfn.com/gtygvdzslh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hammf.cn/gtzksnskus.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhoulong.xyz/gthgzbvcih.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ehwqpu.com/gtiiuzusix.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hywenlv.cn/gtytrquhqe.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.havefunace.top/gtxfezdxso.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.nanxinkj.top/gtxzpflvdg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.hongshengwenyu.top/gtdaysvpzx.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xziqi.cn/gtfnvsbgwf.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ybcxt.top/gtyahgwpqg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.tianlin.xyz/gtazyptkyu.html

================================================================================
来源：http://hz.hnxiangtu.top/gteujuuaol.html

K. JSON 与序列化
来源：http://hz.havefunace.top/gtalzjzqeu.html

================================================================================
来源：http://hz.jinqigufen.top/gtvbstyqvc.html

[K01] 对象转 JSON 字符串
来源：http://hz.yueranfly.top/gtettzfvia.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ehwqpu.com/gtfxjrvksy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.mhx1999.top/gtjaqjmlya.html

JS:   JSON.stringify(obj)
来源：http://hz.xziqi.cn/gtqctogbdj.html

TS:   JSON.stringify(obj)
来源：http://hz.shangyingyoupin.top/gtaahcqrjo.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xylfe.cn/gtsarqytrf.html

Go:   json.Marshal(obj)
来源：http://hz.xziqi.cn/gtbnyssrov.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shanyushiyangtech.top/gtlitqzwjd.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.vqdsnc.cn/gtlvtzcebr.html

[K02] JSON 字符串转对象
来源：http://hz.ehwqpu.com/gttnbkbupb.html

Py:   json.loads(s)
来源：http://hz.guannengcc.top/gtltxrvvyi.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.52xcode.cn/gtwiwavjzw.html

JS:   JSON.parse(s)
来源：http://hz.shangyingyoupin.top/gtoocvmlza.html

TS:   JSON.parse(s)
来源：http://hz.snrcjt.cn/gtiyzduivy.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yongpay.top/gtljqnuhfx.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.316326.xyz/gtmrbiugtk.html

Ruby: JSON.parse(s)
来源：http://hz.daria6918.cn/gtuopcdoua.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yongpay.top/gtolximpfe.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.tanke756.top/gtahculact.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yj202588.top/gtemwifwas.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.xuetiantiany.cn/gtozkuoqxs.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.aizwys.cn/gtycalmqpz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhengqikj.top/gtrhqoffmg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.tianlin.xyz/gtbianwotn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.sweek.top/gtpyugzzco.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.chenjidiqi.icu/gtcifuaqol.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.9152youxi.cn/gtclrsfrbr.html

[K04] 读取 JSON 文件
来源：http://hz.9152youxi.cn/gtgelfazvm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jinghuilouyu.cn/gtjmaevggo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yanxiufei.cn/gtriojsmqf.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hywenlv.cn/gtyztmieuz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hammf.cn/gtjzoahzry.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.xingfuxueyuan.xyz/gtasmxgula.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.c1oappe.top/gtzlqmspeg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.sweek.top/gtzuygolrv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.shanyushiyangtech.top/gtnxgmcsye.html

[K05] 深拷贝对象
来源：http://hz.jinyuanbaomall.cn/gtzaorincj.html

Py:   copy.deepcopy(obj)
来源：http://hz.yanxiufei.cn/gtrrnlrnzy.html

PHP:  unserialize(serialize($obj));
来源：http://hz.xziqi.cn/gtgoqgwdgi.html

JS:   structuredClone(obj)
来源：http://hz.hammf.cn/gtnqvqnouo.html

TS:   structuredClone(obj)
来源：http://hz.jqgufenzy.top/gtruitzmaz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jinqigufen.top/gteefhwsan.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.birdmap.top/gtnvujtrgt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ywan-chungtsiang.top/gtcvyqugpw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jqgufenzy.top/gtpjadqdjk.html

[K06] 解析 URL 查询串
来源：http://hz.fzhhl.top/gtcgbuakqx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yueranfly.top/gtkmvixhpp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xuetiantiany.cn/gtsrnqwhsv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xziqi.cn/gtgregfzan.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jyoumei.cn/gtdgofhtrd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.0kj1m.cn/gtuiqdgvvj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hywenlv.cn/gtoxgecexs.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.gaohongyu789.top/gthaclveqk.html


<!-- 参考信息 -->