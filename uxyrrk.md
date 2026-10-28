代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.wangdashe.top/gtdecgocst.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.nwbrower.top/gtjaduuken.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xuanzx.com/gtjsnttzpc.html

================================================================================
来源：http://hz.52xcode.cn/gtyrdsewue.html

J. 日期与时间
来源：http://hz.nwbrower.top/gtsnamddpl.html

================================================================================
来源：http://hz.hammf.cn/gttvyjmxsj.html

[J01] 获取当前时间
来源：http://hz.guowangkeji.top/gtczrjceet.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.mhx1999.top/gtrmfpxcul.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.shuidangran.top/gtqtvrbslu.html

JS:   new Date();  Date.now()
来源：http://hz.ydjk.org.cn/gtrgyhmhnw.html

TS:   new Date();  Date.now()
来源：http://hz.hammf.cn/gtytvbmytx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.wangshuangyany.cn/gtylkrrnbx.html

Go:   time.Now()
来源：http://hz.cheryme.top/gtaguofnmc.html

Ruby: Time.now
来源：http://hz.zhixingplan.top/gtqjjstnsq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yongpay.top/gtspljgjeo.html

[J02] 格式化输出
来源：http://hz.yuxming.cn/gttdrxjywo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.c1oappe.top/gtzrrbzskp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.cashguo.top/gtbzwxjzvq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.daria6918.cn/gtbsbdvjjj.html

TS:   d.toISOString()
来源：http://hz.yanxiufei.cn/gtrnrcrmlu.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.tanke756.top/gthcfhgklp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.316326.xyz/gtydwhxlrc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yuanzhike.top/gtsghoqkpq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jinqigfzy.top/gtovqziqyp.html

[J03] 字符串解析为日期
来源：http://hz.jlsjyb.cn/gtlxvdbfxt.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.shanyushiyangkeji.top/gtnjylrrhx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.havefunace.top/gttilyhrgg.html

JS:   new Date("2024-01-02")
来源：http://hz.jinqigufen.top/gttnvdlqmb.html

TS:   new Date("2024-01-02")
来源：http://hz.guowangkeji.top/gtmdzmfdbm.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.smart0.xyz/gtmkgrwzhc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhijiandao.cn/gtuwoilgwn.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.wangdashe.top/gtfdeseqoi.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xinyue.icu/gtzfycclpz.html

[J04] 时间戳与日期互转
来源：http://hz.zhongyouzk.top/gtzeabozoo.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.guannengcc.top/gtpfmnongy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.gaohongyu789.top/gtkpgmskiq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yj20258888.top/gtyqikzgjc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yj20258.top/gtdityhccj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ybcxt.top/gtnakfpgce.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hongshengwenyu.top/gttrzcsrvw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.fzhhl.top/gtluskmlcz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yangfankeji.com/gtzsqvfefp.html

[J05] 时间加减（加 7 天）
来源：http://hz.jianghu66.top/gtueppomhk.html

Py:   now + timedelta(days=7)
来源：http://hz.yuxming.cn/gtozygtref.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jinghuilouyu.cn/gtesyktmlq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.wangshuangyany.cn/gtvzennbix.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhixingplan.top/gtmobmnkye.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.havefunace.top/gtsydepljw.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.shanyushiyangkeji.top/gtmketrmch.html

Ruby: Time.now + 7 * 86400
来源：http://hz.pengpengdd.cyou/gtlhvfcokf.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.nanxinkj.top/gtxlocmina.html

[J06] 计算两时间之差
来源：http://hz.xylfe.cn/gtambvqndg.html

Py:   (end - start).total_seconds()
来源：http://hz.pycfn.com/gtjatbmtml.html

PHP:  $end->diff($start)->days;
来源：http://hz.feifeiyinyue.top/gtduzqmqnz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hywenlv.cn/gtyvnmnfco.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jinqigufen.top/gtnbherrrh.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ehwqpu.com/gthckdejbz.html

Go:   end.Sub(start).Hours()
来源：http://hz.yueranfly.top/gtmfhpjlyo.html

Ruby: end - start                 # 返回秒数
来源：http://hz.316326.xyz/gtgcliknvw.html

C#:   (end - start).TotalSeconds
来源：http://hz.yuxming.cn/gtnsouuzey.html

[J07] 比较两个日期
来源：http://hz.chenjidiqi.icu/gtuodzdaru.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hnqzz.top/gtrzcdbcqp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.guannengcc.top/gtkmeybaqb.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.0kj1m.cn/gtgrehmyaz.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jqgufenzy.top/gtmothssym.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.9152youxi.cn/gtujhllgnq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jyoumei.cn/gtkyodyskw.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xingfuxueyuan.xyz/gtlmabzlbk.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.gaohongyu789.top/gtgobbuucz.html

[J08] 提取年月日与星期
来源：http://hz.ybcxt.top/gtysddfkym.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhaomingkeji.xyz/gttyeslzmx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.haohaochexian.top/gtgbceyrbl.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jyoumei.cn/gtdazjahdy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jinghuilouyu.cn/gtjbymzfey.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jinghuilouyu.cn/gtzvowywmu.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yueranfly.top/gtisfvfkhr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ybcxt.top/gtzzritlbz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.gogol.net.cn/gtdazxjnvn.html

[J09] 时区处理
来源：http://hz.xingfuxueyuan.xyz/gtszanoeic.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yj202588.top/gtushmjafz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ppjwa.cn/gtmobvsqzc.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yongpay.top/gtnydocrgd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.iojbl.cn/gtrumpqpgd.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zycfv.cn/gthmpglxfb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.nanxinkj.top/gtjoigoklb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.0kj1m.cn/gtzbkpycjc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.havefunace.top/gtzqudefbr.html

[J10] 取今天 / 本月第一天
来源：http://hz.tian-w.cn/gtnkutijbe.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hysaishi.cn/gtjcmbrrxu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhixingplan.top/gthvlmqwuu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.aibaodan.cn/gtgakhdmgy.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.xuanzx.com/gtrlrgidox.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jyoumei.cn/gtbldmphat.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hywenlv.cn/gtkcirrvht.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ydzc1.top/gtnmwdufis.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.gotoacloud.top/gtxbdtznkk.html

================================================================================
来源：http://hz.gogol.net.cn/gtkkohplzc.html

K. JSON 与序列化
来源：http://hz.ydjk.org.cn/gtbiotiybj.html

================================================================================
来源：http://hz.daxiang520.top/gtyzpkeawv.html

[K01] 对象转 JSON 字符串
来源：http://hz.yj20258.top/gtmehvbcjt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.tanke756.top/gtwliibfok.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yuanzhike.top/gtdbckqrwh.html

JS:   JSON.stringify(obj)
来源：http://hz.zhongyouzk.top/gtuaohpdki.html

TS:   JSON.stringify(obj)
来源：http://hz.ydjk.org.cn/gtivwlfsur.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.andypj.xyz/gtkbworfly.html

Go:   json.Marshal(obj)
来源：http://hz.kuanghao11.cn/gtsoryfosu.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cucudq.cn/gtfaosxutw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.tanke756.top/gtwcenneyl.html

[K02] JSON 字符串转对象
来源：http://hz.hnqzz.top/gtdkgqyzwq.html

Py:   json.loads(s)
来源：http://hz.smart0.xyz/gtyksiyjms.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.vqdsnc.cn/gtzhptpgwf.html

JS:   JSON.parse(s)
来源：http://hz.zdqjudy.top/gtuakzxztp.html

TS:   JSON.parse(s)
来源：http://hz.xuanzx.com/gtmqkezjtq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.52xcode.cn/gtgdsvmwqr.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.sysykeji.top/gtgswtsxoi.html

Ruby: JSON.parse(s)
来源：http://hz.birdmap.top/gtfcnvtxwn.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.sysykeji.top/gtuuhewzbv.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jyoumei.cn/gtawjhtuxu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.dashuyun.cn/gtzwnhrdcq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.aibaodan.cn/gtppaefgun.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shuidangran.top/gtkogebpaz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yvedp.cn/gtubhypdgs.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.xinyue.icu/gtbwyetbvw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xziqi.cn/gtoawvbfqs.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yvedp.cn/gtpfxzrmed.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.gaohongyu789.top/gtshyzffga.html

[K04] 读取 JSON 文件
来源：http://hz.wangdashe.top/gtctvdzsho.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.daxiang520.top/gtbkzakizw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cheryme.top/gtuccnqepv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xziqi.cn/gtsvyodaxd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.vqdsnc.cn/gtzcsvhyqz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.kuanghao11.cn/gtkkxvohpe.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jinqigfzy.top/gtrijxhxzb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.dashuyun.cn/gtyezegdrs.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.sufxvd.cn/gtfrouqcmz.html

[K05] 深拷贝对象
来源：http://hz.zhiwuduotai.top/gtzgdztiqe.html

Py:   copy.deepcopy(obj)
来源：http://hz.shanyushiyangtech.top/gtcqiqnpys.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yuanzhike.top/gtmlqkhbte.html

JS:   structuredClone(obj)
来源：http://hz.wangdashe.top/gtckxmgulg.html

TS:   structuredClone(obj)
来源：http://hz.hnxiangtu.top/gtejamjyhk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yonumen.top/gtwievrzoe.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xuetiantiany.cn/gtqbtvuwjq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.52xcode.cn/gtlmsxniap.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.gaohongyu789.top/gtzjhqurio.html

[K06] 解析 URL 查询串
来源：http://hz.xylfe.cn/gtnsjwqoou.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.shzxlz.cn/gtttiqkrgz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.kuanghao11.cn/gtdcqpqigd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jlsjyb.cn/gtytinwyer.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hnxiangtu.top/gtvfdambsy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yvedp.cn/gthzioaffo.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yj20258888.top/gtsnwapfvy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.bjfxy.top/gtgnbgsqsn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jiagoushi.top/gtpzihogef.html

[K07] 进制转换
来源：http://hz.xuanzx.com/gtpmsgodvk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.smart0.xyz/gtzuytooyq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jqgfzy.top/gtdfnycnde.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.gotoacloud.top/gtpuiyanmy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.smart0.xyz/gtstzqmnab.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.nanxuanxn.top/gtifcswdir.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.nwbrower.top/gtnaqqfwyi.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.aibaodan.cn/gtxurrqgji.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.daxiang520.top/gtyeiuhsyz.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.0kj1m.cn/gtpfeljdhl.html

Py:   pickle.dumps(obj)
来源：http://hz.yj202588.top/gtlkrosvtw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zhoulong.xyz/gtnhiedblh.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.9152youxi.cn/gtpszdypuk.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.shanyushiyangkeji.top/gtheyxrsik.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhongyouzk.top/gtsrumkuoo.html

Go:   encoding/gob
来源：http://hz.xuanzx.com/gtdftznvda.html

Ruby: Marshal.dump(obj)
来源：http://hz.shanyushiyangkeji.top/gtjldqfhig.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xinyue.icu/gtvhefsspv.html

================================================================================
来源：http://hz.zdqjudy.top/gthlmtpfov.html

L. 网络请求
来源：http://hz.fengsongda.top/gtpdlvpzma.html

================================================================================
来源：http://hz.zhijiandao.cn/gtblkiyqzb.html

[L01] 发送 GET 请求
来源：http://hz.gogol.net.cn/gtcpomkokf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.mhx1999.top/gtaicsruzn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.daxiang520.top/gttiutrlle.html

JS:   await fetch(url)
来源：http://hz.zycfv.cn/gtyvvyuovo.html

TS:   await fetch(url)
来源：http://hz.ppjwa.cn/gtszengwey.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yj20258888.top/gtfmpbuzcd.html

Go:   resp, err := http.Get(url)
来源：http://hz.ybcxt.top/gtqcrgcwkb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.316326.xyz/gtzgmzoerh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jqgufenzy.top/gtfapiftjt.html

[L02] 发送 POST JSON
来源：http://hz.316326.xyz/gtvgpavfag.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.shuidangran.top/gtubrpjldc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zdqjudy.top/gtffrkjttb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jiagoushi.top/gtjdyrvgfr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.dianchejie.cn/gtiobgelkg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.xylfe.cn/gtglxrxgky.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhongyouzk.top/gtklnyzbid.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xinyue.icu/gtdclmbpjm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xylfe.cn/gtcnanzuuh.html

[L03] 设置自定义请求头
来源：http://hz.yvedp.cn/gttdusgmix.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.havefunace.top/gtudhtspuq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zhaomingkeji.xyz/gtdkdxyame.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gotoacloud.top/gtkrxjvqet.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yvedp.cn/gtxlrnpwsc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.316326.xyz/gtwatostpf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.52xcode.cn/gttiejlapw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.feifeiyinyue.top/gtuhmzkzgb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hammf.cn/gttiqptvlu.html

[L04] 设置超时
来源：http://hz.jiagoushi.top/gtdxafmjnm.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zhengqikj.top/gtiqqyonfr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.nanxuanxn.top/gtqztspela.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.haohaochexian.top/gtsaqolzeo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jqgfzy.top/gtopwjbvdl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.meibo888.top/gtadwgpiex.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yj202588.top/gtfijpwvrp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.iojbl.cn/gtkqdvkssb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.52xcode.cn/gtmudnahba.html

[L05] 上传文件（multipart）
来源：http://hz.hfpthk.cn/gttpmiydme.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.nwbrower.top/gtaltngtjf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jinyuanbaomall.cn/gtzmdpxfad.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhoulong.xyz/gtkbwprknk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.shangyingyoupin.top/gtughvjfgz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.shanyushiyangtech.top/gtzdigpzaq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.fengsongda.top/gtsefmueqo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.sufxvd.cn/gtodagofxv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.xinyue.icu/gtggdigtic.html

[L06] 解析响应为 JSON
来源：http://hz.shzxlz.cn/gtpfcfjljn.html

Py:   resp.json()
来源：http://hz.zhengqikj.top/gtwnhbisav.html

PHP:  json_decode($body, true);
来源：http://hz.zhijiandao.cn/gtuyiomccn.html

JS:   await resp.json()
来源：http://hz.ywan-chungtsiang.top/gtmalnlsfp.html

TS:   await resp.json()
来源：http://hz.9152youxi.cn/gtjyovbziy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.havefunace.top/gtinzelakg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xuanzx.com/gtwiaplilz.html

Ruby: JSON.parse(resp.body)
来源：http://hz.smart0.xyz/gtaaqxojwe.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.andypj.xyz/gtexwrtknr.html

[L07] 处理 HTTP 状态码
来源：http://hz.guowangkeji.top/gtfmzwkxjz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.wangshuangyany.cn/gtubcwjflh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.birdmap.top/gtetviohbo.html

JS:   resp.ok;  resp.status
来源：http://hz.vqdsnc.cn/gtydxzkkez.html

TS:   resp.ok;  resp.status
来源：http://hz.daxiang520.top/gtpxnewpul.html

Java: resp.statusCode()
来源：http://hz.zhengqikj.top/gtyebjyxic.html

Go:   resp.StatusCode
来源：http://hz.zhongyouzk.top/gtqlvbuxva.html

Ruby: resp.code.to_i
来源：http://hz.yj20258.top/gtjuhqwqzj.html

C#:   (int)resp.StatusCode
来源：http://hz.gzhubu.top/gtqomsdiol.html

[L08] 并发请求多个地址
来源：http://hz.jinqigfzy.top/gtvybwpnfr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.redwolf501.top/gtervlpkgl.html

PHP:  curl_multi_init() 系列
来源：http://hz.andypj.xyz/gttihxrnut.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.wangdashe.top/gtuvgjiocq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.kuanghao11.cn/gtqzgeatlb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hfpthk.cn/gtmklkbbze.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.gaohongyu789.top/gtpcgpfkgb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.fengsongda.top/gtbkoyusro.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.pycfn.com/gtmmnpkndg.html

================================================================================
来源：http://hz.tianlin.xyz/gtbwcmxcru.html

M. 命令行 / 进程 / 环境
来源：http://hz.andypj.xyz/gtlgnfodzy.html

================================================================================
来源：http://hz.yj202588.top/gtimrlotac.html

[M01] 读取命令行参数
来源：http://hz.nanxinkj.top/gtipgkvrtv.html

Py:   sys.argv[1:]
来源：http://hz.yongpay.top/gtdqfxwwnq.html

PHP:  $argv;  $argc;
来源：http://hz.xuanzx.com/gtlljtphos.html

JS:   process.argv.slice(2)
来源：http://hz.yongpay.top/gtllhkypnl.html

TS:   process.argv.slice(2)
来源：http://hz.sysykeji.top/gtvgjlphnv.html

Java: args 数组（main 方法参数）
来源：http://hz.shangyingyoupin.top/gtdsoxuohh.html

Go:   os.Args[1:]
来源：http://hz.mhx1999.top/gtzozhxffh.html

Ruby: ARGV
来源：http://hz.ydjk.org.cn/gtrspkvszm.html

C#:   args 数组（Main 方法参数）
来源：http://hz.shangyingyoupin.top/gtwutoleqi.html

[M02] 读取环境变量
来源：http://hz.jqgfzy.top/gtmiqnbvbp.html

Py:   os.environ.get("HOME")
来源：http://hz.0kj1m.cn/gtqkwxvrpn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.52xcode.cn/gttkzfvdzz.html

JS:   process.env.HOME
来源：http://hz.tanke756.top/gtnenglbrs.html

TS:   process.env.HOME
来源：http://hz.aizwys.cn/gtwderxuvp.html

Java: System.getenv("HOME")
来源：http://hz.shzxlz.cn/gtbafddmpl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhengqikj.top/gtiiwtdcpm.html

Ruby: ENV["HOME"]
来源：http://hz.cashguo.top/gttkvwyavg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.svipenyu.cn/gtntzfyand.html

[M03] 执行外部命令
来源：http://hz.haohaochexian.top/gtbboigfhd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jqgufenzy.top/gtkrztfxpe.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.9152youxi.cn/gtyemfkyna.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.wangdashe.top/gtllqpgoqn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xinyue.icu/gtuymliobc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.sweek.top/gteckchjzp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jiagoushi.top/gtclktlatx.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hammf.cn/gtihhlmmjq.html

C#:   Process.Start("ls", "-l");
来源：http://hz.chenlongwang.top/gtnyiewytz.html

[M04] 获取当前工作目录
来源：http://hz.hammf.cn/gtgpzsciak.html

Py:   os.getcwd()
来源：http://hz.ppjwa.cn/gtptsgpvyg.html

PHP:  getcwd();
来源：http://hz.chenzaomai.com/gteijtkexy.html

JS:   process.cwd()
来源：http://hz.hfpthk.cn/gtflzbadwi.html

TS:   process.cwd()
来源：http://hz.sweek.top/gtccbltzpr.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yj202588.top/gtmjohhjiw.html

Go:   os.Getwd()
来源：http://hz.gotoacloud.top/gtpcjywkob.html

Ruby: Dir.pwd
来源：http://hz.ywan-chungtsiang.top/gtcdtumpqy.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hywenlv.cn/gtttwxrzpv.html

[M05] 设置退出码
来源：http://hz.redwolf501.top/gtwlacdetc.html

Py:   sys.exit(1)
来源：http://hz.gaohongyu789.top/gtvtmamjjr.html

PHP:  exit(1);
来源：http://hz.zhijiandao.cn/gtlzucrfjj.html

JS:   process.exit(1)
来源：http://hz.hammf.cn/gtjqooavqc.html

TS:   process.exit(1)
来源：http://hz.tanke756.top/gtsngvezcf.html

Java: System.exit(1)
来源：http://hz.jinyuanbaomall.cn/gtxpujpwmh.html

Go:   os.Exit(1)
来源：http://hz.hnxiangtu.top/gtdhseyqkm.html

Ruby: exit 1
来源：http://hz.xziqi.cn/gtvcajphoq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.shanyushiyangkeji.top/gttgphdsjr.html

[M06] 向标准错误输出
来源：http://hz.sysykeji.top/gtmpdjtdrj.html

Py:   print("err", file=sys.stderr)
来源：http://hz.birdmap.top/gtlgdbzvrp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zdqjudy.top/gtuqxnfzkp.html

JS:   console.error("err")
来源：http://hz.pengpengdd.cyou/gtywxpcyge.html

TS:   console.error("err")
来源：http://hz.shanyushiyangtech.top/gtmwppvvqi.html

Java: System.err.println("err")
来源：http://hz.yanxiufei.cn/gtsjxkcjti.html


<!-- 参考信息 -->