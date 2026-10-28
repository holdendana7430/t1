代发 wailian999

Ruby: s.scan(/error/i)
来源：http://hz.gogol.net.cn/gtfxmnjfeu.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.shanyushiyangtech.top/gtoagbhesq.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhengqikj.top/gtkbhybjon.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jlsjyb.cn/gtewyegjbw.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yangfankeji.com/gtwjizhjip.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hywenlv.cn/gtzjwoynrl.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gotoacloud.top/gtjpstwtsh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yangfankeji.com/gtqfvubcjc.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.chenlongwang.top/gtkposkbmr.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jiagoushi.top/gtbvqinkpk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yj20258.top/gtcilkvahe.html

================================================================================
来源：http://hz.yuxming.cn/gtvsgwmfqj.html

J. 日期与时间
来源：http://hz.jinqigufen.top/gtqwtetmsb.html

================================================================================
来源：http://hz.316326.xyz/gtuierhgaa.html

[J01] 获取当前时间
来源：http://hz.zhaomingkeji.xyz/gtevlgbswy.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.wangshuangyany.cn/gtkhqtxvlk.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.fengsongda.top/gtyzthfsej.html

JS:   new Date();  Date.now()
来源：http://hz.haohaochexian.top/gtpnpbpjsu.html

TS:   new Date();  Date.now()
来源：http://hz.c1oappe.top/gtixjuitoq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jiagoushi.top/gtjdkcnicy.html

Go:   time.Now()
来源：http://hz.hfpthk.cn/gtctkigpvi.html

Ruby: Time.now
来源：http://hz.smart0.xyz/gtrxzfhgho.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yongpay.top/gtwhwwiqwb.html

[J02] 格式化输出
来源：http://hz.gaohongyu789.top/gtvxsarfwr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cheryme.top/gtsdigvyln.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.mhx1999.top/gtqmryepke.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.fzhhl.top/gtwgqsnxeb.html

TS:   d.toISOString()
来源：http://hz.shangyingyoupin.top/gtcovrdybc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.gzhubu.top/gtxdckaodb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hywenlv.cn/gtvpxdunsg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cqqwz.cn/gtawqcfoxd.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhixingplan.top/gtgcddnxcn.html

[J03] 字符串解析为日期
来源：http://hz.sysykeji.top/gtreaqooon.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xingfuxueyuan.xyz/gtxywjizbh.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.pengpengdd.cyou/gtbiegejnb.html

JS:   new Date("2024-01-02")
来源：http://hz.ehwqpu.com/gtfvoutovn.html

TS:   new Date("2024-01-02")
来源：http://hz.nanxinkj.top/gtomeyxvse.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hnxiangtu.top/gtjkznsiwk.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.kuanghao11.cn/gtzuqlcadu.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.shanyushiyangkeji.top/gtvecvilht.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.nanxinkj.top/gtgqoofmnc.html

[J04] 时间戳与日期互转
来源：http://hz.guannengcc.top/gtxebssvnr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.xuetiantiany.cn/gtyviikxjh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.daxiang520.top/gtitjqqrwq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jlsjyb.cn/gtgmizixvp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.shzxlz.cn/gtkzlfbjmx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xinyue.icu/gthlxgbcsk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.andypj.xyz/gtyjczsgoj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.shzxlz.cn/gtfgzfiamq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.pycfn.com/gtdkmckkql.html

[J05] 时间加减（加 7 天）
来源：http://hz.sufxvd.cn/gtrjhgbqxg.html

Py:   now + timedelta(days=7)
来源：http://hz.hfpthk.cn/gtdrggydsq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.gotoacloud.top/gtcmxnqllc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.snrcjt.cn/gtkpycfyox.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ehwqpu.com/gtgtdaqyqg.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.iojbl.cn/gtpdnitzxd.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yongpay.top/gtdgzfahyn.html

Ruby: Time.now + 7 * 86400
来源：http://hz.aibaodan.cn/gtnocfxfvx.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ydjk.org.cn/gtdzasxfud.html

[J06] 计算两时间之差
来源：http://hz.pengpengdd.cyou/gtfrpennlu.html

Py:   (end - start).total_seconds()
来源：http://hz.ehwqpu.com/gtqjhkgest.html

PHP:  $end->diff($start)->days;
来源：http://hz.yongpay.top/gtpiqrcymd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yj20258888.top/gtjtukzueg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jqgfzy.top/gthgvevgmh.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ydjk.org.cn/gtnivktqpe.html

Go:   end.Sub(start).Hours()
来源：http://hz.sysykeji.top/gtulyuenin.html

Ruby: end - start                 # 返回秒数
来源：http://hz.cucudq.cn/gtnrqobtfn.html

C#:   (end - start).TotalSeconds
来源：http://hz.chenjidiqi.icu/gtyqqcifvb.html

[J07] 比较两个日期
来源：http://hz.shanyushiyangkeji.top/gtmvrgywgj.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhijiandao.cn/gtuesqdxxc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yanxiufei.cn/gtaydfkroe.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.gotoacloud.top/gtymndmedm.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zdqjudy.top/gtculziijs.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.feifeiyinyue.top/gtwrieklna.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hongshengwenyu.top/gtqmxenrbq.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.pengpengdd.cyou/gtpcrjfxuk.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ybcxt.top/gtujwkhatp.html

[J08] 提取年月日与星期
来源：http://hz.yvedp.cn/gtkjseeazx.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.quarkkingdee.top/gtyxizkxdc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zycfv.cn/gtbrwzjjoi.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.haohaochexian.top/gthdbtrwdz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.cqqwz.cn/gtwphnldbv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.haohaochexian.top/gtfdnkkfdd.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yvedp.cn/gtiivntdvs.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.gaohongyu789.top/gtgqbtnwav.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.bjfxy.top/gtjricvvuc.html

[J09] 时区处理
来源：http://hz.yonumen.top/gtaavodoqm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jinqigfzy.top/gtqlyscxfn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jinqigufen.top/gtfdltkfiw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.bjfxy.top/gtwsfrxiyl.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.wangdashe.top/gtrxorcton.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xuetiantiany.cn/gtheelkutz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.pengpengdd.cyou/gtnhqmiknq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zdqjudy.top/gtizeqfjlr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.iojbl.cn/gttqcqnrzg.html

[J10] 取今天 / 本月第一天
来源：http://hz.hfpthk.cn/gtawgoaamc.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.mhx1999.top/gtpliqauux.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.9152youxi.cn/gtfbetdvwa.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.chenjidiqi.icu/gtpaxebmgp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cdnleiting.top/gtgogjccmx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.wangdashe.top/gtcaciigat.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xuanzx.com/gtgtpmmema.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.smart0.xyz/gtvqpgwsis.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jqgfzy.top/gtfusmxklr.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtyltcwbdg.html

K. JSON 与序列化
来源：http://hz.jiagoushi.top/gtjzdftujy.html

================================================================================
来源：http://hz.xylfe.cn/gtbtceuuyt.html

[K01] 对象转 JSON 字符串
来源：http://hz.nwbrower.top/gtynitymwz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yueranfly.top/gtxxaljpcu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jianghu66.top/gtkbqjzxqp.html

JS:   JSON.stringify(obj)
来源：http://hz.nanxuanxn.top/gtczlgdvcf.html

TS:   JSON.stringify(obj)
来源：http://hz.zdqjudy.top/gttvhafaaa.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jinyuanbaomall.cn/gttnrulfog.html

Go:   json.Marshal(obj)
来源：http://hz.ydjk.org.cn/gtzbekpquk.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cucudq.cn/gtsjrhgvwj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhoulong.xyz/gtpyzuhkue.html

[K02] JSON 字符串转对象
来源：http://hz.meibo888.top/gtfqlrpnrs.html

Py:   json.loads(s)
来源：http://hz.yueranfly.top/gtveysygyn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cucudq.cn/gtiwemglly.html

JS:   JSON.parse(s)
来源：http://hz.jyoumei.cn/gtzgmczjrg.html

TS:   JSON.parse(s)
来源：http://hz.tanke756.top/gtffdfjose.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.tanke756.top/gthdefhczv.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhongyouzk.top/gthtehzgdw.html

Ruby: JSON.parse(s)
来源：http://hz.xinyue.icu/gtuvyafkwb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.cqqwz.cn/gtmztajjru.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.sweek.top/gtczbqiyyk.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yuanzhike.top/gtddpjofjj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.xuetiantiany.cn/gtfeulvzrm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.fzhhl.top/gtuqekquee.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xuetiantiany.cn/gtgjaxofji.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.wangshuangyany.cn/gtdehpkhlg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yj20258888.top/gtudzkazxq.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhoulong.xyz/gtzgqecolr.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhiwuduotai.top/gthzrjlsqu.html

[K04] 读取 JSON 文件
来源：http://hz.hysaishi.cn/gtfaxgsfhb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.sufxvd.cn/gtfiacvkop.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ywan-chungtsiang.top/gtuqpzbrid.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yvedp.cn/gtwoztfibw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.pengpengdd.cyou/gtihekreyh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.daxiang520.top/gtkohuspnb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhijiandao.cn/gtroywfibm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.iojbl.cn/gtfxrovjit.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yj20258888.top/gtlcdcaqts.html

[K05] 深拷贝对象
来源：http://hz.316326.xyz/gtfardveob.html

Py:   copy.deepcopy(obj)
来源：http://hz.chenlongwang.top/gtstjagrkc.html

PHP:  unserialize(serialize($obj));
来源：http://hz.snrcjt.cn/gtwwoydnhg.html

JS:   structuredClone(obj)
来源：http://hz.zhoulong.xyz/gtsocqahsv.html

TS:   structuredClone(obj)
来源：http://hz.sxryk.cn/gtbytligmq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ywan-chungtsiang.top/gteoydtnxk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jianghu66.top/gtjkrvhdeb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.gotoacloud.top/gtivkzeegr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.meibo888.top/gtamuzbpcw.html

[K06] 解析 URL 查询串
来源：http://hz.yangfankeji.com/gtybeyoaxv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xylfe.cn/gtbgxtchtg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.feifeiyinyue.top/gtzrlbamwn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jlsjyb.cn/gtumzpeagh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jlsjyb.cn/gtodkqmkyr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ivvv.top/gtqbyqebrp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhixingplan.top/gtnzyggher.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.nanxinkj.top/gtbhgoyavt.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.hammf.cn/gtqxgefrsc.html

[K07] 进制转换
来源：http://hz.jinqigfzy.top/gtqeluemgz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yj202588.top/gtahxwznkl.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jinghuilouyu.cn/gtraudwrmi.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yj20258.top/gtavnbydce.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.shangyingyoupin.top/gtiydwibog.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.quarkkingdee.top/gtmyxtinth.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hongshengwenyu.top/gtpxsfzknz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.dashuyun.cn/gtexujvoln.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.shuidangran.top/gtmvrrdmks.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhiwuduotai.top/gtyqrpidzn.html

Py:   pickle.dumps(obj)
来源：http://hz.vqdsnc.cn/gtrfdtyzzo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.daxiang520.top/gttqououds.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.daxiang520.top/gtkxueajzk.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.chenjidiqi.icu/gtwolpbnca.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.xingfuxueyuan.xyz/gtbepqviup.html

Go:   encoding/gob
来源：http://hz.kuanghao11.cn/gtxlsexehu.html

Ruby: Marshal.dump(obj)
来源：http://hz.jinghuilouyu.cn/gtvlqkxzno.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.hnxiangtu.top/gtmdpwkati.html

================================================================================
来源：http://hz.xuetiantiany.cn/gttedjxexi.html

L. 网络请求
来源：http://hz.ehwqpu.com/gtzxbqctpm.html

================================================================================
来源：http://hz.cqqwz.cn/gtazidsjbj.html

[L01] 发送 GET 请求
来源：http://hz.pengpengdd.cyou/gtjxlgxiqr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.iojbl.cn/gtvtapstzi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ydzc1.top/gtlbscniaj.html

JS:   await fetch(url)
来源：http://hz.hysaishi.cn/gtefnxfgun.html

TS:   await fetch(url)
来源：http://hz.xuetiantiany.cn/gtriwusqbb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.pengpengdd.cyou/gtihyibgzc.html

Go:   resp, err := http.Get(url)
来源：http://hz.zdqjudy.top/gtjyzdueoy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.svipenyu.cn/gteuoimfyt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yvedp.cn/gtanniafgj.html

[L02] 发送 POST JSON
来源：http://hz.ivvv.top/gtplajqqqr.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zdqjudy.top/gtmywjfdwq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xziqi.cn/gtgnqfyyjp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ppjwa.cn/gtlawxwfoq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yanxiufei.cn/gtyqigctyc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.c1oappe.top/gtwigzeovj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ivvv.top/gtlytyyrfz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.nanxuanxn.top/gtvaaycazf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xuetiantiany.cn/gtrpqgleob.html

[L03] 设置自定义请求头
来源：http://hz.hongshengwenyu.top/gtzijpcwvg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yuxming.cn/gtfztpetoq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.redwolf501.top/gtiffxekno.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj202588.top/gtfjkhxfrj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.feifeiyinyue.top/gtqpcezoct.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hywenlv.cn/gtybjglglu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.52xcode.cn/gtbuatljat.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.xinyue.icu/gtglvxwfoa.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhixingplan.top/gtnbwzjrcv.html

[L04] 设置超时
来源：http://hz.chenjidiqi.icu/gtqyvlgbur.html

Py:   requests.get(url, timeout=5)
来源：http://hz.iojbl.cn/gtssbrwgfu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.svipenyu.cn/gtormuhtcj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shanyushiyangkeji.top/gtipexshws.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.bjfxy.top/gtzrlxades.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.wangdashe.top/gtiulrevtj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yvedp.cn/gtsugyjhmi.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.nwbrower.top/gtfxnppmpo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.chenlongwang.top/gtvyfkrxme.html

[L05] 上传文件（multipart）
来源：http://hz.iojbl.cn/gtqwofosgp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhiwuduotai.top/gtsjqqeknb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhixingplan.top/gtfutccgck.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.xziqi.cn/gtxqdrkafn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinyuanbaomall.cn/gtqnsfjreg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.dianchejie.cn/gthyedkkzb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhiwuduotai.top/gtrzbfgnuk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xingfuxueyuan.xyz/gtfjjcanln.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zdqjudy.top/gtqxtbafcb.html

[L06] 解析响应为 JSON
来源：http://hz.gotoacloud.top/gtfqsstogc.html

Py:   resp.json()
来源：http://hz.tanke756.top/gtiqthbpjw.html

PHP:  json_decode($body, true);
来源：http://hz.gotoacloud.top/gtdmsqsqqg.html

JS:   await resp.json()
来源：http://hz.vqdsnc.cn/gtpyzrjvde.html

TS:   await resp.json()
来源：http://hz.pengpengdd.cyou/gtzhtwnpya.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.xuanzx.com/gtkvyybyhm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zycfv.cn/gtpzmkmgdz.html

Ruby: JSON.parse(resp.body)
来源：http://hz.9152youxi.cn/gtzyfqngcd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ydzc1.top/gtazgcsabk.html

[L07] 处理 HTTP 状态码
来源：http://hz.jlsjyb.cn/gtvqahqxqu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xylfe.cn/gtcowonkrj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.c1oappe.top/gtprgbcsqs.html

JS:   resp.ok;  resp.status
来源：http://hz.yj20258.top/gtihpkmuhi.html

TS:   resp.ok;  resp.status
来源：http://hz.jinqigfzy.top/gtdvskwjll.html

Java: resp.statusCode()
来源：http://hz.sysykeji.top/gthkfxjjqr.html

Go:   resp.StatusCode
来源：http://hz.hnxiangtu.top/gtssbdqfeq.html

Ruby: resp.code.to_i
来源：http://hz.aibaodan.cn/gtnixbkucv.html

C#:   (int)resp.StatusCode
来源：http://hz.xingfuxueyuan.xyz/gtjcgllfdr.html

[L08] 并发请求多个地址
来源：http://hz.wangshuangyany.cn/gtxxnbnpzw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.sxryk.cn/gtthhhfhdz.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhengqikj.top/gtoevkobjf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shangyingyoupin.top/gthdeimbcx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenzaomai.com/gtzfmipahq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yongpay.top/gtymhqvjjl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.kuanghao11.cn/gtvtfydewn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zdqjudy.top/gtuqdsdyok.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhoulong.xyz/gtbihzqtql.html

================================================================================
来源：http://hz.haohaochexian.top/gtqpntowoe.html

M. 命令行 / 进程 / 环境
来源：http://hz.shangyingyoupin.top/gtbcwmushe.html

================================================================================
来源：http://hz.aizwys.cn/gtpmgijwtk.html

[M01] 读取命令行参数
来源：http://hz.yuxming.cn/gtrldtjltg.html

Py:   sys.argv[1:]
来源：http://hz.cdnleiting.top/gtztnkyyiu.html

PHP:  $argv;  $argc;
来源：http://hz.cdnleiting.top/gtbcbqakbd.html

JS:   process.argv.slice(2)
来源：http://hz.redwolf501.top/gtgszzstyp.html

TS:   process.argv.slice(2)
来源：http://hz.andypj.xyz/gtqghumghe.html

Java: args 数组（main 方法参数）
来源：http://hz.haohaochexian.top/gtvdbeefdm.html

Go:   os.Args[1:]
来源：http://hz.ivvv.top/gtzmzmkyck.html

Ruby: ARGV
来源：http://hz.jinqigfzy.top/gttgszwwqp.html

C#:   args 数组（Main 方法参数）
来源：http://hz.shanyushiyangtech.top/gthqyxqyva.html

[M02] 读取环境变量
来源：http://hz.sufxvd.cn/gthiabmjeq.html

Py:   os.environ.get("HOME")
来源：http://hz.sweek.top/gtmswztmdd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.xylfe.cn/gtrfqnqsdx.html

JS:   process.env.HOME
来源：http://hz.andypj.xyz/gtbanzsyvg.html

TS:   process.env.HOME
来源：http://hz.cashguo.top/gthagldjeb.html

Java: System.getenv("HOME")
来源：http://hz.dashuyun.cn/gteizcqnbi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.aizwys.cn/gtgoyukymx.html

Ruby: ENV["HOME"]
来源：http://hz.chenlongwang.top/gtisfsbnes.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hnqzz.top/gtxvjbdkxp.html

[M03] 执行外部命令
来源：http://hz.c1oappe.top/gtarjtlyxl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.shzxlz.cn/gtcglfbcal.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zycfv.cn/gtyavedfnm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hywenlv.cn/gtweqelwat.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.sysykeji.top/gtwzrqbpip.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ywan-chungtsiang.top/gtgdzlzmqi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jlsjyb.cn/gtshpusdkl.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.chenzaomai.com/gtrhtamqct.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jqgufenzy.top/gtwvinhdbk.html

[M04] 获取当前工作目录
来源：http://hz.nanxinkj.top/gtfgbxlapo.html

Py:   os.getcwd()
来源：http://hz.dashuyun.cn/gtniitcpyq.html

PHP:  getcwd();
来源：http://hz.nanxuanxn.top/gtmdznfqza.html

JS:   process.cwd()
来源：http://hz.cqqwz.cn/gttnjxsgai.html

TS:   process.cwd()
来源：http://hz.jinqigfzy.top/gtdoeyjnsy.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jinqigfzy.top/gtvbimgybo.html

Go:   os.Getwd()
来源：http://hz.daxiang520.top/gtusboonqn.html

Ruby: Dir.pwd
来源：http://hz.snrcjt.cn/gtihjbagja.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.9152youxi.cn/gttlaeyrre.html

[M05] 设置退出码
来源：http://hz.daxiang520.top/gtksvgkacd.html

Py:   sys.exit(1)
来源：http://hz.fengsongda.top/gttdujwali.html

PHP:  exit(1);
来源：http://hz.zhoulong.xyz/gtngtvoqvw.html

JS:   process.exit(1)
来源：http://hz.ppjwa.cn/gtoczhzsug.html

TS:   process.exit(1)
来源：http://hz.zhiwuduotai.top/gtrvxqoevq.html

Java: System.exit(1)
来源：http://hz.sxryk.cn/gtmazwbtrk.html

Go:   os.Exit(1)
来源：http://hz.jinghuilouyu.cn/gtpizzfltn.html


<!-- 参考信息 -->