代发 wailian999

[J03] 字符串解析为日期
来源：http://hz.xingfuxueyuan.xyz/gtwmwgzlus.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hongshengwenyu.top/gtbydhzwmc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yvedp.cn/gtvnxtbzis.html

JS:   new Date("2024-01-02")
来源：http://hz.shanyushiyangtech.top/gtxthvyhds.html

TS:   new Date("2024-01-02")
来源：http://hz.xylfe.cn/gtotmbhyxu.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.redwolf501.top/gttryrgdkf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.cdnleiting.top/gtevdbihru.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.fengsongda.top/gtryjekrey.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.wangshuangyany.cn/gtvfjjxhvv.html

[J04] 时间戳与日期互转
来源：http://hz.jlsjyb.cn/gtkwnopbcd.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.haohaochexian.top/gtezvkktiv.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.dianchejie.cn/gtubqzkmnv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.wangdashe.top/gtrylbvmwn.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jinyuanbaomall.cn/gtizonzjxi.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.dianchejie.cn/gtevpcosrs.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.tianlin.xyz/gtsbvvlylz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xingfuxueyuan.xyz/gthpkqlnlw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hnxiangtu.top/gtcuhigmme.html

[J05] 时间加减（加 7 天）
来源：http://hz.smart0.xyz/gtptmsnhgs.html

Py:   now + timedelta(days=7)
来源：http://hz.yuxming.cn/gtoqcmobal.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.feifeiyinyue.top/gtvbwhzxbl.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.mhx1999.top/gtfrokndvc.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.fzhhl.top/gtmsbcpjeu.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhaomingkeji.xyz/gtxxsbectg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ydjk.org.cn/gtbrhiqvos.html

Ruby: Time.now + 7 * 86400
来源：http://hz.fengsongda.top/gtqddlpgah.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yueranfly.top/gtlmbkjgqj.html

[J06] 计算两时间之差
来源：http://hz.xingfuxueyuan.xyz/gtfuohgbhc.html

Py:   (end - start).total_seconds()
来源：http://hz.chenjidiqi.icu/gtaryezymn.html

PHP:  $end->diff($start)->days;
来源：http://hz.chenzaomai.com/gthipbngdl.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yuxming.cn/gtviejhvzl.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ivvv.top/gtuyccnbeq.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cqqwz.cn/gtvynorblr.html

Go:   end.Sub(start).Hours()
来源：http://hz.mhx1999.top/gttbkazkxy.html

Ruby: end - start                 # 返回秒数
来源：http://hz.xuanzx.com/gtyadiyhik.html

C#:   (end - start).TotalSeconds
来源：http://hz.zdqjudy.top/gthpgrahud.html

[J07] 比较两个日期
来源：http://hz.zhijiandao.cn/gtgtpofglt.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yj20258888.top/gtwevubnhv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jiagoushi.top/gtrgsawgsy.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258.top/gtdxyaexig.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yonumen.top/gtpahkrwcy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zycfv.cn/gtmfwrsavc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jinyuanbaomall.cn/gtimhjpdmf.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hnqzz.top/gtrgrehcie.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.xinyue.icu/gtkcinbazp.html

[J08] 提取年月日与星期
来源：http://hz.ehwqpu.com/gtneylrhof.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yonumen.top/gtzgbpbmuq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.bjfxy.top/gtqxjgeagr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.cashguo.top/gtxfiexrwj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yanxiufei.cn/gtngpvrglg.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.gotoacloud.top/gtergjqfmr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yuanzhike.top/gtqbpaxdvv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jiagoushi.top/gtclgrgcal.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.pycfn.com/gthvznysro.html

[J09] 时区处理
来源：http://hz.sweek.top/gtwsnrxahe.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.0kj1m.cn/gtkrpvdcki.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ehwqpu.com/gtdhuvhlhm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sufxvd.cn/gtkfmheipf.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nwbrower.top/gtlvfviiaq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xziqi.cn/gtsdmkunll.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.andypj.xyz/gthhztbbnj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.cdnleiting.top/gtgxdsstel.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.xziqi.cn/gtnmovmcwz.html

[J10] 取今天 / 本月第一天
来源：http://hz.xylfe.cn/gtnpjxwrds.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.guowangkeji.top/gtpnwxhxfq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhaomingkeji.xyz/gtvltnohcc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.cdnleiting.top/gtsvgxhtpp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.redwolf501.top/gtqsirurds.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.sysykeji.top/gtnfjphgyk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.0kj1m.cn/gtbfjpvelb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.daxiang520.top/gtdssgghen.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.tian-w.cn/gtekdxkcob.html

================================================================================
来源：http://hz.cqqwz.cn/gtghlofgpx.html

K. JSON 与序列化
来源：http://hz.quarkkingdee.top/gtuffvaqyj.html

================================================================================
来源：http://hz.andypj.xyz/gtqpycljie.html

[K01] 对象转 JSON 字符串
来源：http://hz.yj20258.top/gttvawgruz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.wangdashe.top/gtpnfmfzgs.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.snrcjt.cn/gtcrqfpvzt.html

JS:   JSON.stringify(obj)
来源：http://hz.9152youxi.cn/gtzkjtwyug.html

TS:   JSON.stringify(obj)
来源：http://hz.yuanzhike.top/gtduihsgfg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.dashuyun.cn/gtpeczcwqf.html

Go:   json.Marshal(obj)
来源：http://hz.haohaochexian.top/gtuipwsdyh.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.sysykeji.top/gtptuufbct.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jiagoushi.top/gtdjhqfnis.html

[K02] JSON 字符串转对象
来源：http://hz.yueranfly.top/gtypluttke.html

Py:   json.loads(s)
来源：http://hz.svipenyu.cn/gtujnoihfj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.nanxuanxn.top/gtbrkewqly.html

JS:   JSON.parse(s)
来源：http://hz.yvedp.cn/gttupncqgj.html

TS:   JSON.parse(s)
来源：http://hz.zhixingplan.top/gtotquvnms.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hongshengwenyu.top/gtnmeybvwa.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.andypj.xyz/gtbocalmfi.html

Ruby: JSON.parse(s)
来源：http://hz.shanyushiyangtech.top/gtwlxdmnwj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.c1oappe.top/gtaiaoysjy.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.cdnleiting.top/gtveqkqffv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.shangyingyoupin.top/gtxofwbmzl.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.xuanzx.com/gtcqommsbs.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yongpay.top/gtzfyowtky.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhiwuduotai.top/gtawyihsgh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.sufxvd.cn/gtsusrkgcv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.fzhhl.top/gtbehpcxpl.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.cucudq.cn/gttdwqcfzy.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.quarkkingdee.top/gtutcluszd.html

[K04] 读取 JSON 文件
来源：http://hz.tian-w.cn/gtylnkneos.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yonumen.top/gtsmendrry.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.52xcode.cn/gtoizqyewm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.tian-w.cn/gtbthvjkrj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jlsjyb.cn/gtjvghztwo.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.dianchejie.cn/gtdmrgtkor.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhijiandao.cn/gtervktjjf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.gotoacloud.top/gtztofiehy.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ivvv.top/gtgkqdxsss.html

[K05] 深拷贝对象
来源：http://hz.jlsjyb.cn/gtgfjvepxn.html

Py:   copy.deepcopy(obj)
来源：http://hz.dashuyun.cn/gtxpdatgvt.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cucudq.cn/gtfmnzvkiu.html

JS:   structuredClone(obj)
来源：http://hz.tian-w.cn/gtfghfzjws.html

TS:   structuredClone(obj)
来源：http://hz.haohaochexian.top/gtfhbpypho.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xingfuxueyuan.xyz/gtijalbmar.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hfpthk.cn/gtigniujmf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jyoumei.cn/gtakvwpuea.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.wangshuangyany.cn/gtujfudtgq.html

[K06] 解析 URL 查询串
来源：http://hz.cashguo.top/gtsckxsgrb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jqgfzy.top/gthshcufpd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.nanxuanxn.top/gtgheugajz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zdqjudy.top/gtvsmoskoi.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hongshengwenyu.top/gtshyueesv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.feifeiyinyue.top/gtqdvqymxe.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.tianlin.xyz/gtnxxpfvhq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.cucudq.cn/gtepgasunk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.bjfxy.top/gtdbukvuwa.html

[K07] 进制转换
来源：http://hz.gaohongyu789.top/gtprituuea.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jianghu66.top/gtgrhrizts.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.aizwys.cn/gtnnumsvbv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jyoumei.cn/gtebaphxof.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yvedp.cn/gtfznocfts.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ywan-chungtsiang.top/gticvxemab.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yonumen.top/gtwucxhvwz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.andypj.xyz/gtuzucsmys.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.gzhubu.top/gtvhdjqesj.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.guowangkeji.top/gtrnduflfm.html

Py:   pickle.dumps(obj)
来源：http://hz.jinyuanbaomall.cn/gtkfcygcyy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.pycfn.com/gtjdvnufpx.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.9152youxi.cn/gtfsakhyye.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.nanxuanxn.top/gtqgatejbl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.daxiang520.top/gtbiogfnoa.html

Go:   encoding/gob
来源：http://hz.redwolf501.top/gtbwfufpep.html

Ruby: Marshal.dump(obj)
来源：http://hz.sysykeji.top/gtjzqmpuzr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jianghu66.top/gtjegplpwx.html

================================================================================
来源：http://hz.sysykeji.top/gtngwntsgf.html

L. 网络请求
来源：http://hz.guowangkeji.top/gtgfencxxt.html

================================================================================
来源：http://hz.yongpay.top/gtmgrrfmdc.html

[L01] 发送 GET 请求
来源：http://hz.sxryk.cn/gtphlmrvaq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.chenlongwang.top/gtlvgorwbr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.cucudq.cn/gtjgecgzhq.html

JS:   await fetch(url)
来源：http://hz.daria6918.cn/gtztkiotew.html

TS:   await fetch(url)
来源：http://hz.snrcjt.cn/gtqrzbsvxf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yuanzhike.top/gtvjzdtyfl.html

Go:   resp, err := http.Get(url)
来源：http://hz.xziqi.cn/gttafvppxr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.9152youxi.cn/gtzwvkkmmo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zhijiandao.cn/gtpnjqezrp.html

[L02] 发送 POST JSON
来源：http://hz.andypj.xyz/gtaxbmvagk.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.cdnleiting.top/gtyoflpxvf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.9152youxi.cn/gtmgpprhga.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cqqwz.cn/gtqbfvpeqz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xylfe.cn/gtctamgsae.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhixingplan.top/gtidxqzrfi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ybcxt.top/gtdmeywlbh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jinyuanbaomall.cn/gtvakzinti.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.cqqwz.cn/gtteymkhan.html

[L03] 设置自定义请求头
来源：http://hz.zdqjudy.top/gtwfjemfej.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.vqdsnc.cn/gtaavyihir.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.gogol.net.cn/gtpgblzjix.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jianghu66.top/gtevmdxwcj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cheryme.top/gtmxerpeai.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.feifeiyinyue.top/gtiplfnvgf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yuanzhike.top/gtcnvadxnp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.tanke756.top/gtcdhuoevd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.iojbl.cn/gtspejntwf.html

[L04] 设置超时
来源：http://hz.chenzaomai.com/gttnoafnjk.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yj20258888.top/gtlnhnifcs.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jyoumei.cn/gtzjnibhsn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.snrcjt.cn/gtelphwfwk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shanyushiyangtech.top/gtwvvsingr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jlsjyb.cn/gtuydfuhqe.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zdqjudy.top/gtavawxswq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.guowangkeji.top/gtybgqlevq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.nwbrower.top/gtpqjypnkf.html

[L05] 上传文件（multipart）
来源：http://hz.xylfe.cn/gtjnjkpvkr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.shuidangran.top/gtrbfaadia.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.chenjidiqi.icu/gthpzanimd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jlsjyb.cn/gtbvpltmgq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jiagoushi.top/gtcngdbisw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.cashguo.top/gtoiorbsqy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.wangdashe.top/gtdbnwcpwd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.iojbl.cn/gtvogogtpo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.sweek.top/gttameqhfh.html

[L06] 解析响应为 JSON
来源：http://hz.bjfxy.top/gtrdkuaqmc.html

Py:   resp.json()
来源：http://hz.ivvv.top/gtbhughjoe.html

PHP:  json_decode($body, true);
来源：http://hz.yuanzhike.top/gtkditsalx.html

JS:   await resp.json()
来源：http://hz.hnxiangtu.top/gtrpixoycm.html

TS:   await resp.json()
来源：http://hz.mhx1999.top/gtmwykchvw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.iojbl.cn/gtyxvpoqot.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zycfv.cn/gtopsrdsnv.html

Ruby: JSON.parse(resp.body)
来源：http://hz.shuidangran.top/gtqlipcnfe.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hammf.cn/gtyxlxohyo.html

[L07] 处理 HTTP 状态码
来源：http://hz.xylfe.cn/gtnjzlivnj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.feifeiyinyue.top/gtqyonxgyz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hnxiangtu.top/gtmfisyxta.html

JS:   resp.ok;  resp.status
来源：http://hz.iojbl.cn/gtjfdzxhwb.html

TS:   resp.ok;  resp.status
来源：http://hz.0kj1m.cn/gtgthfujxe.html

Java: resp.statusCode()
来源：http://hz.cucudq.cn/gtcxtgdbfq.html

Go:   resp.StatusCode
来源：http://hz.smart0.xyz/gtmqwdhgmh.html

Ruby: resp.code.to_i
来源：http://hz.chenzaomai.com/gtupphpncx.html

C#:   (int)resp.StatusCode
来源：http://hz.ppjwa.cn/gtafnglryq.html

[L08] 并发请求多个地址
来源：http://hz.zhiwuduotai.top/gtexhjolea.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yuanzhike.top/gthplzybqh.html

PHP:  curl_multi_init() 系列
来源：http://hz.xingfuxueyuan.xyz/gtxpqfzxfx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.daxiang520.top/gtavltsfrm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hysaishi.cn/gtwbbvyjrl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.pycfn.com/gtkjibsqfa.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.chenzaomai.com/gtdzzugorh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.chenzaomai.com/gtlbshpkkd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yonumen.top/gtxtbqrizx.html

================================================================================
来源：http://hz.sysykeji.top/gtziotuyoc.html

M. 命令行 / 进程 / 环境
来源：http://hz.chenzaomai.com/gtcgvkzlav.html

================================================================================
来源：http://hz.mhx1999.top/gtfpninpux.html

[M01] 读取命令行参数
来源：http://hz.sufxvd.cn/gtbmmwktjl.html

Py:   sys.argv[1:]
来源：http://hz.cheryme.top/gtzqzmxbgo.html

PHP:  $argv;  $argc;
来源：http://hz.xylfe.cn/gtmsnmmmaj.html

JS:   process.argv.slice(2)
来源：http://hz.quarkkingdee.top/gtyeblufqr.html

TS:   process.argv.slice(2)
来源：http://hz.birdmap.top/gtijhdwuwr.html

Java: args 数组（main 方法参数）
来源：http://hz.cqqwz.cn/gtlhqxauwz.html

Go:   os.Args[1:]
来源：http://hz.cdnleiting.top/gtuxzoggpx.html

Ruby: ARGV
来源：http://hz.jqgufenzy.top/gtjgqaftmf.html

C#:   args 数组（Main 方法参数）
来源：http://hz.tian-w.cn/gtcfrgmnjr.html

[M02] 读取环境变量
来源：http://hz.zhixingplan.top/gtjhigzzwm.html

Py:   os.environ.get("HOME")
来源：http://hz.xylfe.cn/gtjirwtlgv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.kuanghao11.cn/gtzyhldiio.html

JS:   process.env.HOME
来源：http://hz.snrcjt.cn/gtmdpuuwzj.html

TS:   process.env.HOME
来源：http://hz.tian-w.cn/gtonjmladq.html

Java: System.getenv("HOME")
来源：http://hz.nanxuanxn.top/gtjljpnhsp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yvedp.cn/gtbsxlrxbv.html

Ruby: ENV["HOME"]
来源：http://hz.xziqi.cn/gtotjpluqe.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hysaishi.cn/gtkdcijuvo.html

[M03] 执行外部命令
来源：http://hz.yangfankeji.com/gtngfefeou.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.316326.xyz/gtjzxilxvi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.redwolf501.top/gtaqynobey.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.c1oappe.top/gtkazchzed.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ydzc1.top/gthmmptknu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.pycfn.com/gteyraspft.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.dashuyun.cn/gtvfclbnra.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.fengsongda.top/gtvwvnebgt.html

C#:   Process.Start("ls", "-l");
来源：http://hz.sweek.top/gtzfkeumxk.html

[M04] 获取当前工作目录
来源：http://hz.smart0.xyz/gteohfbhzq.html

Py:   os.getcwd()
来源：http://hz.redwolf501.top/gtivcrbmzs.html

PHP:  getcwd();
来源：http://hz.jyoumei.cn/gtvoatrvur.html

JS:   process.cwd()
来源：http://hz.guannengcc.top/gtwmxpmdzc.html

TS:   process.cwd()
来源：http://hz.chenlongwang.top/gtzegsapnj.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.havefunace.top/gtjczpvpvq.html

Go:   os.Getwd()
来源：http://hz.chenlongwang.top/gtkwpgcllz.html

Ruby: Dir.pwd
来源：http://hz.jianghu66.top/gtvyoydsdb.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.xuetiantiany.cn/gttmwqzlkz.html

[M05] 设置退出码
来源：http://hz.jinyuanbaomall.cn/gtvdopzsgx.html

Py:   sys.exit(1)
来源：http://hz.52xcode.cn/gtkbnhojnp.html

PHP:  exit(1);
来源：http://hz.cheryme.top/gthcomwepu.html

JS:   process.exit(1)
来源：http://hz.xziqi.cn/gtaddgnswq.html

TS:   process.exit(1)
来源：http://hz.dashuyun.cn/gtiradoimm.html

Java: System.exit(1)
来源：http://hz.nanxinkj.top/gtznqreled.html

Go:   os.Exit(1)
来源：http://hz.cqqwz.cn/gtcvofehpc.html

Ruby: exit 1
来源：http://hz.52xcode.cn/gtrkfhbllp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yuxming.cn/gteiemussl.html

[M06] 向标准错误输出
来源：http://hz.andypj.xyz/gtgghjombj.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jqgfzy.top/gtprqimpbc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.dianchejie.cn/gtbmmjjsem.html

JS:   console.error("err")
来源：http://hz.shanyushiyangkeji.top/gtgkwktgdi.html

TS:   console.error("err")
来源：http://hz.jqgfzy.top/gtyqrqpmqe.html

Java: System.err.println("err")
来源：http://hz.sysykeji.top/gtdlmuwgmn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ybcxt.top/gtquctcqln.html

Ruby: warn "err"
来源：http://hz.jiagoushi.top/gtaianbmst.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.xingfuxueyuan.xyz/gttxzklxog.html

[M07] 判断是否为主入口
来源：http://hz.dashuyun.cn/gtezmrnjvj.html

Py:   if __name__ == "__main__":
来源：http://hz.hysaishi.cn/gtqoautrts.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhengqikj.top/gtclelcvya.html

JS:   require.main === module
来源：http://hz.xziqi.cn/gtfvwajnmq.html

TS:   require.main === module
来源：http://hz.xingfuxueyuan.xyz/gtdjlkckib.html

Java: public static void main(String[] args)
来源：http://hz.smart0.xyz/gtvqthueha.html

Go:   func main()
来源：http://hz.sufxvd.cn/gtqhzbzqjg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.hfpthk.cn/gtuowaonzn.html

C#:   static void Main(string[] args)
来源：http://hz.gotoacloud.top/gtesvosxuk.html

[M08] 获取系统与运行时信息
来源：http://hz.sxryk.cn/gttgdvnwrc.html

Py:   platform.system();  platform.python_version()
来源：http://hz.smart0.xyz/gtgcytrnug.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.cheryme.top/gtlwysnocy.html

JS:   process.platform;  process.version
来源：http://hz.shanyushiyangkeji.top/gtgbenkwnm.html

TS:   process.platform;  process.version
来源：http://hz.52xcode.cn/gtdtwegzky.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.mhx1999.top/gtukxpmlkk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.shuidangran.top/gtuzzzjezq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.chenjidiqi.icu/gtodgkwtky.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hnqzz.top/gtdyfeqwio.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtcgkypger.html

N. 数据结构与算法
来源：http://hz.fzhhl.top/gttdsiidtm.html

================================================================================
来源：http://hz.chenzaomai.com/gtqnvtlgjh.html


<!-- 参考信息 -->