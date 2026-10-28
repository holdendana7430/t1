代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jqgufenzy.top/gtggbabxxf.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xingfuxueyuan.xyz/gtzepnuhdq.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.nanxuanxn.top/gtsufulykj.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.quarkkingdee.top/gtkivdwqot.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hnxiangtu.top/gtxojnsnuh.html

Ruby: rescue ArgumentError => e
来源：http://hz.aibaodan.cn/gtodppiott.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.dashuyun.cn/gtqiljqwyv.html

[H06] 可选值 / 空值安全访问
来源：http://hz.gaohongyu789.top/gtihnhtwwx.html

Py:   value = d.get("k") or default
来源：http://hz.aizwys.cn/gtqrsiowfs.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.tian-w.cn/gtwesurxgo.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xinyue.icu/gtlpdlcgmg.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.daxiang520.top/gtuomqpnbt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.quarkkingdee.top/gtjhmctexr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.nanxuanxn.top/gtleomfwby.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jlsjyb.cn/gtobbwvglp.html

C#:   obj?.A?.B ?? default
来源：http://hz.ehwqpu.com/gtvuphyvar.html

[H07] 断言
来源：http://hz.aibaodan.cn/gttctzqkgl.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yangfankeji.com/gtxdebgkdh.html

PHP:  assert($x > 0);
来源：http://hz.52xcode.cn/gtjwrvhjna.html

JS:   console.assert(x > 0);
来源：http://hz.xuetiantiany.cn/gtnjnkzlec.html

TS:   console.assert(x > 0);
来源：http://hz.zhiwuduotai.top/gtlmskfnyf.html

Java: assert x > 0 : "必须为正";
来源：http://hz.hnqzz.top/gtbvfxrvqg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zdqjudy.top/gtdejitryz.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.316326.xyz/gtgvjswqop.html

C#:   Debug.Assert(x > 0);
来源：http://hz.hnqzz.top/gtmluhuyjo.html

[H08] 获取错误信息与堆栈
来源：http://hz.ybcxt.top/gtpsiaamwl.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jyoumei.cn/gtcwyrqovy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.nanxinkj.top/gtycgpvhuy.html

JS:   e.message;  e.stack
来源：http://hz.guannengcc.top/gtdcszteca.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.tianlin.xyz/gtzgibnlzt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.chenjidiqi.icu/gtkpxvvehz.html

Go:   err.Error()
来源：http://hz.pycfn.com/gtyhgqwaco.html

Ruby: e.message;  e.backtrace
来源：http://hz.cheryme.top/gtvljkynny.html

C#:   e.Message;  e.StackTrace
来源：http://hz.fengsongda.top/gtrqbozwtr.html

[H09] 带错误码的异常
来源：http://hz.daxiang520.top/gtyuobpvny.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.guowangkeji.top/gtaihrasbn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.gotoacloud.top/gtzmoogvjk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhongyouzk.top/gtorlaqady.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yangfankeji.com/gtleokgoyu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ivvv.top/gtmwcddryk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhengqikj.top/gtiselhilz.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yueranfly.top/gtugmcvmaw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hongshengwenyu.top/gtqhmojpgi.html

[H10] 资源自动释放
来源：http://hz.guowangkeji.top/gtsxwvvpmy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.daxiang520.top/gtmikmojnu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.iojbl.cn/gtkflgdcec.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.9152youxi.cn/gthabezjbe.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xylfe.cn/gtmruknoir.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jianghu66.top/gtflugobug.html

Go:   defer f.Close()
来源：http://hz.fzhhl.top/gtbmvxngqe.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.ivvv.top/gttbdnekvv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.snrcjt.cn/gtqzcjxlzm.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtujjafmtn.html

I. 正则表达式
来源：http://hz.andypj.xyz/gtsnuxzwas.html

================================================================================
来源：http://hz.ivvv.top/gtcangiwpy.html

[I01] 判断是否匹配
来源：http://hz.quarkkingdee.top/gtztekxyfc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.shzxlz.cn/gtcvzwvgid.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.cdnleiting.top/gtzjfpldnx.html

JS:   /\d+/.test(s)
来源：http://hz.xuetiantiany.cn/gtgtglnnpr.html

TS:   /\d+/.test(s)
来源：http://hz.haohaochexian.top/gtxfaebgws.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.0kj1m.cn/gtvrpbgbwf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ywan-chungtsiang.top/gtnngsleqv.html

Ruby: s.match?(/\d+/)
来源：http://hz.bjfxy.top/gtbcvvvhmr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.cqqwz.cn/gtkyggsshi.html

[I02] 提取所有匹配
来源：http://hz.tianlin.xyz/gtrlzytmny.html

Py:   re.findall(r"\d+", s)
来源：http://hz.316326.xyz/gtuanvmhlu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.fzhhl.top/gtbjbqstwe.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.fengsongda.top/gtamlfkdxc.html

TS:   s.match(/\d+/g)
来源：http://hz.cashguo.top/gtzaaykqzq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.pengpengdd.cyou/gtaskdxxrs.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.cdnleiting.top/gtwylsqtgt.html

Ruby: s.scan(/\d+/)
来源：http://hz.ehwqpu.com/gtorjlkujc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.c1oappe.top/gturgygdow.html

[I03] 提取捕获分组
来源：http://hz.sufxvd.cn/gtkzlslxvw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yanxiufei.cn/gtltniccaw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.sysykeji.top/gtgyllsrvg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ybcxt.top/gtymauujix.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hywenlv.cn/gtyczibimv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yuanzhike.top/gtleiuunlj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.havefunace.top/gttiqpidff.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.pycfn.com/gthrffibef.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.hongshengwenyu.top/gtugnwppor.html

[I04] 正则替换
来源：http://hz.xuetiantiany.cn/gtnqpfrexr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hammf.cn/gtnwphziho.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.0kj1m.cn/gtujpqcuvi.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zhijiandao.cn/gtseuxgzyj.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.sufxvd.cn/gtnvvuhpzo.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.daxiang520.top/gtunqsozsh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.chenzaomai.com/gtcayuesff.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ydzc1.top/gteoayggau.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jqgufenzy.top/gtrnkoanup.html

[I05] 按正则拆分
来源：http://hz.quarkkingdee.top/gtltvfwxhg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ivvv.top/gtytlvuwpi.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jyoumei.cn/gtfqiqwtlf.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.nanxinkj.top/gtmnmwwgth.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhixingplan.top/gtwspgyuat.html

Java: s.split("\\s*,\\s*")
来源：http://hz.tian-w.cn/gttywqklvg.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.smart0.xyz/gtvqytcsfo.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.wangdashe.top/gtmdqxskcz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhoulong.xyz/gtjkgopwgg.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.cucudq.cn/gtbxymiuqq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.kuanghao11.cn/gtzblwtesd.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.shanyushiyangkeji.top/gtxiuzzjab.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.daria6918.cn/gtxibampqh.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yueranfly.top/gthkjayeuc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.pycfn.com/gtkmzcnwvg.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.chenlongwang.top/gtrohsnxsb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhixingplan.top/gtsqiwkmvb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.sufxvd.cn/gtjsaaluwo.html

[I07] 忽略大小写与多行模式
来源：http://hz.gotoacloud.top/gtejkukoft.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.shzxlz.cn/gtrdtjrtdo.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xuetiantiany.cn/gttrreuyxb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.shzxlz.cn/gtwpyuvnkr.html

TS:   /error/gim
来源：http://hz.ivvv.top/gthvtlsjdb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.quarkkingdee.top/gtojxnljvv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.tanke756.top/gttjjixiek.html

Ruby: s.scan(/error/i)
来源：http://hz.quarkkingdee.top/gtbgxnoucv.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.aizwys.cn/gtddmvlliu.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.52xcode.cn/gtkmmlzhly.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhongyouzk.top/gtwlcyhnki.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yj202588.top/gtxvhxpdnj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hongshengwenyu.top/gtswfotrto.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yuanzhike.top/gtkwnrtyel.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jqgufenzy.top/gtdoihcsjj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gaohongyu789.top/gtqhdelrep.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shangyingyoupin.top/gtzsqiujoz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.daria6918.cn/gtfxunrrnv.html

================================================================================
来源：http://hz.cqqwz.cn/gtgvtrysvs.html

J. 日期与时间
来源：http://hz.hysaishi.cn/gtafozmtqt.html

================================================================================
来源：http://hz.zhoulong.xyz/gtkbxmblcf.html

[J01] 获取当前时间
来源：http://hz.cqqwz.cn/gtcsraqeqk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.daxiang520.top/gtzaphtgky.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.tianlin.xyz/gtqwbxwnmz.html

JS:   new Date();  Date.now()
来源：http://hz.haohaochexian.top/gtdgidjywd.html

TS:   new Date();  Date.now()
来源：http://hz.hongshengwenyu.top/gtrfngdyro.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.iojbl.cn/gteurzmlir.html

Go:   time.Now()
来源：http://hz.feifeiyinyue.top/gterumjuux.html

Ruby: Time.now
来源：http://hz.hnqzz.top/gtvlncfrsm.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.316326.xyz/gtxwoxbbsu.html

[J02] 格式化输出
来源：http://hz.havefunace.top/gtjjywxwyl.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.iojbl.cn/gtoxndhapl.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.nanxinkj.top/gtqynsujud.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.gogol.net.cn/gtqlbujuwo.html

TS:   d.toISOString()
来源：http://hz.zhongyouzk.top/gtytpaxwlx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.dianchejie.cn/gtckyfkxny.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhongyouzk.top/gtyabeogam.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.dashuyun.cn/gtibgcthsa.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.chenzaomai.com/gtqmymxjlz.html

[J03] 字符串解析为日期
来源：http://hz.hammf.cn/gtluzbdmpq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.shanyushiyangkeji.top/gtknaeooxq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ybcxt.top/gtoplldpas.html

JS:   new Date("2024-01-02")
来源：http://hz.zhaomingkeji.xyz/gtbqchvyix.html

TS:   new Date("2024-01-02")
来源：http://hz.shangyingyoupin.top/gtymvogbja.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.vqdsnc.cn/gtsyavzork.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.bjfxy.top/gtnkgamgzj.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yongpay.top/gtwmbzzhuq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.wangdashe.top/gthprswbey.html

[J04] 时间戳与日期互转
来源：http://hz.hongshengwenyu.top/gttelznqzm.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.9152youxi.cn/gtyzvsmsmu.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hnqzz.top/gtfjiomhbq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.vqdsnc.cn/gtyacyvsro.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.quarkkingdee.top/gtdbzzsfde.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.gzhubu.top/gtlhhxybda.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.nwbrower.top/gtevizyjkg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xuetiantiany.cn/gtomvqvvqf.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ivvv.top/gthbmtzhlr.html

[J05] 时间加减（加 7 天）
来源：http://hz.meibo888.top/gtcifpkrpk.html

Py:   now + timedelta(days=7)
来源：http://hz.zhoulong.xyz/gtajoidvms.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jqgufenzy.top/gtalgmqkhy.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yangfankeji.com/gtbnmhkpmp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jyoumei.cn/gtgohdkfqq.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.pengpengdd.cyou/gtnayyabdf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.gogol.net.cn/gtslegwsrm.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xziqi.cn/gtsdvbhunl.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.wangdashe.top/gtcfidtcpg.html

[J06] 计算两时间之差
来源：http://hz.nanxinkj.top/gtjnengsmv.html

Py:   (end - start).total_seconds()
来源：http://hz.gzhubu.top/gtwfqarmbv.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhengqikj.top/gtjqcbvqat.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhiwuduotai.top/gtuhkudosu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.xziqi.cn/gtpgcbtlkm.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.c1oappe.top/gtukqnkabt.html

Go:   end.Sub(start).Hours()
来源：http://hz.guannengcc.top/gtahmptoav.html

Ruby: end - start                 # 返回秒数
来源：http://hz.kuanghao11.cn/gtpxnhsrfw.html

C#:   (end - start).TotalSeconds
来源：http://hz.shanyushiyangtech.top/gtktcuoloh.html

[J07] 比较两个日期
来源：http://hz.yvedp.cn/gtylnuetjt.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.dianchejie.cn/gtndvqmbpm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.quarkkingdee.top/gtqloaiqty.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.bjfxy.top/gtgxwwtomi.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jinqigufen.top/gtoncqqkro.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.9152youxi.cn/gthjhmsown.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.gaohongyu789.top/gtalsodard.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zycfv.cn/gtcphhxuxb.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ppjwa.cn/gtargddoss.html

[J08] 提取年月日与星期
来源：http://hz.vqdsnc.cn/gtrifxtedd.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.sxryk.cn/gtnnkpjdzg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jiagoushi.top/gtiznpsetr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jqgufenzy.top/gtyrcwzpab.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.fzhhl.top/gtwkhizfss.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jqgufenzy.top/gtegipelwh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jianghu66.top/gtwiihgxrw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.nanxuanxn.top/gtiniqdkqp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.chenlongwang.top/gttmdsnjtw.html

[J09] 时区处理
来源：http://hz.hysaishi.cn/gtayhsaull.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.birdmap.top/gtpxdueopb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.xuanzx.com/gthijldtkt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.chenzaomai.com/gttnhbmoxc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhoulong.xyz/gthvdlrlsa.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhaomingkeji.xyz/gtlzzircua.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.birdmap.top/gtqsaxbhgq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zdqjudy.top/gtpehluhmv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.gzhubu.top/gtzszjcdft.html

[J10] 取今天 / 本月第一天
来源：http://hz.jianghu66.top/gtxfmnvjwv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.mhx1999.top/gtvaphwxom.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.redwolf501.top/gtahwnvyab.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.havefunace.top/gtunvktzrm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.haohaochexian.top/gtkswekujl.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yuxming.cn/gtyvdyciyy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yvedp.cn/gtfinejlmz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.aibaodan.cn/gtqwlcarxb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.haohaochexian.top/gteyppjhfd.html

================================================================================
来源：http://hz.havefunace.top/gtjpfjcmlq.html

K. JSON 与序列化
来源：http://hz.ywan-chungtsiang.top/gtbqewuymq.html

================================================================================
来源：http://hz.havefunace.top/gtqyzhwaqk.html

[K01] 对象转 JSON 字符串
来源：http://hz.gzhubu.top/gttgcqmjbp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shanyushiyangkeji.top/gtgiyxwwqb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.chenlongwang.top/gtoveoqfsu.html

JS:   JSON.stringify(obj)
来源：http://hz.chenzaomai.com/gtzsmeiuty.html

TS:   JSON.stringify(obj)
来源：http://hz.hysaishi.cn/gteeqglkox.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.sxryk.cn/gtaknnmmwv.html

Go:   json.Marshal(obj)
来源：http://hz.andypj.xyz/gtpwoiakse.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cdnleiting.top/gtadlgdrjw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.c1oappe.top/gtblbeccji.html

[K02] JSON 字符串转对象
来源：http://hz.jlsjyb.cn/gtotakfuat.html

Py:   json.loads(s)
来源：http://hz.hfpthk.cn/gtqcqkwpgv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hfpthk.cn/gtkhyqnots.html

JS:   JSON.parse(s)
来源：http://hz.hongshengwenyu.top/gtqipdrvvj.html

TS:   JSON.parse(s)
来源：http://hz.aibaodan.cn/gtoqdfzdvr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.ydjk.org.cn/gtrisjewuy.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.cashguo.top/gthxrubzcn.html

Ruby: JSON.parse(s)
来源：http://hz.chenzaomai.com/gtyhridmmp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.aizwys.cn/gtblhsmody.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.dianchejie.cn/gtlphqvmkk.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.daria6918.cn/gtmevvidrn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.daria6918.cn/gtcwcjueic.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yueranfly.top/gtawavybjr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cqqwz.cn/gtygmuvkxk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hysaishi.cn/gtflbkkpas.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhiwuduotai.top/gtxvqdapul.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhixingplan.top/gtulujanfq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jinqigfzy.top/gtgxubqolc.html

[K04] 读取 JSON 文件
来源：http://hz.dashuyun.cn/gtrejrrfci.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.gaohongyu789.top/gthlzehulk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yj20258888.top/gtozyjmwko.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zycfv.cn/gtsksuubui.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shanyushiyangtech.top/gtmwpduyby.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jinqigfzy.top/gtijkpryun.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhiwuduotai.top/gtxqaclvau.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.birdmap.top/gtjlddrcst.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.wangshuangyany.cn/gtkgaoxrfo.html

[K05] 深拷贝对象
来源：http://hz.pengpengdd.cyou/gtaboauvsg.html

Py:   copy.deepcopy(obj)
来源：http://hz.snrcjt.cn/gtdvwqbzzx.html

PHP:  unserialize(serialize($obj));
来源：http://hz.aibaodan.cn/gtsdrclbfs.html

JS:   structuredClone(obj)
来源：http://hz.52xcode.cn/gtzlbahdnp.html

TS:   structuredClone(obj)
来源：http://hz.jyoumei.cn/gtcpcvdjti.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.gogol.net.cn/gtuzcgpfsg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.chenzaomai.com/gtccsnklta.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.vqdsnc.cn/gtreyjdqub.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.gotoacloud.top/gtvjctxtno.html

[K06] 解析 URL 查询串
来源：http://hz.hywenlv.cn/gtttzvyida.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jqgfzy.top/gtbviffnyk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.quarkkingdee.top/gtihnpladr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shanyushiyangtech.top/gtnwepwarc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.9152youxi.cn/gtxzemguxl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hfpthk.cn/gtlxfcjcva.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.havefunace.top/gtrdjbalxh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.aibaodan.cn/gtuhzaqvuz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.andypj.xyz/gtqysuzwzs.html

[K07] 进制转换
来源：http://hz.yvedp.cn/gtbsjflhsd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yj202588.top/gtetaqspyw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xuanzx.com/gtxjaderqj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.dianchejie.cn/gtemxzywev.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.xuetiantiany.cn/gtsxevtpax.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.aizwys.cn/gtbvnlqfya.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jinqigufen.top/gtnmyvyyts.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jiagoushi.top/gtmynkqoej.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.pycfn.com/gtrakjuqdp.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yj20258.top/gtootrrriu.html

Py:   pickle.dumps(obj)
来源：http://hz.zycfv.cn/gtucykzsbr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yanxiufei.cn/gttyaljskl.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.nanxuanxn.top/gtotsskwxh.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.kuanghao11.cn/gthboqbohe.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.mhx1999.top/gtyqzicfwu.html

Go:   encoding/gob
来源：http://hz.zhiwuduotai.top/gtnhvhgalc.html

Ruby: Marshal.dump(obj)
来源：http://hz.ybcxt.top/gtjlfqddtz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.kuanghao11.cn/gtqnwsjlom.html

================================================================================
来源：http://hz.0kj1m.cn/gtbxabvsvz.html

L. 网络请求
来源：http://hz.ehwqpu.com/gtcorcubgg.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtoqrdmogw.html

[L01] 发送 GET 请求
来源：http://hz.wangshuangyany.cn/gtelwgkibw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zhongyouzk.top/gtbsidzolx.html


<!-- 参考信息 -->