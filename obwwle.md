代发 wailian999

TS:   throw new Error("错误信息");
来源：http://hz.zycfv.cn/gtlvegonwj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cucudq.cn/gtqpoqqiii.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hysaishi.cn/gtafnmyyud.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhaomingkeji.xyz/gtcgsglcap.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.pycfn.com/gtsjisxoyd.html

[H04] 自定义异常类型
来源：http://hz.andypj.xyz/gtweojbcgk.html

Py:   class MyError(Exception): pass
来源：http://hz.feifeiyinyue.top/gtsaatmyzv.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yvedp.cn/gtmapcjria.html

JS:   class MyError extends Error {}
来源：http://hz.wangshuangyany.cn/gtnuopwpfl.html

TS:   class MyError extends Error {}
来源：http://hz.jinyuanbaomall.cn/gtfoxojkrn.html

Java: class MyException extends RuntimeException {}
来源：http://hz.aizwys.cn/gtxsvafhrh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.nanxinkj.top/gtwjtmagba.html

Ruby: class MyError < StandardError; end
来源：http://hz.jlsjyb.cn/gtucpdjhgw.html

C#:   class MyException : Exception {}
来源：http://hz.jlsjyb.cn/gtgactiflb.html

[H05] 捕获特定类型
来源：http://hz.gzhubu.top/gtpjulgstb.html

Py:   except ValueError as e:
来源：http://hz.yj20258888.top/gtebxwfjyd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yueranfly.top/gtktymywgi.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.cheryme.top/gtjphezgxi.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yangfankeji.com/gthxrhsgtc.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.gzhubu.top/gtkiaspomt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.nanxuanxn.top/gtficdrbrk.html

Ruby: rescue ArgumentError => e
来源：http://hz.havefunace.top/gtzmloqyaz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ivvv.top/gtjvopcuor.html

[H06] 可选值 / 空值安全访问
来源：http://hz.dianchejie.cn/gtcixalslo.html

Py:   value = d.get("k") or default
来源：http://hz.nwbrower.top/gtmclkmflx.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hysaishi.cn/gtwuzzoyac.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.svipenyu.cn/gtskgdwnlt.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.haohaochexian.top/gthjkcfpak.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.xylfe.cn/gtopdpuwqm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.daria6918.cn/gtkzjnlxcg.html

Ruby: d&.dig(:a, :b)
来源：http://hz.svipenyu.cn/gttvmbkitm.html

C#:   obj?.A?.B ?? default
来源：http://hz.snrcjt.cn/gtalehrbea.html

[H07] 断言
来源：http://hz.hywenlv.cn/gtrqogznln.html

Py:   assert x > 0, "必须为正"
来源：http://hz.snrcjt.cn/gtmnfanzet.html

PHP:  assert($x > 0);
来源：http://hz.ybcxt.top/gthtkfdkye.html

JS:   console.assert(x > 0);
来源：http://hz.zhoulong.xyz/gtwylpmyuz.html

TS:   console.assert(x > 0);
来源：http://hz.zhongyouzk.top/gtymgogdgf.html

Java: assert x > 0 : "必须为正";
来源：http://hz.sxryk.cn/gteuzrrgel.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.gotoacloud.top/gtdnblhwke.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.chenlongwang.top/gtwjogcsxf.html

C#:   Debug.Assert(x > 0);
来源：http://hz.hnqzz.top/gtvbxqzqzw.html

[H08] 获取错误信息与堆栈
来源：http://hz.jianghu66.top/gtsaeyhapu.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.316326.xyz/gtfhwwzrlk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ydzc1.top/gtpkjoxuog.html

JS:   e.message;  e.stack
来源：http://hz.hysaishi.cn/gttvhcitdv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yuxming.cn/gtgeppqlfq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.guannengcc.top/gtnbihnzfc.html

Go:   err.Error()
来源：http://hz.shanyushiyangtech.top/gterzgvmjf.html

Ruby: e.message;  e.backtrace
来源：http://hz.xuetiantiany.cn/gteokbrvvs.html

C#:   e.Message;  e.StackTrace
来源：http://hz.quarkkingdee.top/gtvaphygmu.html

[H09] 带错误码的异常
来源：http://hz.andypj.xyz/gtnhhmtpma.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.haohaochexian.top/gtapoaveiz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yongpay.top/gtzvaakeyi.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jqgufenzy.top/gtffvtxpie.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.daria6918.cn/gtxvkwuapt.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ybcxt.top/gtgynvehub.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hongshengwenyu.top/gtxlrnlxpr.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.gotoacloud.top/gtpjxvlvmm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.xziqi.cn/gthfnkedrc.html

[H10] 资源自动释放
来源：http://hz.wangdashe.top/gtsqrydmcn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ivvv.top/gtaewrmwlc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xinyue.icu/gtwbeiyhrq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yonumen.top/gtsomgtjnq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cashguo.top/gtjsnkvyjg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.havefunace.top/gtpcjbukkk.html

Go:   defer f.Close()
来源：http://hz.zhoulong.xyz/gtalhzthpj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.andypj.xyz/gtffjchwee.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xylfe.cn/gtrhfnbmys.html

================================================================================
来源：http://hz.yj202588.top/gtzdutzoji.html

I. 正则表达式
来源：http://hz.tianlin.xyz/gtnyridojl.html

================================================================================
来源：http://hz.wangdashe.top/gtoppkdnyx.html

[I01] 判断是否匹配
来源：http://hz.shzxlz.cn/gtgrlaxcqr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.daria6918.cn/gtodrgujot.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.chenzaomai.com/gttocnodgx.html

JS:   /\d+/.test(s)
来源：http://hz.mhx1999.top/gtapbrpxog.html

TS:   /\d+/.test(s)
来源：http://hz.shuidangran.top/gtybsixjgx.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jqgufenzy.top/gtesyrrpih.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.9152youxi.cn/gtqmaopsfk.html

Ruby: s.match?(/\d+/)
来源：http://hz.hongshengwenyu.top/gtrxtibgit.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jqgufenzy.top/gtgvskzlld.html

[I02] 提取所有匹配
来源：http://hz.xuetiantiany.cn/gtvvufnrvo.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yvedp.cn/gtppdyhepe.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.dianchejie.cn/gtprxgmobe.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.iojbl.cn/gtxryddmmg.html

TS:   s.match(/\d+/g)
来源：http://hz.tian-w.cn/gtraazunkk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.nanxinkj.top/gtsojwdpqe.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.cdnleiting.top/gtkyxltvxm.html

Ruby: s.scan(/\d+/)
来源：http://hz.haohaochexian.top/gtnebwjelj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jinqigufen.top/gtoiivdnlm.html

[I03] 提取捕获分组
来源：http://hz.cucudq.cn/gtmhflvznc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.gzhubu.top/gtegavxxsw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.chenjidiqi.icu/gtitxkqeyq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.smart0.xyz/gtmzjtpome.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yj20258.top/gttsbesnia.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.hongshengwenyu.top/gtipijzasu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jyoumei.cn/gtvbfoopjd.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhoulong.xyz/gteorlwrms.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.xinyue.icu/gtjkfpaiex.html

[I04] 正则替换
来源：http://hz.meibo888.top/gtkavjprrj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.shangyingyoupin.top/gtzgccriqr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.smart0.xyz/gtntvuciyk.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.meibo888.top/gthjyphtur.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.ydjk.org.cn/gtvghdueya.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.pycfn.com/gtkwetceum.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yj20258.top/gtcsylmqvf.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.shanyushiyangtech.top/gtxpanqbni.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.daxiang520.top/gtwflcssya.html

[I05] 按正则拆分
来源：http://hz.pycfn.com/gtvsqknmiz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zhengqikj.top/gtadbqfoxc.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.cashguo.top/gtkrcuqrdk.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.gaohongyu789.top/gtcvtfgldx.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.chenzaomai.com/gtdckwmhdz.html

Java: s.split("\\s*,\\s*")
来源：http://hz.birdmap.top/gtmnswkqhz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.feifeiyinyue.top/gtvswutlqd.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.pycfn.com/gtrwqqhntq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.gotoacloud.top/gtgsfgnycp.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.redwolf501.top/gtczgnooli.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.nanxuanxn.top/gtsuyvvxeh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.iojbl.cn/gtsrcfusuq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhijiandao.cn/gtgfiddsks.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.kuanghao11.cn/gtsdodchyj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jyoumei.cn/gtmeftaeef.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jqgfzy.top/gtzgqnjbue.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.guannengcc.top/gtbuqcfwcm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.gotoacloud.top/gtsehbqedt.html

[I07] 忽略大小写与多行模式
来源：http://hz.jqgufenzy.top/gtwoyoilvo.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.cucudq.cn/gtrdlqqrim.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hammf.cn/gtafwadfpp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhijiandao.cn/gtgjrnkhpp.html

TS:   /error/gim
来源：http://hz.tianlin.xyz/gtjvgykfna.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.xingfuxueyuan.xyz/gtzckhschx.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.aizwys.cn/gtmhqugytf.html

Ruby: s.scan(/error/i)
来源：http://hz.dashuyun.cn/gtdoyuggub.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.cqqwz.cn/gtxaiwlqal.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.fengsongda.top/gtfottjsdd.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jyoumei.cn/gtineyrqcf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.gzhubu.top/gtdrdmfezy.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.daxiang520.top/gtbyupafib.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sysykeji.top/gtmgelqcky.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.cheryme.top/gtqumdppwi.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.dianchejie.cn/gttvsjhnvq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ydzc1.top/gtjooaoqls.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.shangyingyoupin.top/gtmqlktejk.html

================================================================================
来源：http://hz.ydjk.org.cn/gtehhtdrre.html

J. 日期与时间
来源：http://hz.guowangkeji.top/gtrtrfltiw.html

================================================================================
来源：http://hz.jianghu66.top/gthunpsdqd.html

[J01] 获取当前时间
来源：http://hz.yj202588.top/gtyxmxnnam.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yj20258.top/gtduazvwsr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.svipenyu.cn/gtslvqtxot.html

JS:   new Date();  Date.now()
来源：http://hz.chenzaomai.com/gtbihodzfv.html

TS:   new Date();  Date.now()
来源：http://hz.ppjwa.cn/gtevuesiby.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shuidangran.top/gtoowqetfy.html

Go:   time.Now()
来源：http://hz.meibo888.top/gtgjzfitxu.html

Ruby: Time.now
来源：http://hz.smart0.xyz/gtpsefueiv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.0kj1m.cn/gtxewsfdje.html

[J02] 格式化输出
来源：http://hz.zhixingplan.top/gtpebwlasv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jqgfzy.top/gtdnqcerlw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.guannengcc.top/gtxiearclt.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.dianchejie.cn/gtxkjqzcic.html

TS:   d.toISOString()
来源：http://hz.bjfxy.top/gtuawhpmbt.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xingfuxueyuan.xyz/gtrvpftgij.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.316326.xyz/gtavhphsuv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cucudq.cn/gtwtcpjuao.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.aibaodan.cn/gtvhhiyzdx.html

[J03] 字符串解析为日期
来源：http://hz.mhx1999.top/gtewsjrpts.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.chenlongwang.top/gtfyadljlk.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.guannengcc.top/gtbaafritz.html

JS:   new Date("2024-01-02")
来源：http://hz.fzhhl.top/gtkdbtriby.html

TS:   new Date("2024-01-02")
来源：http://hz.nanxuanxn.top/gtdkhfgcsq.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jinqigufen.top/gtrvhfreev.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.nanxinkj.top/gtqfowustt.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yongpay.top/gtzcoupznb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.vqdsnc.cn/gtndhjebqj.html

[J04] 时间戳与日期互转
来源：http://hz.hysaishi.cn/gtojagdisn.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hammf.cn/gtkdrjehql.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.cashguo.top/gtndpygqkg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.guannengcc.top/gtohygawjo.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.tianlin.xyz/gtkrvgqbyz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhaomingkeji.xyz/gtyzueqgsp.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.tian-w.cn/gtyqowbnmt.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xziqi.cn/gthvxiczey.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.kuanghao11.cn/gtbvoeawab.html

[J05] 时间加减（加 7 天）
来源：http://hz.fengsongda.top/gtiltjkxwo.html

Py:   now + timedelta(days=7)
来源：http://hz.hnqzz.top/gtsadkkvbc.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.cqqwz.cn/gtzvovzzty.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yonumen.top/gtizxrrkto.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.daria6918.cn/gtxvtdyowc.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hongshengwenyu.top/gtxonaqmsq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhengqikj.top/gtngzlvsjv.html

Ruby: Time.now + 7 * 86400
来源：http://hz.sweek.top/gtvfcjlciz.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cheryme.top/gtivqudkpd.html

[J06] 计算两时间之差
来源：http://hz.tian-w.cn/gtiypmchqh.html

Py:   (end - start).total_seconds()
来源：http://hz.zhixingplan.top/gttofrzqjt.html

PHP:  $end->diff($start)->days;
来源：http://hz.ppjwa.cn/gtfxbqvibh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.svipenyu.cn/gtuyyflgnq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.sxryk.cn/gtuoduatul.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yangfankeji.com/gtqggxctkx.html

Go:   end.Sub(start).Hours()
来源：http://hz.fzhhl.top/gtnzqgjmph.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yanxiufei.cn/gtybuqseqy.html

C#:   (end - start).TotalSeconds
来源：http://hz.yonumen.top/gtebiktdaa.html

[J07] 比较两个日期
来源：http://hz.dianchejie.cn/gtuxfdmiks.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yuxming.cn/gtzjguhfxn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhijiandao.cn/gtfnnrfqjk.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.xuetiantiany.cn/gtndflwyfr.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.0kj1m.cn/gtwtjpbaxj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xuetiantiany.cn/gtgwwlijsg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.aibaodan.cn/gtbtzshamj.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xylfe.cn/gtvrrvdgll.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.wangshuangyany.cn/gtlkaqouxz.html

[J08] 提取年月日与星期
来源：http://hz.zhongyouzk.top/gtcqqphhoi.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhengqikj.top/gtouxdoqgu.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.sxryk.cn/gtulxarnox.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.wangshuangyany.cn/gthbobiuvo.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.tian-w.cn/gtidhpuvbv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.quarkkingdee.top/gtrjklswyk.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hfpthk.cn/gtcrhttksc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hywenlv.cn/gtiadjoqkt.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hysaishi.cn/gtsejyypyc.html

[J09] 时区处理
来源：http://hz.wangshuangyany.cn/gtvczgodvb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.svipenyu.cn/gtncinflnb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yj20258.top/gtmhnkhyvs.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.chenlongwang.top/gtghoboxeu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hnxiangtu.top/gtffbaokuh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ywan-chungtsiang.top/gtreeibiog.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ydjk.org.cn/gtbchijnhq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.316326.xyz/gtgkedsywx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.svipenyu.cn/gtnfbjgpst.html

[J10] 取今天 / 本月第一天
来源：http://hz.sweek.top/gtermxlclx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shanyushiyangkeji.top/gtdtynbhhw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.sweek.top/gtetmxhnwg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.chenjidiqi.icu/gtzswfvvcz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hongshengwenyu.top/gtmuxwgjef.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.0kj1m.cn/gtpnjzutta.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.chenlongwang.top/gthuodilts.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.gaohongyu789.top/gtrxyuffrn.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.dianchejie.cn/gtwhyycmqn.html

================================================================================
来源：http://hz.hnqzz.top/gtvafnwopc.html

K. JSON 与序列化
来源：http://hz.svipenyu.cn/gtrfhnahvf.html

================================================================================
来源：http://hz.jinqigfzy.top/gtctiewdfa.html

[K01] 对象转 JSON 字符串
来源：http://hz.sysykeji.top/gtbsjhpsyu.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.chenzaomai.com/gtzyqksvgk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xuetiantiany.cn/gtjcgwokmm.html

JS:   JSON.stringify(obj)
来源：http://hz.nanxuanxn.top/gtpfzrxbbg.html

TS:   JSON.stringify(obj)
来源：http://hz.gogol.net.cn/gtkuooftva.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhixingplan.top/gthvdbtwua.html

Go:   json.Marshal(obj)
来源：http://hz.guowangkeji.top/gtvfhmuuza.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.xingfuxueyuan.xyz/gtvjreviin.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zycfv.cn/gtllfxfnoa.html

[K02] JSON 字符串转对象
来源：http://hz.daria6918.cn/gtcyxwlrgc.html

Py:   json.loads(s)
来源：http://hz.zhongyouzk.top/gttbweqott.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yj20258888.top/gtamkvkhnj.html

JS:   JSON.parse(s)
来源：http://hz.hammf.cn/gtqrnjrcpq.html

TS:   JSON.parse(s)
来源：http://hz.ywan-chungtsiang.top/gtoxnxcfog.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.feifeiyinyue.top/gtvqopozjp.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jinqigfzy.top/gtldjadlns.html

Ruby: JSON.parse(s)
来源：http://hz.shuidangran.top/gtewpzjrrx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.cdnleiting.top/gtnlrjlgla.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.52xcode.cn/gtuvwqxmlg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.sxryk.cn/gtsbuihbgs.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jlsjyb.cn/gtkjdboeul.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jiagoushi.top/gteoimywez.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xuetiantiany.cn/gttpjlqtuw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zhijiandao.cn/gtimuynnmx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ehwqpu.com/gtwvkolmya.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zdqjudy.top/gtfsurwogm.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.52xcode.cn/gtpekjnrwq.html

[K04] 读取 JSON 文件
来源：http://hz.sufxvd.cn/gtulxebutg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zycfv.cn/gtxnmzbjmq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.feifeiyinyue.top/gtufqgyxry.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ywan-chungtsiang.top/gtrzgozlra.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yongpay.top/gtdcvyipzx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jyoumei.cn/gttnztlpvr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xingfuxueyuan.xyz/gtlbdimbfs.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yonumen.top/gtsubbxouf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.vqdsnc.cn/gtpdmftrny.html

[K05] 深拷贝对象
来源：http://hz.nanxinkj.top/gtowxnsfkq.html

Py:   copy.deepcopy(obj)
来源：http://hz.sysykeji.top/gtyrksxsqw.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hammf.cn/gtgpzvkuri.html

JS:   structuredClone(obj)
来源：http://hz.c1oappe.top/gtmeyxaryb.html

TS:   structuredClone(obj)
来源：http://hz.iojbl.cn/gtauahwqbf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hfpthk.cn/gthzxuzklp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hfpthk.cn/gtpmbogtit.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.9152youxi.cn/gthvzarjji.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.shanyushiyangkeji.top/gtvlsrolzu.html

[K06] 解析 URL 查询串
来源：http://hz.tian-w.cn/gtqzgdnpyi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhoulong.xyz/gtfcqeqirl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.pengpengdd.cyou/gtmtvqeoql.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yuanzhike.top/gtefkclecu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.dianchejie.cn/gtesibbhbw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jinqigufen.top/gtfkoouors.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jqgfzy.top/gtsstmdhnu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ivvv.top/gtkedxwnjf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yj20258.top/gtpoiiofjs.html

[K07] 进制转换
来源：http://hz.316326.xyz/gtrgbozioc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.xylfe.cn/gtluuhhxen.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yanxiufei.cn/gtajuxyeqf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jinghuilouyu.cn/gthzzbmhjg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.feifeiyinyue.top/gtsnuhzbni.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zdqjudy.top/gtgrfrtclz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xingfuxueyuan.xyz/gtlveyxeyu.html


<!-- 参考信息 -->