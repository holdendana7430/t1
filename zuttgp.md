代发 wailian999

Py:   value = d.get("k") or default
来源：http://hz.nanxuanxn.top/gtnygkgceb.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yuanzhike.top/gtzygcmeao.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zhaomingkeji.xyz/gtphnhhzcy.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.shuidangran.top/gtzjkrdwyl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yuxming.cn/gtwziebrla.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.vqdsnc.cn/gtofgdzknw.html

Ruby: d&.dig(:a, :b)
来源：http://hz.snrcjt.cn/gtexdficxf.html

C#:   obj?.A?.B ?? default
来源：http://hz.guannengcc.top/gtybqkrfqi.html

[H07] 断言
来源：http://hz.cucudq.cn/gtaudktqfj.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yj202588.top/gtjzkpgovh.html

PHP:  assert($x > 0);
来源：http://hz.zhoulong.xyz/gtkmzjjjtf.html

JS:   console.assert(x > 0);
来源：http://hz.shzxlz.cn/gtphiyzyno.html

TS:   console.assert(x > 0);
来源：http://hz.tianlin.xyz/gtfmcwtghb.html

Java: assert x > 0 : "必须为正";
来源：http://hz.sysykeji.top/gtndaqvwlu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.sxryk.cn/gtjknkxwms.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.quarkkingdee.top/gtaxxzpaeq.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhoulong.xyz/gtjtuuatrk.html

[H08] 获取错误信息与堆栈
来源：http://hz.snrcjt.cn/gtloukkvni.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yj202588.top/gtvlltewdu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jinyuanbaomall.cn/gtqqjvomvc.html

JS:   e.message;  e.stack
来源：http://hz.nanxuanxn.top/gttkteqcra.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yuanzhike.top/gttermiufx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jqgufenzy.top/gtgpwysmuh.html

Go:   err.Error()
来源：http://hz.shzxlz.cn/gtmacukxdm.html

Ruby: e.message;  e.backtrace
来源：http://hz.ywan-chungtsiang.top/gtumuyalmb.html

C#:   e.Message;  e.StackTrace
来源：http://hz.sxryk.cn/gtnkqobwev.html

[H09] 带错误码的异常
来源：http://hz.ivvv.top/gtgucozalh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.nanxinkj.top/gtuolxeafx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hnxiangtu.top/gtxrxtxwpj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.quarkkingdee.top/gtlquwueag.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.kuanghao11.cn/gtnisdqofu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.feifeiyinyue.top/gtmfkfjrel.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.haohaochexian.top/gtljlqesru.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.wangshuangyany.cn/gtfetorqnz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhaomingkeji.xyz/gtfdsxdbwx.html

[H10] 资源自动释放
来源：http://hz.hysaishi.cn/gtqgyeqswk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hammf.cn/gthsqupclr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.kuanghao11.cn/gtewmkyxhe.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xylfe.cn/gtzfukxgjc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yangfankeji.com/gtnocotelr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.mhx1999.top/gtxoqbetvu.html

Go:   defer f.Close()
来源：http://hz.zhiwuduotai.top/gtbselosrw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zhengqikj.top/gtoehwwdul.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.sysykeji.top/gtldjmkxow.html

================================================================================
来源：http://hz.cheryme.top/gtdacmrufi.html

I. 正则表达式
来源：http://hz.hongshengwenyu.top/gtydblfgst.html

================================================================================
来源：http://hz.ppjwa.cn/gttgblpxgq.html

[I01] 判断是否匹配
来源：http://hz.9152youxi.cn/gtpradvuue.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.meibo888.top/gtloqviejs.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.cashguo.top/gtpkidkdoc.html

JS:   /\d+/.test(s)
来源：http://hz.9152youxi.cn/gtvbpbyjer.html

TS:   /\d+/.test(s)
来源：http://hz.zhengqikj.top/gtzwvosvxi.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.nanxuanxn.top/gtdoptubrz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jqgufenzy.top/gtmnworxsm.html

Ruby: s.match?(/\d+/)
来源：http://hz.xuetiantiany.cn/gtrtczmkll.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hongshengwenyu.top/gthsimjaut.html

[I02] 提取所有匹配
来源：http://hz.tanke756.top/gtajlqtnrq.html

Py:   re.findall(r"\d+", s)
来源：http://hz.tanke756.top/gtgiyqskti.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.chenjidiqi.icu/gtthhfytvs.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.shzxlz.cn/gtxalahvsz.html

TS:   s.match(/\d+/g)
来源：http://hz.svipenyu.cn/gtebbdxira.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.xylfe.cn/gtuxkdjmij.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.sysykeji.top/gtrauwitlx.html

Ruby: s.scan(/\d+/)
来源：http://hz.guowangkeji.top/gtucnqmczy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yangfankeji.com/gthydzcvmc.html

[I03] 提取捕获分组
来源：http://hz.feifeiyinyue.top/gtzfobjprh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhongyouzk.top/gtpupucyao.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zhongyouzk.top/gtbthxeyyc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.kuanghao11.cn/gtbmaysvtq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.birdmap.top/gtbznhzduf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.cdnleiting.top/gtjufzdord.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ehwqpu.com/gtafwugcaj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.pycfn.com/gterddlder.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhongyouzk.top/gtissbdenj.html

[I04] 正则替换
来源：http://hz.jianghu66.top/gtrgteszyo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ydzc1.top/gtmzflfidg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.316326.xyz/gthrxtbtso.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ybcxt.top/gtfmduxaek.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.cqqwz.cn/gtslipoaxp.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yangfankeji.com/gtmfyselwc.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.316326.xyz/gttusikvfo.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jinqigufen.top/gttfyiyewt.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.0kj1m.cn/gtqoocmbvi.html

[I05] 按正则拆分
来源：http://hz.shangyingyoupin.top/gtslwhrnna.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jinqigfzy.top/gtywwkevvd.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ydjk.org.cn/gthnhqscfm.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yonumen.top/gtanenqnsy.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hammf.cn/gttdwuudsv.html

Java: s.split("\\s*,\\s*")
来源：http://hz.guannengcc.top/gtgzsaajzg.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.c1oappe.top/gtiaoyajlz.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.tianlin.xyz/gtxvepvjzv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.chenlongwang.top/gtmcseepvj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.0kj1m.cn/gtmxikgtlm.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhiwuduotai.top/gtkahbxuwm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ybcxt.top/gtywofzzmw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.feifeiyinyue.top/gteotgdvlo.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xylfe.cn/gtieikrqyk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.aizwys.cn/gtqjtlrbpi.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zdqjudy.top/gtwdqhkgwp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hywenlv.cn/gtlriwoung.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yuanzhike.top/gtomdhfbqp.html

[I07] 忽略大小写与多行模式
来源：http://hz.pengpengdd.cyou/gtbeszehex.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.shzxlz.cn/gtizqpbujo.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jianghu66.top/gtejykfwml.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yuxming.cn/gtcbxsknbc.html

TS:   /error/gim
来源：http://hz.yuanzhike.top/gtiimhklvk.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhengqikj.top/gtysksmnag.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.sysykeji.top/gthvmgrvos.html

Ruby: s.scan(/error/i)
来源：http://hz.jqgfzy.top/gtmdzhwaif.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ppjwa.cn/gtigelnurh.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.0kj1m.cn/gtcadrpzgb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jqgfzy.top/gtppzanakv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.vqdsnc.cn/gtrmqakhwm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ehwqpu.com/gtuvlmxkrq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinyuanbaomall.cn/gtdcuyepgi.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jianghu66.top/gtbnxpnqhc.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zycfv.cn/gtaubmsjeg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zhongyouzk.top/gtppbhfppn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jqgufenzy.top/gttydnkggo.html

================================================================================
来源：http://hz.hfpthk.cn/gtuipuixfn.html

J. 日期与时间
来源：http://hz.zhongyouzk.top/gtdskfkhth.html

================================================================================
来源：http://hz.ydjk.org.cn/gtkbmueecn.html

[J01] 获取当前时间
来源：http://hz.guowangkeji.top/gtkcpugrqb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.xuanzx.com/gtduiwxuju.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.pycfn.com/gtpvwafdfe.html

JS:   new Date();  Date.now()
来源：http://hz.hnqzz.top/gtulhotryl.html

TS:   new Date();  Date.now()
来源：http://hz.xylfe.cn/gtafuptexl.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ydzc1.top/gthksgkuon.html

Go:   time.Now()
来源：http://hz.ydzc1.top/gtponqivdq.html

Ruby: Time.now
来源：http://hz.cucudq.cn/gtpmnlunwo.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.gogol.net.cn/gtsosppytf.html

[J02] 格式化输出
来源：http://hz.zhiwuduotai.top/gtapkdbodb.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.0kj1m.cn/gtkcmtuyhp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yanxiufei.cn/gtcfgzwpuk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hywenlv.cn/gtjoumoyhe.html

TS:   d.toISOString()
来源：http://hz.jqgufenzy.top/gtmhkscjxy.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.haohaochexian.top/gtrapawdrc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.shanyushiyangkeji.top/gtlmwpsdon.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj20258.top/gthotdbadk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hysaishi.cn/gtvbcqcsjw.html

[J03] 字符串解析为日期
来源：http://hz.jinyuanbaomall.cn/gteyjwqpnx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhiwuduotai.top/gtwqeqfbgv.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.sweek.top/gtpdalyucq.html

JS:   new Date("2024-01-02")
来源：http://hz.chenjidiqi.icu/gtbdxqtqtg.html

TS:   new Date("2024-01-02")
来源：http://hz.yonumen.top/gtduirdvdw.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhijiandao.cn/gtzgyiiiay.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.52xcode.cn/gtwwvdjupw.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yongpay.top/gtzugoqnqz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xingfuxueyuan.xyz/gttegdwnhs.html

[J04] 时间戳与日期互转
来源：http://hz.sufxvd.cn/gtfrpsvfia.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.chenlongwang.top/gtzcdkpixn.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.cdnleiting.top/gtjdkshcdk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.haohaochexian.top/gtnxozdpwp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zhengqikj.top/gtbduwlqgx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.sufxvd.cn/gtgavdqthi.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.gotoacloud.top/gtcrqdjbba.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.pycfn.com/gtuspcsgwi.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.sufxvd.cn/gtsuvuikup.html

[J05] 时间加减（加 7 天）
来源：http://hz.guowangkeji.top/gtfeqjkluq.html

Py:   now + timedelta(days=7)
来源：http://hz.bjfxy.top/gtnvzejavs.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jqgufenzy.top/gtwfcvbxhb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.smart0.xyz/gtmsgpkbrm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhiwuduotai.top/gtndaqrsoy.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hfpthk.cn/gtbqxcpanu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ywan-chungtsiang.top/gtuofwtslo.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zdqjudy.top/gtlcsgcybd.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.mhx1999.top/gtpfajgjab.html

[J06] 计算两时间之差
来源：http://hz.zdqjudy.top/gtpsjcujaj.html

Py:   (end - start).total_seconds()
来源：http://hz.jinyuanbaomall.cn/gtyzvfdglo.html

PHP:  $end->diff($start)->days;
来源：http://hz.yvedp.cn/gtyoohfpbf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.xuetiantiany.cn/gtexuyjuvr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yangfankeji.com/gtvwfwyubt.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yvedp.cn/gtdrspprxu.html

Go:   end.Sub(start).Hours()
来源：http://hz.jiagoushi.top/gtqbohudqf.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hongshengwenyu.top/gtxorqwrxp.html

C#:   (end - start).TotalSeconds
来源：http://hz.fengsongda.top/gtslzhnvst.html

[J07] 比较两个日期
来源：http://hz.fengsongda.top/gtknjgrpid.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.shzxlz.cn/gtxklhnufa.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.aibaodan.cn/gttowludau.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.feifeiyinyue.top/gtmrkeetix.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.smart0.xyz/gtzsikjpey.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.nanxuanxn.top/gtevtedvxv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.wangshuangyany.cn/gtsfffdgzg.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ivvv.top/gtsozbaflf.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.feifeiyinyue.top/gthvfxjlnt.html

[J08] 提取年月日与星期
来源：http://hz.aizwys.cn/gtpmiyayai.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.cdnleiting.top/gthrogkdfs.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xingfuxueyuan.xyz/gtedddpysi.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.sweek.top/gtqkfuofma.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.bjfxy.top/gtprvctywu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.316326.xyz/gtdcjgsatr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.xingfuxueyuan.xyz/gthksxkdxf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.snrcjt.cn/gtpvnevtcv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.quarkkingdee.top/gtduximeuo.html

[J09] 时区处理
来源：http://hz.ppjwa.cn/gterjowrci.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.iojbl.cn/gtyucwsxkg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yueranfly.top/gtyrruvzlj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj20258.top/gtcrpvynkh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hnxiangtu.top/gtgeenrljj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.dashuyun.cn/gtcukwbset.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.andypj.xyz/gtzuolxtbu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.316326.xyz/gtenbrrjxg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.gzhubu.top/gtvnhwlrhq.html

[J10] 取今天 / 本月第一天
来源：http://hz.sufxvd.cn/gtejzcomfa.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ehwqpu.com/gthwxkgkrk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.gotoacloud.top/gtnoowssdx.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jinqigufen.top/gtxkngmiof.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hywenlv.cn/gtictgsorx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.hywenlv.cn/gtactsdtgc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jinqigfzy.top/gtriwenctk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.bjfxy.top/gtvmubyano.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jinqigfzy.top/gtawogcpuw.html

================================================================================
来源：http://hz.0kj1m.cn/gtvodncaee.html

K. JSON 与序列化
来源：http://hz.daria6918.cn/gtruotgomz.html

================================================================================
来源：http://hz.jianghu66.top/gtdksniddz.html

[K01] 对象转 JSON 字符串
来源：http://hz.cqqwz.cn/gtfqlpkido.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.sysykeji.top/gtqjbxuhfp.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.pengpengdd.cyou/gtmbzlazlr.html

JS:   JSON.stringify(obj)
来源：http://hz.shzxlz.cn/gtjguejehc.html

TS:   JSON.stringify(obj)
来源：http://hz.316326.xyz/gtgdimdfva.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jianghu66.top/gtssmtvzyr.html

Go:   json.Marshal(obj)
来源：http://hz.yonumen.top/gtgukzxtzu.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jinqigfzy.top/gtxismrfyc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.chenjidiqi.icu/gtncozviyz.html

[K02] JSON 字符串转对象
来源：http://hz.jqgfzy.top/gtqqhgiqwx.html

Py:   json.loads(s)
来源：http://hz.cqqwz.cn/gtdrvjepln.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.feifeiyinyue.top/gtcsymypyq.html

JS:   JSON.parse(s)
来源：http://hz.snrcjt.cn/gthkhlgkbc.html

TS:   JSON.parse(s)
来源：http://hz.andypj.xyz/gtvrxefkav.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.0kj1m.cn/gtvqdkmbjf.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.birdmap.top/gtefwabjnh.html

Ruby: JSON.parse(s)
来源：http://hz.tianlin.xyz/gtuzksxkpu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.nanxuanxn.top/gtnlprwkjc.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.nanxuanxn.top/gtpbcvmbno.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.52xcode.cn/gtcafujkpo.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.tian-w.cn/gtkcqoxdoc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.sweek.top/gttzwfekuz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.daria6918.cn/gtptdrgjwk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yonumen.top/gtqgitsatj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.gogol.net.cn/gtmfsobxii.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yueranfly.top/gtafqpfnwd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.guannengcc.top/gtsswehncb.html

[K04] 读取 JSON 文件
来源：http://hz.ydzc1.top/gteowlxvfy.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.sufxvd.cn/gtsynwimva.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jqgfzy.top/gtdkljxyll.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xinyue.icu/gtmdkthgtt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yongpay.top/gtowltgvsg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.daria6918.cn/gtmboutkeb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.kuanghao11.cn/gtvnfaabwy.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhengqikj.top/gtuppsyejw.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ivvv.top/gtvitjrpob.html

[K05] 深拷贝对象
来源：http://hz.cqqwz.cn/gttyjaunnq.html

Py:   copy.deepcopy(obj)
来源：http://hz.yonumen.top/gtilxadtwt.html

PHP:  unserialize(serialize($obj));
来源：http://hz.9152youxi.cn/gtvgzemess.html

JS:   structuredClone(obj)
来源：http://hz.iojbl.cn/gtkemrezqw.html

TS:   structuredClone(obj)
来源：http://hz.kuanghao11.cn/gtpobbvxaj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hnxiangtu.top/gtwkohbvxv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.gogol.net.cn/gtatoxglak.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.dianchejie.cn/gtkcqjvife.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.andypj.xyz/gtbaabnojo.html

[K06] 解析 URL 查询串
来源：http://hz.sysykeji.top/gtgalcjpll.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jqgufenzy.top/gtvvkbjlti.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jinyuanbaomall.cn/gtfvtyiush.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhiwuduotai.top/gtrktcfvoh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cheryme.top/gtlqbtprda.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yj20258.top/gtwurbpyck.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.fengsongda.top/gteibupola.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.chenjidiqi.icu/gtyhttdcfg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jinqigfzy.top/gtvenjqxmf.html

[K07] 进制转换
来源：http://hz.xylfe.cn/gtqzlthumx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.nanxuanxn.top/gtvbpwufmn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yj202588.top/gtsuahhwyl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.9152youxi.cn/gtpmckship.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yangfankeji.com/gtymxqakrn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ppjwa.cn/gtgoqissoh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhoulong.xyz/gttszlqjpd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ppjwa.cn/gtqtahyflm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.iojbl.cn/gtwgryrhrt.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yongpay.top/gtqrfewbzo.html

Py:   pickle.dumps(obj)
来源：http://hz.xuanzx.com/gtpszrosxg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zhengqikj.top/gtskiqowou.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shanyushiyangtech.top/gtwozfbnzm.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.birdmap.top/gtgmxsernp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.52xcode.cn/gtzaaltbtu.html

Go:   encoding/gob
来源：http://hz.vqdsnc.cn/gtfqecsabd.html

Ruby: Marshal.dump(obj)
来源：http://hz.yonumen.top/gtpqecoebd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.chenzaomai.com/gtpuzsqttz.html

================================================================================
来源：http://hz.zhijiandao.cn/gtcghrpcaz.html

L. 网络请求
来源：http://hz.cucudq.cn/gtfiqhbhlo.html

================================================================================
来源：http://hz.yj20258888.top/gtsznwdorz.html

[L01] 发送 GET 请求
来源：http://hz.zycfv.cn/gtylcbprns.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yuxming.cn/gtkqzeojsf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.vqdsnc.cn/gtydvmdpoa.html

JS:   await fetch(url)
来源：http://hz.ydjk.org.cn/gtgnnkypkx.html

TS:   await fetch(url)
来源：http://hz.zhongyouzk.top/gtjnqqfcxn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.cheryme.top/gtmzrdlnzy.html

Go:   resp, err := http.Get(url)
来源：http://hz.yueranfly.top/gtwlgaohgq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.sxryk.cn/gthnzxsbqk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.shangyingyoupin.top/gthawsxtdp.html

[L02] 发送 POST JSON
来源：http://hz.jyoumei.cn/gtwopglchh.html


<!-- 参考信息 -->