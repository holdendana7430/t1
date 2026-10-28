代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.daria6918.cn/gtahdrfnmg.html

Ruby: rescue ArgumentError => e
来源：http://hz.yvedp.cn/gtzyddgipq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.xylfe.cn/gtnpptksnj.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hnqzz.top/gtqofbemtc.html

Py:   value = d.get("k") or default
来源：http://hz.jyoumei.cn/gtoanpaaua.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jiagoushi.top/gtpskiptlj.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hnxiangtu.top/gtvnmegtyd.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yueranfly.top/gtwbqvcsnz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.havefunace.top/gtjegqlgon.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.xuetiantiany.cn/gtdcaoskbd.html

Ruby: d&.dig(:a, :b)
来源：http://hz.0kj1m.cn/gtzpkkcwji.html

C#:   obj?.A?.B ?? default
来源：http://hz.xingfuxueyuan.xyz/gtcctwtaba.html

[H07] 断言
来源：http://hz.fzhhl.top/gtatnivkqi.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jinqigfzy.top/gtfkrebpsc.html

PHP:  assert($x > 0);
来源：http://hz.cqqwz.cn/gtogqpxhxa.html

JS:   console.assert(x > 0);
来源：http://hz.meibo888.top/gtcuhwcura.html

TS:   console.assert(x > 0);
来源：http://hz.sweek.top/gtwyuuermj.html

Java: assert x > 0 : "必须为正";
来源：http://hz.chenzaomai.com/gtlyfkvaeb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.shangyingyoupin.top/gtvzivlkhs.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jyoumei.cn/gtfhhxqnvg.html

C#:   Debug.Assert(x > 0);
来源：http://hz.hongshengwenyu.top/gtycrxfkxb.html

[H08] 获取错误信息与堆栈
来源：http://hz.cqqwz.cn/gtvlttjgns.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yuxming.cn/gtldokiqdo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jlsjyb.cn/gtbsnpoewm.html

JS:   e.message;  e.stack
来源：http://hz.hysaishi.cn/gtchbxdemh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yanxiufei.cn/gtmccdjxtr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.iojbl.cn/gtqinjufpq.html

Go:   err.Error()
来源：http://hz.meibo888.top/gtmxmhxbng.html

Ruby: e.message;  e.backtrace
来源：http://hz.hysaishi.cn/gtbszwgkqb.html

C#:   e.Message;  e.StackTrace
来源：http://hz.shanyushiyangkeji.top/gtyofturgp.html

[H09] 带错误码的异常
来源：http://hz.xingfuxueyuan.xyz/gtntnarioh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jianghu66.top/gtunxzvmro.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.daria6918.cn/gtcfqibock.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.daxiang520.top/gtesrnxhjo.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xinyue.icu/gtswmziyat.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jiagoushi.top/gttulkhenj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.dashuyun.cn/gtihbftxyt.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.gogol.net.cn/gtkrrridkq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhijiandao.cn/gtbvvtwhih.html

[H10] 资源自动释放
来源：http://hz.sweek.top/gtpwzfremb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhijiandao.cn/gtmaaawvfx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.gzhubu.top/gthcogsjow.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shanyushiyangkeji.top/gtnfldiepx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.wangshuangyany.cn/gtufkisjwj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yuanzhike.top/gtthpwfpqs.html

Go:   defer f.Close()
来源：http://hz.ehwqpu.com/gtiyjhhrwk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.smart0.xyz/gtvuywnymb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yvedp.cn/gtujgjezme.html

================================================================================
来源：http://hz.pycfn.com/gtywavltpf.html

I. 正则表达式
来源：http://hz.daria6918.cn/gtmkjygpnz.html

================================================================================
来源：http://hz.xinyue.icu/gtycylonsr.html

[I01] 判断是否匹配
来源：http://hz.cqqwz.cn/gtvvtpuikq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jinqigufen.top/gtwvfcupuk.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.meibo888.top/gtfwblfgak.html

JS:   /\d+/.test(s)
来源：http://hz.zhongyouzk.top/gtdbvrcuhy.html

TS:   /\d+/.test(s)
来源：http://hz.cashguo.top/gtiaykgqhb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.wangshuangyany.cn/gtlaxinbkx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.bjfxy.top/gtrqngbyos.html

Ruby: s.match?(/\d+/)
来源：http://hz.nanxuanxn.top/gtnmtbfeno.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hongshengwenyu.top/gttthofqmz.html

[I02] 提取所有匹配
来源：http://hz.jlsjyb.cn/gtxywsvnue.html

Py:   re.findall(r"\d+", s)
来源：http://hz.fengsongda.top/gtjwqlosib.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.quarkkingdee.top/gtlljznjdv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.daria6918.cn/gthyefcmhk.html

TS:   s.match(/\d+/g)
来源：http://hz.shanyushiyangkeji.top/gtrkyhjtxz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shanyushiyangkeji.top/gtuxiqahco.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xingfuxueyuan.xyz/gtcqjttfug.html

Ruby: s.scan(/\d+/)
来源：http://hz.jinyuanbaomall.cn/gtwejmxyuq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.haohaochexian.top/gtcvneodqj.html

[I03] 提取捕获分组
来源：http://hz.shanyushiyangtech.top/gtnxyexrhr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yueranfly.top/gtyaihrvwz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zhoulong.xyz/gtejelqtje.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.svipenyu.cn/gtqftfcqha.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.wangshuangyany.cn/gtdgzncmvl.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhoulong.xyz/gtpqpmmcpq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yj20258.top/gtswgcpffs.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.svipenyu.cn/gtlgiosidz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.chenjidiqi.icu/gtoxkyvnoa.html

[I04] 正则替换
来源：http://hz.sweek.top/gtastycofn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.meibo888.top/gtltakfobp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.wangshuangyany.cn/gtfqnkaxfy.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.tianlin.xyz/gtrbbgxlki.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jyoumei.cn/gtqqcehrzl.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.birdmap.top/gtwtqdllft.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.sxryk.cn/gttnyturij.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhaomingkeji.xyz/gtncfjebzy.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yj202588.top/gtvldqsxog.html

[I05] 按正则拆分
来源：http://hz.c1oappe.top/gttvdpsuje.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ybcxt.top/gtthzbhzjt.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.tianlin.xyz/gthdrhqyzb.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zhijiandao.cn/gtnfpyiurf.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zdqjudy.top/gtdbjouhbq.html

Java: s.split("\\s*,\\s*")
来源：http://hz.nwbrower.top/gtbkjgdluj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.shangyingyoupin.top/gtyjtzlkir.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.meibo888.top/gtbijjqjyi.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhixingplan.top/gtteficnxs.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xylfe.cn/gtyhggkdtm.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hammf.cn/gtlgkkvmsx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.sufxvd.cn/gtqzkmbkmr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.kuanghao11.cn/gtwzjwmsrp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hongshengwenyu.top/gtxrgpsnut.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhengqikj.top/gtzpebgrcz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.shzxlz.cn/gtgbweyjbr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.svipenyu.cn/gtyjuglwsx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hnqzz.top/gtggcffgcs.html

[I07] 忽略大小写与多行模式
来源：http://hz.tian-w.cn/gtqgqypfwh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.nanxuanxn.top/gtrprdgvny.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.shanyushiyangkeji.top/gtucpmljhc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhoulong.xyz/gtskqzblrn.html

TS:   /error/gim
来源：http://hz.mhx1999.top/gtruyymjxv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yvedp.cn/gtghazrmjm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yj20258888.top/gthnkfpdnp.html

Ruby: s.scan(/error/i)
来源：http://hz.zhiwuduotai.top/gthjfhoocc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.gaohongyu789.top/gtlipdyjvk.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.dianchejie.cn/gtnsmzsvwy.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.haohaochexian.top/gtzvbhorsm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.haohaochexian.top/gtwwtllgwv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jqgfzy.top/gtbcgjdnvc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yueranfly.top/gtixmurnfa.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.cucudq.cn/gtwnmdfwvc.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.vqdsnc.cn/gtuzzxfjgn.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jiagoushi.top/gtggdgulgt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zycfv.cn/gtwhwyjbgf.html

================================================================================
来源：http://hz.yueranfly.top/gtwpqblmir.html

J. 日期与时间
来源：http://hz.nanxinkj.top/gtotnbqnnv.html

================================================================================
来源：http://hz.hysaishi.cn/gtbfmcpxog.html

[J01] 获取当前时间
来源：http://hz.guannengcc.top/gtuzfwpxbb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.pycfn.com/gthshkqllj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.shangyingyoupin.top/gtdmsvpqza.html

JS:   new Date();  Date.now()
来源：http://hz.aizwys.cn/gtlxtlkllr.html

TS:   new Date();  Date.now()
来源：http://hz.shanyushiyangtech.top/gtmmmsyzja.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zhengqikj.top/gtxftjuiru.html

Go:   time.Now()
来源：http://hz.shanyushiyangkeji.top/gtwowsxcll.html

Ruby: Time.now
来源：http://hz.xziqi.cn/gtoiwkjlrc.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.aizwys.cn/gtkmtqszuk.html

[J02] 格式化输出
来源：http://hz.xingfuxueyuan.xyz/gtxjfjjpgu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tianlin.xyz/gteupmaqsj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yuxming.cn/gtytunyhfx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.aizwys.cn/gtywcexcsp.html

TS:   d.toISOString()
来源：http://hz.dashuyun.cn/gtiagakrhn.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.ehwqpu.com/gttczttaoi.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.tian-w.cn/gtmffwraeh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.vqdsnc.cn/gtxojbyzlx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhijiandao.cn/gtbdukjjfb.html

[J03] 字符串解析为日期
来源：http://hz.ppjwa.cn/gtmgfuiedd.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.chenjidiqi.icu/gtkjeyxeck.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.tianlin.xyz/gtrjhuwisi.html

JS:   new Date("2024-01-02")
来源：http://hz.yueranfly.top/gtymwlvkjp.html

TS:   new Date("2024-01-02")
来源：http://hz.meibo888.top/gtgycpltfv.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.nanxinkj.top/gtauegjjxa.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.xziqi.cn/gtcwcrvsmp.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.gaohongyu789.top/gtsqlrldlr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jianghu66.top/gtftntetfh.html

[J04] 时间戳与日期互转
来源：http://hz.svipenyu.cn/gthhiayxzq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yongpay.top/gteyybnzru.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yuanzhike.top/gtmchymfbh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.sxryk.cn/gtwjepnoqk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yueranfly.top/gtkdpzmdiv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ydzc1.top/gtreilftup.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.feifeiyinyue.top/gtwvoniuwr.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xylfe.cn/gtopaeodqn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jiagoushi.top/gtumfqrghn.html

[J05] 时间加减（加 7 天）
来源：http://hz.birdmap.top/gtmpvjecgo.html

Py:   now + timedelta(days=7)
来源：http://hz.shanyushiyangkeji.top/gtrrashxgb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.feifeiyinyue.top/gtorxlbcdc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xuetiantiany.cn/gtxrsdnces.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.feifeiyinyue.top/gtugvavkqs.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.52xcode.cn/gtdvzqhdql.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zycfv.cn/gtmbnzsnpq.html

Ruby: Time.now + 7 * 86400
来源：http://hz.tian-w.cn/gtfrjvhcrv.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.iojbl.cn/gtletsnkqh.html

[J06] 计算两时间之差
来源：http://hz.chenzaomai.com/gtnuriqyve.html

Py:   (end - start).total_seconds()
来源：http://hz.kuanghao11.cn/gteidrujvv.html

PHP:  $end->diff($start)->days;
来源：http://hz.guowangkeji.top/gtvdldhaog.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yangfankeji.com/gtwrmoqpbe.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.316326.xyz/gtkcuassso.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.sxryk.cn/gtoatlcjvv.html

Go:   end.Sub(start).Hours()
来源：http://hz.shanyushiyangtech.top/gtqaxuuweb.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jinyuanbaomall.cn/gtppfamfhq.html

C#:   (end - start).TotalSeconds
来源：http://hz.jiagoushi.top/gtjxiudtku.html

[J07] 比较两个日期
来源：http://hz.ydzc1.top/gthqqgrzwd.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hywenlv.cn/gtuhegtykk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.shangyingyoupin.top/gtkzbkjhdq.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jinqigufen.top/gtwgatazbx.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jinqigufen.top/gtvghofjwl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.chenzaomai.com/gtsrahxplx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.chenjidiqi.icu/gtuxwxekjw.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.9152youxi.cn/gtbkaszxhm.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.shangyingyoupin.top/gtcnkjwkjx.html

[J08] 提取年月日与星期
来源：http://hz.yuanzhike.top/gtcustsalc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.shzxlz.cn/gtksaoczit.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yj202588.top/gtovpufiqi.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.ivvv.top/gtdqsmcmvi.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.xylfe.cn/gtvvuemlhv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.redwolf501.top/gtwqwifzim.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.fzhhl.top/gtzwpaovdl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.sweek.top/gturdazpxu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.shuidangran.top/gtgwcseqpf.html

[J09] 时区处理
来源：http://hz.cashguo.top/gtmbshnjjv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jianghu66.top/gtsklvabxh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.fzhhl.top/gtbwyoipyk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cashguo.top/gtiemhltty.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tian-w.cn/gtwerslxbg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhongyouzk.top/gtpvaxdanf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ydjk.org.cn/gtlgnlhzlv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.cashguo.top/gtlqkwhdbl.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.nanxuanxn.top/gtlivzives.html

[J10] 取今天 / 本月第一天
来源：http://hz.cqqwz.cn/gtyfrpdgwb.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.tian-w.cn/gtgkhpmrgf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.iojbl.cn/gtzztepxvy.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.mhx1999.top/gttdovvivs.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhengqikj.top/gtfiqpebzx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yangfankeji.com/gtgvljqqri.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.vqdsnc.cn/gtnkvukwoe.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.dashuyun.cn/gttbpypubk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.cdnleiting.top/gtszpdscom.html

================================================================================
来源：http://hz.shuidangran.top/gtphogkblg.html

K. JSON 与序列化
来源：http://hz.ybcxt.top/gthgrqybau.html

================================================================================
来源：http://hz.guannengcc.top/gttggdwkqw.html

[K01] 对象转 JSON 字符串
来源：http://hz.jlsjyb.cn/gteovlkwsd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.tanke756.top/gtpsehdfgh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hammf.cn/gtuukwzkap.html

JS:   JSON.stringify(obj)
来源：http://hz.zycfv.cn/gtxdgwxkrb.html

TS:   JSON.stringify(obj)
来源：http://hz.316326.xyz/gthxkkhicg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hywenlv.cn/gtyjmjbgfa.html

Go:   json.Marshal(obj)
来源：http://hz.52xcode.cn/gteaxlxtvb.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hywenlv.cn/gtmvclsajz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.bjfxy.top/gtngoeigjt.html

[K02] JSON 字符串转对象
来源：http://hz.iojbl.cn/gtiyytxjlg.html

Py:   json.loads(s)
来源：http://hz.ydjk.org.cn/gtavhetcxo.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.chenlongwang.top/gtsgjlqwzm.html

JS:   JSON.parse(s)
来源：http://hz.nanxuanxn.top/gtdkglivba.html

TS:   JSON.parse(s)
来源：http://hz.vqdsnc.cn/gtzqenlegc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.gaohongyu789.top/gtykeasxhh.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jqgufenzy.top/gtgeyngzbz.html

Ruby: JSON.parse(s)
来源：http://hz.xuetiantiany.cn/gtprgmkbyd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.cucudq.cn/gtwtbrwryh.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.gaohongyu789.top/gtisuvnwrr.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.gzhubu.top/gtciyghcdt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhengqikj.top/gtfbnfbtzy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ybcxt.top/gtkstcahta.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.ywan-chungtsiang.top/gttmezsbwv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.tanke756.top/gtclvqhfit.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yangfankeji.com/gtiejvjdha.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ydzc1.top/gtcmlngaji.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.nwbrower.top/gtbhmmucay.html

[K04] 读取 JSON 文件
来源：http://hz.xuetiantiany.cn/gtjksiiham.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.nwbrower.top/gtuuupuufu.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cheryme.top/gtkptmmufc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.feifeiyinyue.top/gtjncaqhaj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yj20258.top/gtjfsrelbl.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.sxryk.cn/gttfhzypzo.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.shuidangran.top/gttmzptiri.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.shuidangran.top/gtymubzmaa.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jqgufenzy.top/gtwgfjmpij.html

[K05] 深拷贝对象
来源：http://hz.yj20258888.top/gtnirtglsq.html

Py:   copy.deepcopy(obj)
来源：http://hz.jlsjyb.cn/gtakvorfon.html

PHP:  unserialize(serialize($obj));
来源：http://hz.c1oappe.top/gtltxvemdv.html

JS:   structuredClone(obj)
来源：http://hz.ydzc1.top/gtfdgnswsc.html

TS:   structuredClone(obj)
来源：http://hz.ehwqpu.com/gtpiynitjx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.shuidangran.top/gtstojnmge.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.pengpengdd.cyou/gtnhilrlte.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhongyouzk.top/gtsvfymmob.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.pengpengdd.cyou/gtbsmpzigq.html

[K06] 解析 URL 查询串
来源：http://hz.shzxlz.cn/gtcscqdopt.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.pycfn.com/gtutuahlzw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.daria6918.cn/gtsezepufv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jqgfzy.top/gtxncsyzkq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tianlin.xyz/gtfgianggi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.mhx1999.top/gtklpodqzy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.daria6918.cn/gthwzlwrji.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.c1oappe.top/gtcwpkltvp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.tianlin.xyz/gttuxhcbst.html

[K07] 进制转换
来源：http://hz.zhongyouzk.top/gtssoteoym.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.gzhubu.top/gtotmpmvzm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.iojbl.cn/gtfumuzcoe.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hammf.cn/gtdtocdexz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ydzc1.top/gtlckmgrgr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hnxiangtu.top/gtfaapkfpa.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yvedp.cn/gtvihrqwfw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.dashuyun.cn/gtgrovuyml.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.quarkkingdee.top/gtnozeyndd.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhongyouzk.top/gtwyyvnrxx.html

Py:   pickle.dumps(obj)
来源：http://hz.yj20258.top/gtzgdwtlue.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yj202588.top/gtsmxjylva.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yangfankeji.com/gttqhpcjhc.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.gogol.net.cn/gtoltomgwu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.quarkkingdee.top/gtrepdcuuz.html

Go:   encoding/gob
来源：http://hz.hnxiangtu.top/gtycndrxif.html

Ruby: Marshal.dump(obj)
来源：http://hz.hnxiangtu.top/gtagmarozl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.chenzaomai.com/gtnmgnhxcl.html

================================================================================
来源：http://hz.shuidangran.top/gtibkzuusv.html

L. 网络请求
来源：http://hz.jqgfzy.top/gtarbanblo.html

================================================================================
来源：http://hz.316326.xyz/gtiyoqsavm.html

[L01] 发送 GET 请求
来源：http://hz.havefunace.top/gttjpirzph.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.xinyue.icu/gtyilmjhlh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.pengpengdd.cyou/gtinylzedh.html

JS:   await fetch(url)
来源：http://hz.cucudq.cn/gtishvbdrg.html

TS:   await fetch(url)
来源：http://hz.snrcjt.cn/gtunqabgyw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jinyuanbaomall.cn/gtjncevbbh.html


<!-- 参考信息 -->