代发 wailian999

JS:   class MyError extends Error {}
来源：http://hz.ivvv.top/gtvcxszvhl.html

TS:   class MyError extends Error {}
来源：http://hz.ydjk.org.cn/gtxzpjeqbr.html

Java: class MyException extends RuntimeException {}
来源：http://hz.haohaochexian.top/gtgytfvxjf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.hysaishi.cn/gtfsennbfm.html

Ruby: class MyError < StandardError; end
来源：http://hz.shzxlz.cn/gtnciqfwlm.html

C#:   class MyException : Exception {}
来源：http://hz.yueranfly.top/gtlkqelnpf.html

[H05] 捕获特定类型
来源：http://hz.jqgfzy.top/gtpdhdbnjn.html

Py:   except ValueError as e:
来源：http://hz.mhx1999.top/gtpvdzhvfn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hywenlv.cn/gtrscitbft.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.52xcode.cn/gtmddrtgud.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.sysykeji.top/gtjxhrrmkv.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yj20258888.top/gtlvvjlagk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.andypj.xyz/gtnvyqqbbj.html

Ruby: rescue ArgumentError => e
来源：http://hz.daxiang520.top/gtfszlcytx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hammf.cn/gtsywzpwmw.html

[H06] 可选值 / 空值安全访问
来源：http://hz.pengpengdd.cyou/gtftyfeewc.html

Py:   value = d.get("k") or default
来源：http://hz.xuetiantiany.cn/gtsxyavezg.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.quarkkingdee.top/gtemwcmrrq.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.aizwys.cn/gtgifhehfp.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yuxming.cn/gtaovcohcn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ydjk.org.cn/gtramnlism.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhijiandao.cn/gtkhkzqowf.html

Ruby: d&.dig(:a, :b)
来源：http://hz.shangyingyoupin.top/gtbjeaosdu.html

C#:   obj?.A?.B ?? default
来源：http://hz.sxryk.cn/gtnkgyobiq.html

[H07] 断言
来源：http://hz.hywenlv.cn/gtydgjlkaz.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yvedp.cn/gteqdsuaer.html

PHP:  assert($x > 0);
来源：http://hz.ydzc1.top/gtbopnlseg.html

JS:   console.assert(x > 0);
来源：http://hz.dashuyun.cn/gtunvtlewl.html

TS:   console.assert(x > 0);
来源：http://hz.pengpengdd.cyou/gtenrjgnxh.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yj202588.top/gtcltcgkke.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jqgfzy.top/gtmsbtfbdv.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jinyuanbaomall.cn/gtwiqlfjxz.html

C#:   Debug.Assert(x > 0);
来源：http://hz.xylfe.cn/gtybjgcvyz.html

[H08] 获取错误信息与堆栈
来源：http://hz.meibo888.top/gtktoifahk.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.0kj1m.cn/gtawomvwua.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.c1oappe.top/gtsbjoziee.html

JS:   e.message;  e.stack
来源：http://hz.shanyushiyangkeji.top/gtgzbpolsq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.c1oappe.top/gtknbphqej.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhengqikj.top/gtogixglgp.html

Go:   err.Error()
来源：http://hz.hywenlv.cn/gtwavgwilh.html

Ruby: e.message;  e.backtrace
来源：http://hz.bjfxy.top/gtwpopjmcm.html

C#:   e.Message;  e.StackTrace
来源：http://hz.quarkkingdee.top/gtyhnhnvci.html

[H09] 带错误码的异常
来源：http://hz.shanyushiyangkeji.top/gtrjnvsqhn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.shanyushiyangtech.top/gtcdwmccfw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.nanxinkj.top/gtxvjevbed.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.tanke756.top/gtnxrlmrgv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yuxming.cn/gtzzhhcnbp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.meibo888.top/gtvwifgccw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.pengpengdd.cyou/gtbohxbkpq.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.tian-w.cn/gtgonwxdfh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ppjwa.cn/gtgdxvkiqp.html

[H10] 资源自动释放
来源：http://hz.cucudq.cn/gtgeuyrgcu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.gogol.net.cn/gtnaukdxvv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.shanyushiyangkeji.top/gtmqochdvr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhixingplan.top/gtowlirtou.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.fengsongda.top/gthmecvtvx.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.aizwys.cn/gtnkgricgx.html

Go:   defer f.Close()
来源：http://hz.chenjidiqi.icu/gtpqcwuuwz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.ydzc1.top/gtjnujkbxu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.aibaodan.cn/gtojdvoewk.html

================================================================================
来源：http://hz.dianchejie.cn/gtmxuqtxki.html

I. 正则表达式
来源：http://hz.jqgufenzy.top/gtcutzujie.html

================================================================================
来源：http://hz.iojbl.cn/gtufnsygie.html

[I01] 判断是否匹配
来源：http://hz.ybcxt.top/gtrwsfcogr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.guannengcc.top/gtiuqqtzwg.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.haohaochexian.top/gtkyueoifx.html

JS:   /\d+/.test(s)
来源：http://hz.tanke756.top/gtpdfuvmyw.html

TS:   /\d+/.test(s)
来源：http://hz.tianlin.xyz/gtrwfmdvbw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hywenlv.cn/gtgivwellg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.aibaodan.cn/gtsuoyqqfl.html

Ruby: s.match?(/\d+/)
来源：http://hz.shangyingyoupin.top/gtblggudro.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.c1oappe.top/gtmkgvomtj.html

[I02] 提取所有匹配
来源：http://hz.zhijiandao.cn/gtaqolzkek.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yangfankeji.com/gtlpqjrtis.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.316326.xyz/gtclwcnfgi.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.nanxuanxn.top/gthknxhmsr.html

TS:   s.match(/\d+/g)
来源：http://hz.yvedp.cn/gtoakgzatt.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.vqdsnc.cn/gtdqtooaww.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.cucudq.cn/gtqoswjxwb.html

Ruby: s.scan(/\d+/)
来源：http://hz.wangshuangyany.cn/gtwipqebhf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xylfe.cn/gtpklmpjie.html

[I03] 提取捕获分组
来源：http://hz.yonumen.top/gtziwsryrt.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ybcxt.top/gtezyfdkmj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xinyue.icu/gtmuhvybfe.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.xuetiantiany.cn/gtouewxvxu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yj202588.top/gtsjuefkvt.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jqgfzy.top/gtivlsieok.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.gotoacloud.top/gtnkrbebzw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.nanxinkj.top/gttrgqfsiy.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.shuidangran.top/gtuamvzzhm.html

[I04] 正则替换
来源：http://hz.wangdashe.top/gtxvgcbgeg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.fzhhl.top/gtpbvyudll.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.316326.xyz/gtojeutkjf.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.shanyushiyangkeji.top/gtqzpjnued.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.gotoacloud.top/gtciioimpn.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jlsjyb.cn/gtvllekolh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.svipenyu.cn/gtvitechvb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhaomingkeji.xyz/gtzuarektl.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yueranfly.top/gtocyuhtna.html

[I05] 按正则拆分
来源：http://hz.jyoumei.cn/gtexpddvum.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.nanxuanxn.top/gtxqampfwu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.0kj1m.cn/gticgtjsxn.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.pengpengdd.cyou/gtimkwbrwm.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.quarkkingdee.top/gtlopbejcx.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jqgufenzy.top/gtpyzamflr.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhongyouzk.top/gthblekmhi.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yonumen.top/gtayvxipdz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hongshengwenyu.top/gtuzujrlca.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jinqigfzy.top/gtkktqdxyu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.c1oappe.top/gtwaxviudq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hywenlv.cn/gtehvbjmxl.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinqigfzy.top/gthtpuwvmq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hnqzz.top/gtwoijdzkw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.52xcode.cn/gtucfjyjel.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.feifeiyinyue.top/gtkkmkqkqr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jiagoushi.top/gtynnbhzqe.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.havefunace.top/gtccjdxjqo.html

[I07] 忽略大小写与多行模式
来源：http://hz.tanke756.top/gtfkrrrzrd.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.sysykeji.top/gtgfldpabp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.tianlin.xyz/gthsmbuanh.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yuxming.cn/gthhschkvh.html

TS:   /error/gim
来源：http://hz.wangdashe.top/gtfzdcwhbs.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.shuidangran.top/gtvkjhigme.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.shuidangran.top/gtjsdsgsoh.html

Ruby: s.scan(/error/i)
来源：http://hz.ydjk.org.cn/gtpfkxqfad.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yuanzhike.top/gtvawhxqgj.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yj20258.top/gtgchhmpus.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yueranfly.top/gtztssjzft.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.andypj.xyz/gtoqsyfrex.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.meibo888.top/gtuofuaedd.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.9152youxi.cn/gtvgcyktgw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hnqzz.top/gtoukbirzc.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jinqigfzy.top/gtlavyuhse.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.aibaodan.cn/gtgqmwzegq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.haohaochexian.top/gtgxmrabov.html

================================================================================
来源：http://hz.xylfe.cn/gtbwfarqrz.html

J. 日期与时间
来源：http://hz.chenlongwang.top/gtpxcbrisn.html

================================================================================
来源：http://hz.yj20258888.top/gtuxuqmxuz.html

[J01] 获取当前时间
来源：http://hz.yanxiufei.cn/gtkomkzdpm.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.guowangkeji.top/gtjpujbobe.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhengqikj.top/gtrueaubuy.html

JS:   new Date();  Date.now()
来源：http://hz.yueranfly.top/gtpugoidna.html

TS:   new Date();  Date.now()
来源：http://hz.wangshuangyany.cn/gtngrkepmg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zdqjudy.top/gtyaxksqus.html

Go:   time.Now()
来源：http://hz.nanxuanxn.top/gtuycvolzk.html

Ruby: Time.now
来源：http://hz.jinqigufen.top/gtmyflmeok.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ybcxt.top/gtgeghyexe.html

[J02] 格式化输出
来源：http://hz.dianchejie.cn/gtrrvkuhdf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinyuanbaomall.cn/gtkbfukkfy.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.fzhhl.top/gtisxjtapg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.nwbrower.top/gtsbauildp.html

TS:   d.toISOString()
来源：http://hz.zhengqikj.top/gtkqzmawvw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.cqqwz.cn/gteydscteh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hongshengwenyu.top/gtaslrwzml.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.dianchejie.cn/gtsdtvrosi.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.kuanghao11.cn/gteokzyihw.html

[J03] 字符串解析为日期
来源：http://hz.yanxiufei.cn/gthdelrilt.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.cucudq.cn/gtjmpxjabc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.shuidangran.top/gtvvyffdkl.html

JS:   new Date("2024-01-02")
来源：http://hz.yuxming.cn/gteypyxozo.html

TS:   new Date("2024-01-02")
来源：http://hz.shanyushiyangkeji.top/gtzxtwvlqq.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xinyue.icu/gtcqwmcpic.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zycfv.cn/gtrcpckmrz.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.shuidangran.top/gteczdyfdv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yuxming.cn/gtgnelxrdt.html

[J04] 时间戳与日期互转
来源：http://hz.gaohongyu789.top/gtholtmsmu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.xuetiantiany.cn/gtnapramqe.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.nwbrower.top/gtriceovbo.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.nanxuanxn.top/gtdgxsgkrg.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.gotoacloud.top/gttejpqfet.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.tianlin.xyz/gtyvurmizy.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yj20258.top/gtxaxgmnsn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.sxryk.cn/gtznjrqilm.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.gotoacloud.top/gtkmxykhtq.html

[J05] 时间加减（加 7 天）
来源：http://hz.chenzaomai.com/gtihfcmbbm.html

Py:   now + timedelta(days=7)
来源：http://hz.shzxlz.cn/gtevohgwlf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ydjk.org.cn/gtvqlixzer.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.feifeiyinyue.top/gtfktngodq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nanxinkj.top/gticwauwqp.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.ivvv.top/gtoocsdxzl.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.meibo888.top/gthfycjrbu.html

Ruby: Time.now + 7 * 86400
来源：http://hz.9152youxi.cn/gtxgierzfn.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zdqjudy.top/gtmahbifkq.html

[J06] 计算两时间之差
来源：http://hz.ehwqpu.com/gtwkjjyslq.html

Py:   (end - start).total_seconds()
来源：http://hz.cheryme.top/gtclfdossy.html

PHP:  $end->diff($start)->days;
来源：http://hz.jianghu66.top/gtjrmjoatf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.shuidangran.top/gtflfyldrf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.havefunace.top/gtsnjcuopy.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yangfankeji.com/gtitvkdcbz.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhiwuduotai.top/gtyuxmvsui.html

Ruby: end - start                 # 返回秒数
来源：http://hz.tian-w.cn/gtgdwzjblq.html

C#:   (end - start).TotalSeconds
来源：http://hz.birdmap.top/gtyeondywr.html

[J07] 比较两个日期
来源：http://hz.yj202588.top/gtbmssxjmw.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.daria6918.cn/gtyysbflsi.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.52xcode.cn/gtgkwsrbpf.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.feifeiyinyue.top/gtgsyofubp.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.iojbl.cn/gttfimxsgg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.quarkkingdee.top/gtjuozqlgv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hfpthk.cn/gtkfsowaez.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.sxryk.cn/gtnwkowhmj.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.cheryme.top/gteckpccur.html

[J08] 提取年月日与星期
来源：http://hz.hnxiangtu.top/gtklcafsrv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.nwbrower.top/gtkwzsaymd.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jiagoushi.top/gthtscjlvk.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yonumen.top/gtunlmgjxm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jinqigfzy.top/gtisyyednw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.vqdsnc.cn/gtzdjtbqdt.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zdqjudy.top/gtsqaquhbm.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yj20258.top/gtwqqaopie.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hywenlv.cn/gthxrenfcz.html

[J09] 时区处理
来源：http://hz.wangshuangyany.cn/gtqtwkdmoz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ydjk.org.cn/gtvnsbnxfq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.daxiang520.top/gthaijfzdf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zdqjudy.top/gthzvthhsa.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ydzc1.top/gtalltoxcg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xziqi.cn/gtkqjruqfg.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jinyuanbaomall.cn/gtlxpvprfr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.xuanzx.com/gtohmvmnfq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.c1oappe.top/gtqdpkqnua.html

[J10] 取今天 / 本月第一天
来源：http://hz.feifeiyinyue.top/gtaqbntvfa.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yvedp.cn/gtkpmnimxh.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hysaishi.cn/gtpbvsunuw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.snrcjt.cn/gtucakhopa.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ivvv.top/gtfuevxfhh.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jqgufenzy.top/gtyclqirpe.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.redwolf501.top/gtbnhjszaz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhengqikj.top/gtiomoltbr.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.9152youxi.cn/gtvjvtybpk.html

================================================================================
来源：http://hz.sweek.top/gtcyjlkpch.html

K. JSON 与序列化
来源：http://hz.yanxiufei.cn/gtmxenpajr.html

================================================================================
来源：http://hz.cdnleiting.top/gtuewakqti.html

[K01] 对象转 JSON 字符串
来源：http://hz.yj20258.top/gtpotqiaxo.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.nwbrower.top/gtlpypztok.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.iojbl.cn/gtovoyksbi.html

JS:   JSON.stringify(obj)
来源：http://hz.jqgfzy.top/gtnmrakilq.html

TS:   JSON.stringify(obj)
来源：http://hz.fengsongda.top/gtrxoqqnns.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jyoumei.cn/gtwsuozkjs.html

Go:   json.Marshal(obj)
来源：http://hz.jinyuanbaomall.cn/gtzzdqgzni.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cdnleiting.top/gtcwwxnsnk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.c1oappe.top/gtbpwxexwd.html

[K02] JSON 字符串转对象
来源：http://hz.yuxming.cn/gtsufptgve.html

Py:   json.loads(s)
来源：http://hz.smart0.xyz/gtsnybgekp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jqgfzy.top/gtidhdmhtv.html

JS:   JSON.parse(s)
来源：http://hz.gaohongyu789.top/gtfbkuajfl.html

TS:   JSON.parse(s)
来源：http://hz.havefunace.top/gtbsyfjrjb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.nwbrower.top/gtlbjkauey.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.gzhubu.top/gtbkaqrgdg.html

Ruby: JSON.parse(s)
来源：http://hz.gogol.net.cn/gttuizsjjm.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ivvv.top/gthroevcpv.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ivvv.top/gtrkhqblgl.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hywenlv.cn/gtvmfcyktb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhiwuduotai.top/gtocroqlhj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ppjwa.cn/gtesrcstnj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhixingplan.top/gttttuzuqc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.cheryme.top/gtdnuworji.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhijiandao.cn/gtnkxzgwem.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.svipenyu.cn/gtbtukjedz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.shangyingyoupin.top/gtpejfkjvd.html

[K04] 读取 JSON 文件
来源：http://hz.shangyingyoupin.top/gtfibpptio.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.bjfxy.top/gtswhefbbo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.meibo888.top/gtnigowbgu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jlsjyb.cn/gtvihdijme.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.havefunace.top/gtbpwgdhhe.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yonumen.top/gtjemhfvlt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jianghu66.top/gtszchyhdl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jqgfzy.top/gtuikoaeqc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.feifeiyinyue.top/gtoisqgjav.html

[K05] 深拷贝对象
来源：http://hz.haohaochexian.top/gturqemhtz.html

Py:   copy.deepcopy(obj)
来源：http://hz.daxiang520.top/gtmtclgtin.html

PHP:  unserialize(serialize($obj));
来源：http://hz.0kj1m.cn/gtynuqrhmw.html

JS:   structuredClone(obj)
来源：http://hz.pengpengdd.cyou/gtikxozrwf.html

TS:   structuredClone(obj)
来源：http://hz.pengpengdd.cyou/gtpuhrhdpt.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.sufxvd.cn/gtzqeawzat.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.meibo888.top/gteifwdfxg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jlsjyb.cn/gtthkdrxxp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.aizwys.cn/gtbcdilcru.html

[K06] 解析 URL 查询串
来源：http://hz.yuanzhike.top/gtumbvrnos.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jinqigfzy.top/gtauztsheh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hammf.cn/gtfkycnyop.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ehwqpu.com/gtnxybvtyu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.pycfn.com/gtdovgnmbv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.xziqi.cn/gtgmxowdzt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhiwuduotai.top/gtzqfkdbka.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.shzxlz.cn/gtuoafofvb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ivvv.top/gtwneizkkz.html

[K07] 进制转换
来源：http://hz.shuidangran.top/gtrdlrffhy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.gzhubu.top/gtuaoenkal.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.cucudq.cn/gtlkcxnfjb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhaomingkeji.xyz/gtmxmrqzpo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhaomingkeji.xyz/gthkiygrjm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cqqwz.cn/gtmrtlerih.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhongyouzk.top/gtdustajdq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xylfe.cn/gthugewbql.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.daxiang520.top/gthvsgyljb.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.cqqwz.cn/gtzrojemkk.html

Py:   pickle.dumps(obj)
来源：http://hz.cdnleiting.top/gtjfpzdvgo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hnqzz.top/gtnhdgwpbe.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yangfankeji.com/gtvqhebrdr.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.sxryk.cn/gtimetfwbs.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.shangyingyoupin.top/gthaabhfvh.html


<!-- 参考信息 -->