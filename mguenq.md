代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.svipenyu.cn/gtrnrigtlv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.haohaochexian.top/gtoypikngy.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.daxiang520.top/gtzdzurdem.html

================================================================================
来源：http://hz.dashuyun.cn/gtwrbdswem.html

J. 日期与时间
来源：http://hz.pengpengdd.cyou/gtlgpconrd.html

================================================================================
来源：http://hz.cqqwz.cn/gtvjrrvkus.html

[J01] 获取当前时间
来源：http://hz.chenzaomai.com/gtbrjpmkmk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.kuanghao11.cn/gtbcfqkksf.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xylfe.cn/gtkrplnojy.html

JS:   new Date();  Date.now()
来源：http://hz.jiagoushi.top/gtpghcxikf.html

TS:   new Date();  Date.now()
来源：http://hz.chenjidiqi.icu/gtnkpdempz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.bjfxy.top/gtmoxspkzn.html

Go:   time.Now()
来源：http://hz.nanxuanxn.top/gtvmvcnake.html

Ruby: Time.now
来源：http://hz.wangdashe.top/gtmldqvjzx.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ywan-chungtsiang.top/gtyvluicay.html

[J02] 格式化输出
来源：http://hz.nanxinkj.top/gtunfftotp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cdnleiting.top/gthnlywmcu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.xinyue.icu/gtjbuvclht.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hammf.cn/gtselvujop.html

TS:   d.toISOString()
来源：http://hz.wangshuangyany.cn/gtbjssamiu.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.gogol.net.cn/gtybonaubc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.sufxvd.cn/gtqsynlmxb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jyoumei.cn/gtwuhfxkhy.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhoulong.xyz/gtczgmmrjd.html

[J03] 字符串解析为日期
来源：http://hz.pycfn.com/gttzecdcik.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hongshengwenyu.top/gtdenvitxc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.guannengcc.top/gtoqioqbus.html

JS:   new Date("2024-01-02")
来源：http://hz.birdmap.top/gtldgehkgd.html

TS:   new Date("2024-01-02")
来源：http://hz.hnqzz.top/gtrqoyyoyj.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yueranfly.top/gtrrfokzgn.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hongshengwenyu.top/gtohvfmbvc.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.smart0.xyz/gtzuovjnkt.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zdqjudy.top/gtgjnifxuh.html

[J04] 时间戳与日期互转
来源：http://hz.guowangkeji.top/gtbpvofrjq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.gotoacloud.top/gtaxydshzj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xylfe.cn/gtjqtixpzy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.meibo888.top/gtonnmfuae.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.mhx1999.top/gttnexsmlh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.316326.xyz/gtbhahnzat.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jyoumei.cn/gtxsonrnns.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zycfv.cn/gtkowreugr.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.vqdsnc.cn/gtduafgtyg.html

[J05] 时间加减（加 7 天）
来源：http://hz.fengsongda.top/gthbymztkj.html

Py:   now + timedelta(days=7)
来源：http://hz.ybcxt.top/gtergcpucb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jinghuilouyu.cn/gtbwipwbkz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yangfankeji.com/gthrmkvdxu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shangyingyoupin.top/gtkkpthrtx.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zdqjudy.top/gtjmaygpdk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ehwqpu.com/gtsuwztsve.html

Ruby: Time.now + 7 * 86400
来源：http://hz.tian-w.cn/gttfzlmagq.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cheryme.top/gtwuhupbfn.html

[J06] 计算两时间之差
来源：http://hz.yanxiufei.cn/gtgedrslrj.html

Py:   (end - start).total_seconds()
来源：http://hz.nanxinkj.top/gthjkxbzzc.html

PHP:  $end->diff($start)->days;
来源：http://hz.iojbl.cn/gtbptlgdem.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jinghuilouyu.cn/gtptnakapy.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ivvv.top/gttlhnlevn.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yangfankeji.com/gtavteqfci.html

Go:   end.Sub(start).Hours()
来源：http://hz.mhx1999.top/gtyezbnzjx.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yuanzhike.top/gtvalrdubq.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhoulong.xyz/gttpjxwsgy.html

[J07] 比较两个日期
来源：http://hz.guannengcc.top/gtswklljvr.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhijiandao.cn/gtnhaspnvz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hnqzz.top/gtahufmzaf.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.andypj.xyz/gtsgpqpeby.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.meibo888.top/gtbwzgvoiu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jinqigfzy.top/gthubxrulr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhijiandao.cn/gtfsdqkkrl.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.iojbl.cn/gtyqnjgzft.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.vqdsnc.cn/gtuptajnbf.html

[J08] 提取年月日与星期
来源：http://hz.shuidangran.top/gtfzuoznfx.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.haohaochexian.top/gtetyrfasg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jqgfzy.top/gtvnmzzpmd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinqigufen.top/gtxloehqfq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhengqikj.top/gtiyvkhdft.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yangfankeji.com/gtywuqgero.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ppjwa.cn/gtxlejwipt.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ydzc1.top/gtuqoxvkbi.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.daxiang520.top/gtlqbnznlo.html

[J09] 时区处理
来源：http://hz.gaohongyu789.top/gtvwpswyqi.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ydjk.org.cn/gtblazdvie.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jinqigfzy.top/gtgmcwvsnr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jlsjyb.cn/gtbbqvpswh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jyoumei.cn/gtvceivpou.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhijiandao.cn/gtbjomziut.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yongpay.top/gtpgulorht.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.xylfe.cn/gtnswjospf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.guowangkeji.top/gtjltkziyz.html

[J10] 取今天 / 本月第一天
来源：http://hz.jinyuanbaomall.cn/gtingliuqg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cdnleiting.top/gtbgxggdcb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.bjfxy.top/gttdxrcocz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.pycfn.com/gtgxtgdwfk.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.xylfe.cn/gtvnotsbwx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yj20258.top/gtpmqglxcz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hongshengwenyu.top/gtxeugicka.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.svipenyu.cn/gtmwiyawdx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.dianchejie.cn/gtuexzqrew.html

================================================================================
来源：http://hz.tian-w.cn/gtcbzovceq.html

K. JSON 与序列化
来源：http://hz.cashguo.top/gtxfeurxib.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtdapxhihv.html

[K01] 对象转 JSON 字符串
来源：http://hz.shzxlz.cn/gtcjbulgju.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yongpay.top/gtfrvznpau.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ydjk.org.cn/gthzysvwxw.html

JS:   JSON.stringify(obj)
来源：http://hz.jiagoushi.top/gtjxeksgvu.html

TS:   JSON.stringify(obj)
来源：http://hz.tianlin.xyz/gtsnioxvbi.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.wangdashe.top/gtlrkikztq.html

Go:   json.Marshal(obj)
来源：http://hz.52xcode.cn/gtzitcrpyw.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cashguo.top/gttcnbjnuh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zycfv.cn/gtragkqojb.html

[K02] JSON 字符串转对象
来源：http://hz.zhongyouzk.top/gtpqqpmlzs.html

Py:   json.loads(s)
来源：http://hz.svipenyu.cn/gtpixjvsah.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.fzhhl.top/gtudwjfzyd.html

JS:   JSON.parse(s)
来源：http://hz.dianchejie.cn/gtpakkfahx.html

TS:   JSON.parse(s)
来源：http://hz.tianlin.xyz/gtsfxbqogy.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jinqigfzy.top/gtalvujmeh.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.sysykeji.top/gtwpdweejd.html

Ruby: JSON.parse(s)
来源：http://hz.tanke756.top/gtzezlhbzh.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ydjk.org.cn/gtsgcnstyj.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.pycfn.com/gtsfnxxzhv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.fengsongda.top/gtbixerxwv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.xingfuxueyuan.xyz/gtxqbhtvcu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shanyushiyangtech.top/gtggsvlwwa.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.sxryk.cn/gtwxygkmqs.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yanxiufei.cn/gtxtjkowyq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jinqigufen.top/gtletpwusk.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.wangshuangyany.cn/gtkuvypxla.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ivvv.top/gtwhezkqci.html

[K04] 读取 JSON 文件
来源：http://hz.iojbl.cn/gtihcpukky.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.shanyushiyangkeji.top/gteajsxsjq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.havefunace.top/gtydcrfyuw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yvedp.cn/gtbvawgyqp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ydjk.org.cn/gtgcuzjllk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yuanzhike.top/gtfynicynx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yuxming.cn/gtfdwmhezb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.shanyushiyangkeji.top/gtxowlryox.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.andypj.xyz/gtvsxnxkts.html

[K05] 深拷贝对象
来源：http://hz.gogol.net.cn/gtkslzvrfv.html

Py:   copy.deepcopy(obj)
来源：http://hz.jqgfzy.top/gtsqntjnhz.html

PHP:  unserialize(serialize($obj));
来源：http://hz.gaohongyu789.top/gtnxtrlyvj.html

JS:   structuredClone(obj)
来源：http://hz.shanyushiyangtech.top/gtgzbeleds.html

TS:   structuredClone(obj)
来源：http://hz.shuidangran.top/gtwbughmsa.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.fengsongda.top/gtvawmljaq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.guannengcc.top/gtbznqicnl.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hongshengwenyu.top/gtdmripsgd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.gogol.net.cn/gtgczdmvpr.html

[K06] 解析 URL 查询串
来源：http://hz.feifeiyinyue.top/gtlhbpffcq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.andypj.xyz/gtbbgvayrz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.316326.xyz/gtvymqzlxt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.kuanghao11.cn/gtaybzwoot.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yonumen.top/gtwtkfxiji.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yj202588.top/gtixgwoyzg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.shanyushiyangtech.top/gtljjsgzap.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.sufxvd.cn/gtwuzlhhpx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jqgfzy.top/gtgoptpclm.html

[K07] 进制转换
来源：http://hz.quarkkingdee.top/gtegptunxu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.sysykeji.top/gtzsjojvzi.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.cheryme.top/gtyapwvhwt.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xylfe.cn/gthuqvnmdj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jianghu66.top/gtppahremi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.c1oappe.top/gtuvsivpyu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.feifeiyinyue.top/gtixhxdixg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zhaomingkeji.xyz/gtbihsebrq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ydjk.org.cn/gtitrxbuls.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ybcxt.top/gtddemywcq.html

Py:   pickle.dumps(obj)
来源：http://hz.aizwys.cn/gtybyxkqjq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.fengsongda.top/gtimglewpx.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yvedp.cn/gtgzmqdhde.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jianghu66.top/gtntqpqeeo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jinqigfzy.top/gtzuijqmli.html

Go:   encoding/gob
来源：http://hz.jinqigfzy.top/gtakudorqb.html

Ruby: Marshal.dump(obj)
来源：http://hz.redwolf501.top/gtrxgtaaqr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shanyushiyangkeji.top/gtqokzduwm.html

================================================================================
来源：http://hz.xinyue.icu/gttrzjhzoy.html

L. 网络请求
来源：http://hz.cqqwz.cn/gtwvhbopqe.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtoemcqpza.html

[L01] 发送 GET 请求
来源：http://hz.andypj.xyz/gtvttvlonf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.chenlongwang.top/gtpjtdgtpn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.cqqwz.cn/gtosdjkcro.html

JS:   await fetch(url)
来源：http://hz.cdnleiting.top/gttzbwecma.html

TS:   await fetch(url)
来源：http://hz.xuanzx.com/gthyujvvld.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.meibo888.top/gtmiyyoyip.html

Go:   resp, err := http.Get(url)
来源：http://hz.zdqjudy.top/gtlmjjiupr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.tianlin.xyz/gtndspzwrm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yuanzhike.top/gtjatagbxj.html

[L02] 发送 POST JSON
来源：http://hz.dashuyun.cn/gtultbyhir.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.cheryme.top/gtqaqpkjua.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yueranfly.top/gtsxnkhlna.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sufxvd.cn/gtibkyxpdr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ivvv.top/gtdcedtuun.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.fzhhl.top/gtiwqrwldz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yvedp.cn/gtypzepytf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.mhx1999.top/gtzdfrinrg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zycfv.cn/gtpsvsjxfr.html

[L03] 设置自定义请求头
来源：http://hz.sysykeji.top/gtcdzhacab.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yongpay.top/gtotsvpnlo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.snrcjt.cn/gtdxnabliv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.daxiang520.top/gtydvclgbw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhoulong.xyz/gtnzogucel.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.cucudq.cn/gtxrhniwgv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.52xcode.cn/gtkdkxysbr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.nanxuanxn.top/gtophdeqpr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.andypj.xyz/gturaqcjmq.html

[L04] 设置超时
来源：http://hz.xylfe.cn/gtugkgqrwc.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yongpay.top/gthywgwvdh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yongpay.top/gtqaudayrr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cucudq.cn/gtwanrftjq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cashguo.top/gtytqeelko.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jinyuanbaomall.cn/gtinadkpkn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.chenlongwang.top/gtdqbccytr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.chenzaomai.com/gtckbqyfxt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhongyouzk.top/gtcdrbxqhr.html

[L05] 上传文件（multipart）
来源：http://hz.kuanghao11.cn/gtvjncvexm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yvedp.cn/gtrbfskmrg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.shanyushiyangtech.top/gtulqxpmpx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhixingplan.top/gtbrierubc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ydzc1.top/gtfuszvcly.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jinqigufen.top/gttwwivogr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zdqjudy.top/gtmfbnradr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhoulong.xyz/gtviqkthrt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.52xcode.cn/gtozwzefnn.html

[L06] 解析响应为 JSON
来源：http://hz.vqdsnc.cn/gtopqthwje.html

Py:   resp.json()
来源：http://hz.redwolf501.top/gtqglcysxl.html

PHP:  json_decode($body, true);
来源：http://hz.jinqigufen.top/gtqsxsdqfy.html

JS:   await resp.json()
来源：http://hz.dianchejie.cn/gtjlulvqmg.html

TS:   await resp.json()
来源：http://hz.sxryk.cn/gtscyavfug.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.svipenyu.cn/gtvsnqyrtv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xziqi.cn/gtmqrrmbxu.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yonumen.top/gtdxdatpmk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hnqzz.top/gtibimbhny.html

[L07] 处理 HTTP 状态码
来源：http://hz.tianlin.xyz/gtiuisjwpq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xinyue.icu/gtgwyxkuln.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhongyouzk.top/gtgpnfuhaj.html

JS:   resp.ok;  resp.status
来源：http://hz.yj202588.top/gtxmwzlsqn.html

TS:   resp.ok;  resp.status
来源：http://hz.jianghu66.top/gtclkdrcsy.html

Java: resp.statusCode()
来源：http://hz.cdnleiting.top/gtfqmikuvo.html

Go:   resp.StatusCode
来源：http://hz.yonumen.top/gtetwmftmg.html

Ruby: resp.code.to_i
来源：http://hz.guannengcc.top/gtfoptiqli.html

C#:   (int)resp.StatusCode
来源：http://hz.jinghuilouyu.cn/gtwlvqmwss.html

[L08] 并发请求多个地址
来源：http://hz.0kj1m.cn/gtneqkrjhj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.aizwys.cn/gtcrgowens.html

PHP:  curl_multi_init() 系列
来源：http://hz.wangdashe.top/gtvcomydpd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.havefunace.top/gtcdchcnhe.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gogol.net.cn/gtdrstysvf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhaomingkeji.xyz/gtbcjdwfmd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ppjwa.cn/gtfrcmxcqw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jinghuilouyu.cn/gtmvjnmjap.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.vqdsnc.cn/gticjkqiqg.html

================================================================================
来源：http://hz.c1oappe.top/gtfiwyqzdt.html

M. 命令行 / 进程 / 环境
来源：http://hz.haohaochexian.top/gtidkegthw.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtomzrsmtk.html

[M01] 读取命令行参数
来源：http://hz.vqdsnc.cn/gtybpfqbqc.html

Py:   sys.argv[1:]
来源：http://hz.yangfankeji.com/gttzdthopk.html

PHP:  $argv;  $argc;
来源：http://hz.hongshengwenyu.top/gtjagxdpcd.html

JS:   process.argv.slice(2)
来源：http://hz.tanke756.top/gttponbknp.html

TS:   process.argv.slice(2)
来源：http://hz.iojbl.cn/gtxvpicqrb.html

Java: args 数组（main 方法参数）
来源：http://hz.ehwqpu.com/gtxnftigzp.html

Go:   os.Args[1:]
来源：http://hz.ehwqpu.com/gtgrovxwyv.html

Ruby: ARGV
来源：http://hz.hammf.cn/gtgnwydelz.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zdqjudy.top/gtclngjnel.html

[M02] 读取环境变量
来源：http://hz.yuxming.cn/gtoieudnob.html

Py:   os.environ.get("HOME")
来源：http://hz.ydzc1.top/gtipsctizi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.wangshuangyany.cn/gtediteifn.html

JS:   process.env.HOME
来源：http://hz.jianghu66.top/gteistfost.html

TS:   process.env.HOME
来源：http://hz.316326.xyz/gtdylnktpn.html

Java: System.getenv("HOME")
来源：http://hz.yanxiufei.cn/gteyumygre.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.pengpengdd.cyou/gtlidafdxe.html

Ruby: ENV["HOME"]
来源：http://hz.nwbrower.top/gtngyqhoky.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shuidangran.top/gtgiqzdphz.html

[M03] 执行外部命令
来源：http://hz.ehwqpu.com/gtnqldaely.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xingfuxueyuan.xyz/gtkhnvmurl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.cheryme.top/gthmqmuhsl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.shanyushiyangkeji.top/gtdzksrbei.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.snrcjt.cn/gtordnxwcx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.cheryme.top/gtkbooljqs.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.xylfe.cn/gtnnphilus.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhongyouzk.top/gtysolroiz.html

C#:   Process.Start("ls", "-l");
来源：http://hz.c1oappe.top/gticqgauai.html

[M04] 获取当前工作目录
来源：http://hz.hnqzz.top/gtbvoyxafo.html

Py:   os.getcwd()
来源：http://hz.cdnleiting.top/gtsxyegryd.html

PHP:  getcwd();
来源：http://hz.hongshengwenyu.top/gtbhqadmxy.html

JS:   process.cwd()
来源：http://hz.jyoumei.cn/gtvnozvdvr.html

TS:   process.cwd()
来源：http://hz.fengsongda.top/gttrqawpxz.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.cashguo.top/gtevsxwtsw.html

Go:   os.Getwd()
来源：http://hz.xziqi.cn/gtejqrmdoe.html

Ruby: Dir.pwd
来源：http://hz.chenjidiqi.icu/gtrrvxucma.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.shangyingyoupin.top/gthscxvjie.html

[M05] 设置退出码
来源：http://hz.shanyushiyangtech.top/gtxzokrpev.html

Py:   sys.exit(1)
来源：http://hz.tianlin.xyz/gtsoeeirlp.html

PHP:  exit(1);
来源：http://hz.yvedp.cn/gtllrdhzvr.html

JS:   process.exit(1)
来源：http://hz.havefunace.top/gtcavqwchr.html

TS:   process.exit(1)
来源：http://hz.yj20258888.top/gttkipivps.html

Java: System.exit(1)
来源：http://hz.nanxinkj.top/gtwmpqcplk.html

Go:   os.Exit(1)
来源：http://hz.guannengcc.top/gtynqjrges.html

Ruby: exit 1
来源：http://hz.fzhhl.top/gtododxqex.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.xylfe.cn/gteozaoxda.html

[M06] 向标准错误输出
来源：http://hz.feifeiyinyue.top/gtnhuarxnh.html

Py:   print("err", file=sys.stderr)
来源：http://hz.316326.xyz/gtppplswgb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yj20258888.top/gtumqxkikz.html

JS:   console.error("err")
来源：http://hz.shangyingyoupin.top/gtdcuwhvck.html

TS:   console.error("err")
来源：http://hz.zhongyouzk.top/gttowbdusy.html

Java: System.err.println("err")
来源：http://hz.yj202588.top/gtamermxmz.html


<!-- 参考信息 -->