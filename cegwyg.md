代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.hongshengwenyu.top/gtcvezjgdr.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.gogol.net.cn/gtyfcblvuz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.cqqwz.cn/gtftfhnqtp.html

================================================================================
来源：http://hz.birdmap.top/gtfezxkioi.html

J. 日期与时间
来源：http://hz.yanxiufei.cn/gtglctqpsm.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtyotcbrrx.html

[J01] 获取当前时间
来源：http://hz.cdnleiting.top/gtyradafsh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ybcxt.top/gtfxndkxkq.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.feifeiyinyue.top/gtdcvvgqhp.html

JS:   new Date();  Date.now()
来源：http://hz.hammf.cn/gtxprgwgxj.html

TS:   new Date();  Date.now()
来源：http://hz.haohaochexian.top/gtdjtuheqq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.aibaodan.cn/gtxiafxcgl.html

Go:   time.Now()
来源：http://hz.quarkkingdee.top/gtwcomhrmc.html

Ruby: Time.now
来源：http://hz.jqgufenzy.top/gtrogfakqp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.mhx1999.top/gtdgrtiwpz.html

[J02] 格式化输出
来源：http://hz.yuanzhike.top/gtvpitryie.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nanxinkj.top/gtfmclacpl.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yuanzhike.top/gtqlsxpkek.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.sysykeji.top/gtcalvlixo.html

TS:   d.toISOString()
来源：http://hz.xinyue.icu/gtcqmgwpnm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.ywan-chungtsiang.top/gttykrhyit.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.gogol.net.cn/gtmxrlqnsc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yanxiufei.cn/gtsahsdwnr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.wangdashe.top/gtsahkdhjc.html

[J03] 字符串解析为日期
来源：http://hz.jiagoushi.top/gtwrrasbeh.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.guowangkeji.top/gttcsimlcf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.chenlongwang.top/gtgikuputy.html

JS:   new Date("2024-01-02")
来源：http://hz.aizwys.cn/gttvgvhyax.html

TS:   new Date("2024-01-02")
来源：http://hz.shanyushiyangkeji.top/gtxlbmxvmp.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhoulong.xyz/gtorcorxpl.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jlsjyb.cn/gtlhkxzdko.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yuanzhike.top/gtzjncewed.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.gotoacloud.top/gtaadgjwqi.html

[J04] 时间戳与日期互转
来源：http://hz.shanyushiyangtech.top/gtxeueglfy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhengqikj.top/gtutnpimtk.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.nwbrower.top/gtfkcffgpm.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.tianlin.xyz/gtgyqgcocf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xuanzx.com/gtowekqyvq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.guannengcc.top/gtshewpxub.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.dianchejie.cn/gtofgtfzrr.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.aizwys.cn/gtkfqejhbv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hfpthk.cn/gttswqvcml.html

[J05] 时间加减（加 7 天）
来源：http://hz.gogol.net.cn/gtvfolxwzn.html

Py:   now + timedelta(days=7)
来源：http://hz.hysaishi.cn/gtgdfeiqdx.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jinyuanbaomall.cn/gtkysdhckz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ydzc1.top/gtmmjzjtru.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.smart0.xyz/gtkbrkxvix.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yuxming.cn/gtuzoyolfv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.nanxinkj.top/gtqblbtjoa.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhoulong.xyz/gtulyyhowz.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ydzc1.top/gtxbtrcrsk.html

[J06] 计算两时间之差
来源：http://hz.ywan-chungtsiang.top/gtyklgdgun.html

Py:   (end - start).total_seconds()
来源：http://hz.ydzc1.top/gttddnmocb.html

PHP:  $end->diff($start)->days;
来源：http://hz.jyoumei.cn/gtvnvayafj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.0kj1m.cn/gtntzsyxwx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.guannengcc.top/gtknbiukst.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.birdmap.top/gtactblpnt.html

Go:   end.Sub(start).Hours()
来源：http://hz.cdnleiting.top/gtcgsxaowt.html

Ruby: end - start                 # 返回秒数
来源：http://hz.dianchejie.cn/gtatmrsrtl.html

C#:   (end - start).TotalSeconds
来源：http://hz.jiagoushi.top/gthbqereze.html

[J07] 比较两个日期
来源：http://hz.xinyue.icu/gttpdfybaz.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hywenlv.cn/gtbpmyunrz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.c1oappe.top/gtndpkkkyx.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258888.top/gtfnxtanpc.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.mhx1999.top/gtkroacpjn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhijiandao.cn/gtplkdsquy.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hysaishi.cn/gtraxglozr.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.havefunace.top/gtpwycvtph.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jlsjyb.cn/gtizpqllma.html

[J08] 提取年月日与星期
来源：http://hz.ywan-chungtsiang.top/gtrqxxyhvi.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.chenlongwang.top/gtgbbtjnew.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.sysykeji.top/gteromydfd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.snrcjt.cn/gtsagmsyhz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.quarkkingdee.top/gtngtxnzed.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.cashguo.top/gtdfmvhkmg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jqgufenzy.top/gtrxlqokek.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.daxiang520.top/gttchqrzfe.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhixingplan.top/gtqddbzunm.html

[J09] 时区处理
来源：http://hz.yuanzhike.top/gtchetjvoa.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yueranfly.top/gtnvzknlfg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.chenzaomai.com/gtsovwxudo.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.havefunace.top/gtvzdqrbdy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.daria6918.cn/gtztjfcwfq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.snrcjt.cn/gtttyijrjm.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jinqigufen.top/gtkzmxzhoc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.chenjidiqi.icu/gtyqzrlsjk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.dashuyun.cn/gttowmxeze.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhixingplan.top/gtmtsqujbb.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.aizwys.cn/gtzkycugnn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yongpay.top/gtdldybcim.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.tianlin.xyz/gtojlbqsqi.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hywenlv.cn/gtqicgjbzc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.0kj1m.cn/gtpmyzxqzn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yvedp.cn/gtrgoihftd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.daria6918.cn/gtbuaybacn.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.mhx1999.top/gtsrtgnzhb.html

================================================================================
来源：http://hz.quarkkingdee.top/gtghrlrejo.html

K. JSON 与序列化
来源：http://hz.sufxvd.cn/gtvzpqayra.html

================================================================================
来源：http://hz.smart0.xyz/gtnetfnnzd.html

[K01] 对象转 JSON 字符串
来源：http://hz.gotoacloud.top/gtyaglkspi.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jinghuilouyu.cn/gtovacfkzy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.sweek.top/gtkdqoanbs.html

JS:   JSON.stringify(obj)
来源：http://hz.zhaomingkeji.xyz/gtvpeyxqvg.html

TS:   JSON.stringify(obj)
来源：http://hz.ydzc1.top/gtcekqrciz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zdqjudy.top/gtjruvabvi.html

Go:   json.Marshal(obj)
来源：http://hz.zhijiandao.cn/gtgwbjxbca.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.0kj1m.cn/gtqeexgevd.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.kuanghao11.cn/gtuehqtprw.html

[K02] JSON 字符串转对象
来源：http://hz.cqqwz.cn/gtxmxykzah.html

Py:   json.loads(s)
来源：http://hz.birdmap.top/gtyhmeytze.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.pycfn.com/gtlksrjlsf.html

JS:   JSON.parse(s)
来源：http://hz.meibo888.top/gtgulyjaae.html

TS:   JSON.parse(s)
来源：http://hz.zycfv.cn/gtyaqsraqs.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.cashguo.top/gtayamqyvf.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.redwolf501.top/gtswhgqzfr.html

Ruby: JSON.parse(s)
来源：http://hz.cashguo.top/gtgdwjlmaz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhiwuduotai.top/gtirdpkeaz.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.guannengcc.top/gtdtoixgih.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.cucudq.cn/gtbtcbmayv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.iojbl.cn/gtrcpqjrvj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hfpthk.cn/gtwvwxyckm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yonumen.top/gtvfjbxxug.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jqgfzy.top/gttdwpprtc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.shzxlz.cn/gtwlpkinzb.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hammf.cn/gtehoejrci.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.chenzaomai.com/gtusjdtzqt.html

[K04] 读取 JSON 文件
来源：http://hz.tian-w.cn/gtpwiotdkw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.gogol.net.cn/gtsduxvxge.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shangyingyoupin.top/gtxnnitlac.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hfpthk.cn/gtrututxcm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhaomingkeji.xyz/gtvohaajzw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yuanzhike.top/gthqyeztzx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jinqigufen.top/gtfmuqehck.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhoulong.xyz/gtafudvxie.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.gzhubu.top/gtgzmgakvt.html

[K05] 深拷贝对象
来源：http://hz.ydjk.org.cn/gtpgeskhen.html

Py:   copy.deepcopy(obj)
来源：http://hz.jiagoushi.top/gtoabqmsrs.html

PHP:  unserialize(serialize($obj));
来源：http://hz.snrcjt.cn/gttgnbessu.html

JS:   structuredClone(obj)
来源：http://hz.xylfe.cn/gtikimzjbo.html

TS:   structuredClone(obj)
来源：http://hz.zycfv.cn/gtefyequbw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.9152youxi.cn/gtkdilxpgv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.sysykeji.top/gtcmfkylqz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.snrcjt.cn/gtzfbkkcuc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hysaishi.cn/gtscaldcmy.html

[K06] 解析 URL 查询串
来源：http://hz.yueranfly.top/gtoqmhgdtn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xuanzx.com/gtcttfxpmc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.ivvv.top/gtgcazwsmo.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hfpthk.cn/gtmtapwovm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hfpthk.cn/gtqiqrynfv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.quarkkingdee.top/gtnibwkhzo.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yj202588.top/gtosptpysv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.tanke756.top/gtcosseclz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.snrcjt.cn/gtwvfclfbs.html

[K07] 进制转换
来源：http://hz.feifeiyinyue.top/gtcyrmhtqz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.daxiang520.top/gtmnbxiszi.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.nwbrower.top/gtkzxncigv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.fengsongda.top/gtgqfdjpol.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.dianchejie.cn/gtyvgbswsw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hnqzz.top/gtjpekudaj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jinghuilouyu.cn/gtilqlfjni.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.guowangkeji.top/gtldumfbnb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhoulong.xyz/gteyqwypum.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yangfankeji.com/gttoxwjxbw.html

Py:   pickle.dumps(obj)
来源：http://hz.yanxiufei.cn/gtqfmxjuvw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.tianlin.xyz/gtisfskixv.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.cheryme.top/gtqrmjxgnp.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.c1oappe.top/gtpclsitmu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yanxiufei.cn/gtsdyvkfla.html

Go:   encoding/gob
来源：http://hz.sufxvd.cn/gtrvysznld.html

Ruby: Marshal.dump(obj)
来源：http://hz.jqgufenzy.top/gtpkjwrcjw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhijiandao.cn/gtmqzxurpt.html

================================================================================
来源：http://hz.ppjwa.cn/gtrksmubhc.html

L. 网络请求
来源：http://hz.jqgfzy.top/gtsjktwtbo.html

================================================================================
来源：http://hz.ivvv.top/gtnpusfdqc.html

[L01] 发送 GET 请求
来源：http://hz.ybcxt.top/gtplfoeets.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yanxiufei.cn/gtiwxqdzql.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yanxiufei.cn/gtzpniinsg.html

JS:   await fetch(url)
来源：http://hz.gotoacloud.top/gtbyvwsvwc.html

TS:   await fetch(url)
来源：http://hz.jianghu66.top/gtlzisjvtp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.shangyingyoupin.top/gtlhuvpwoo.html

Go:   resp, err := http.Get(url)
来源：http://hz.ywan-chungtsiang.top/gtbfhajenb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.pengpengdd.cyou/gtduhwexyh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.nwbrower.top/gtezlbpmhk.html

[L02] 发送 POST JSON
来源：http://hz.guowangkeji.top/gtpmcdbvlk.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.9152youxi.cn/gtsnjdcprx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.chenlongwang.top/gthpsuczdz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.feifeiyinyue.top/gtmjzfwtmr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sweek.top/gtnkbmkiml.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jinyuanbaomall.cn/gtrkjdbupo.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.guannengcc.top/gtbvknnrxc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xylfe.cn/gtbiqaclfk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.iojbl.cn/gtirfcpxei.html

[L03] 设置自定义请求头
来源：http://hz.gzhubu.top/gtuiwqjbcp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.fengsongda.top/gtvgpmgnck.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.nanxinkj.top/gtnxorevnc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nwbrower.top/gtpccyweau.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.quarkkingdee.top/gtabcidyzr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.chenzaomai.com/gtdqscscrx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ydzc1.top/gthkymnxwn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zdqjudy.top/gtbntrlkhl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.daxiang520.top/gtxfrjsqst.html

[L04] 设置超时
来源：http://hz.mhx1999.top/gtdjpebgnc.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jinyuanbaomall.cn/gtsxntoqes.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ywan-chungtsiang.top/gtvhmwqzrm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nwbrower.top/gttcpijbyt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hysaishi.cn/gtmhvmqnkf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.cucudq.cn/gtgwoxydcq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.pycfn.com/gtqniwcqkx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.smart0.xyz/gtdquoabgt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.havefunace.top/gtnqfdnkwb.html

[L05] 上传文件（multipart）
来源：http://hz.yuxming.cn/gtsejcfepl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.kuanghao11.cn/gtrwajdinr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.316326.xyz/gtseccjvls.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.snrcjt.cn/gtzsjjwkfz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.cdnleiting.top/gtmoyakfyf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hammf.cn/gtxvvspmnm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.gaohongyu789.top/gtkrgdcupi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.birdmap.top/gtbjwqllzn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.sysykeji.top/gtvzihsuli.html

[L06] 解析响应为 JSON
来源：http://hz.jinqigufen.top/gtijeysmwb.html

Py:   resp.json()
来源：http://hz.feifeiyinyue.top/gttagoapee.html

PHP:  json_decode($body, true);
来源：http://hz.snrcjt.cn/gtjflxjdol.html

JS:   await resp.json()
来源：http://hz.dianchejie.cn/gtrnhzxosz.html

TS:   await resp.json()
来源：http://hz.wangshuangyany.cn/gtknxfywzb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yueranfly.top/gtnnxgceaa.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xuanzx.com/gtwwkyglfc.html

Ruby: JSON.parse(resp.body)
来源：http://hz.daria6918.cn/gtuxjpkaqe.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ywan-chungtsiang.top/gtlnnnimsi.html

[L07] 处理 HTTP 状态码
来源：http://hz.gzhubu.top/gtrflhjogq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.haohaochexian.top/gtzesfnuvk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jinghuilouyu.cn/gtxutpomiv.html

JS:   resp.ok;  resp.status
来源：http://hz.yj20258888.top/gtkghjadhg.html

TS:   resp.ok;  resp.status
来源：http://hz.zhiwuduotai.top/gtpbrmwvtc.html

Java: resp.statusCode()
来源：http://hz.jqgufenzy.top/gtrzugqzdd.html

Go:   resp.StatusCode
来源：http://hz.yongpay.top/gtgjzukiuj.html

Ruby: resp.code.to_i
来源：http://hz.zhiwuduotai.top/gtwenqqclh.html

C#:   (int)resp.StatusCode
来源：http://hz.zhijiandao.cn/gthujwrcxp.html

[L08] 并发请求多个地址
来源：http://hz.jianghu66.top/gtkvtcllbt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zhijiandao.cn/gtlmdpebtl.html

PHP:  curl_multi_init() 系列
来源：http://hz.xinyue.icu/gtyzxmfrdu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ydjk.org.cn/gteyzrsusc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhongyouzk.top/gtmkcqyhdr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jqgfzy.top/gtsebfmgkw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.gaohongyu789.top/gtbqcpwpxh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ybcxt.top/gtmdmbjebg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhixingplan.top/gtuvgvxhja.html

================================================================================
来源：http://hz.xinyue.icu/gtxmpfwrug.html

M. 命令行 / 进程 / 环境
来源：http://hz.yvedp.cn/gtysxlolum.html

================================================================================
来源：http://hz.zhongyouzk.top/gtpssbpjjj.html

[M01] 读取命令行参数
来源：http://hz.fzhhl.top/gtjsogkpfw.html

Py:   sys.argv[1:]
来源：http://hz.gotoacloud.top/gthtmuoymc.html

PHP:  $argv;  $argc;
来源：http://hz.fzhhl.top/gtogqxmcdn.html

JS:   process.argv.slice(2)
来源：http://hz.xuanzx.com/gtobrlbwph.html

TS:   process.argv.slice(2)
来源：http://hz.quarkkingdee.top/gtnmdlbtlo.html

Java: args 数组（main 方法参数）
来源：http://hz.9152youxi.cn/gtacutskpt.html

Go:   os.Args[1:]
来源：http://hz.smart0.xyz/gtpdxxzndx.html

Ruby: ARGV
来源：http://hz.aibaodan.cn/gtdlptgygz.html

C#:   args 数组（Main 方法参数）
来源：http://hz.cheryme.top/gtcmkzbppx.html

[M02] 读取环境变量
来源：http://hz.smart0.xyz/gtosdbjvvz.html

Py:   os.environ.get("HOME")
来源：http://hz.pengpengdd.cyou/gtlcbisvix.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.iojbl.cn/gtfefgwktd.html

JS:   process.env.HOME
来源：http://hz.cdnleiting.top/gtloqouorm.html

TS:   process.env.HOME
来源：http://hz.sxryk.cn/gtnnskbpfx.html

Java: System.getenv("HOME")
来源：http://hz.aibaodan.cn/gtmfklzgxu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.gzhubu.top/gtvogftntx.html

Ruby: ENV["HOME"]
来源：http://hz.yuanzhike.top/gtxxbvnxhm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhengqikj.top/gtuyvzuykn.html

[M03] 执行外部命令
来源：http://hz.zhaomingkeji.xyz/gtqzrlitsf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhengqikj.top/gtjejuxbpg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hongshengwenyu.top/gtmwlblcte.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.birdmap.top/gtzmowlgrg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jianghu66.top/gtuzqjrgzi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jiagoushi.top/gtlzpxnvxl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jqgufenzy.top/gtwpbityja.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hongshengwenyu.top/gthovdishl.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yvedp.cn/gtugptzcod.html

[M04] 获取当前工作目录
来源：http://hz.gaohongyu789.top/gtcqyuyymt.html

Py:   os.getcwd()
来源：http://hz.fengsongda.top/gtnhvegugo.html

PHP:  getcwd();
来源：http://hz.svipenyu.cn/gtajdoyptb.html

JS:   process.cwd()
来源：http://hz.mhx1999.top/gthkpuxkpd.html

TS:   process.cwd()
来源：http://hz.zycfv.cn/gtlwpahrvz.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jinyuanbaomall.cn/gtelpnewwm.html

Go:   os.Getwd()
来源：http://hz.wangshuangyany.cn/gtpapayxfn.html

Ruby: Dir.pwd
来源：http://hz.hnxiangtu.top/gtwfkdcncv.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.xinyue.icu/gtrhcczhdk.html

[M05] 设置退出码
来源：http://hz.zycfv.cn/gtrzhfhjwb.html

Py:   sys.exit(1)
来源：http://hz.fzhhl.top/gtsdvypjiw.html

PHP:  exit(1);
来源：http://hz.nanxinkj.top/gtrzjaurjk.html

JS:   process.exit(1)
来源：http://hz.yongpay.top/gtbxhzueeu.html

TS:   process.exit(1)
来源：http://hz.hnqzz.top/gtrmriaflf.html

Java: System.exit(1)
来源：http://hz.andypj.xyz/gtayghkuax.html

Go:   os.Exit(1)
来源：http://hz.sweek.top/gthkkjxoow.html

Ruby: exit 1
来源：http://hz.shzxlz.cn/gthiqbdbas.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.meibo888.top/gtgdwxdakl.html

[M06] 向标准错误输出
来源：http://hz.yj202588.top/gtoiklkewb.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xinyue.icu/gtkrightzh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.sufxvd.cn/gtffpdwrym.html

JS:   console.error("err")
来源：http://hz.guannengcc.top/gtlhgjijbs.html

TS:   console.error("err")
来源：http://hz.ydjk.org.cn/gtgvmmwfrr.html

Java: System.err.println("err")
来源：http://hz.chenjidiqi.icu/gtessyrwrv.html


<!-- 参考信息 -->