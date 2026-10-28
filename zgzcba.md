代发 wailian999

JS:   class MyError extends Error {}
来源：http://hz.ydjk.org.cn/gtekvatdsi.html

TS:   class MyError extends Error {}
来源：http://hz.daxiang520.top/gtqdkjjcnb.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yj20258.top/gtbywwwivt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.smart0.xyz/gtzycwhjyt.html

Ruby: class MyError < StandardError; end
来源：http://hz.snrcjt.cn/gtfrstwznd.html

C#:   class MyException : Exception {}
来源：http://hz.feifeiyinyue.top/gtrnpaxzdk.html

[H05] 捕获特定类型
来源：http://hz.jqgfzy.top/gtaztmqroo.html

Py:   except ValueError as e:
来源：http://hz.dashuyun.cn/gtqwbjyuyc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yj20258888.top/gtolfhlzsd.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.havefunace.top/gtgpkghelm.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yj20258888.top/gtpubgdcsh.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.pycfn.com/gtmdhrjlzu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.nanxinkj.top/gtceqidmul.html

Ruby: rescue ArgumentError => e
来源：http://hz.ywan-chungtsiang.top/gtljjymror.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ivvv.top/gtnlvbrhyl.html

[H06] 可选值 / 空值安全访问
来源：http://hz.daria6918.cn/gtqcjjpfju.html

Py:   value = d.get("k") or default
来源：http://hz.jiagoushi.top/gtbcjoxtfe.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.nwbrower.top/gtqbxhgjcg.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yj20258888.top/gthhxupzuk.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.tian-w.cn/gtchrhgvua.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhaomingkeji.xyz/gtqkjtifkv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.birdmap.top/gtzqsxdyag.html

Ruby: d&.dig(:a, :b)
来源：http://hz.daxiang520.top/gtuxtjoaoc.html

C#:   obj?.A?.B ?? default
来源：http://hz.hywenlv.cn/gtxkeramxq.html

[H07] 断言
来源：http://hz.daxiang520.top/gtrhcoyiye.html

Py:   assert x > 0, "必须为正"
来源：http://hz.tianlin.xyz/gtasdfeowk.html

PHP:  assert($x > 0);
来源：http://hz.zhengqikj.top/gtosrjgsgd.html

JS:   console.assert(x > 0);
来源：http://hz.hysaishi.cn/gtprwlpizr.html

TS:   console.assert(x > 0);
来源：http://hz.xziqi.cn/gtcyealpic.html

Java: assert x > 0 : "必须为正";
来源：http://hz.nanxinkj.top/gtxrkojzmr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.shzxlz.cn/gtnnzxfxrd.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhixingplan.top/gtowqjdjld.html

C#:   Debug.Assert(x > 0);
来源：http://hz.xingfuxueyuan.xyz/gtgojqlnru.html

[H08] 获取错误信息与堆栈
来源：http://hz.yangfankeji.com/gtcpkcmstj.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.havefunace.top/gtjinwehit.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.fengsongda.top/gtldzgnomp.html

JS:   e.message;  e.stack
来源：http://hz.guowangkeji.top/gtcpajzwnx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.0kj1m.cn/gtdxsrbufo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.svipenyu.cn/gtbpzgqbpc.html

Go:   err.Error()
来源：http://hz.haohaochexian.top/gttdzusrim.html

Ruby: e.message;  e.backtrace
来源：http://hz.tianlin.xyz/gtpkyjjgcn.html

C#:   e.Message;  e.StackTrace
来源：http://hz.birdmap.top/gtqcxhpqzy.html

[H09] 带错误码的异常
来源：http://hz.yonumen.top/gtdqzowiwe.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yueranfly.top/gtxunecmgw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hnqzz.top/gtcoveuasj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.dashuyun.cn/gtlsfpvbrp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.guannengcc.top/gtxfnahjlj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.aizwys.cn/gtzwdblbye.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.mhx1999.top/gthbtqejrf.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.52xcode.cn/gtysmnwuhz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jinghuilouyu.cn/gtzvscxwii.html

[H10] 资源自动释放
来源：http://hz.yvedp.cn/gtuaicjvpo.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.dashuyun.cn/gtodcjatup.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xingfuxueyuan.xyz/gtilesfuvs.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yueranfly.top/gtibltsuiy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.52xcode.cn/gtlrwtnupm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.nwbrower.top/gteqotkije.html

Go:   defer f.Close()
来源：http://hz.cucudq.cn/gtstrrnsks.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yueranfly.top/gtxrlxvrlq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xylfe.cn/gtamkcmhfx.html

================================================================================
来源：http://hz.haohaochexian.top/gtbfmcrvmm.html

I. 正则表达式
来源：http://hz.smart0.xyz/gtqmwdbxhc.html

================================================================================
来源：http://hz.gaohongyu789.top/gtltpyqvqv.html

[I01] 判断是否匹配
来源：http://hz.jinqigfzy.top/gtztkikmuc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jiagoushi.top/gthcpaaqoz.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jiagoushi.top/gtdnmaffty.html

JS:   /\d+/.test(s)
来源：http://hz.smart0.xyz/gtasonyfaa.html

TS:   /\d+/.test(s)
来源：http://hz.cheryme.top/gtfwbpugom.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.havefunace.top/gtvixnnwph.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yanxiufei.cn/gtlvqnqucr.html

Ruby: s.match?(/\d+/)
来源：http://hz.chenlongwang.top/gtqxjrbuuh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.chenjidiqi.icu/gtfujqinyf.html

[I02] 提取所有匹配
来源：http://hz.gogol.net.cn/gtfkjtutmv.html

Py:   re.findall(r"\d+", s)
来源：http://hz.guowangkeji.top/gtzhokimox.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.meibo888.top/gtmywtytqc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xuanzx.com/gtictvchdf.html

TS:   s.match(/\d+/g)
来源：http://hz.cashguo.top/gtewqvbrvq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ivvv.top/gtxqjbyqnr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jinghuilouyu.cn/gtatshubqz.html

Ruby: s.scan(/\d+/)
来源：http://hz.jinyuanbaomall.cn/gtrcoznaog.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ydzc1.top/gtgsjfqqwz.html

[I03] 提取捕获分组
来源：http://hz.ehwqpu.com/gtcdvvadvt.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.svipenyu.cn/gttumykpzf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yvedp.cn/gtsbneolel.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.vqdsnc.cn/gtlmlakkig.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yj20258888.top/gtebbwciqi.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.fengsongda.top/gtkqjsrjky.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhaomingkeji.xyz/gtollehkvp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.birdmap.top/gtqveliter.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.meibo888.top/gtuxmrmcid.html

[I04] 正则替换
来源：http://hz.gogol.net.cn/gtocdbtjsp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jianghu66.top/gtsjtgbypq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yj20258888.top/gtopghmvmo.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hammf.cn/gtpapzzrov.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.316326.xyz/gtatmaakfj.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.feifeiyinyue.top/gtvrjvkqyn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.guannengcc.top/gtokqgtzki.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.nanxuanxn.top/gtzxfhkxve.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.fengsongda.top/gtjkfxrqji.html

[I05] 按正则拆分
来源：http://hz.daria6918.cn/gtsvyawqxe.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.tianlin.xyz/gtzvbrwluk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ybcxt.top/gtcpxnzvro.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.mhx1999.top/gtdeajtpbz.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhoulong.xyz/gtivubjaxj.html

Java: s.split("\\s*,\\s*")
来源：http://hz.cdnleiting.top/gtjpdvvzfy.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ywan-chungtsiang.top/gtffblvvdh.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xylfe.cn/gtotbqdkhr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yj20258.top/gtbyyazwwx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhaomingkeji.xyz/gtrqfenbxa.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.redwolf501.top/gtcjqkiokf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.meibo888.top/gtmuwmwbre.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ywan-chungtsiang.top/gthjgohepz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hfpthk.cn/gtnjwmmqlk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.daxiang520.top/gtcmbxxfhx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ydzc1.top/gtsvxjclqk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.ywan-chungtsiang.top/gtamnhdjqm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.daria6918.cn/gtljpyucba.html

[I07] 忽略大小写与多行模式
来源：http://hz.ywan-chungtsiang.top/gthgkbpfws.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.shanyushiyangkeji.top/gtdgspkocj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ivvv.top/gtlxfcrczh.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.316326.xyz/gtwheluqts.html

TS:   /error/gim
来源：http://hz.shzxlz.cn/gtymkqmaxt.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jiagoushi.top/gtaisgekob.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.nanxuanxn.top/gtkurozzkc.html

Ruby: s.scan(/error/i)
来源：http://hz.dianchejie.cn/gtwgpfdaxs.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.havefunace.top/gtgrtceklm.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.sweek.top/gthbmxkmtw.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.tian-w.cn/gtrozknans.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ppjwa.cn/gtgjzxsmjz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hnqzz.top/gttordbxur.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.kuanghao11.cn/gtkqvoyjex.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jinqigufen.top/gtaewjxdcm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xziqi.cn/gtnfkflrey.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.snrcjt.cn/gtnbzjkzgc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.sxryk.cn/gtqyjurohk.html

================================================================================
来源：http://hz.yvedp.cn/gtogfnypze.html

J. 日期与时间
来源：http://hz.dashuyun.cn/gtycjcnbml.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtowmzhwtr.html

[J01] 获取当前时间
来源：http://hz.sweek.top/gtbucgbcxy.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.vqdsnc.cn/gttapllmel.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.hnqzz.top/gtvmxffjba.html

JS:   new Date();  Date.now()
来源：http://hz.ydjk.org.cn/gtfuzxfgev.html

TS:   new Date();  Date.now()
来源：http://hz.guannengcc.top/gttyawvtkb.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.chenzaomai.com/gtyailfyda.html

Go:   time.Now()
来源：http://hz.chenzaomai.com/gtrfoqqpae.html

Ruby: Time.now
来源：http://hz.cdnleiting.top/gtwdraqzfc.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hysaishi.cn/gtsubqpbpt.html

[J02] 格式化输出
来源：http://hz.c1oappe.top/gtxquihrpx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zycfv.cn/gtrsohfxyn.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.xingfuxueyuan.xyz/gtootiniga.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.gogol.net.cn/gtzcwqwbrq.html

TS:   d.toISOString()
来源：http://hz.snrcjt.cn/gtrwxsztdi.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.ydzc1.top/gtxcaospat.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jinqigufen.top/gtklybrbzb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinyuanbaomall.cn/gtwkgdlqtt.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.sweek.top/gtuorfpxzl.html

[J03] 字符串解析为日期
来源：http://hz.jinyuanbaomall.cn/gtrhjqzytp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hysaishi.cn/gtmxxcbjzi.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.sufxvd.cn/gttgwlrgib.html

JS:   new Date("2024-01-02")
来源：http://hz.ywan-chungtsiang.top/gtwgywjzig.html

TS:   new Date("2024-01-02")
来源：http://hz.ydjk.org.cn/gtsaiztluo.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hfpthk.cn/gtdbqxrole.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yj20258888.top/gtykbcxudo.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.sweek.top/gtyksxtrlt.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.52xcode.cn/gtoqngyysb.html

[J04] 时间戳与日期互转
来源：http://hz.xziqi.cn/gtelvibztb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hnxiangtu.top/gtmjxbkslh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.pengpengdd.cyou/gtwzptdzab.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.sweek.top/gtjoaloyfk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.mhx1999.top/gttqejbhiu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ybcxt.top/gtubiylqej.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yongpay.top/gtwwsmages.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.cdnleiting.top/gtqjazxyiq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.wangshuangyany.cn/gtxafxpfml.html

[J05] 时间加减（加 7 天）
来源：http://hz.vqdsnc.cn/gtialowhtj.html

Py:   now + timedelta(days=7)
来源：http://hz.daria6918.cn/gthqclrodo.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.sufxvd.cn/gtnfnrbkra.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.feifeiyinyue.top/gtfbdzkklj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jyoumei.cn/gtidkyyffw.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hywenlv.cn/gtdjhmvuip.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yvedp.cn/gtkthzdnmj.html

Ruby: Time.now + 7 * 86400
来源：http://hz.chenjidiqi.icu/gtrjnsvear.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yangfankeji.com/gtihmrdnnl.html

[J06] 计算两时间之差
来源：http://hz.ydzc1.top/gthfszvedm.html

Py:   (end - start).total_seconds()
来源：http://hz.316326.xyz/gtagyjakks.html

PHP:  $end->diff($start)->days;
来源：http://hz.jlsjyb.cn/gtwdmmbtge.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.kuanghao11.cn/gtaxmjyvqb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yj20258.top/gtwgrryhym.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.svipenyu.cn/gtixkluctj.html

Go:   end.Sub(start).Hours()
来源：http://hz.cashguo.top/gtvhwytubp.html

Ruby: end - start                 # 返回秒数
来源：http://hz.andypj.xyz/gtpydkuyvs.html

C#:   (end - start).TotalSeconds
来源：http://hz.hfpthk.cn/gtvfohobdm.html

[J07] 比较两个日期
来源：http://hz.zhengqikj.top/gtvmrcccal.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.birdmap.top/gteecsezrx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yongpay.top/gtxuydanmw.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jinghuilouyu.cn/gtomvhozas.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yueranfly.top/gtnkvrtqfl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cashguo.top/gthuwchpfc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.fengsongda.top/gtaykwhthj.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.quarkkingdee.top/gtawvgnkuq.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yueranfly.top/gtbokfnfvb.html

[J08] 提取年月日与星期
来源：http://hz.jinqigufen.top/gtmlxptkod.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.daria6918.cn/gtxnnowsbs.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yj20258.top/gtbrjfripp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.ppjwa.cn/gtrykougxa.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.gotoacloud.top/gtwhiiyshl.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.chenlongwang.top/gtfxulazyc.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.gzhubu.top/gtbzkskqeo.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.bjfxy.top/gtmzdayphi.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.chenzaomai.com/gtiivopnqw.html

[J09] 时区处理
来源：http://hz.xziqi.cn/gtnxovrhai.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jinghuilouyu.cn/gtyqkdcoug.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ppjwa.cn/gttpmuteqr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hongshengwenyu.top/gtjueujxjq.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.wangshuangyany.cn/gtogbzqzko.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.9152youxi.cn/gtgeuwoxsw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jinghuilouyu.cn/gtpesblnxy.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yonumen.top/gtkltxgyhd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yuanzhike.top/gtudhbvdqn.html

[J10] 取今天 / 本月第一天
来源：http://hz.birdmap.top/gtfvqdxlmm.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.fengsongda.top/gtjwdaywgq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jiagoushi.top/gtkeublkjw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.cashguo.top/gtvpacveio.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yueranfly.top/gtinfziczc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.hfpthk.cn/gtyffmlqxm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.aibaodan.cn/gtuoqzotsl.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yj20258.top/gtyekeiukb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jyoumei.cn/gtlzvdozle.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtjheyaxjo.html

K. JSON 与序列化
来源：http://hz.yj202588.top/gtewewlnpy.html

================================================================================
来源：http://hz.hnqzz.top/gtfznwotrw.html

[K01] 对象转 JSON 字符串
来源：http://hz.smart0.xyz/gtdqstogmb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.dianchejie.cn/gttfdvlqvt.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yanxiufei.cn/gtbqqkpvyx.html

JS:   JSON.stringify(obj)
来源：http://hz.cashguo.top/gtydynrleb.html

TS:   JSON.stringify(obj)
来源：http://hz.xylfe.cn/gtsjmkbvco.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.9152youxi.cn/gtoprdohyj.html

Go:   json.Marshal(obj)
来源：http://hz.yonumen.top/gtyaqcyzgh.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.iojbl.cn/gtgdykojya.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.daxiang520.top/gthjeiejks.html

[K02] JSON 字符串转对象
来源：http://hz.fzhhl.top/gtcwoklpbp.html

Py:   json.loads(s)
来源：http://hz.tian-w.cn/gtunxbjzkf.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.svipenyu.cn/gthtxfiqce.html

JS:   JSON.parse(s)
来源：http://hz.wangshuangyany.cn/gtpyrfgqaj.html

TS:   JSON.parse(s)
来源：http://hz.jlsjyb.cn/gtpwatamhe.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.bjfxy.top/gtyojawilx.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.haohaochexian.top/gthtxmzqjs.html

Ruby: JSON.parse(s)
来源：http://hz.jqgufenzy.top/gthvboysgv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.tianlin.xyz/gtmhxaotkk.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yangfankeji.com/gtrkazwwkm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.sysykeji.top/gtufszgahn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yj202588.top/gtjjnjevyy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ivvv.top/gtrbycdowr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.kuanghao11.cn/gthcwfoatc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.haohaochexian.top/gtopghjwby.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jinqigfzy.top/gtznjotcxb.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.redwolf501.top/gtnkclawmx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ivvv.top/gtpwigbkqj.html

[K04] 读取 JSON 文件
来源：http://hz.zhijiandao.cn/gtnvtkxlyd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zdqjudy.top/gtgzuaitpr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.hnxiangtu.top/gtretnofkd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.chenjidiqi.icu/gtwwosvgwn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shuidangran.top/gtvwoxqivl.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yonumen.top/gtacgqdcle.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jqgufenzy.top/gttnjxdcyq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jinghuilouyu.cn/gtaobtmgcl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.sysykeji.top/gtzykhgdtb.html

[K05] 深拷贝对象
来源：http://hz.ehwqpu.com/gtxfwtcgpd.html

Py:   copy.deepcopy(obj)
来源：http://hz.yuxming.cn/gteuvppqfs.html

PHP:  unserialize(serialize($obj));
来源：http://hz.sxryk.cn/gtqjphwsvn.html

JS:   structuredClone(obj)
来源：http://hz.cucudq.cn/gtfpgeeuhd.html

TS:   structuredClone(obj)
来源：http://hz.yvedp.cn/gtcpccjonc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jinghuilouyu.cn/gttityfqnv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jqgfzy.top/gtltiyzwtn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jqgufenzy.top/gtlxptofjo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yvedp.cn/gtekztnfes.html

[K06] 解析 URL 查询串
来源：http://hz.kuanghao11.cn/gtjarhyxif.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jqgufenzy.top/gtfuyswemx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.tanke756.top/gtnochgzuk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.feifeiyinyue.top/gtvxyzzfan.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinghuilouyu.cn/gtuskpqhxw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yonumen.top/gtfnkeclsn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.snrcjt.cn/gtnhgyjmhj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jyoumei.cn/gtpamuimvx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.xinyue.icu/gtybtcvagm.html

[K07] 进制转换
来源：http://hz.cdnleiting.top/gtbqtckcay.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.xinyue.icu/gtneaohvij.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jinyuanbaomall.cn/gtscgtgkto.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jqgfzy.top/gtgkuvgohs.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.andypj.xyz/gtbfebjoek.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hnqzz.top/gtqxpzylyi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.meibo888.top/gtrftqijgp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.hammf.cn/gthystxycp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.316326.xyz/gtfvasnkfs.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.hywenlv.cn/gtxgwvsjzv.html

Py:   pickle.dumps(obj)
来源：http://hz.9152youxi.cn/gtxpdmcjcu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.redwolf501.top/gtddttnavg.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hywenlv.cn/gtoxwfbomk.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.gaohongyu789.top/gtebmlzdog.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hysaishi.cn/gtvshnyldv.html


<!-- 参考信息 -->