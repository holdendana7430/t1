代发 wailian999

TS:   throw new Error("错误信息");
来源：http://hz.sufxvd.cn/gtbofybfuc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.daria6918.cn/gthkcrgywh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yonumen.top/gtwtpqbcgk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.dianchejie.cn/gtgduswvkn.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zhiwuduotai.top/gteuwzjfhp.html

[H04] 自定义异常类型
来源：http://hz.zhoulong.xyz/gtzzywwwif.html

Py:   class MyError(Exception): pass
来源：http://hz.haohaochexian.top/gttldrxuvb.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yj20258.top/gtqwitknbf.html

JS:   class MyError extends Error {}
来源：http://hz.nanxuanxn.top/gtcuvybqfc.html

TS:   class MyError extends Error {}
来源：http://hz.shuidangran.top/gtpxkfyufk.html

Java: class MyException extends RuntimeException {}
来源：http://hz.tianlin.xyz/gtvkpnmhzt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.daria6918.cn/gtpmctmeuo.html

Ruby: class MyError < StandardError; end
来源：http://hz.xingfuxueyuan.xyz/gthwofoksv.html

C#:   class MyException : Exception {}
来源：http://hz.pengpengdd.cyou/gtptznxrgf.html

[H05] 捕获特定类型
来源：http://hz.cheryme.top/gtsukmbnko.html

Py:   except ValueError as e:
来源：http://hz.zhijiandao.cn/gtpkdoelho.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.shuidangran.top/gtzrppmmif.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.sxryk.cn/gtioscgsnc.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.nanxinkj.top/gtycuktmoc.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.xinyue.icu/gtzyshipxn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.redwolf501.top/gtvmjhcsvk.html

Ruby: rescue ArgumentError => e
来源：http://hz.guowangkeji.top/gtcrebzwkh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hywenlv.cn/gttaxpjstr.html

[H06] 可选值 / 空值安全访问
来源：http://hz.cucudq.cn/gthojgfyyn.html

Py:   value = d.get("k") or default
来源：http://hz.cdnleiting.top/gtqixjkdpz.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.daxiang520.top/gtdjhqpjkb.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.daxiang520.top/gtwcyfrhzp.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.tianlin.xyz/gtttpbmlwi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.cdnleiting.top/gtqoyfywkk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.guowangkeji.top/gtfyyxetjv.html

Ruby: d&.dig(:a, :b)
来源：http://hz.xuetiantiany.cn/gtjzjdiufh.html

C#:   obj?.A?.B ?? default
来源：http://hz.pycfn.com/gtndelarph.html

[H07] 断言
来源：http://hz.havefunace.top/gtksjhmqwo.html

Py:   assert x > 0, "必须为正"
来源：http://hz.snrcjt.cn/gtkxukfxrs.html

PHP:  assert($x > 0);
来源：http://hz.dianchejie.cn/gtxggdnueq.html

JS:   console.assert(x > 0);
来源：http://hz.xziqi.cn/gtlfaocmfr.html

TS:   console.assert(x > 0);
来源：http://hz.meibo888.top/gthxgeogga.html

Java: assert x > 0 : "必须为正";
来源：http://hz.dianchejie.cn/gtmfzvamlz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.shanyushiyangtech.top/gtkhmeciwx.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.gotoacloud.top/gtjkrhangh.html

C#:   Debug.Assert(x > 0);
来源：http://hz.aizwys.cn/gtqfmfrfkq.html

[H08] 获取错误信息与堆栈
来源：http://hz.guowangkeji.top/gtswbdbfdk.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.redwolf501.top/gtkpukxyow.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yuanzhike.top/gtuwqqlffs.html

JS:   e.message;  e.stack
来源：http://hz.zhijiandao.cn/gtqhebuzhq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yj20258888.top/gtvhviicgf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.iojbl.cn/gtmwrhykht.html

Go:   err.Error()
来源：http://hz.zhongyouzk.top/gtbtbqeiry.html

Ruby: e.message;  e.backtrace
来源：http://hz.meibo888.top/gtrnheiabl.html

C#:   e.Message;  e.StackTrace
来源：http://hz.bjfxy.top/gtzdzfmigw.html

[H09] 带错误码的异常
来源：http://hz.sysykeji.top/gtjeqnjoye.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.andypj.xyz/gtkpvtcsvh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.9152youxi.cn/gtwwxpfecl.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.kuanghao11.cn/gtxjqvwqpm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.chenlongwang.top/gtqklgaxtb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yj202588.top/gthuuwjbls.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jiagoushi.top/gtpadpehbq.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.nanxinkj.top/gtjcsuiovq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.aibaodan.cn/gtexawulfp.html

[H10] 资源自动释放
来源：http://hz.sxryk.cn/gtmlnawdak.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.guowangkeji.top/gtflpmmbzq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jqgufenzy.top/gtpvgfzxaj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zycfv.cn/gtpvovibrc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.snrcjt.cn/gtuebclcrx.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.quarkkingdee.top/gtcosfxkbw.html

Go:   defer f.Close()
来源：http://hz.zhongyouzk.top/gtmhwgzkmm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.ybcxt.top/gtdlvctgrr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hnqzz.top/gtszvekzob.html

================================================================================
来源：http://hz.yj20258888.top/gtvgkawexp.html

I. 正则表达式
来源：http://hz.svipenyu.cn/gtjimjkefu.html

================================================================================
来源：http://hz.zhengqikj.top/gtxwjixxwo.html

[I01] 判断是否匹配
来源：http://hz.nwbrower.top/gtmuyvdvrx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.mhx1999.top/gtkleificm.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.xinyue.icu/gtuffubreh.html

JS:   /\d+/.test(s)
来源：http://hz.havefunace.top/gtjltlolhu.html

TS:   /\d+/.test(s)
来源：http://hz.yangfankeji.com/gtrpikirmm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hysaishi.cn/gtvctvsfsn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jqgfzy.top/gtaqfopowu.html

Ruby: s.match?(/\d+/)
来源：http://hz.jqgufenzy.top/gtfymeegas.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.vqdsnc.cn/gtcwrtkhir.html

[I02] 提取所有匹配
来源：http://hz.ybcxt.top/gtdeeoyued.html

Py:   re.findall(r"\d+", s)
来源：http://hz.svipenyu.cn/gthoswtcaa.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.ywan-chungtsiang.top/gtueyawrpv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhoulong.xyz/gtqukxsxfd.html

TS:   s.match(/\d+/g)
来源：http://hz.shanyushiyangkeji.top/gtgjsnxpqr.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.daria6918.cn/gtaiwxjogi.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jinqigfzy.top/gtynotgmsg.html

Ruby: s.scan(/\d+/)
来源：http://hz.hywenlv.cn/gtkbvwwcay.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.svipenyu.cn/gtxudlswra.html

[I03] 提取捕获分组
来源：http://hz.daxiang520.top/gtqafcfhbf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhaomingkeji.xyz/gtrmyfrncx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xylfe.cn/gtawcymzyy.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zycfv.cn/gtgllizyav.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.gotoacloud.top/gtusqkljne.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xuanzx.com/gtugagbtof.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.fengsongda.top/gtaapbeexb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.snrcjt.cn/gtzrmmdaxq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.chenlongwang.top/gtpabtjqkv.html

[I04] 正则替换
来源：http://hz.316326.xyz/gtugfjpvia.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yongpay.top/gtqkqjtxvi.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.shzxlz.cn/gtypmjljza.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.shangyingyoupin.top/gtgginlduu.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.ppjwa.cn/gtceofdmfi.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yj20258.top/gthvxdbufr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.bjfxy.top/gtgqzhcbri.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.gaohongyu789.top/gtdtuuwmer.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.xingfuxueyuan.xyz/gtlcaiovgi.html

[I05] 按正则拆分
来源：http://hz.haohaochexian.top/gthwkvqhxk.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.vqdsnc.cn/gtimmenkdj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.9152youxi.cn/gtefkgtlum.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.dianchejie.cn/gtxcuktigr.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ydjk.org.cn/gtibxdgdiz.html

Java: s.split("\\s*,\\s*")
来源：http://hz.gotoacloud.top/gtcoizjgay.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yj20258.top/gtlfuxvmgw.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xziqi.cn/gtfieienhx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.shzxlz.cn/gtdkewfxeg.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.gzhubu.top/gtiwloszzt.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.redwolf501.top/gtjpsmeutv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.vqdsnc.cn/gtudxetkyz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.daria6918.cn/gtcshclhgj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yonumen.top/gtuearyfdq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.chenlongwang.top/gthzyflojs.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zhaomingkeji.xyz/gtyznhpyda.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.shanyushiyangtech.top/gteejhdghf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.gotoacloud.top/gthttxjdjy.html

[I07] 忽略大小写与多行模式
来源：http://hz.zhixingplan.top/gtbdreyoho.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ehwqpu.com/gtsbwizbzu.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.aibaodan.cn/gtslnpgiui.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jqgufenzy.top/gtxdjpkmcd.html

TS:   /error/gim
来源：http://hz.cucudq.cn/gtmpbjigls.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhaomingkeji.xyz/gttzevkvwa.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yuxming.cn/gthwovotaa.html

Ruby: s.scan(/error/i)
来源：http://hz.kuanghao11.cn/gtblwiwhrp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.bjfxy.top/gtgirfsxce.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.nanxuanxn.top/gtogfikygy.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jqgfzy.top/gttafnmtld.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhijiandao.cn/gtclaxdlla.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gaohongyu789.top/gtgbsdpoti.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xinyue.icu/gtetyoafbc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yonumen.top/gtcuueypjq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.c1oappe.top/gtwitiqslk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yonumen.top/gtvmlxdgfr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.hywenlv.cn/gtljzjdrxi.html

================================================================================
来源：http://hz.fengsongda.top/gtuxcmyymf.html

J. 日期与时间
来源：http://hz.haohaochexian.top/gtwyowrjay.html

================================================================================
来源：http://hz.iojbl.cn/gtuknnriom.html

[J01] 获取当前时间
来源：http://hz.cdnleiting.top/gtmhrfezbs.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yuanzhike.top/gteollcbck.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.bjfxy.top/gtwezmdeyt.html

JS:   new Date();  Date.now()
来源：http://hz.snrcjt.cn/gtuxjwzbbd.html

TS:   new Date();  Date.now()
来源：http://hz.feifeiyinyue.top/gtyioqzosc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.0kj1m.cn/gtbeppmbbi.html

Go:   time.Now()
来源：http://hz.mhx1999.top/gtdslqmysy.html

Ruby: Time.now
来源：http://hz.andypj.xyz/gtxqkijtkb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jqgufenzy.top/gtwpdnwfyp.html

[J02] 格式化输出
来源：http://hz.c1oappe.top/gtzuilgzol.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nanxuanxn.top/gtyiodgiva.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jinqigufen.top/gtebatfvhx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.havefunace.top/gtbfaflwcx.html

TS:   d.toISOString()
来源：http://hz.daxiang520.top/gtkdyaoxwq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.shanyushiyangkeji.top/gtsjgmmqeu.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.cashguo.top/gtsqqkomqq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.pengpengdd.cyou/gtciilewvd.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yanxiufei.cn/gtldgdmoku.html

[J03] 字符串解析为日期
来源：http://hz.guowangkeji.top/gtwqgrjits.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.tanke756.top/gtmanpjpct.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yj20258888.top/gthprgmsuy.html

JS:   new Date("2024-01-02")
来源：http://hz.kuanghao11.cn/gtgepacgnz.html

TS:   new Date("2024-01-02")
来源：http://hz.chenjidiqi.icu/gtvolokqmn.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.dianchejie.cn/gtifkjwxor.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.pycfn.com/gttzoyrknv.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.kuanghao11.cn/gthmeunjgz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.chenjidiqi.icu/gtfjwxcvus.html

[J04] 时间戳与日期互转
来源：http://hz.tianlin.xyz/gticgqyopw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.sufxvd.cn/gtgnqxuriy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jinyuanbaomall.cn/gtjqjiqrok.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zhixingplan.top/gtypvofbff.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yj20258.top/gtwazdzsts.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.0kj1m.cn/gtbnhyctkp.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.shangyingyoupin.top/gtgqiszpur.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.sweek.top/gtlrbdlrnp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.xuanzx.com/gtjiyqlbzq.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhijiandao.cn/gtcqdhjrwe.html

Py:   now + timedelta(days=7)
来源：http://hz.hnxiangtu.top/gtlvquxcgn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.xuetiantiany.cn/gtfftxihnl.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shzxlz.cn/gtbescgnwn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yj20258888.top/gtbwzmhzhn.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.nwbrower.top/gtcrxeroec.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.snrcjt.cn/gtavwbltpn.html

Ruby: Time.now + 7 * 86400
来源：http://hz.vqdsnc.cn/gtmgdjbtaz.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ybcxt.top/gtyvpzdhic.html

[J06] 计算两时间之差
来源：http://hz.haohaochexian.top/gtmxmsajet.html

Py:   (end - start).total_seconds()
来源：http://hz.jinqigufen.top/gtlpfaqkgp.html

PHP:  $end->diff($start)->days;
来源：http://hz.zdqjudy.top/gtbmpjsgay.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ybcxt.top/gtfmgtvxyg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.nwbrower.top/gtkhakzqrv.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cqqwz.cn/gtcyipoyii.html

Go:   end.Sub(start).Hours()
来源：http://hz.pengpengdd.cyou/gtdavmfmbr.html

Ruby: end - start                 # 返回秒数
来源：http://hz.gogol.net.cn/gtlgmdtcru.html

C#:   (end - start).TotalSeconds
来源：http://hz.ppjwa.cn/gtwxjvowsh.html

[J07] 比较两个日期
来源：http://hz.ehwqpu.com/gtwrucahpi.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.shuidangran.top/gtexaoqqyq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.cucudq.cn/gtnraijega.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.quarkkingdee.top/gtrdwyehlq.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yuxming.cn/gtdnwkajqo.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hywenlv.cn/gturahyarx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.0kj1m.cn/gthdqoihil.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zhengqikj.top/gtshxxkcwb.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.shzxlz.cn/gthnbnokkl.html

[J08] 提取年月日与星期
来源：http://hz.hnqzz.top/gtpcsubwgl.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.pycfn.com/gtmpysmddp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.tianlin.xyz/gthwhutxar.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yueranfly.top/gtqbsdhlya.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shuidangran.top/gtswgccuye.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yj202588.top/gtyseldufu.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.xingfuxueyuan.xyz/gttadvyftl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cheryme.top/gtpziceibr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hfpthk.cn/gthyiajwzf.html

[J09] 时区处理
来源：http://hz.ivvv.top/gtcwxerzfa.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.birdmap.top/gtzaludzgr.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.aizwys.cn/gthjmkbonp.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jlsjyb.cn/gtgffvfvdj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nanxinkj.top/gtqqfxucns.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.redwolf501.top/gtkafitdho.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yonumen.top/gtejockran.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.tian-w.cn/gtpnkuiimj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.pengpengdd.cyou/gtthzpvmpy.html

[J10] 取今天 / 本月第一天
来源：http://hz.cucudq.cn/gtnecgcjzi.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.sysykeji.top/gttogdhpyl.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xinyue.icu/gthwdszims.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.redwolf501.top/gthpymvogu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ivvv.top/gtsdkbtxjs.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jinqigfzy.top/gttqjlqpss.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.quarkkingdee.top/gtkmyiysay.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.9152youxi.cn/gtjycbnoth.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.feifeiyinyue.top/gtaviqwpuw.html

================================================================================
来源：http://hz.jiagoushi.top/gtjbescbua.html

K. JSON 与序列化
来源：http://hz.xuanzx.com/gtbpnfmusc.html

================================================================================
来源：http://hz.aizwys.cn/gtajmpyada.html

[K01] 对象转 JSON 字符串
来源：http://hz.ydzc1.top/gttkaeoleu.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jqgfzy.top/gtfotcxgzb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.haohaochexian.top/gtbyrrmdjm.html

JS:   JSON.stringify(obj)
来源：http://hz.fzhhl.top/gtfiickfjp.html

TS:   JSON.stringify(obj)
来源：http://hz.yuxming.cn/gtpezwpdnz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yj20258888.top/gtbsaixoma.html

Go:   json.Marshal(obj)
来源：http://hz.fengsongda.top/gtscoxgvws.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.xinyue.icu/gttrnsxopx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.sysykeji.top/gtrmsdfoga.html

[K02] JSON 字符串转对象
来源：http://hz.yj20258.top/gtuyblqbgk.html

Py:   json.loads(s)
来源：http://hz.xingfuxueyuan.xyz/gtjgugvdwe.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.guowangkeji.top/gtlwkkjvsh.html

JS:   JSON.parse(s)
来源：http://hz.cqqwz.cn/gtufyptlcw.html

TS:   JSON.parse(s)
来源：http://hz.mhx1999.top/gtgqkluqnq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhiwuduotai.top/gtllxjdvnn.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.kuanghao11.cn/gtzzbxpabz.html

Ruby: JSON.parse(s)
来源：http://hz.zhixingplan.top/gtajepbbhk.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hammf.cn/gtjyqaewvr.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yanxiufei.cn/gtjhojdace.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.bjfxy.top/gtadzdyywg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.gaohongyu789.top/gtwacjvrvy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xinyue.icu/gtxxbvmerl.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yonumen.top/gtweinahqi.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.xingfuxueyuan.xyz/gtjzscbdxb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.sweek.top/gtkudmkovl.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.0kj1m.cn/gtwmnwhwrg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hywenlv.cn/gtzddcpoty.html

[K04] 读取 JSON 文件
来源：http://hz.tianlin.xyz/gtonfcceeq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hammf.cn/gtlvnhfthx.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.quarkkingdee.top/gtfytynwvk.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hnxiangtu.top/gtxgxumapq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ehwqpu.com/gtsshhhvvn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.pycfn.com/gtmmfgkcnm.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhiwuduotai.top/gtquosdboj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.andypj.xyz/gtjnkjzyyo.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jinqigufen.top/gtsjcqxvjh.html

[K05] 深拷贝对象
来源：http://hz.hysaishi.cn/gtuqlnwowp.html

Py:   copy.deepcopy(obj)
来源：http://hz.shzxlz.cn/gttclewwgv.html

PHP:  unserialize(serialize($obj));
来源：http://hz.quarkkingdee.top/gtdyjvflgf.html

JS:   structuredClone(obj)
来源：http://hz.xingfuxueyuan.xyz/gteytjlsme.html

TS:   structuredClone(obj)
来源：http://hz.sufxvd.cn/gtxszthlgf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.52xcode.cn/gtlmhwbasx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.birdmap.top/gtjkmcedmq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.gaohongyu789.top/gtmhqrthef.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.shangyingyoupin.top/gtfgbmbgnz.html

[K06] 解析 URL 查询串
来源：http://hz.shanyushiyangtech.top/gthvorgzxs.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.sweek.top/gtcjjughxw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.quarkkingdee.top/gthweazxcr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sweek.top/gttlxkoqid.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.birdmap.top/gtvbylgwce.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.daxiang520.top/gtuszwtlke.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.aizwys.cn/gtvqesqxaf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.tianlin.xyz/gtyodjmorr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.svipenyu.cn/gtqgwxetju.html

[K07] 进制转换
来源：http://hz.zhijiandao.cn/gtpusinnbr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cdnleiting.top/gtyafcisck.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.chenjidiqi.icu/gtfrochmqc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yj20258.top/gtdtbxogqt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.aizwys.cn/gtaemftjds.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yangfankeji.com/gtdrimnwhv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jqgfzy.top/gtqnkfkhvi.html


<!-- 参考信息 -->