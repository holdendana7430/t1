代发 wailian999

TS:   throw new Error("错误信息");
来源：http://hz.hywenlv.cn/gtyigjprqk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.aizwys.cn/gtgkdwdwku.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.xinyue.icu/gtfotndnan.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhongyouzk.top/gtaqijtdfu.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.redwolf501.top/gtkfpwsbai.html

[H04] 自定义异常类型
来源：http://hz.0kj1m.cn/gtuakysqap.html

Py:   class MyError(Exception): pass
来源：http://hz.ybcxt.top/gtguzmgmjc.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.birdmap.top/gtpyllhbpb.html

JS:   class MyError extends Error {}
来源：http://hz.hnxiangtu.top/gthtlretne.html

TS:   class MyError extends Error {}
来源：http://hz.jyoumei.cn/gtwnvxoelf.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhongyouzk.top/gtptrikpau.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.svipenyu.cn/gtnyrsvjje.html

Ruby: class MyError < StandardError; end
来源：http://hz.jlsjyb.cn/gtsqirusof.html

C#:   class MyException : Exception {}
来源：http://hz.jinghuilouyu.cn/gtcgyvgnex.html

[H05] 捕获特定类型
来源：http://hz.feifeiyinyue.top/gtafhqwjuf.html

Py:   except ValueError as e:
来源：http://hz.fengsongda.top/gtinorruqm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.sxryk.cn/gtckskvdwq.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhijiandao.cn/gteexhgaaj.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.smart0.xyz/gtwbhjykgi.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jianghu66.top/gtounjomdu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yongpay.top/gtujfqaixx.html

Ruby: rescue ArgumentError => e
来源：http://hz.yvedp.cn/gtedvfgjuq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.chenlongwang.top/gtqmlbimct.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hongshengwenyu.top/gtwybovnst.html

Py:   value = d.get("k") or default
来源：http://hz.yongpay.top/gtdmufrimt.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhengqikj.top/gtoqttrqiq.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ydzc1.top/gtvmduircr.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yvedp.cn/gtmgspkofa.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yj202588.top/gtggqnvivk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.tian-w.cn/gteydcabmw.html

Ruby: d&.dig(:a, :b)
来源：http://hz.gogol.net.cn/gtremkqoiu.html

C#:   obj?.A?.B ?? default
来源：http://hz.hfpthk.cn/gthchylwhk.html

[H07] 断言
来源：http://hz.hfpthk.cn/gtnrdyvrni.html

Py:   assert x > 0, "必须为正"
来源：http://hz.meibo888.top/gtefupfiqc.html

PHP:  assert($x > 0);
来源：http://hz.mhx1999.top/gtoevjlrik.html

JS:   console.assert(x > 0);
来源：http://hz.tanke756.top/gttnmxrsdf.html

TS:   console.assert(x > 0);
来源：http://hz.52xcode.cn/gtpvehgslh.html

Java: assert x > 0 : "必须为正";
来源：http://hz.pengpengdd.cyou/gtcsfrlzei.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.mhx1999.top/gtkgqryrry.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ppjwa.cn/gtfxjrqgct.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhaomingkeji.xyz/gtzydpigyr.html

[H08] 获取错误信息与堆栈
来源：http://hz.tianlin.xyz/gtmkcrbkql.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.tianlin.xyz/gticnpcufu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ivvv.top/gtioijeybh.html

JS:   e.message;  e.stack
来源：http://hz.birdmap.top/gthaikqfbo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jinqigufen.top/gtbfcqlwxr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hysaishi.cn/gtqidfmjmo.html

Go:   err.Error()
来源：http://hz.hywenlv.cn/gtmqwtvcpr.html

Ruby: e.message;  e.backtrace
来源：http://hz.jinghuilouyu.cn/gttgvlwuml.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhongyouzk.top/gtkyafwmtt.html

[H09] 带错误码的异常
来源：http://hz.nanxuanxn.top/gtusadluof.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.cucudq.cn/gtlxybevkr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hywenlv.cn/gtwfcvvilo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jqgfzy.top/gtwmgjhhto.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.cqqwz.cn/gtfgopsecu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jinqigufen.top/gtdphmwjjv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhongyouzk.top/gthzqrpwji.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.nanxuanxn.top/gtpnpobdit.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.cucudq.cn/gtdyyzxgoy.html

[H10] 资源自动释放
来源：http://hz.hfpthk.cn/gtbbbbsrep.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shanyushiyangtech.top/gthaalotjy.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yuxming.cn/gtmpvsruzy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hnqzz.top/gtvbmuuaxt.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.c1oappe.top/gtplgvfkou.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hnqzz.top/gtrdhneprw.html

Go:   defer f.Close()
来源：http://hz.sweek.top/gtddgdspvs.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jyoumei.cn/gtvorswjwb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtwnfcfnft.html

================================================================================
来源：http://hz.jinqigfzy.top/gturozsuch.html

I. 正则表达式
来源：http://hz.chenjidiqi.icu/gtvehoxjtd.html

================================================================================
来源：http://hz.xylfe.cn/gtqwdjgrst.html

[I01] 判断是否匹配
来源：http://hz.ehwqpu.com/gtumbwgisq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yueranfly.top/gteqqqhvpq.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.gzhubu.top/gtspzqjflb.html

JS:   /\d+/.test(s)
来源：http://hz.fengsongda.top/gtzzofdyer.html

TS:   /\d+/.test(s)
来源：http://hz.cdnleiting.top/gttgqjpcxw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.aizwys.cn/gtigabieab.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhijiandao.cn/gtkyhhjhts.html

Ruby: s.match?(/\d+/)
来源：http://hz.cucudq.cn/gtcpxhypse.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.fengsongda.top/gtdleixpnf.html

[I02] 提取所有匹配
来源：http://hz.zycfv.cn/gtofxjrlyl.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jinqigfzy.top/gtscevqhnb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.ppjwa.cn/gtvkwekbbt.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.chenjidiqi.icu/gtypllcmba.html

TS:   s.match(/\d+/g)
来源：http://hz.zhengqikj.top/gtapsamvtd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.9152youxi.cn/gtqtmvqmnh.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.shangyingyoupin.top/gtqlhbbflw.html

Ruby: s.scan(/\d+/)
来源：http://hz.ppjwa.cn/gtluzgdwnc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.smart0.xyz/gtvgydngbf.html

[I03] 提取捕获分组
来源：http://hz.yj20258.top/gttspsiiws.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ydzc1.top/gtedwpnnyp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.vqdsnc.cn/gtyhfrnolj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jinqigfzy.top/gtomwwmakr.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hnxiangtu.top/gtogfcmqef.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.sysykeji.top/gtupqauzyy.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.sufxvd.cn/gtzqoxncaj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yvedp.cn/gtpziwvmiv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.wangdashe.top/gtizhbhjro.html

[I04] 正则替换
来源：http://hz.redwolf501.top/gthxmqwgyc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yj202588.top/gtyjhdtwgm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.chenzaomai.com/gtbeinbtei.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zhiwuduotai.top/gtsfahadqw.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.gaohongyu789.top/gtqyqvkqxe.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.bjfxy.top/gttxkbwxjj.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yongpay.top/gtwephrrdn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.sufxvd.cn/gtvvulhqhz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.guannengcc.top/gtvysgoxpq.html

[I05] 按正则拆分
来源：http://hz.xingfuxueyuan.xyz/gtjvyejdxa.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yueranfly.top/gtuvtsamox.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.shanyushiyangkeji.top/gtzdvpbctx.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jyoumei.cn/gtlswhipzq.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yanxiufei.cn/gtryigannk.html

Java: s.split("\\s*,\\s*")
来源：http://hz.gotoacloud.top/gtaevblnmy.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yuxming.cn/gthrtlfive.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.feifeiyinyue.top/gtumugjiit.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.birdmap.top/gtyidwjflc.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.tianlin.xyz/gtfamwlolv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.tianlin.xyz/gtagxognwy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.meibo888.top/gtkfrwuiwi.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.52xcode.cn/gtvybsfpbs.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xinyue.icu/gttzntdwfu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yuanzhike.top/gtbsdsztjc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.shuidangran.top/gtgxijnhgn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yj202588.top/gtbhydurdj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xziqi.cn/gtzuwtynsf.html

[I07] 忽略大小写与多行模式
来源：http://hz.iojbl.cn/gtfudzskpb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ybcxt.top/gtpqakqbbo.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xziqi.cn/gtmednvfdy.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.daxiang520.top/gtyoxdopsk.html

TS:   /error/gim
来源：http://hz.ivvv.top/gtnstixert.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hnqzz.top/gtnanncdig.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.xuanzx.com/gtzkuubbts.html

Ruby: s.scan(/error/i)
来源：http://hz.yuxming.cn/gtougxiofl.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.hnqzz.top/gtmwrxkiwo.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.quarkkingdee.top/gtmkhrekoz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ydzc1.top/gtadcrmske.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.shanyushiyangtech.top/gtnvadozyb.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sysykeji.top/gtfosmhxad.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.aizwys.cn/gtlmewzuoe.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.shangyingyoupin.top/gtnpovsmyi.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.hysaishi.cn/gtwfaoeeml.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jiagoushi.top/gthzprrhqq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xinyue.icu/gthoalbndn.html

================================================================================
来源：http://hz.zhijiandao.cn/gtroazrxze.html

J. 日期与时间
来源：http://hz.daria6918.cn/gtwmqfahhd.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtnqnhtrio.html

[J01] 获取当前时间
来源：http://hz.aizwys.cn/gtwfjcehok.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yj20258888.top/gtnwbqwrwo.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ehwqpu.com/gturefihsi.html

JS:   new Date();  Date.now()
来源：http://hz.shuidangran.top/gtwusqkgjo.html

TS:   new Date();  Date.now()
来源：http://hz.sweek.top/gtarvawqcj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.smart0.xyz/gttfspguzn.html

Go:   time.Now()
来源：http://hz.tian-w.cn/gtpqxfahcq.html

Ruby: Time.now
来源：http://hz.yj20258.top/gtfibwaxec.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.daxiang520.top/gtcfqbtoyz.html

[J02] 格式化输出
来源：http://hz.cucudq.cn/gtbbrikngn.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.feifeiyinyue.top/gtngbgecrq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jlsjyb.cn/gtyljhplbn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.tanke756.top/gtghihfywx.html

TS:   d.toISOString()
来源：http://hz.52xcode.cn/gtnaqttocx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.tianlin.xyz/gtqmegizis.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.birdmap.top/gtnzdquasi.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj202588.top/gttdhpgaxd.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhijiandao.cn/gthwwjdvwq.html

[J03] 字符串解析为日期
来源：http://hz.svipenyu.cn/gtlqlklfth.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.snrcjt.cn/gtfskmgxef.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hysaishi.cn/gttmvomdtu.html

JS:   new Date("2024-01-02")
来源：http://hz.zdqjudy.top/gttfiargpm.html

TS:   new Date("2024-01-02")
来源：http://hz.xziqi.cn/gttrrdywxb.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.ybcxt.top/gtqiolquei.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.shuidangran.top/gtjrvzynrn.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cheryme.top/gtrszxeoix.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ydjk.org.cn/gtkjawgazv.html

[J04] 时间戳与日期互转
来源：http://hz.jyoumei.cn/gtfmxzmotl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jinyuanbaomall.cn/gtfwtgqcji.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.gotoacloud.top/gtxybkymxp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.svipenyu.cn/gtvosmcemn.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hammf.cn/gtogfbnzku.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.redwolf501.top/gtzuuvgbje.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.sufxvd.cn/gtheypglew.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.0kj1m.cn/gthrjnxqpd.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jqgfzy.top/gtnqmdnvaa.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhaomingkeji.xyz/gtdjexoutr.html

Py:   now + timedelta(days=7)
来源：http://hz.wangdashe.top/gtrlnzejtt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.meibo888.top/gtdgbamtol.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.quarkkingdee.top/gtfbyxztzo.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.daria6918.cn/gtrmrbhydz.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yongpay.top/gtlvguigwf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jinghuilouyu.cn/gtnqwryhif.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xuanzx.com/gtnaqjlecq.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jlsjyb.cn/gtztgenmdx.html

[J06] 计算两时间之差
来源：http://hz.haohaochexian.top/gtgicdisbh.html

Py:   (end - start).total_seconds()
来源：http://hz.meibo888.top/gtxhkuerjz.html

PHP:  $end->diff($start)->days;
来源：http://hz.cdnleiting.top/gtaflledhe.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.9152youxi.cn/gtcbpnfmqb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.pengpengdd.cyou/gtizutejek.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hnqzz.top/gtgriohzyl.html

Go:   end.Sub(start).Hours()
来源：http://hz.hnqzz.top/gtitlnablw.html

Ruby: end - start                 # 返回秒数
来源：http://hz.redwolf501.top/gtdwmtkjrc.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhoulong.xyz/gtfmawqene.html

[J07] 比较两个日期
来源：http://hz.nwbrower.top/gtpfxehknr.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ybcxt.top/gtvuzvpslc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xinyue.icu/gtvhvuxabj.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.fengsongda.top/gtgutfuzse.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jqgfzy.top/gtilryzfnu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhijiandao.cn/gtshldtxxh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.guowangkeji.top/gtmaplhofn.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.wangshuangyany.cn/gtbaamakdy.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hnqzz.top/gtityaguwm.html

[J08] 提取年月日与星期
来源：http://hz.gotoacloud.top/gttmslsbel.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.sweek.top/gtbigcwrof.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xinyue.icu/gtyuucozjh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.gotoacloud.top/gtgkflqypw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.iojbl.cn/gtwthorxpy.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.tanke756.top/gtqysatgxy.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jlsjyb.cn/gtffwzxugh.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.andypj.xyz/gtfpsretma.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xuetiantiany.cn/gtzcdaabwg.html

[J09] 时区处理
来源：http://hz.yuxming.cn/gtnemunhzh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jqgufenzy.top/gtdkzdovrc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jqgufenzy.top/gtbdgnkmwi.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.chenjidiqi.icu/gtwwlnoasb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.meibo888.top/gtgqkiyywb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zycfv.cn/gtwahddieq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yj20258888.top/gtsoibwhwq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhijiandao.cn/gtqvysafkf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.sweek.top/gtgukrzocx.html

[J10] 取今天 / 本月第一天
来源：http://hz.xinyue.icu/gtefeezryx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.xuanzx.com/gtjikbkqgy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.havefunace.top/gtggxeboxu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jlsjyb.cn/gtheoiiulx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.nanxinkj.top/gtdlthmisu.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhengqikj.top/gtjsjstfrv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.smart0.xyz/gtyekxvlit.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xuetiantiany.cn/gtqcimjhst.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yvedp.cn/gtbezrytxm.html

================================================================================
来源：http://hz.yuxming.cn/gtjxbmbski.html

K. JSON 与序列化
来源：http://hz.zhoulong.xyz/gtgdulviyg.html

================================================================================
来源：http://hz.guowangkeji.top/gtlhzneqmq.html

[K01] 对象转 JSON 字符串
来源：http://hz.cdnleiting.top/gtmovtbecn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zhaomingkeji.xyz/gtzlgzewnr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.sufxvd.cn/gtpgyahgnc.html

JS:   JSON.stringify(obj)
来源：http://hz.jiagoushi.top/gtzbetydub.html

TS:   JSON.stringify(obj)
来源：http://hz.zhongyouzk.top/gtvikwegek.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hywenlv.cn/gtyaugzvoz.html

Go:   json.Marshal(obj)
来源：http://hz.shuidangran.top/gtglzbwpfv.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cucudq.cn/gtajdyydiy.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.cucudq.cn/gtetiiwtfn.html

[K02] JSON 字符串转对象
来源：http://hz.yonumen.top/gtxvaexznl.html

Py:   json.loads(s)
来源：http://hz.52xcode.cn/gtkazlzscd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.meibo888.top/gtauyffzzq.html

JS:   JSON.parse(s)
来源：http://hz.ybcxt.top/gtnyvpwuia.html

TS:   JSON.parse(s)
来源：http://hz.xylfe.cn/gtmgucvskk.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yvedp.cn/gtsmqbrdve.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ehwqpu.com/gthqxrqotc.html

Ruby: JSON.parse(s)
来源：http://hz.cucudq.cn/gtioepnnro.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.smart0.xyz/gtcyvkwhcx.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jinqigufen.top/gtfvjyysvs.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.cheryme.top/gtfllawizp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.chenlongwang.top/gtvmkiwdth.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.smart0.xyz/gtxmybvxek.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhongyouzk.top/gtdttwahkc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jqgufenzy.top/gthepxkzvk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhijiandao.cn/gtbuoihhbu.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ehwqpu.com/gtroszojwm.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.svipenyu.cn/gtygoetbuy.html

[K04] 读取 JSON 文件
来源：http://hz.sweek.top/gtddzqvafo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jinqigufen.top/gtljxqcdew.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.gogol.net.cn/gttajgbuun.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.aizwys.cn/gtloyzpiug.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.snrcjt.cn/gtcbvzcivc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yonumen.top/gtdrfdoywg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.0kj1m.cn/gtsxkvptza.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hnxiangtu.top/gthidqdayf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.fengsongda.top/gtzyospofa.html

[K05] 深拷贝对象
来源：http://hz.ydzc1.top/gtqvmbvxjv.html

Py:   copy.deepcopy(obj)
来源：http://hz.gotoacloud.top/gtoqjvmttj.html

PHP:  unserialize(serialize($obj));
来源：http://hz.aibaodan.cn/gtwfsjfybg.html

JS:   structuredClone(obj)
来源：http://hz.yangfankeji.com/gtzxppqdhf.html

TS:   structuredClone(obj)
来源：http://hz.cdnleiting.top/gtxresnfmz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.shangyingyoupin.top/gtvsjjksks.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ywan-chungtsiang.top/gtfycuhuhh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.mhx1999.top/gtxsfoqhde.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.wangshuangyany.cn/gtcmzgozex.html

[K06] 解析 URL 查询串
来源：http://hz.redwolf501.top/gtcqadqbue.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yueranfly.top/gtpaytqexd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.0kj1m.cn/gtjkjtbhzo.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jqgfzy.top/gtoyhrsyve.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tianlin.xyz/gtqanmbvui.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jyoumei.cn/gttehugyyf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.smart0.xyz/gtgmdvxnnu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.chenzaomai.com/gtrnbzesnd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cashguo.top/gtoeleagkf.html

[K07] 进制转换
来源：http://hz.daxiang520.top/gtlmuxfzdq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.wangdashe.top/gtboadktbr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.sufxvd.cn/gtofttpvpm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hnxiangtu.top/gtmogbnfcj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.gotoacloud.top/gtevtufvtn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhixingplan.top/gtvogsrxfl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.tanke756.top/gtxrqfetdn.html


<!-- 参考信息 -->