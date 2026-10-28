代发 wailian999

TS:   throw new Error("错误信息");
来源：http://hz.yangfankeji.com/gtozzlqood.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhongyouzk.top/gttrslumlu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.mhx1999.top/gtundpnwmp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jinqigfzy.top/gtdwnemqav.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.andypj.xyz/gtqhqeavdk.html

[H04] 自定义异常类型
来源：http://hz.sxryk.cn/gtslqcmrby.html

Py:   class MyError(Exception): pass
来源：http://hz.xingfuxueyuan.xyz/gtxkvhczfz.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.sxryk.cn/gtfuxpcjey.html

JS:   class MyError extends Error {}
来源：http://hz.tanke756.top/gtaiiigcuk.html

TS:   class MyError extends Error {}
来源：http://hz.fzhhl.top/gtrumprfpq.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yuanzhike.top/gtsfwvljyn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ydjk.org.cn/gtwvwusfec.html

Ruby: class MyError < StandardError; end
来源：http://hz.nwbrower.top/gtlqcllsvn.html

C#:   class MyException : Exception {}
来源：http://hz.jlsjyb.cn/gteczyjuku.html

[H05] 捕获特定类型
来源：http://hz.cucudq.cn/gtejhigaiv.html

Py:   except ValueError as e:
来源：http://hz.aizwys.cn/gtaljkjhlk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.snrcjt.cn/gtuyrturyh.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.redwolf501.top/gtkiwhsvsh.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.wangshuangyany.cn/gtkwnisimd.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.xylfe.cn/gtupgwpwnf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.shangyingyoupin.top/gtgzkxmhse.html

Ruby: rescue ArgumentError => e
来源：http://hz.ywan-chungtsiang.top/gtsvibsvdk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.meibo888.top/gtbmvlylci.html

[H06] 可选值 / 空值安全访问
来源：http://hz.chenzaomai.com/gtzfuauxzc.html

Py:   value = d.get("k") or default
来源：http://hz.xuetiantiany.cn/gtvuigtoqn.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yonumen.top/gtncgkkitq.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ywan-chungtsiang.top/gtxzhfsjud.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ybcxt.top/gtgjrnjxcj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.xinyue.icu/gthxbuxrnb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.daxiang520.top/gtogslzdpz.html

Ruby: d&.dig(:a, :b)
来源：http://hz.dianchejie.cn/gtgltigjrj.html

C#:   obj?.A?.B ?? default
来源：http://hz.jlsjyb.cn/gtatcrxjdc.html

[H07] 断言
来源：http://hz.xingfuxueyuan.xyz/gtybqcwsog.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yj20258.top/gtbqvobhyd.html

PHP:  assert($x > 0);
来源：http://hz.jinqigufen.top/gtcibfyksi.html

JS:   console.assert(x > 0);
来源：http://hz.chenjidiqi.icu/gtqmwrahsh.html

TS:   console.assert(x > 0);
来源：http://hz.mhx1999.top/gtduazjyit.html

Java: assert x > 0 : "必须为正";
来源：http://hz.wangdashe.top/gtcglytymz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yvedp.cn/gtvqfnthrl.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.xuetiantiany.cn/gtpdotpcpu.html

C#:   Debug.Assert(x > 0);
来源：http://hz.0kj1m.cn/gtwigaczbg.html

[H08] 获取错误信息与堆栈
来源：http://hz.cdnleiting.top/gtbldymbzm.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zycfv.cn/gtvezlbort.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.fzhhl.top/gtpaehduvy.html

JS:   e.message;  e.stack
来源：http://hz.yangfankeji.com/gtspjhweqw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yuxming.cn/gtwtftyuyx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yueranfly.top/gtggeyfsmn.html

Go:   err.Error()
来源：http://hz.jqgfzy.top/gttxfnhnaq.html

Ruby: e.message;  e.backtrace
来源：http://hz.shuidangran.top/gtebhlawyx.html

C#:   e.Message;  e.StackTrace
来源：http://hz.sufxvd.cn/gtxjyegwvu.html

[H09] 带错误码的异常
来源：http://hz.cdnleiting.top/gtrithrirb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.haohaochexian.top/gtyfxfmjsc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jqgufenzy.top/gtkbceowea.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yanxiufei.cn/gtvfhyynwo.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.kuanghao11.cn/gtajlshbzc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yj202588.top/gtkduaogns.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.birdmap.top/gtyhjsnmus.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.iojbl.cn/gtjsadrkqn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.tanke756.top/gtyeuyjzfy.html

[H10] 资源自动释放
来源：http://hz.yueranfly.top/gtcqmzrnmd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hysaishi.cn/gtzfsnrspj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zhoulong.xyz/gtyzqhlepd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ydjk.org.cn/gtekbnjnyl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.birdmap.top/gtthvalspr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yj20258888.top/gtncrqmzsf.html

Go:   defer f.Close()
来源：http://hz.wangshuangyany.cn/gtxoyxtagg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yueranfly.top/gtxhyyzvcs.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hywenlv.cn/gtbarysdkc.html

================================================================================
来源：http://hz.yj20258888.top/gtfjsjaodl.html

I. 正则表达式
来源：http://hz.iojbl.cn/gtikcvjthb.html

================================================================================
来源：http://hz.hysaishi.cn/gtjhzhuqxq.html

[I01] 判断是否匹配
来源：http://hz.chenjidiqi.icu/gtyztohugu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.dianchejie.cn/gtjifabwen.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.xylfe.cn/gtzlwxxkwq.html

JS:   /\d+/.test(s)
来源：http://hz.tianlin.xyz/gtpqmaukdi.html

TS:   /\d+/.test(s)
来源：http://hz.ydzc1.top/gtseawinvt.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ivvv.top/gtzenwjibo.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.guannengcc.top/gtfvnmkrhb.html

Ruby: s.match?(/\d+/)
来源：http://hz.sysykeji.top/gtuebwicrz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.shanyushiyangtech.top/gtzhiybtjq.html

[I02] 提取所有匹配
来源：http://hz.guowangkeji.top/gtdcdxthqy.html

Py:   re.findall(r"\d+", s)
来源：http://hz.dianchejie.cn/gtsokzktld.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hysaishi.cn/gtxknuzhep.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xuetiantiany.cn/gtvbsfrzah.html

TS:   s.match(/\d+/g)
来源：http://hz.jlsjyb.cn/gtexelyqjq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.wangdashe.top/gtkmaikfam.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.cqqwz.cn/gtoxgwvyrb.html

Ruby: s.scan(/\d+/)
来源：http://hz.sxryk.cn/gtkgoiidsk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xuanzx.com/gtnlwqulyc.html

[I03] 提取捕获分组
来源：http://hz.shanyushiyangkeji.top/gtwpjbvofk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.tanke756.top/gtlboanznq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.316326.xyz/gtstqmqphd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.c1oappe.top/gtvszuehed.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.fzhhl.top/gtafsotjuh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.tian-w.cn/gtiifvqtnu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ydzc1.top/gtcyzyqlmw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ivvv.top/gttszfmbjm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.tanke756.top/gtpqjxzowq.html

[I04] 正则替换
来源：http://hz.bjfxy.top/gtugjhaykb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.andypj.xyz/gtxxbgrrgh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.wangdashe.top/gtgcdaasea.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.pycfn.com/gtlvzvwioi.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhixingplan.top/gtdijdmkrl.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jianghu66.top/gtbdugyymj.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhongyouzk.top/gtpjiroonf.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jlsjyb.cn/gtkouogcft.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.andypj.xyz/gtbipbrcdt.html

[I05] 按正则拆分
来源：http://hz.hammf.cn/gtvdhedfsy.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.mhx1999.top/gtclessnhh.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.aibaodan.cn/gtfihfxlid.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.aizwys.cn/gtbvowhbhu.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jianghu66.top/gtgahckeej.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xingfuxueyuan.xyz/gtradcmhcz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhijiandao.cn/gtvdqpgvmi.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ydzc1.top/gtlnouvfgq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.0kj1m.cn/gtcrpbevbs.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.meibo888.top/gtunbjndbi.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.52xcode.cn/gtgjlgzevd.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hnqzz.top/gtqfcxjcnt.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ivvv.top/gtbxcuctek.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ppjwa.cn/gtcbpwltoh.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.xingfuxueyuan.xyz/gtmobnrwet.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.sxryk.cn/gtgfwnqnkj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.cheryme.top/gtpwzdmlty.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yvedp.cn/gtvktzehqc.html

[I07] 忽略大小写与多行模式
来源：http://hz.jinqigufen.top/gtbkswcyxn.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.9152youxi.cn/gtfwruztjw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhengqikj.top/gtjlgdvwds.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.dianchejie.cn/gtzulumfah.html

TS:   /error/gim
来源：http://hz.birdmap.top/gtkjsaswgz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.xuanzx.com/gtdohoexdo.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhaomingkeji.xyz/gttzwymjlk.html

Ruby: s.scan(/error/i)
来源：http://hz.zycfv.cn/gtbixomqpq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jinghuilouyu.cn/gtrqwcsvgj.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yangfankeji.com/gtfcvjkmna.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jinyuanbaomall.cn/gtasknfzsr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ybcxt.top/gtdzhcyhtu.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.feifeiyinyue.top/gthhyshfef.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hammf.cn/gtnmbxfycn.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hongshengwenyu.top/gtbnttenfh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.kuanghao11.cn/gtnwahdpia.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.sweek.top/gtyvhqosqr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.shanyushiyangkeji.top/gtulqywbdx.html

================================================================================
来源：http://hz.yongpay.top/gttpjivzvu.html

J. 日期与时间
来源：http://hz.shanyushiyangtech.top/gtlkwdkcsp.html

================================================================================
来源：http://hz.daria6918.cn/gtjzsgflvz.html

[J01] 获取当前时间
来源：http://hz.cqqwz.cn/gtjtikukbw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hfpthk.cn/gtiedusaig.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.vqdsnc.cn/gtkfgviksg.html

JS:   new Date();  Date.now()
来源：http://hz.yanxiufei.cn/gtgindampl.html

TS:   new Date();  Date.now()
来源：http://hz.cashguo.top/gtvgzjskxh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ivvv.top/gtwhnghdfj.html

Go:   time.Now()
来源：http://hz.xinyue.icu/gtlhydjvdw.html

Ruby: Time.now
来源：http://hz.ydzc1.top/gtxqspxrsc.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.cqqwz.cn/gtresnnktd.html

[J02] 格式化输出
来源：http://hz.guannengcc.top/gtoiwypsla.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cheryme.top/gtiwcamxsd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.quarkkingdee.top/gtjlmosoqt.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.9152youxi.cn/gtmhpwysgg.html

TS:   d.toISOString()
来源：http://hz.hammf.cn/gtgfhunimr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.pengpengdd.cyou/gtcsjvyaeh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yvedp.cn/gtcsbmvjhs.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shanyushiyangkeji.top/gtrkchkibl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.shzxlz.cn/gttmvzhndx.html

[J03] 字符串解析为日期
来源：http://hz.sysykeji.top/gthvhgopmt.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhengqikj.top/gtnquqlrcq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.c1oappe.top/gthazzcuot.html

JS:   new Date("2024-01-02")
来源：http://hz.jinqigufen.top/gtoaycyhyn.html

TS:   new Date("2024-01-02")
来源：http://hz.daxiang520.top/gtmyqkzjir.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.guannengcc.top/gtretzkzda.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.chenjidiqi.icu/gtxcolxboe.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yonumen.top/gtjafelzxc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.cqqwz.cn/gtckuckrob.html

[J04] 时间戳与日期互转
来源：http://hz.birdmap.top/gtuauujxqu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.fengsongda.top/gtmcsrfeso.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhongyouzk.top/gtgyzfokua.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yuanzhike.top/gtovdpsmmp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.quarkkingdee.top/gtewrmqnvz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jqgufenzy.top/gtfeoybzoc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.vqdsnc.cn/gtazzybkij.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jinqigufen.top/gtkijuovfp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jyoumei.cn/gtlhrxpmpq.html

[J05] 时间加减（加 7 天）
来源：http://hz.shuidangran.top/gtgoefflbf.html

Py:   now + timedelta(days=7)
来源：http://hz.316326.xyz/gtejfyynbq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.sufxvd.cn/gtllbbaryu.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nwbrower.top/gtdeimntss.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhengqikj.top/gtznczabht.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.chenlongwang.top/gtulnlhvhf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.daxiang520.top/gtihjtqxoo.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hammf.cn/gtuwcrytwe.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.hysaishi.cn/gthszdbbcn.html

[J06] 计算两时间之差
来源：http://hz.tian-w.cn/gtlodlbnar.html

Py:   (end - start).total_seconds()
来源：http://hz.yvedp.cn/gtlnenpnbe.html

PHP:  $end->diff($start)->days;
来源：http://hz.hammf.cn/gtjtwcrtun.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.aizwys.cn/gtekhenvuu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yanxiufei.cn/gtyarsozgg.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hnqzz.top/gtxlsvqqay.html

Go:   end.Sub(start).Hours()
来源：http://hz.hnqzz.top/gtmacluprw.html

Ruby: end - start                 # 返回秒数
来源：http://hz.andypj.xyz/gtkysoolzg.html

C#:   (end - start).TotalSeconds
来源：http://hz.redwolf501.top/gtbidpuhfd.html

[J07] 比较两个日期
来源：http://hz.shangyingyoupin.top/gtirvfecwr.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zdqjudy.top/gtkeaqchhq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.dashuyun.cn/gtcduhfpzg.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jiagoushi.top/gtjmvltron.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.nanxinkj.top/gtlzhqnvlg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.shuidangran.top/gtastfyztb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhijiandao.cn/gtpbipbass.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hongshengwenyu.top/gtdtnijjsn.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jinqigfzy.top/gtohvpmkvu.html

[J08] 提取年月日与星期
来源：http://hz.jinyuanbaomall.cn/gtbusnkcpa.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.gotoacloud.top/gtopkqnymf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hywenlv.cn/gtuoiiwlxc.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.cdnleiting.top/gtwiltfzot.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.sysykeji.top/gtaxnfmxsr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ydjk.org.cn/gtesliijrm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zycfv.cn/gtnqxyfcsr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.haohaochexian.top/gtpnjchegf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yj20258.top/gtsfrjljzt.html

[J09] 时区处理
来源：http://hz.havefunace.top/gtrxluolms.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zhijiandao.cn/gtwcmdltkb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jqgfzy.top/gtyftknjmd.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhaomingkeji.xyz/gtfjtrimtu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hywenlv.cn/gtyvllmlwj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ehwqpu.com/gtdloyjczv.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.sysykeji.top/gtmwesjpqs.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.mhx1999.top/gtjvumwbtq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.gotoacloud.top/gtnwzsgmgz.html

[J10] 取今天 / 本月第一天
来源：http://hz.zycfv.cn/gtiykjrhji.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zycfv.cn/gthxpyabxa.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.shuidangran.top/gtxcievedr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yj20258888.top/gtbotxzvns.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.andypj.xyz/gtlxwndyko.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.fzhhl.top/gtqykgxfkj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hfpthk.cn/gtnqnmjemc.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.gotoacloud.top/gtfhotlxhq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.mhx1999.top/gtcdvafqrf.html

================================================================================
来源：http://hz.yonumen.top/gtynzpggdh.html

K. JSON 与序列化
来源：http://hz.yongpay.top/gtygxvtwjr.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gthjhvejpd.html

[K01] 对象转 JSON 字符串
来源：http://hz.yueranfly.top/gthtwxstys.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yangfankeji.com/gtkzhksgjj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xingfuxueyuan.xyz/gtslpmunwg.html

JS:   JSON.stringify(obj)
来源：http://hz.xylfe.cn/gtfapqgedl.html

TS:   JSON.stringify(obj)
来源：http://hz.yonumen.top/gtruoiwses.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.dianchejie.cn/gtopqqlqln.html

Go:   json.Marshal(obj)
来源：http://hz.jinghuilouyu.cn/gtivqdnxrn.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jqgfzy.top/gtodwuttin.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.quarkkingdee.top/gtyibkonjw.html

[K02] JSON 字符串转对象
来源：http://hz.svipenyu.cn/gtqycxapke.html

Py:   json.loads(s)
来源：http://hz.jinqigufen.top/gtvzgfddgr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.shzxlz.cn/gtwexcnebw.html

JS:   JSON.parse(s)
来源：http://hz.zycfv.cn/gtyfbvlxvg.html

TS:   JSON.parse(s)
来源：http://hz.yonumen.top/gtzorddumz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.bjfxy.top/gtkifsluev.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hysaishi.cn/gtfummsade.html

Ruby: JSON.parse(s)
来源：http://hz.zhixingplan.top/gtpeuusclr.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hnxiangtu.top/gtuxxgenel.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.wangdashe.top/gtrvvitwmg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.nwbrower.top/gtgvodntnp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.shanyushiyangtech.top/gtgcniixkb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.nanxinkj.top/gtgzznfnmh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhixingplan.top/gtpawifghx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zhaomingkeji.xyz/gteiedsigu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.shanyushiyangtech.top/gtemkcndlo.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.shanyushiyangkeji.top/gtyhzmqsrk.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ivvv.top/gtznbtpgxp.html

[K04] 读取 JSON 文件
来源：http://hz.birdmap.top/gthrmtpyuc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ehwqpu.com/gtaqgcsjak.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhaomingkeji.xyz/gtnhyjykat.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.redwolf501.top/gtetaqshnv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.0kj1m.cn/gtmfwkqjmk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yonumen.top/gthkccclkr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hammf.cn/gtvewhfafx.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.gaohongyu789.top/gtedwrcygv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.cashguo.top/gtifnxmazb.html

[K05] 深拷贝对象
来源：http://hz.xylfe.cn/gtmxvrjuqd.html

Py:   copy.deepcopy(obj)
来源：http://hz.316326.xyz/gtjkwasxhm.html

PHP:  unserialize(serialize($obj));
来源：http://hz.xylfe.cn/gtbazfjccc.html

JS:   structuredClone(obj)
来源：http://hz.nwbrower.top/gtlexwzpsv.html

TS:   structuredClone(obj)
来源：http://hz.yuxming.cn/gtvvcmtixg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhaomingkeji.xyz/gtjrdngeam.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yuanzhike.top/gtzwnbdhzx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.cqqwz.cn/gtuqwziyha.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.pycfn.com/gtjpmniuxs.html

[K06] 解析 URL 查询串
来源：http://hz.tanke756.top/gtcuhelfla.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.daxiang520.top/gtnyxvtftz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.tian-w.cn/gtppldyhba.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.guannengcc.top/gtljlkpxve.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ehwqpu.com/gthmlppxsy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zycfv.cn/gtamwghing.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.shanyushiyangtech.top/gtahyeggdm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.gotoacloud.top/gtlgtfklvs.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.fengsongda.top/gtaupwohzp.html

[K07] 进制转换
来源：http://hz.jianghu66.top/gtkhhthnnz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.sweek.top/gtpfofujqk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhaomingkeji.xyz/gtfisyatkh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zdqjudy.top/gtsajqybbh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.nwbrower.top/gtkgifiann.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xinyue.icu/gtvfzagujo.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jyoumei.cn/gtaoqrgoci.html


<!-- 参考信息 -->