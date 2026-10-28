代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://hz.xziqi.cn/gtsckknuxc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.shzxlz.cn/gtdzrhmduy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.aizwys.cn/gtqjzsnkkw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.aibaodan.cn/gtqenypmyp.html

[H03] 主动抛出异常
来源：http://hz.daria6918.cn/gtbzbthfmh.html

Py:   raise ValueError("错误信息")
来源：http://hz.smart0.xyz/gtwhzocchw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jinqigufen.top/gthpwplaeu.html

JS:   throw new Error("错误信息");
来源：http://hz.hysaishi.cn/gtdppdmipm.html

TS:   throw new Error("错误信息");
来源：http://hz.jyoumei.cn/gtnfcufnbj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.fengsongda.top/gtzhjkbufr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jyoumei.cn/gtxvwuisvn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.smart0.xyz/gtlpbizjyi.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jqgufenzy.top/gtytlbgrpd.html

[H04] 自定义异常类型
来源：http://hz.yanxiufei.cn/gtbswokobv.html

Py:   class MyError(Exception): pass
来源：http://hz.yj20258888.top/gtkyzzlkzu.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.ehwqpu.com/gtgnmvpfwc.html

JS:   class MyError extends Error {}
来源：http://hz.pengpengdd.cyou/gtoiwwoboz.html

TS:   class MyError extends Error {}
来源：http://hz.hammf.cn/gtvdavqrvy.html

Java: class MyException extends RuntimeException {}
来源：http://hz.snrcjt.cn/gtpsdejnfb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jinghuilouyu.cn/gthhajtgvt.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhoulong.xyz/gtnpzemsdf.html

C#:   class MyException : Exception {}
来源：http://hz.wangshuangyany.cn/gthosbwtou.html

[H05] 捕获特定类型
来源：http://hz.gogol.net.cn/gtoyyffnov.html

Py:   except ValueError as e:
来源：http://hz.hfpthk.cn/gtkbfelktv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.fzhhl.top/gtfhlfixee.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.shuidangran.top/gtrdycvkzl.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hnqzz.top/gthcjixbyq.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhijiandao.cn/gtnzlmkmeq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.wangshuangyany.cn/gtpcydndna.html

Ruby: rescue ArgumentError => e
来源：http://hz.guannengcc.top/gtokwpzotj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.tanke756.top/gtwhjdotkb.html

[H06] 可选值 / 空值安全访问
来源：http://hz.cashguo.top/gtttzhqudt.html

Py:   value = d.get("k") or default
来源：http://hz.andypj.xyz/gtsprurhpr.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jinyuanbaomall.cn/gtpdvrqueh.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yueranfly.top/gtxtpicuin.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hywenlv.cn/gtdboccjoi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jinghuilouyu.cn/gtsynwkzyl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jianghu66.top/gtbqbjiouu.html

Ruby: d&.dig(:a, :b)
来源：http://hz.dashuyun.cn/gtczwueowi.html

C#:   obj?.A?.B ?? default
来源：http://hz.ppjwa.cn/gtnfiuknaf.html

[H07] 断言
来源：http://hz.havefunace.top/gtkdtsffjv.html

Py:   assert x > 0, "必须为正"
来源：http://hz.cqqwz.cn/gtuppsksoe.html

PHP:  assert($x > 0);
来源：http://hz.chenzaomai.com/gtovlbtrtz.html

JS:   console.assert(x > 0);
来源：http://hz.yanxiufei.cn/gtwpjfhqhx.html

TS:   console.assert(x > 0);
来源：http://hz.cashguo.top/gtpdpfajqk.html

Java: assert x > 0 : "必须为正";
来源：http://hz.c1oappe.top/gtwmtprixj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.pengpengdd.cyou/gttvnlwrdc.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jqgufenzy.top/gtjetahbnf.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jinqigufen.top/gthprxqnnc.html

[H08] 获取错误信息与堆栈
来源：http://hz.yueranfly.top/gtfumujeuj.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.wangshuangyany.cn/gtowuvktky.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yonumen.top/gtsagdownw.html

JS:   e.message;  e.stack
来源：http://hz.shanyushiyangtech.top/gtdmlgitkb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.iojbl.cn/gtqfcodkqu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.meibo888.top/gtyacticvs.html

Go:   err.Error()
来源：http://hz.chenjidiqi.icu/gtvzmhvcal.html

Ruby: e.message;  e.backtrace
来源：http://hz.xuetiantiany.cn/gtepkwucxn.html

C#:   e.Message;  e.StackTrace
来源：http://hz.dianchejie.cn/gtefkcjstm.html

[H09] 带错误码的异常
来源：http://hz.cheryme.top/gtcucvfmpk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yanxiufei.cn/gtwhrvornj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.chenlongwang.top/gtigaseycc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.sufxvd.cn/gtvpdqtqgi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.chenlongwang.top/gtryyaqtfp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.wangshuangyany.cn/gtavhveazy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.xuetiantiany.cn/gtoiriqzag.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.xingfuxueyuan.xyz/gttjjdekvv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhoulong.xyz/gtcohypbum.html

[H10] 资源自动释放
来源：http://hz.dashuyun.cn/gtjlentcwf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.guannengcc.top/gthdlxtcid.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ppjwa.cn/gtuwuvvejv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cheryme.top/gtqredmwur.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hnqzz.top/gtqrywwvik.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.0kj1m.cn/gtoecqtblq.html

Go:   defer f.Close()
来源：http://hz.shanyushiyangtech.top/gtmtyparey.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jiagoushi.top/gtyellwdgp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.0kj1m.cn/gtbbsbbyti.html

================================================================================
来源：http://hz.yonumen.top/gtfovffqmg.html

I. 正则表达式
来源：http://hz.snrcjt.cn/gtskcrhiox.html

================================================================================
来源：http://hz.snrcjt.cn/gtetlikmlt.html

[I01] 判断是否匹配
来源：http://hz.yj20258888.top/gtfpjscfev.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.daria6918.cn/gtpyoxozvw.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jiagoushi.top/gtqywcwkfc.html

JS:   /\d+/.test(s)
来源：http://hz.shanyushiyangkeji.top/gtyxzyyxgl.html

TS:   /\d+/.test(s)
来源：http://hz.pengpengdd.cyou/gtcunoetyp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.feifeiyinyue.top/gttsyfypex.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jyoumei.cn/gtrzysvulr.html

Ruby: s.match?(/\d+/)
来源：http://hz.aibaodan.cn/gtktgjkruu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.cqqwz.cn/gttixpjnap.html

[I02] 提取所有匹配
来源：http://hz.shzxlz.cn/gtajfgkyke.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ydjk.org.cn/gtwrwjbzaf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.feifeiyinyue.top/gtcpxdzdwn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hongshengwenyu.top/gtaoewhpek.html

TS:   s.match(/\d+/g)
来源：http://hz.yuxming.cn/gtqbmvvnhx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.fzhhl.top/gttybhakvr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.nanxinkj.top/gthrwnwnxn.html

Ruby: s.scan(/\d+/)
来源：http://hz.9152youxi.cn/gtelwdwvuc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.shanyushiyangtech.top/gtluvkddoo.html

[I03] 提取捕获分组
来源：http://hz.yueranfly.top/gtxjatjsvb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ywan-chungtsiang.top/gtktvgnhje.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.shangyingyoupin.top/gtutnkhbma.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.pengpengdd.cyou/gtcvcbowfb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.aizwys.cn/gtiqlhjwho.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.hongshengwenyu.top/gtfwpqocmm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.birdmap.top/gthruqjszd.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ehwqpu.com/gttdlljrwq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zycfv.cn/gtyfhczeho.html

[I04] 正则替换
来源：http://hz.0kj1m.cn/gtfjqicisq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.aizwys.cn/gtpcybmotf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.nwbrower.top/gtnrodrheh.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.cashguo.top/gtojlaarcz.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.nwbrower.top/gtiyplrksk.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jiagoushi.top/gtbxcrweaj.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jinyuanbaomall.cn/gtslxxtdby.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.fengsongda.top/gtgsmpedyi.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.gotoacloud.top/gtjbxgfggy.html

[I05] 按正则拆分
来源：http://hz.ivvv.top/gttrbvrycd.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ybcxt.top/gtcmaryaqp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hysaishi.cn/gtyhnztkzw.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yonumen.top/gtttejwdpg.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.wangdashe.top/gttpnxayfo.html

Java: s.split("\\s*,\\s*")
来源：http://hz.guannengcc.top/gtebdhlnko.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yueranfly.top/gtndufaovm.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.0kj1m.cn/gtmnrdrumm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.wangdashe.top/gtnkayfyax.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yangfankeji.com/gtaesrwkmj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.cqqwz.cn/gtejkbqzrs.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yonumen.top/gtobirtcca.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gogol.net.cn/gtlgzthaaz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sufxvd.cn/gtbsxhojhd.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.fengsongda.top/gttkalktbv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.fengsongda.top/gtirhaakpm.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.ydjk.org.cn/gtkglkemkl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.nanxinkj.top/gtlzdtirqg.html

[I07] 忽略大小写与多行模式
来源：http://hz.0kj1m.cn/gtllsavqlh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.pengpengdd.cyou/gtgxfemxdp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jqgufenzy.top/gtndwsmbtz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yj20258.top/gtbpsyzoaa.html

TS:   /error/gim
来源：http://hz.jinqigfzy.top/gtesojjlfw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.chenlongwang.top/gtjnhiwjmv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.tianlin.xyz/gtauidpixw.html

Ruby: s.scan(/error/i)
来源：http://hz.nwbrower.top/gtzorzstty.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jqgufenzy.top/gtjgjyfklh.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yongpay.top/gtebenzeho.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.fzhhl.top/gtsinimaou.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hongshengwenyu.top/gtxptvqkjz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.guowangkeji.top/gtmtngvgby.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cucudq.cn/gtgrvngmpt.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.xuetiantiany.cn/gtykjxuuby.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.wangdashe.top/gtvdvgrpdj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.meibo888.top/gteohyxunc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yongpay.top/gtbqdxerwa.html

================================================================================
来源：http://hz.ehwqpu.com/gtvhalnful.html

J. 日期与时间
来源：http://hz.zhoulong.xyz/gthbsumcmb.html

================================================================================
来源：http://hz.hnqzz.top/gtfsyzayoi.html

[J01] 获取当前时间
来源：http://hz.chenlongwang.top/gtzxthlwvo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.gogol.net.cn/gtgkesaodt.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yanxiufei.cn/gteauvbelv.html

JS:   new Date();  Date.now()
来源：http://hz.yj20258.top/gtnpqrquyy.html

TS:   new Date();  Date.now()
来源：http://hz.gzhubu.top/gtqjbdkyks.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.pycfn.com/gtsgdjynww.html

Go:   time.Now()
来源：http://hz.wangdashe.top/gtlubhlbvd.html

Ruby: Time.now
来源：http://hz.jiagoushi.top/gtbgrnjynh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hnxiangtu.top/gtnbmoamkt.html

[J02] 格式化输出
来源：http://hz.guowangkeji.top/gtxxorhdmt.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.redwolf501.top/gtdodltuwq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ivvv.top/gtrmqnjbwr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.sysykeji.top/gtkaubzusg.html

TS:   d.toISOString()
来源：http://hz.yangfankeji.com/gtofltmkqv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yongpay.top/gtqrulslsb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.52xcode.cn/gtvjsdomkb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cucudq.cn/gtvofjflbx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.xinyue.icu/gtdigmxmcm.html

[J03] 字符串解析为日期
来源：http://hz.daria6918.cn/gthcryuxdn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xingfuxueyuan.xyz/gthvdetrxm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.shangyingyoupin.top/gtyzulpybp.html

JS:   new Date("2024-01-02")
来源：http://hz.9152youxi.cn/gtnhececss.html

TS:   new Date("2024-01-02")
来源：http://hz.fengsongda.top/gtmbgikgby.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhaomingkeji.xyz/gtxyvigawj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.wangshuangyany.cn/gtlocuyopp.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zycfv.cn/gtfiginipo.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhiwuduotai.top/gtycggnvox.html

[J04] 时间戳与日期互转
来源：http://hz.jiagoushi.top/gtswjxszgk.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.ybcxt.top/gtlisaxomi.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.gotoacloud.top/gtixafhxtg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hfpthk.cn/gtainpshgo.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.andypj.xyz/gtceyzdzzy.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.bjfxy.top/gttuhpkxci.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yangfankeji.com/gtdjwhzoru.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.daxiang520.top/gtsrjyczcs.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ywan-chungtsiang.top/gtagndodrr.html

[J05] 时间加减（加 7 天）
来源：http://hz.meibo888.top/gtefnnumpk.html

Py:   now + timedelta(days=7)
来源：http://hz.aizwys.cn/gtntrsbbld.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hywenlv.cn/gtyuuejqga.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hywenlv.cn/gtqeyvnqkm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhijiandao.cn/gtuirwlkfw.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jinyuanbaomall.cn/gtnovdfjkg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yueranfly.top/gttdiiamxx.html

Ruby: Time.now + 7 * 86400
来源：http://hz.sweek.top/gtvtgtdofz.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xinyue.icu/gtzoczlagb.html

[J06] 计算两时间之差
来源：http://hz.xylfe.cn/gtowcdxyho.html

Py:   (end - start).total_seconds()
来源：http://hz.316326.xyz/gtakjfhhai.html

PHP:  $end->diff($start)->days;
来源：http://hz.tianlin.xyz/gthgsbrexz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.smart0.xyz/gtpoycuatl.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jinqigfzy.top/gtszrcnxjq.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jianghu66.top/gtfhmsbmwf.html

Go:   end.Sub(start).Hours()
来源：http://hz.zycfv.cn/gtctlmkkkr.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ppjwa.cn/gtspheubtl.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhixingplan.top/gtqvohtyyc.html

[J07] 比较两个日期
来源：http://hz.pycfn.com/gtbkpqnfwu.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ydzc1.top/gtkutisdvu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hysaishi.cn/gtvhcqaqxs.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zdqjudy.top/gtvwjmdbds.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jianghu66.top/gtimcyzybd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.chenzaomai.com/gtrvkybriy.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hysaishi.cn/gtldmvgwbk.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xinyue.icu/gtnalrpjrp.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhixingplan.top/gtgfakczap.html

[J08] 提取年月日与星期
来源：http://hz.hammf.cn/gtwnzryjjr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.52xcode.cn/gtkdfvwjrr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yanxiufei.cn/gtiwhemxvx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.sysykeji.top/gttfxjeylr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jqgufenzy.top/gtsmktbpkd.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yongpay.top/gthkykvagx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.meibo888.top/gtboxgirgi.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yangfankeji.com/gtrhdaapfh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.cdnleiting.top/gtsneqscmu.html

[J09] 时区处理
来源：http://hz.zhoulong.xyz/gtyvacsueh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.316326.xyz/gtktgopzrw.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.cqqwz.cn/gtugklrsdy.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yanxiufei.cn/gtoxpdvnrz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.bjfxy.top/gtfzwqjgaw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.nanxuanxn.top/gtwnlofiuw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhiwuduotai.top/gtiscjybkm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.tian-w.cn/gtwtbjbnhv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhoulong.xyz/gtrunvhbzy.html

[J10] 取今天 / 本月第一天
来源：http://hz.jyoumei.cn/gtpjcldtue.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.xingfuxueyuan.xyz/gtbibezflb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jqgfzy.top/gtmxofaect.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.smart0.xyz/gteljoqdmz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.9152youxi.cn/gtkjzutsbd.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yuxming.cn/gtznjlbyss.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ivvv.top/gtvgqptgzg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xuetiantiany.cn/gtcxsxscbf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.cqqwz.cn/gtfrzttmhq.html

================================================================================
来源：http://hz.birdmap.top/gtqndvbtkv.html

K. JSON 与序列化
来源：http://hz.ydjk.org.cn/gtsgbxdrbu.html

================================================================================
来源：http://hz.guowangkeji.top/gtspwzhjsb.html

[K01] 对象转 JSON 字符串
来源：http://hz.jinghuilouyu.cn/gtsdapwpuw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zycfv.cn/gtzbbojudj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.bjfxy.top/gtrtdtbuhq.html

JS:   JSON.stringify(obj)
来源：http://hz.9152youxi.cn/gtkdcgabfy.html

TS:   JSON.stringify(obj)
来源：http://hz.tianlin.xyz/gtkykimwpe.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yueranfly.top/gtpmqbkrmg.html

Go:   json.Marshal(obj)
来源：http://hz.jinqigfzy.top/gttvsmmkiz.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.xingfuxueyuan.xyz/gtyblpejnq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.feifeiyinyue.top/gtojweavsn.html

[K02] JSON 字符串转对象
来源：http://hz.birdmap.top/gtjgbydupp.html

Py:   json.loads(s)
来源：http://hz.jinqigfzy.top/gtmssrviae.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.snrcjt.cn/gtscoimhym.html

JS:   JSON.parse(s)
来源：http://hz.yanxiufei.cn/gttsorucfi.html

TS:   JSON.parse(s)
来源：http://hz.yonumen.top/gtrailntir.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.chenjidiqi.icu/gtcmnhoymy.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhaomingkeji.xyz/gtlcjvwxza.html

Ruby: JSON.parse(s)
来源：http://hz.chenjidiqi.icu/gtuoqnfmvp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhaomingkeji.xyz/gtegjguuty.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yvedp.cn/gtabdeiogf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.smart0.xyz/gtzlaukeft.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yj20258888.top/gtawjyqnfp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.sweek.top/gttecpqopi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.9152youxi.cn/gtflneceox.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.nwbrower.top/gtzszrhqbv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jinghuilouyu.cn/gtlgjvbbef.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.9152youxi.cn/gteprhcvub.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yanxiufei.cn/gtltwqvoll.html

[K04] 读取 JSON 文件
来源：http://hz.ywan-chungtsiang.top/gttlsqnxzn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hywenlv.cn/gtzxlxaqjy.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.nanxuanxn.top/gtcfzsabed.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.andypj.xyz/gtqopxrjfk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.havefunace.top/gtwuskuwel.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ybcxt.top/gtoqivrfcu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhaomingkeji.xyz/gtjtznilse.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.wangshuangyany.cn/gtxdzmsvlc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jyoumei.cn/gtibdgdowv.html

[K05] 深拷贝对象
来源：http://hz.shangyingyoupin.top/gtemejtvxv.html

Py:   copy.deepcopy(obj)
来源：http://hz.fengsongda.top/gtyeootvrx.html

PHP:  unserialize(serialize($obj));
来源：http://hz.quarkkingdee.top/gtbouoikqo.html

JS:   structuredClone(obj)
来源：http://hz.yj20258.top/gtvpbubfdf.html

TS:   structuredClone(obj)
来源：http://hz.ydzc1.top/gtgewcyjgs.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ydjk.org.cn/gtsjkpflzd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.havefunace.top/gtqirzmyif.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.gogol.net.cn/gttwdnootg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.kuanghao11.cn/gtggrtehjj.html

[K06] 解析 URL 查询串
来源：http://hz.jinyuanbaomall.cn/gtejudvnec.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.tianlin.xyz/gtetorzjtp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.nwbrower.top/gttfzffbnx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jiagoushi.top/gtoipgywvz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hnxiangtu.top/gteppsszfg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.52xcode.cn/gtjxtfqryn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.tianlin.xyz/gtskfnwfco.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yj20258.top/gtntycpjkl.html


<!-- 参考信息 -->