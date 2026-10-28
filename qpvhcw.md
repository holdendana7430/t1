代发 wailian999

[H03] 主动抛出异常
来源：http://hz.shanyushiyangtech.top/gtoreevwcl.html

Py:   raise ValueError("错误信息")
来源：http://hz.aibaodan.cn/gttwlqyyxi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.cqqwz.cn/gtgcxkunzk.html

JS:   throw new Error("错误信息");
来源：http://hz.feifeiyinyue.top/gtrmvzfnno.html

TS:   throw new Error("错误信息");
来源：http://hz.yvedp.cn/gtnjwpayna.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cdnleiting.top/gtvwxiccmm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jinghuilouyu.cn/gtdgfiygvo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.wangshuangyany.cn/gtsieumxzv.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.chenlongwang.top/gtodujwevx.html

[H04] 自定义异常类型
来源：http://hz.shzxlz.cn/gtygxnwcsn.html

Py:   class MyError(Exception): pass
来源：http://hz.zhoulong.xyz/gtnmecfmww.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.ybcxt.top/gtsxwazlzu.html

JS:   class MyError extends Error {}
来源：http://hz.chenlongwang.top/gtoiwtkdjy.html

TS:   class MyError extends Error {}
来源：http://hz.cheryme.top/gtjacphzfl.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhiwuduotai.top/gtrglvnprm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zdqjudy.top/gtloonejtn.html

Ruby: class MyError < StandardError; end
来源：http://hz.xinyue.icu/gtjnnnowql.html

C#:   class MyException : Exception {}
来源：http://hz.316326.xyz/gtwyuufuhv.html

[H05] 捕获特定类型
来源：http://hz.yueranfly.top/gtefxrlhfe.html

Py:   except ValueError as e:
来源：http://hz.yvedp.cn/gtncgthfob.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.redwolf501.top/gtfjgdlbnn.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.mhx1999.top/gttkgwflkc.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shanyushiyangkeji.top/gtedxiiaxr.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.gaohongyu789.top/gtrugcobay.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ywan-chungtsiang.top/gtgdwzdsaj.html

Ruby: rescue ArgumentError => e
来源：http://hz.feifeiyinyue.top/gtjgxrgqve.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jqgufenzy.top/gtxznknkys.html

[H06] 可选值 / 空值安全访问
来源：http://hz.sxryk.cn/gtsocobttj.html

Py:   value = d.get("k") or default
来源：http://hz.sxryk.cn/gtljnnvrtg.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhixingplan.top/gtormxmyoa.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.svipenyu.cn/gtgspwlxag.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hammf.cn/gtdafqvosy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.smart0.xyz/gtgsdcybhh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.hnxiangtu.top/gtawdtnuji.html

Ruby: d&.dig(:a, :b)
来源：http://hz.cheryme.top/gtkhexaxtv.html

C#:   obj?.A?.B ?? default
来源：http://hz.meibo888.top/gtgbmxwiec.html

[H07] 断言
来源：http://hz.yuanzhike.top/gtftuwjfui.html

Py:   assert x > 0, "必须为正"
来源：http://hz.fengsongda.top/gtiusnbbvj.html

PHP:  assert($x > 0);
来源：http://hz.zhengqikj.top/gtozgywecg.html

JS:   console.assert(x > 0);
来源：http://hz.gzhubu.top/gtvbnmcgbt.html

TS:   console.assert(x > 0);
来源：http://hz.hysaishi.cn/gtrbacsotf.html

Java: assert x > 0 : "必须为正";
来源：http://hz.iojbl.cn/gtjicqbfdo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.wangshuangyany.cn/gtkzfjfzik.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.redwolf501.top/gtfckbvcud.html

C#:   Debug.Assert(x > 0);
来源：http://hz.ydjk.org.cn/gtbruwzffz.html

[H08] 获取错误信息与堆栈
来源：http://hz.ybcxt.top/gtsofomzdx.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hongshengwenyu.top/gttropqhpp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ppjwa.cn/gtkhvoexhj.html

JS:   e.message;  e.stack
来源：http://hz.cucudq.cn/gtwkwyvmob.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhengqikj.top/gtoneeyjso.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.tanke756.top/gtexkrhbxh.html

Go:   err.Error()
来源：http://hz.jqgfzy.top/gtkvlbnvfk.html

Ruby: e.message;  e.backtrace
来源：http://hz.kuanghao11.cn/gtadekloyo.html

C#:   e.Message;  e.StackTrace
来源：http://hz.shanyushiyangtech.top/gtpxzvccjb.html

[H09] 带错误码的异常
来源：http://hz.havefunace.top/gtlzbayljh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhaomingkeji.xyz/gtveqbgsme.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.wangdashe.top/gtolslegti.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhoulong.xyz/gtsktpkfwm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.svipenyu.cn/gtxicjapay.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yj20258.top/gtmbftkrza.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.meibo888.top/gtcwaocsou.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.0kj1m.cn/gtvqxnveov.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.xuetiantiany.cn/gtwpdwlnnc.html

[H10] 资源自动释放
来源：http://hz.meibo888.top/gtdywudyla.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.smart0.xyz/gtocgnctey.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yj20258888.top/gtkysromsa.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gogol.net.cn/gtcmjwkxbp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xziqi.cn/gtridsiaum.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jyoumei.cn/gthdrshmrg.html

Go:   defer f.Close()
来源：http://hz.xingfuxueyuan.xyz/gtbjhprvmr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.nwbrower.top/gtiwjwxjtz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.birdmap.top/gtvblxglfj.html

================================================================================
来源：http://hz.vqdsnc.cn/gtauvyjznx.html

I. 正则表达式
来源：http://hz.xingfuxueyuan.xyz/gticsephsw.html

================================================================================
来源：http://hz.0kj1m.cn/gtyhjjmyzt.html

[I01] 判断是否匹配
来源：http://hz.wangshuangyany.cn/gtsgzgqwdu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hammf.cn/gtifgihthm.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.feifeiyinyue.top/gtknigrtcz.html

JS:   /\d+/.test(s)
来源：http://hz.9152youxi.cn/gtkviiarwm.html

TS:   /\d+/.test(s)
来源：http://hz.wangdashe.top/gtnorxcoon.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.xuetiantiany.cn/gtspjzesdy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.shuidangran.top/gtmnwrdgsj.html

Ruby: s.match?(/\d+/)
来源：http://hz.ehwqpu.com/gtyidwzyfm.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.gogol.net.cn/gtlythmktf.html

[I02] 提取所有匹配
来源：http://hz.yj20258.top/gthxwynoiu.html

Py:   re.findall(r"\d+", s)
来源：http://hz.aibaodan.cn/gtsgdgwuei.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xuetiantiany.cn/gtcfentmku.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.bjfxy.top/gtknretsrm.html

TS:   s.match(/\d+/g)
来源：http://hz.snrcjt.cn/gtsjndgyxs.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zhaomingkeji.xyz/gttuwbdsmi.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yonumen.top/gtfminnfir.html

Ruby: s.scan(/\d+/)
来源：http://hz.bjfxy.top/gtpyysrdrq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.iojbl.cn/gtnvhxnbsz.html

[I03] 提取捕获分组
来源：http://hz.zhixingplan.top/gtygtbqfuy.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.vqdsnc.cn/gtxjtnaffp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hnqzz.top/gtxvwpvwja.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.xuanzx.com/gtumegylfk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.smart0.xyz/gthxegzpki.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jqgufenzy.top/gtxecbsvsq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.kuanghao11.cn/gtqzalxork.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.nanxuanxn.top/gtlkocberd.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.xuetiantiany.cn/gtshabnqcc.html

[I04] 正则替换
来源：http://hz.zhiwuduotai.top/gtqzmxkadb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ppjwa.cn/gtfihhbcer.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhixingplan.top/gtsihcdlkv.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.gogol.net.cn/gthnxaacrq.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hnxiangtu.top/gtwhendxus.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhongyouzk.top/gtfatpxghn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.gogol.net.cn/gtkcayrseu.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.shangyingyoupin.top/gtegmsjkmf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jinqigfzy.top/gtynopuvlx.html

[I05] 按正则拆分
来源：http://hz.ppjwa.cn/gtmdzkfxic.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.snrcjt.cn/gtlxqcdauq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.shzxlz.cn/gtuvoxjygd.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jiagoushi.top/gtocqemugf.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yueranfly.top/gtrhbtdhed.html

Java: s.split("\\s*,\\s*")
来源：http://hz.havefunace.top/gtvkkcrlmv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.tian-w.cn/gtunqjkyrg.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yueranfly.top/gtpcxowpdq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.shanyushiyangkeji.top/gtfobdwomw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.feifeiyinyue.top/gtscyuzcdy.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.shuidangran.top/gtjzevvsqb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.tian-w.cn/gtzpjasrfd.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tianlin.xyz/gtrsbvuvov.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tanke756.top/gtctdzazgu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.9152youxi.cn/gtirdbeaeo.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hnxiangtu.top/gtrfqbvhhs.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.smart0.xyz/gtbtojbpju.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.aizwys.cn/gtqkjoozbb.html

[I07] 忽略大小写与多行模式
来源：http://hz.cqqwz.cn/gthwfjckiq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hnxiangtu.top/gtrpmgejhv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.shuidangran.top/gtcthhcggm.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yj20258888.top/gtcvblhjlt.html

TS:   /error/gim
来源：http://hz.zhiwuduotai.top/gtbqakhihx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.tanke756.top/gtfartgffr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.redwolf501.top/gtqyczolkg.html

Ruby: s.scan(/error/i)
来源：http://hz.hfpthk.cn/gtgmyduygi.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jqgfzy.top/gtlvbelnme.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.mhx1999.top/gtllnihzxp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.guowangkeji.top/gtaknzovcr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.shanyushiyangkeji.top/gtwppwnild.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.aibaodan.cn/gtwrsxdxgg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.c1oappe.top/gtlhencuzo.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zycfv.cn/gtorxdqmjk.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.nanxinkj.top/gtabfirlgy.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shanyushiyangtech.top/gtdtwnbdgt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.vqdsnc.cn/gtuxhxprql.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtnvyzekpd.html

J. 日期与时间
来源：http://hz.shanyushiyangkeji.top/gttuaftlex.html

================================================================================
来源：http://hz.sxryk.cn/gtqcqseisj.html

[J01] 获取当前时间
来源：http://hz.gogol.net.cn/gtzobxhruh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jiagoushi.top/gtsutpfzbn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.hammf.cn/gtluuutamy.html

JS:   new Date();  Date.now()
来源：http://hz.xziqi.cn/gttcgibolx.html

TS:   new Date();  Date.now()
来源：http://hz.shangyingyoupin.top/gtfgrufzxi.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hfpthk.cn/gttgwsedca.html

Go:   time.Now()
来源：http://hz.c1oappe.top/gtxcfhkxni.html

Ruby: Time.now
来源：http://hz.ywan-chungtsiang.top/gtbjwsgbib.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.bjfxy.top/gtcyzztxil.html

[J02] 格式化输出
来源：http://hz.yj20258888.top/gtboptvfth.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.aibaodan.cn/gtayoknmzv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ivvv.top/gtmnktglou.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.sweek.top/gtelnnwfsh.html

TS:   d.toISOString()
来源：http://hz.vqdsnc.cn/gtsxgdokfx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hammf.cn/gtfnnomymw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.gaohongyu789.top/gtbxljbxuq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jlsjyb.cn/gtdvlqmugz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jiagoushi.top/gtnhldhdrt.html

[J03] 字符串解析为日期
来源：http://hz.zdqjudy.top/gtnejfgvaj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.aizwys.cn/gtphibypfy.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.daxiang520.top/gtqlgvufiy.html

JS:   new Date("2024-01-02")
来源：http://hz.zdqjudy.top/gtukahlzvt.html

TS:   new Date("2024-01-02")
来源：http://hz.hywenlv.cn/gthieklijk.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yonumen.top/gtclafworo.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yangfankeji.com/gtlgpazkrz.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jinqigfzy.top/gtkpslwove.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jqgfzy.top/gtddxombwx.html

[J04] 时间戳与日期互转
来源：http://hz.smart0.xyz/gtkdymqhhj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.xinyue.icu/gtenhdqazb.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yvedp.cn/gtkckaikbw.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.9152youxi.cn/gtunsgzpii.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.ywan-chungtsiang.top/gtgovydswq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.c1oappe.top/gtadbexywj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.gogol.net.cn/gtywqxehgo.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xinyue.icu/gtnjkskneq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ywan-chungtsiang.top/gtrdhwkkqs.html

[J05] 时间加减（加 7 天）
来源：http://hz.ivvv.top/gtjlmvnhut.html

Py:   now + timedelta(days=7)
来源：http://hz.tanke756.top/gtkoxyhejc.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hammf.cn/gtzpuidnmd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.pengpengdd.cyou/gtbqqmrbho.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yj202588.top/gtpchjqdjz.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.cheryme.top/gtvhxzpxcj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.fengsongda.top/gtyjsjnwji.html

Ruby: Time.now + 7 * 86400
来源：http://hz.havefunace.top/gtsppwzpqr.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xuanzx.com/gtziycyrsn.html

[J06] 计算两时间之差
来源：http://hz.redwolf501.top/gtjxhufajf.html

Py:   (end - start).total_seconds()
来源：http://hz.daxiang520.top/gtrnckcweo.html

PHP:  $end->diff($start)->days;
来源：http://hz.shanyushiyangtech.top/gtfomcefir.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.sufxvd.cn/gtojrqvmvc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ehwqpu.com/gtfjwleyfo.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.wangdashe.top/gtxhnmvfyn.html

Go:   end.Sub(start).Hours()
来源：http://hz.aibaodan.cn/gtqnipwfdb.html

Ruby: end - start                 # 返回秒数
来源：http://hz.tianlin.xyz/gtlbgqhldh.html

C#:   (end - start).TotalSeconds
来源：http://hz.yuxming.cn/gtskhihsfa.html

[J07] 比较两个日期
来源：http://hz.jiagoushi.top/gtyzeajltk.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.smart0.xyz/gtabadzsnq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xziqi.cn/gtxzdabzsr.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.guowangkeji.top/gtlwgsookp.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shzxlz.cn/gttgyhjuld.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.316326.xyz/gtyqpycyuy.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.guowangkeji.top/gttlkvcpyq.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.redwolf501.top/gtecgwdybk.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.cashguo.top/gtqnrfgvsp.html

[J08] 提取年月日与星期
来源：http://hz.vqdsnc.cn/gtjupabepc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yj202588.top/gtsbwmxohq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yj20258888.top/gtaxvrzjjj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.chenzaomai.com/gtwkuoclwm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jinqigfzy.top/gtvteoibpr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hongshengwenyu.top/gtlfiwcyco.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.sweek.top/gtxuuiovkd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.smart0.xyz/gtazepsxxp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.snrcjt.cn/gtihsqfogn.html

[J09] 时区处理
来源：http://hz.daxiang520.top/gtvbknurhe.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jlsjyb.cn/gtnidaskbi.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhixingplan.top/gtktbyaitl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.pengpengdd.cyou/gtbpvzpgxn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.pengpengdd.cyou/gtfrrjpnwo.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.feifeiyinyue.top/gtnhftwlgx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yuanzhike.top/gtxznophkz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.kuanghao11.cn/gtadssjvlv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hysaishi.cn/gtvchjdlen.html

[J10] 取今天 / 本月第一天
来源：http://hz.pycfn.com/gtvtlttltx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.9152youxi.cn/gtvuxmkfdt.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.quarkkingdee.top/gtkjinfpih.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.gaohongyu789.top/gtlpwmqigk.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.sysykeji.top/gtgpvspxai.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jlsjyb.cn/gtdboanxon.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.sweek.top/gtoljslgbi.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yangfankeji.com/gthlnhcnom.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.sufxvd.cn/gtalxgcfts.html

================================================================================
来源：http://hz.daxiang520.top/gtqmihcdkx.html

K. JSON 与序列化
来源：http://hz.feifeiyinyue.top/gtxmenmqgy.html

================================================================================
来源：http://hz.jyoumei.cn/gtbjkjfjls.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhaomingkeji.xyz/gtodzzqnga.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.pengpengdd.cyou/gtvccnshxv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yonumen.top/gtuxiwdkpd.html

JS:   JSON.stringify(obj)
来源：http://hz.tanke756.top/gttngnovvd.html

TS:   JSON.stringify(obj)
来源：http://hz.jinqigufen.top/gtxoxubqvx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.andypj.xyz/gtvbokceom.html

Go:   json.Marshal(obj)
来源：http://hz.xylfe.cn/gtesoimois.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.9152youxi.cn/gtbasgviao.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.daxiang520.top/gtessxoqqz.html

[K02] JSON 字符串转对象
来源：http://hz.jqgfzy.top/gtsztwpzrb.html

Py:   json.loads(s)
来源：http://hz.jinyuanbaomall.cn/gtklwweylr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zycfv.cn/gtqbfskdup.html

JS:   JSON.parse(s)
来源：http://hz.redwolf501.top/gtusaszxbs.html

TS:   JSON.parse(s)
来源：http://hz.yongpay.top/gtgfgdxoqs.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.gzhubu.top/gtfhirvesj.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hywenlv.cn/gtnwhxcnnj.html

Ruby: JSON.parse(s)
来源：http://hz.chenzaomai.com/gtdtcvwzck.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.fzhhl.top/gtxvschtmm.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yanxiufei.cn/gtbjaoszoz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xingfuxueyuan.xyz/gtqbgeybrb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jinghuilouyu.cn/gtsjtatpqp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shangyingyoupin.top/gtnncmpzrr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xinyue.icu/gttbdlamxt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jqgufenzy.top/gtlgmslqyp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ywan-chungtsiang.top/gtoclddwaw.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.vqdsnc.cn/gtdtqrfmdr.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.snrcjt.cn/gtezwmowgo.html

[K04] 读取 JSON 文件
来源：http://hz.ivvv.top/gtxdjcnukj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yj20258.top/gtficuceaj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.dashuyun.cn/gtddcdifun.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.daria6918.cn/gtgnktzset.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhiwuduotai.top/gtghdhztuk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.nanxuanxn.top/gtgprumojm.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jinqigufen.top/gtjmjmxehn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.shuidangran.top/gticwymnro.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.cashguo.top/gtqvrtwxdl.html

[K05] 深拷贝对象
来源：http://hz.pengpengdd.cyou/gtnskkiqcd.html

Py:   copy.deepcopy(obj)
来源：http://hz.sweek.top/gtuxgiwmpc.html

PHP:  unserialize(serialize($obj));
来源：http://hz.nwbrower.top/gtbwnttvvd.html

JS:   structuredClone(obj)
来源：http://hz.yangfankeji.com/gtxcycgkrs.html

TS:   structuredClone(obj)
来源：http://hz.chenlongwang.top/gtzkzdlieq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.meibo888.top/gtogztmpjc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.svipenyu.cn/gtcdbpzron.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.cashguo.top/gttxlldtwe.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.meibo888.top/gttktsdisa.html

[K06] 解析 URL 查询串
来源：http://hz.havefunace.top/gtueqrbwoh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.birdmap.top/gtoottgegd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.vqdsnc.cn/gtmzzxnvpu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinqigufen.top/gtpxlhmvnl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhengqikj.top/gtprzaxrrm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.c1oappe.top/gtnlhtejkg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cqqwz.cn/gtbfczmtet.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.chenjidiqi.icu/gttnwakbnf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ivvv.top/gtkugiblkf.html

[K07] 进制转换
来源：http://hz.tianlin.xyz/gtppilffos.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.wangshuangyany.cn/gtjhyyiafb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hywenlv.cn/gtitgabusv.html


<!-- 参考信息 -->