代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.nanxinkj.top/gtnuobdlps.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.kuanghao11.cn/gtgmpyvfef.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.aizwys.cn/gttfgfbvxm.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hfpthk.cn/gtmmxdojej.html

Java: s.split("\\s*,\\s*")
来源：http://hz.chenlongwang.top/gtlrcblczx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.tian-w.cn/gtsxarznpm.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.shangyingyoupin.top/gtpsdeliie.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.gaohongyu789.top/gtorqtbvac.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.feifeiyinyue.top/gteragwfql.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhijiandao.cn/gtnddjqbkw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.pycfn.com/gtgchgsvgb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yonumen.top/gtnrlzvrgg.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.kuanghao11.cn/gtdunsqbbv.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.feifeiyinyue.top/gttkosbqnl.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.daxiang520.top/gtgvrziltz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.tanke756.top/gteszwalty.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.feifeiyinyue.top/gtdcdnzteu.html

[I07] 忽略大小写与多行模式
来源：http://hz.zhongyouzk.top/gtwmjavknj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.snrcjt.cn/gtbdkhgegy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ppjwa.cn/gtlctripxz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.feifeiyinyue.top/gtthivfuyz.html

TS:   /error/gim
来源：http://hz.ydzc1.top/gtdizouckv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.daria6918.cn/gtzpvfeacx.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.cheryme.top/gtolierlfn.html

Ruby: s.scan(/error/i)
来源：http://hz.cucudq.cn/gthrljfrsx.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.hnqzz.top/gtpbqdcqxa.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.sysykeji.top/gtrgfhoxyp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.hnqzz.top/gtwqbcsgsf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hnxiangtu.top/gtsiiuhjwx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.havefunace.top/gtrfqzfiup.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.wangdashe.top/gtqczrxxze.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yj20258.top/gtlaiwdpsa.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.haohaochexian.top/gtdnzlmucz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.aibaodan.cn/gtgfdezdcd.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.fzhhl.top/gtseeyzhep.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtrrekjtvf.html

J. 日期与时间
来源：http://hz.hongshengwenyu.top/gtzyunrjyo.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtqbpxyonl.html

[J01] 获取当前时间
来源：http://hz.gotoacloud.top/gtnnqeblgg.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.sweek.top/gtaawpmora.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ppjwa.cn/gtbwoluyuz.html

JS:   new Date();  Date.now()
来源：http://hz.hongshengwenyu.top/gtucyponkq.html

TS:   new Date();  Date.now()
来源：http://hz.nwbrower.top/gttsxpvnzw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hnxiangtu.top/gtboatxrak.html

Go:   time.Now()
来源：http://hz.guowangkeji.top/gtihlmwpqo.html

Ruby: Time.now
来源：http://hz.hfpthk.cn/gtlxuxggxs.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.quarkkingdee.top/gtrvhwaauj.html

[J02] 格式化输出
来源：http://hz.shanyushiyangkeji.top/gttwbyokbe.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xuanzx.com/gtndelsuvp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.iojbl.cn/gtgwdcdwgk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jianghu66.top/gtmbiufemb.html

TS:   d.toISOString()
来源：http://hz.hnxiangtu.top/gtvbadbmqx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hnxiangtu.top/gtppzdvbea.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jinyuanbaomall.cn/gtuwlnjesi.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ppjwa.cn/gtnttbyadt.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.nanxuanxn.top/gtgnkuvvsp.html

[J03] 字符串解析为日期
来源：http://hz.jinqigufen.top/gtfavpyzsp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.havefunace.top/gtdwfozdbp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhoulong.xyz/gtuzauwmww.html

JS:   new Date("2024-01-02")
来源：http://hz.cheryme.top/gtumhtjyzf.html

TS:   new Date("2024-01-02")
来源：http://hz.xinyue.icu/gtejsgtvvy.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.quarkkingdee.top/gtcvixdbun.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.xylfe.cn/gteovqremv.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zycfv.cn/gtqugnqshg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.9152youxi.cn/gtvlvorzhz.html

[J04] 时间戳与日期互转
来源：http://hz.ydjk.org.cn/gtbfpgwauc.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yongpay.top/gtvrpkggfk.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.fzhhl.top/gttfhligaa.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.316326.xyz/gtxmqtwnbg.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xingfuxueyuan.xyz/gtuidgcgig.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jiagoushi.top/gtfpkpbgwb.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhijiandao.cn/gtrdkzmgxd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.gogol.net.cn/gtbfkcacku.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.wangshuangyany.cn/gtupuhzsft.html

[J05] 时间加减（加 7 天）
来源：http://hz.cucudq.cn/gtmgwpizbi.html

Py:   now + timedelta(days=7)
来源：http://hz.fengsongda.top/gtqcccftun.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.mhx1999.top/gtxufgeium.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.0kj1m.cn/gtcwrpgecz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.daxiang520.top/gtgudzmbei.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.shangyingyoupin.top/gtbwxaqqfx.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yj20258.top/gtmtmlgndd.html

Ruby: Time.now + 7 * 86400
来源：http://hz.wangdashe.top/gtruoolegu.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhoulong.xyz/gtzsndkuyb.html

[J06] 计算两时间之差
来源：http://hz.nanxuanxn.top/gtbiatrpqi.html

Py:   (end - start).total_seconds()
来源：http://hz.yuxming.cn/gtkpyimgyt.html

PHP:  $end->diff($start)->days;
来源：http://hz.9152youxi.cn/gtsgtupxqu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jiagoushi.top/gtipwxnmeg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jinqigufen.top/gtlcnnywoj.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhengqikj.top/gtasijfzdd.html

Go:   end.Sub(start).Hours()
来源：http://hz.yueranfly.top/gtvxhktnzq.html

Ruby: end - start                 # 返回秒数
来源：http://hz.snrcjt.cn/gtgwehnjch.html

C#:   (end - start).TotalSeconds
来源：http://hz.cdnleiting.top/gtahqmsidu.html

[J07] 比较两个日期
来源：http://hz.hnqzz.top/gtucirfkjz.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.shzxlz.cn/gtfydfnotg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.nanxinkj.top/gtnxxycsfd.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.cheryme.top/gtzunvfkvd.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.wangshuangyany.cn/gtqrgtbami.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.wangdashe.top/gtmfoowtcy.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.wangshuangyany.cn/gtyxwkqglu.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.svipenyu.cn/gtfvmslyoy.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yangfankeji.com/gtbbnksckl.html

[J08] 提取年月日与星期
来源：http://hz.yonumen.top/gtbzzxwbmq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.nanxuanxn.top/gtcevmoaqg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.feifeiyinyue.top/gtvcdfbtit.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinyuanbaomall.cn/gtpfugoqmr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhijiandao.cn/gtajlxrljw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.cqqwz.cn/gtmfiocnqc.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hywenlv.cn/gtktnrfxfj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.aizwys.cn/gttpbirlsi.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.shangyingyoupin.top/gtpcspizdj.html

[J09] 时区处理
来源：http://hz.yuanzhike.top/gttpzneyqw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.meibo888.top/gtemvlkzzk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yj202588.top/gtwthkshra.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yuxming.cn/gtbyqmspti.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hammf.cn/gtxialomtd.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.sweek.top/gtsfxtletp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.andypj.xyz/gtdjnlguvv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jqgfzy.top/gtygjxxiid.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.nanxinkj.top/gtfxcmhniy.html

[J10] 取今天 / 本月第一天
来源：http://hz.ehwqpu.com/gtgzgxdcnt.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.fzhhl.top/gtcwhfcwhn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.shangyingyoupin.top/gtnbowczvh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.cashguo.top/gtxzbqyywh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yanxiufei.cn/gtqynairkr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.svipenyu.cn/gtqgisiqof.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.fengsongda.top/gticiuudwl.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xuanzx.com/gtiubahtht.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zhijiandao.cn/gtkckvkkcz.html

================================================================================
来源：http://hz.jianghu66.top/gttrfahfot.html

K. JSON 与序列化
来源：http://hz.svipenyu.cn/gtorrgcong.html

================================================================================
来源：http://hz.guowangkeji.top/gtryizlqzr.html

[K01] 对象转 JSON 字符串
来源：http://hz.fengsongda.top/gthxttluqg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.xuetiantiany.cn/gtltgkgoam.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yj20258.top/gtbnkiqgzo.html

JS:   JSON.stringify(obj)
来源：http://hz.sweek.top/gtzubjdudj.html

TS:   JSON.stringify(obj)
来源：http://hz.hnqzz.top/gtzkhkzwio.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xylfe.cn/gtryscqzdq.html

Go:   json.Marshal(obj)
来源：http://hz.guowangkeji.top/gtameobnsh.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.bjfxy.top/gtavpavpfz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.pengpengdd.cyou/gtkvyhgarx.html

[K02] JSON 字符串转对象
来源：http://hz.zdqjudy.top/gttqwfoook.html

Py:   json.loads(s)
来源：http://hz.chenlongwang.top/gtcwxkqnaw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhaomingkeji.xyz/gtgsmxnfme.html

JS:   JSON.parse(s)
来源：http://hz.zhijiandao.cn/gteretalxd.html

TS:   JSON.parse(s)
来源：http://hz.cdnleiting.top/gtoavkkpbs.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hywenlv.cn/gtlhyrwydc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xingfuxueyuan.xyz/gtmzhfixmm.html

Ruby: JSON.parse(s)
来源：http://hz.chenzaomai.com/gtmwfeskzg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.feifeiyinyue.top/gthszcarhu.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.dashuyun.cn/gtggewrkxm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.cheryme.top/gtvmyeyqbn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.shuidangran.top/gtnlamckaq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.bjfxy.top/gthggtxppw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhengqikj.top/gtquniuiqp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.meibo888.top/gtnkilgfts.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhaomingkeji.xyz/gtsqjgihnl.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ybcxt.top/gtgoykxpeb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hammf.cn/gtwjmaihjl.html

[K04] 读取 JSON 文件
来源：http://hz.meibo888.top/gtnzrhxykp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.shzxlz.cn/gtvyuercex.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.316326.xyz/gtgcquxbbx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yangfankeji.com/gtjfrhzfio.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yonumen.top/gtswlgstkw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhoulong.xyz/gtowevjjgd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jiagoushi.top/gtkfthoqgm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jinghuilouyu.cn/gtujcqlfed.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.birdmap.top/gtpbjdlgba.html

[K05] 深拷贝对象
来源：http://hz.gaohongyu789.top/gttsrntgdw.html

Py:   copy.deepcopy(obj)
来源：http://hz.gotoacloud.top/gtzvtynjbu.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cucudq.cn/gtxbfhadcs.html

JS:   structuredClone(obj)
来源：http://hz.bjfxy.top/gtgywcuoft.html

TS:   structuredClone(obj)
来源：http://hz.bjfxy.top/gtiukmizrf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.tianlin.xyz/gthfsncnsf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.gaohongyu789.top/gtwcdbyctn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.svipenyu.cn/gtqxnvfrhx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zycfv.cn/gttmbswzkm.html

[K06] 解析 URL 查询串
来源：http://hz.shzxlz.cn/gtbkewidsa.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.sxryk.cn/gtkmcecrao.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yongpay.top/gtlftarmfi.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.mhx1999.top/gtpouxllfi.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinghuilouyu.cn/gtwtvkpskc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.daria6918.cn/gtabzgwckc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.vqdsnc.cn/gtjnsamyzn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.wangshuangyany.cn/gtdsulyvrr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jlsjyb.cn/gtjbjjqyff.html

[K07] 进制转换
来源：http://hz.wangdashe.top/gtktqnxcdg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jqgfzy.top/gttciashli.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yuxming.cn/gtampgbbyd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jinqigfzy.top/gtftjmgney.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hysaishi.cn/gtamjgnxyq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jlsjyb.cn/gtkfzgrpdk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.nwbrower.top/gtfprrkhbd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zhixingplan.top/gttfdlxtje.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.guannengcc.top/gtygyhsulr.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhoulong.xyz/gtruomfynb.html

Py:   pickle.dumps(obj)
来源：http://hz.sxryk.cn/gtmengmqvv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.aibaodan.cn/gtwvuaeooh.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yj202588.top/gtfkaktuhg.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ehwqpu.com/gtxppcdwuq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.pycfn.com/gtwrbvkooa.html

Go:   encoding/gob
来源：http://hz.jinghuilouyu.cn/gtjjyhicvr.html

Ruby: Marshal.dump(obj)
来源：http://hz.aibaodan.cn/gtmrfouqrc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.haohaochexian.top/gtcpefxgrz.html

================================================================================
来源：http://hz.ehwqpu.com/gtigmkkjzi.html

L. 网络请求
来源：http://hz.chenzaomai.com/gttffwledk.html

================================================================================
来源：http://hz.wangdashe.top/gtnmaxmtak.html

[L01] 发送 GET 请求
来源：http://hz.yangfankeji.com/gtwebkfaqf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jinqigfzy.top/gtnyoauihg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ydzc1.top/gtsrsfgkfy.html

JS:   await fetch(url)
来源：http://hz.zdqjudy.top/gtelxlpoef.html

TS:   await fetch(url)
来源：http://hz.tian-w.cn/gttztsvgtu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.gzhubu.top/gtslrcsevq.html

Go:   resp, err := http.Get(url)
来源：http://hz.meibo888.top/gtlqjfutdr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.gaohongyu789.top/gtfiuqdvpu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.shangyingyoupin.top/gtaofwkkqz.html

[L02] 发送 POST JSON
来源：http://hz.tanke756.top/gtdxfwwdtn.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.9152youxi.cn/gtnrgovkan.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.feifeiyinyue.top/gtmbrrocnb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.fzhhl.top/gtgfgteizc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yueranfly.top/gtrzhlcuky.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yuxming.cn/gtragufinu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yj202588.top/gtcrnvyrss.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.sxryk.cn/gtvrofnira.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zhaomingkeji.xyz/gtjluzdqcz.html

[L03] 设置自定义请求头
来源：http://hz.aizwys.cn/gtqmrqthjv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jqgufenzy.top/gtbkvmthpu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.xinyue.icu/gtemzgmmng.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.vqdsnc.cn/gtijdxmrmh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.bjfxy.top/gtvttumuvo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.snrcjt.cn/gtpnwrlchk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jiagoushi.top/gtwrtkzilh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.sweek.top/gtpdlidndw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.52xcode.cn/gtskltziic.html

[L04] 设置超时
来源：http://hz.yj20258.top/gtssecaepk.html

Py:   requests.get(url, timeout=5)
来源：http://hz.dianchejie.cn/gtvhtjmkgz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.nanxuanxn.top/gtcqpcadnq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xuetiantiany.cn/gtdfjiomkj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.guannengcc.top/gtdkhsveim.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yvedp.cn/gthzihbkmp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.shanyushiyangkeji.top/gtsfspucoe.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yangfankeji.com/gtohcoefsx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.cdnleiting.top/gttvmzlxvo.html

[L05] 上传文件（multipart）
来源：http://hz.0kj1m.cn/gtvjkdpgus.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhongyouzk.top/gtmuxriqtd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.mhx1999.top/gtpuhwpqes.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.xingfuxueyuan.xyz/gtckottgfa.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.xylfe.cn/gtkdxoooph.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yueranfly.top/gtqjsrjngg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jlsjyb.cn/gtiaiovmlu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yvedp.cn/gtnenswqfl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jlsjyb.cn/gtmcipwirl.html

[L06] 解析响应为 JSON
来源：http://hz.cdnleiting.top/gtqnpjwrus.html

Py:   resp.json()
来源：http://hz.shanyushiyangtech.top/gtywwebmjf.html

PHP:  json_decode($body, true);
来源：http://hz.nwbrower.top/gtvuoxmrsr.html

JS:   await resp.json()
来源：http://hz.jianghu66.top/gtseukscpg.html

TS:   await resp.json()
来源：http://hz.svipenyu.cn/gtazqxxmfx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.52xcode.cn/gtikpfkseo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jyoumei.cn/gtuqaxvwga.html

Ruby: JSON.parse(resp.body)
来源：http://hz.sysykeji.top/gtelxsrrvl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jianghu66.top/gtstgajegg.html

[L07] 处理 HTTP 状态码
来源：http://hz.aizwys.cn/gteanxshjp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.nwbrower.top/gttftfgpqo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.xuetiantiany.cn/gtiifwzsjv.html

JS:   resp.ok;  resp.status
来源：http://hz.xylfe.cn/gtxjggsfdy.html

TS:   resp.ok;  resp.status
来源：http://hz.cqqwz.cn/gtoakznxfe.html

Java: resp.statusCode()
来源：http://hz.jqgfzy.top/gthjdkrluq.html

Go:   resp.StatusCode
来源：http://hz.nanxinkj.top/gtqmjtwptk.html

Ruby: resp.code.to_i
来源：http://hz.feifeiyinyue.top/gtdjyebvxe.html

C#:   (int)resp.StatusCode
来源：http://hz.xinyue.icu/gtrtrgvscw.html

[L08] 并发请求多个地址
来源：http://hz.wangdashe.top/gtnvkcbxpa.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zycfv.cn/gtflhmahrg.html

PHP:  curl_multi_init() 系列
来源：http://hz.jiagoushi.top/gtkypncsfn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.quarkkingdee.top/gteympwqul.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhengqikj.top/gtlesndgjg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ywan-chungtsiang.top/gtbxfcdncc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hongshengwenyu.top/gtwecsgloh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hammf.cn/gtygfxixkr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.quarkkingdee.top/gtmmxdauml.html

================================================================================
来源：http://hz.hywenlv.cn/gtywbcfcnz.html

M. 命令行 / 进程 / 环境
来源：http://hz.zycfv.cn/gttekmropv.html

================================================================================
来源：http://hz.aibaodan.cn/gtnvmjjpyt.html

[M01] 读取命令行参数
来源：http://hz.yj20258888.top/gtgenizxcz.html

Py:   sys.argv[1:]
来源：http://hz.havefunace.top/gtaooztakm.html

PHP:  $argv;  $argc;
来源：http://hz.ywan-chungtsiang.top/gtoubovuxi.html

JS:   process.argv.slice(2)
来源：http://hz.yanxiufei.cn/gtpvtiqqdd.html

TS:   process.argv.slice(2)
来源：http://hz.sysykeji.top/gtbwktkhjz.html

Java: args 数组（main 方法参数）
来源：http://hz.pengpengdd.cyou/gtlncrlgbs.html

Go:   os.Args[1:]
来源：http://hz.hnqzz.top/gtwkubzuqk.html

Ruby: ARGV
来源：http://hz.meibo888.top/gtvgqldpzk.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jinqigufen.top/gtvgyegduw.html

[M02] 读取环境变量
来源：http://hz.daria6918.cn/gtrhoylvum.html

Py:   os.environ.get("HOME")
来源：http://hz.316326.xyz/gtjhcpameb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hywenlv.cn/gtjrvirkod.html

JS:   process.env.HOME
来源：http://hz.jlsjyb.cn/gtteszexog.html

TS:   process.env.HOME
来源：http://hz.yj20258888.top/gtreaigdrk.html

Java: System.getenv("HOME")
来源：http://hz.tian-w.cn/gtswliwyuz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.fengsongda.top/gtcbmrlbmp.html

Ruby: ENV["HOME"]
来源：http://hz.iojbl.cn/gtexewoxew.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jqgfzy.top/gtrkrlvugo.html

[M03] 执行外部命令
来源：http://hz.snrcjt.cn/gtmqvsfidp.html


<!-- 参考信息 -->