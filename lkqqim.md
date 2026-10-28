代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hywenlv.cn/gtvmtcnhfm.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ppjwa.cn/gtqidvblmm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.gzhubu.top/gtabcauaqw.html

[I05] 按正则拆分
来源：http://hz.xylfe.cn/gtlkqaacav.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.vqdsnc.cn/gtiqvulotz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jiagoushi.top/gtgcgxfjjs.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.shzxlz.cn/gtsvakqvat.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.dianchejie.cn/gtreffhupi.html

Java: s.split("\\s*,\\s*")
来源：http://hz.tian-w.cn/gttpokffcb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.fzhhl.top/gtnbkdyiox.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xingfuxueyuan.xyz/gtsixkowks.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.bjfxy.top/gtkddfuphy.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.guowangkeji.top/gtqiniarrg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hnxiangtu.top/gtaqgukjic.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jinqigufen.top/gtrfdnjcxb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yvedp.cn/gtoqubeaob.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.dashuyun.cn/gtnrdczevh.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.ehwqpu.com/gtmfqwzhgp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zhixingplan.top/gtrvmdufli.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.gzhubu.top/gtgqpcetzh.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hysaishi.cn/gtffurguey.html

[I07] 忽略大小写与多行模式
来源：http://hz.yuxming.cn/gtazouguss.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yj20258.top/gthjvapafk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xziqi.cn/gtmdwdbbgu.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jinghuilouyu.cn/gtzeepcunz.html

TS:   /error/gim
来源：http://hz.yanxiufei.cn/gtwhpuhhjj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.52xcode.cn/gtyckyzkgn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.nwbrower.top/gtnwhvhncr.html

Ruby: s.scan(/error/i)
来源：http://hz.ydzc1.top/gtabhdzkjm.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhijiandao.cn/gtemowvrwn.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.cdnleiting.top/gtuphvlxgl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jlsjyb.cn/gtfawrzqeh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.svipenyu.cn/gtybsablto.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.wangshuangyany.cn/gtfyoklnoy.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.redwolf501.top/gtazccnctt.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.havefunace.top/gtclhirtfp.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zhongyouzk.top/gtzwsuslxk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zhaomingkeji.xyz/gtlnwsdsgv.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xziqi.cn/gtkgbgrvbw.html

================================================================================
来源：http://hz.jiagoushi.top/gtkumdbkri.html

J. 日期与时间
来源：http://hz.xingfuxueyuan.xyz/gtpfnmvief.html

================================================================================
来源：http://hz.ivvv.top/gtvsspzuub.html

[J01] 获取当前时间
来源：http://hz.yuxming.cn/gtpdqcqpve.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.c1oappe.top/gtcrngvnox.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhixingplan.top/gtkgbxpvkj.html

JS:   new Date();  Date.now()
来源：http://hz.xuetiantiany.cn/gtxuqvyemy.html

TS:   new Date();  Date.now()
来源：http://hz.hongshengwenyu.top/gtfeucytwi.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.snrcjt.cn/gtiwnpyugr.html

Go:   time.Now()
来源：http://hz.guowangkeji.top/gtiyblvxde.html

Ruby: Time.now
来源：http://hz.birdmap.top/gthqbewhfa.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ydjk.org.cn/gtcjokbspo.html

[J02] 格式化输出
来源：http://hz.shanyushiyangkeji.top/gtzwwsbdlm.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ydjk.org.cn/gtqjqbxjxb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.daria6918.cn/gtftjeegfn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jianghu66.top/gtvsfiexfc.html

TS:   d.toISOString()
来源：http://hz.zycfv.cn/gtetmvhhvf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.c1oappe.top/gtwuqtfebm.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.cqqwz.cn/gtmkmogzhh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ydzc1.top/gtjsriqzwf.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.pengpengdd.cyou/gtotyuuyww.html

[J03] 字符串解析为日期
来源：http://hz.wangshuangyany.cn/gtloxvfbcb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.wangdashe.top/gteeaqgfrn.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.quarkkingdee.top/gtnthxhoki.html

JS:   new Date("2024-01-02")
来源：http://hz.jinyuanbaomall.cn/gtplvkmvcw.html

TS:   new Date("2024-01-02")
来源：http://hz.cashguo.top/gtnoruypdl.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.meibo888.top/gtemosbeye.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.cashguo.top/gtrcfeukgi.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cucudq.cn/gtptghwhxr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ybcxt.top/gtwbjlgrrm.html

[J04] 时间戳与日期互转
来源：http://hz.jqgfzy.top/gtpfggoxaw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jinghuilouyu.cn/gthaccfzrk.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jianghu66.top/gtjwqndfxn.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.aibaodan.cn/gtzivutdwe.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.redwolf501.top/gtjnhlfpug.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhengqikj.top/gtudobpfek.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.quarkkingdee.top/gthciiqkfg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.gzhubu.top/gtywewvzca.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yangfankeji.com/gtrfsthehe.html

[J05] 时间加减（加 7 天）
来源：http://hz.guowangkeji.top/gtpkaxmkod.html

Py:   now + timedelta(days=7)
来源：http://hz.meibo888.top/gtugktzwoi.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zdqjudy.top/gtcsvjyptn.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.aibaodan.cn/gtvgyvbdwj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hfpthk.cn/gtpshtnqqe.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.nanxinkj.top/gtabwjnuiz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jinqigfzy.top/gtsdjpciwb.html

Ruby: Time.now + 7 * 86400
来源：http://hz.pengpengdd.cyou/gtchfwprjo.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ydzc1.top/gtqloktsya.html

[J06] 计算两时间之差
来源：http://hz.yuxming.cn/gtxcsqwzop.html

Py:   (end - start).total_seconds()
来源：http://hz.sufxvd.cn/gtkgpcflbo.html

PHP:  $end->diff($start)->days;
来源：http://hz.ybcxt.top/gtuptqsyyn.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.52xcode.cn/gtpmehsiar.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.meibo888.top/gtiyahigmp.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jinqigufen.top/gtgtlqhpxy.html

Go:   end.Sub(start).Hours()
来源：http://hz.bjfxy.top/gtikiwalqr.html

Ruby: end - start                 # 返回秒数
来源：http://hz.daria6918.cn/gttrbizews.html

C#:   (end - start).TotalSeconds
来源：http://hz.c1oappe.top/gthzovvxqb.html

[J07] 比较两个日期
来源：http://hz.shangyingyoupin.top/gtsgkvtawq.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jyoumei.cn/gtxdzgqlvk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.c1oappe.top/gtrycpbrrs.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.havefunace.top/gtyfdyfswb.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ivvv.top/gtqmiurjka.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.shuidangran.top/gtpxwrwfnx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.guannengcc.top/gtrbuasybq.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.c1oappe.top/gtognddcfh.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jqgfzy.top/gtosumalak.html

[J08] 提取年月日与星期
来源：http://hz.zhongyouzk.top/gtixkvngch.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yonumen.top/gtqehmofgg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.shanyushiyangtech.top/gtkzwfsmut.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinqigfzy.top/gtchzxjlps.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jinqigufen.top/gttqhnzajz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.snrcjt.cn/gtcvfrtavh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.wangdashe.top/gtpnuzoqal.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hnqzz.top/gtajlldhvc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zycfv.cn/gtwffohopb.html

[J09] 时区处理
来源：http://hz.guowangkeji.top/gtmgvrhonu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.9152youxi.cn/gtggdninnm.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.sufxvd.cn/gtvcwarpak.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gzhubu.top/gtmffoecjl.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhiwuduotai.top/gtdpqynmjf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.tianlin.xyz/gtxsyuxtmj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yangfankeji.com/gtgakfkcyd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.vqdsnc.cn/gtmwbjlxcm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.wangdashe.top/gtaizkplhi.html

[J10] 取今天 / 本月第一天
来源：http://hz.zdqjudy.top/gtxnuesssh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yuanzhike.top/gtkngylyvf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.smart0.xyz/gtqeqgrjbo.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.shanyushiyangkeji.top/gtwyggwsky.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.bjfxy.top/gttgesorgy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jlsjyb.cn/gtizoxayoz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xingfuxueyuan.xyz/gthwpvredb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhoulong.xyz/gtrakytrks.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xingfuxueyuan.xyz/gtgijwgkth.html

================================================================================
来源：http://hz.hywenlv.cn/gtqfbgnwka.html

K. JSON 与序列化
来源：http://hz.hnxiangtu.top/gtyietmhzv.html

================================================================================
来源：http://hz.ydjk.org.cn/gtbswrhboi.html

[K01] 对象转 JSON 字符串
来源：http://hz.chenzaomai.com/gtnqryuude.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.birdmap.top/gtysdpnabj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhixingplan.top/gtvdkuabkr.html

JS:   JSON.stringify(obj)
来源：http://hz.fzhhl.top/gtbmncgtwf.html

TS:   JSON.stringify(obj)
来源：http://hz.0kj1m.cn/gtrlwazwba.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.snrcjt.cn/gtjsstgjbh.html

Go:   json.Marshal(obj)
来源：http://hz.ywan-chungtsiang.top/gtwwhwdhbt.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hnqzz.top/gtujgmvhdx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.smart0.xyz/gtkroiaelr.html

[K02] JSON 字符串转对象
来源：http://hz.9152youxi.cn/gtyyemslrj.html

Py:   json.loads(s)
来源：http://hz.xuetiantiany.cn/gtccatamtu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.smart0.xyz/gtzqnegosb.html

JS:   JSON.parse(s)
来源：http://hz.zycfv.cn/gtjrbpflss.html

TS:   JSON.parse(s)
来源：http://hz.chenlongwang.top/gtawtovmes.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jinqigufen.top/gtzeawotib.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jiagoushi.top/gtraohzbhg.html

Ruby: JSON.parse(s)
来源：http://hz.pycfn.com/gtumqrojlg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jlsjyb.cn/gtydzoegha.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ydzc1.top/gthrpsftac.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jinqigfzy.top/gtimnitqtp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.mhx1999.top/gtyjcmccyw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.gzhubu.top/gtwmvlaerp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yuxming.cn/gtsaffzvbp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zhengqikj.top/gtznenxtyg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.aizwys.cn/gtsxxjqhpr.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hnqzz.top/gtydgpqaif.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.chenlongwang.top/gtsrtacszr.html

[K04] 读取 JSON 文件
来源：http://hz.cqqwz.cn/gtzskmjgay.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.smart0.xyz/gtpexokfgc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.wangshuangyany.cn/gtmlogtjrn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sufxvd.cn/gtqicsnxjy.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hfpthk.cn/gtvmtfmcvb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hysaishi.cn/gtufrfyodd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jlsjyb.cn/gtemavlwjb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.xuetiantiany.cn/gtpnkabnze.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.0kj1m.cn/gtfpuwfrig.html

[K05] 深拷贝对象
来源：http://hz.zhaomingkeji.xyz/gtmrkamznv.html

Py:   copy.deepcopy(obj)
来源：http://hz.quarkkingdee.top/gtckhrrjan.html

PHP:  unserialize(serialize($obj));
来源：http://hz.316326.xyz/gtoosvamrb.html

JS:   structuredClone(obj)
来源：http://hz.xuetiantiany.cn/gtnczqctgt.html

TS:   structuredClone(obj)
来源：http://hz.meibo888.top/gtqwjnxebw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.cashguo.top/gtdnertijb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yj20258888.top/gtkuqkezwf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shanyushiyangkeji.top/gttcyiykbk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.316326.xyz/gtjcetptqd.html

[K06] 解析 URL 查询串
来源：http://hz.yj20258888.top/gtfvoovwhp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.iojbl.cn/gtkhhzmrcn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xylfe.cn/gtpqikqbqo.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yonumen.top/gtflcqhrwy.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nanxuanxn.top/gtidsuazav.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yj20258888.top/gtbglmctxn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.sweek.top/gttyymamoh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.nanxinkj.top/gtordcoflv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.birdmap.top/gtpaczcxtz.html

[K07] 进制转换
来源：http://hz.jinqigufen.top/gtxmzmckgn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ywan-chungtsiang.top/gtkyodlflt.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhiwuduotai.top/gtlqguhuvv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.gaohongyu789.top/gtipqvhaur.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ywan-chungtsiang.top/gtbuvmjftb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.tianlin.xyz/gtzpcwyept.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.gaohongyu789.top/gtsljgfpcx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.gotoacloud.top/gtosdcyyzx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.dianchejie.cn/gtawnklgcx.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.gzhubu.top/gtkurbpttu.html

Py:   pickle.dumps(obj)
来源：http://hz.jinqigfzy.top/gtrcbyrezx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.52xcode.cn/gtbdxqviyz.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ehwqpu.com/gtsrpctlfp.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.daria6918.cn/gtyefffnjf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.tanke756.top/gtoqrcfeck.html

Go:   encoding/gob
来源：http://hz.guannengcc.top/gthnfkival.html

Ruby: Marshal.dump(obj)
来源：http://hz.nwbrower.top/gtvnsvzfck.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ydzc1.top/gtwmcmfben.html

================================================================================
来源：http://hz.cdnleiting.top/gtyctwssxn.html

L. 网络请求
来源：http://hz.ivvv.top/gtfzpqlecz.html

================================================================================
来源：http://hz.havefunace.top/gtltyfsxxp.html

[L01] 发送 GET 请求
来源：http://hz.birdmap.top/gtsyxxvlbp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.52xcode.cn/gthvdezktg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jinghuilouyu.cn/gtdelrqwzz.html

JS:   await fetch(url)
来源：http://hz.fzhhl.top/gtvpxabmlz.html

TS:   await fetch(url)
来源：http://hz.hongshengwenyu.top/gtcvdrheme.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.316326.xyz/gtdhdzjzxb.html

Go:   resp, err := http.Get(url)
来源：http://hz.pycfn.com/gtcewayhrm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.nanxuanxn.top/gtjqobajfu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hongshengwenyu.top/gtbatqvcva.html

[L02] 发送 POST JSON
来源：http://hz.fzhhl.top/gtfookollw.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.nanxinkj.top/gtaayyvpmt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.wangdashe.top/gtelpcudwi.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.nwbrower.top/gtlmriuobr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinqigufen.top/gtwohamiqr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yj20258.top/gterxhcgbf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hnxiangtu.top/gtkfecivcr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yueranfly.top/gtyvpxggbc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zycfv.cn/gtxgdkuptm.html

[L03] 设置自定义请求头
来源：http://hz.sysykeji.top/gtspiwobas.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hammf.cn/gthhqrwyoe.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ehwqpu.com/gtenyrjhyw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nanxuanxn.top/gtchcvmygb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jiagoushi.top/gtxxljslka.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jinyuanbaomall.cn/gtikfyvzep.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.316326.xyz/gtbczgxmzl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.pycfn.com/gteyazpcsv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.nanxuanxn.top/gtfqwqbgfk.html

[L04] 设置超时
来源：http://hz.gotoacloud.top/gtjsvhbldz.html

Py:   requests.get(url, timeout=5)
来源：http://hz.andypj.xyz/gtvxpfiusz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.xylfe.cn/gthwejnjhw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ivvv.top/gtrkqjvyrn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.guannengcc.top/gtqxxmfdnn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xingfuxueyuan.xyz/gtcczvamsr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.sysykeji.top/gtvsbmipib.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.birdmap.top/gtlbgvvzaa.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.svipenyu.cn/gtddaqzheg.html

[L05] 上传文件（multipart）
来源：http://hz.jianghu66.top/gtlrbozfnp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.pengpengdd.cyou/gtqeranmkd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yanxiufei.cn/gtuhrfvhbg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhengqikj.top/gtetwkzojg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.gogol.net.cn/gtbwzcnntp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.cucudq.cn/gtorxfdrea.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yvedp.cn/gtjyqgoxbd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.hongshengwenyu.top/gtmybjlyah.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.aizwys.cn/gtpxnuzyax.html

[L06] 解析响应为 JSON
来源：http://hz.kuanghao11.cn/gthxxupoyd.html

Py:   resp.json()
来源：http://hz.zhaomingkeji.xyz/gteyreesbd.html

PHP:  json_decode($body, true);
来源：http://hz.sufxvd.cn/gtefbhkfdk.html

JS:   await resp.json()
来源：http://hz.zhijiandao.cn/gtqgaoexkk.html

TS:   await resp.json()
来源：http://hz.zhaomingkeji.xyz/gtlyjbwpre.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hysaishi.cn/gtzkxusjjo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jianghu66.top/gtkvsdfqtg.html

Ruby: JSON.parse(resp.body)
来源：http://hz.sweek.top/gtjqtvdpqs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhiwuduotai.top/gtqklqssna.html

[L07] 处理 HTTP 状态码
来源：http://hz.andypj.xyz/gtaikwhhhd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhoulong.xyz/gtkctmvwnz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.vqdsnc.cn/gtddvtjuve.html

JS:   resp.ok;  resp.status
来源：http://hz.tian-w.cn/gtszcmtzfr.html

TS:   resp.ok;  resp.status
来源：http://hz.hnxiangtu.top/gttlvgfihz.html

Java: resp.statusCode()
来源：http://hz.yj20258888.top/gtwxxpvxdq.html

Go:   resp.StatusCode
来源：http://hz.ehwqpu.com/gtutschhfs.html

Ruby: resp.code.to_i
来源：http://hz.zhiwuduotai.top/gtqyznkhsl.html

C#:   (int)resp.StatusCode
来源：http://hz.52xcode.cn/gtvopohimp.html

[L08] 并发请求多个地址
来源：http://hz.zhijiandao.cn/gtdkekribw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yonumen.top/gtdfojcjmq.html

PHP:  curl_multi_init() 系列
来源：http://hz.guowangkeji.top/gtjugccjpc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yuxming.cn/gtmyycdmwi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shangyingyoupin.top/gtnpnqpvoc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yuxming.cn/gtduqjuhom.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhaomingkeji.xyz/gtrlqrtkgu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.nwbrower.top/gthdeoyizd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.dianchejie.cn/gtrtrwbhkw.html

================================================================================
来源：http://hz.ppjwa.cn/gtgbwinzlz.html

M. 命令行 / 进程 / 环境
来源：http://hz.pengpengdd.cyou/gtmsacyonf.html

================================================================================
来源：http://hz.ehwqpu.com/gtinrgiplp.html

[M01] 读取命令行参数
来源：http://hz.aibaodan.cn/gtkkwzzthn.html

Py:   sys.argv[1:]
来源：http://hz.hnqzz.top/gtzpxrgbax.html

PHP:  $argv;  $argc;
来源：http://hz.ydjk.org.cn/gthvhrewut.html

JS:   process.argv.slice(2)
来源：http://hz.mhx1999.top/gtsojmkqlk.html

TS:   process.argv.slice(2)
来源：http://hz.guowangkeji.top/gtzoksqnke.html

Java: args 数组（main 方法参数）
来源：http://hz.yuanzhike.top/gtegdizdel.html

Go:   os.Args[1:]
来源：http://hz.gaohongyu789.top/gtbwkhnsxy.html

Ruby: ARGV
来源：http://hz.aibaodan.cn/gtdwyvnwhh.html

C#:   args 数组（Main 方法参数）
来源：http://hz.cucudq.cn/gthtkcijep.html

[M02] 读取环境变量
来源：http://hz.havefunace.top/gtfomtstjt.html

Py:   os.environ.get("HOME")
来源：http://hz.zycfv.cn/gtnoofnndv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.meibo888.top/gtewcvkwzo.html

JS:   process.env.HOME
来源：http://hz.yj20258888.top/gthwvokymd.html

TS:   process.env.HOME
来源：http://hz.ydjk.org.cn/gteofutxdj.html

Java: System.getenv("HOME")
来源：http://hz.gaohongyu789.top/gtpihkomez.html


<!-- 参考信息 -->