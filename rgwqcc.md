代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jqgfzy.top/gtecspznxb.html

[J04] 时间戳与日期互转
来源：http://hz.jinghuilouyu.cn/gtzljoqhwc.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.wangdashe.top/gtzmqgcewn.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.tian-w.cn/gtefcravnp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.quarkkingdee.top/gtydicxlyo.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.daxiang520.top/gtirggclhp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.andypj.xyz/gtmzeisumb.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.gotoacloud.top/gtajghorqi.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.9152youxi.cn/gtwztmbvfz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.xuetiantiany.cn/gtorrksrev.html

[J05] 时间加减（加 7 天）
来源：http://hz.jinyuanbaomall.cn/gtexgpwywc.html

Py:   now + timedelta(days=7)
来源：http://hz.sxryk.cn/gtaksniyns.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.chenjidiqi.icu/gtymqwgcaj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cdnleiting.top/gtemimfxom.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.havefunace.top/gtvmmnvdyx.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.gotoacloud.top/gtroyigarh.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhengqikj.top/gtfwuatqwr.html

Ruby: Time.now + 7 * 86400
来源：http://hz.chenzaomai.com/gtibkwfqyu.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.shanyushiyangtech.top/gtzppeqnjh.html

[J06] 计算两时间之差
来源：http://hz.ivvv.top/gtkwwybstr.html

Py:   (end - start).total_seconds()
来源：http://hz.jlsjyb.cn/gtkitlsdds.html

PHP:  $end->diff($start)->days;
来源：http://hz.gzhubu.top/gtsisoumkm.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.nanxuanxn.top/gtdnturxaz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.cashguo.top/gtrdlzrbkk.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.shanyushiyangtech.top/gtfnflmuzk.html

Go:   end.Sub(start).Hours()
来源：http://hz.jyoumei.cn/gthecsoqdv.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zhaomingkeji.xyz/gtnwgxkvgg.html

C#:   (end - start).TotalSeconds
来源：http://hz.yuxming.cn/gtsctaruag.html

[J07] 比较两个日期
来源：http://hz.jlsjyb.cn/gtnuvrrbjb.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.316326.xyz/gtxvilpbhk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yueranfly.top/gtewjypjkv.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhoulong.xyz/gtjsbpmhef.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shuidangran.top/gttzsznsuu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhengqikj.top/gtedkpciya.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.daria6918.cn/gtgxujwmxs.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yj20258888.top/gtecmkrvwf.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.quarkkingdee.top/gtmwsouwqu.html

[J08] 提取年月日与星期
来源：http://hz.andypj.xyz/gtkrtmwxub.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.meibo888.top/gtxkgxoksa.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jinqigfzy.top/gtblkjynqz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.aibaodan.cn/gtzxlxzczw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.sxryk.cn/gtlpfjbwha.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.c1oappe.top/gtrvkbljnn.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.andypj.xyz/gtpmmcadwv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhoulong.xyz/gtlzgswdqz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yongpay.top/gtyhxsjzej.html

[J09] 时区处理
来源：http://hz.pycfn.com/gticpxjjmf.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.sweek.top/gttwdlohma.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.cqqwz.cn/gtbkxubfyn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yuxming.cn/gtlltuwbqv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhijiandao.cn/gtbhkxlemc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhiwuduotai.top/gtlcnkvbww.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhengqikj.top/gtkaptxvgo.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.tanke756.top/gtfpmzgsas.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ywan-chungtsiang.top/gtzirdqsqs.html

[J10] 取今天 / 本月第一天
来源：http://hz.jianghu66.top/gtejiontev.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhiwuduotai.top/gtuglhiqvy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zycfv.cn/gtetogthco.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.vqdsnc.cn/gtnwjuabcw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.wangdashe.top/gtvgxjnyck.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.kuanghao11.cn/gtjkelgfpu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.shuidangran.top/gtcquxxagk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.vqdsnc.cn/gteodhptjk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.hfpthk.cn/gttraqozox.html

================================================================================
来源：http://hz.yj20258888.top/gtayudqpvh.html

K. JSON 与序列化
来源：http://hz.smart0.xyz/gtvkhvhxpx.html

================================================================================
来源：http://hz.ybcxt.top/gtutacvhvc.html

[K01] 对象转 JSON 字符串
来源：http://hz.feifeiyinyue.top/gtewtkrcpo.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.daxiang520.top/gtuugfldpj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhaomingkeji.xyz/gthfhmhcqy.html

JS:   JSON.stringify(obj)
来源：http://hz.jinqigufen.top/gtmjsuznop.html

TS:   JSON.stringify(obj)
来源：http://hz.ppjwa.cn/gtdsiclile.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jiagoushi.top/gtoxmvrsya.html

Go:   json.Marshal(obj)
来源：http://hz.nanxinkj.top/gtdamjnnce.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.redwolf501.top/gtyamsrpcn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yvedp.cn/gtiogigzmu.html

[K02] JSON 字符串转对象
来源：http://hz.yanxiufei.cn/gtqmvtqvvh.html

Py:   json.loads(s)
来源：http://hz.xuanzx.com/gtmmsjcias.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.pycfn.com/gtlvnarrzx.html

JS:   JSON.parse(s)
来源：http://hz.cqqwz.cn/gtxxvyvxsu.html

TS:   JSON.parse(s)
来源：http://hz.bjfxy.top/gtrktcyryh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.ppjwa.cn/gtwoieqkij.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.chenjidiqi.icu/gtgcnuukdf.html

Ruby: JSON.parse(s)
来源：http://hz.chenjidiqi.icu/gtmmsbnapa.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xuetiantiany.cn/gtjdxapxtf.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jlsjyb.cn/gtuqmaehru.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.wangdashe.top/gtnqffycku.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.chenlongwang.top/gthgmbjfsj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jlsjyb.cn/gtbylixvbe.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jqgufenzy.top/gthisdgfjy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.fzhhl.top/gtenggzpik.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.mhx1999.top/gtuzavlfpk.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hnqzz.top/gteuwojgas.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.quarkkingdee.top/gtirdznqvb.html

[K04] 读取 JSON 文件
来源：http://hz.shanyushiyangkeji.top/gtxrlmdmxg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.dianchejie.cn/gtywwdrhsr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.0kj1m.cn/gtuazxrfhr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.havefunace.top/gthuaoocrw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hnxiangtu.top/gtoxktqvuc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hysaishi.cn/gtzrlvwrmq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xziqi.cn/gtrikgdcfr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.wangdashe.top/gtzruxepti.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.nanxuanxn.top/gtcltlsrwr.html

[K05] 深拷贝对象
来源：http://hz.jqgufenzy.top/gtutytwkte.html

Py:   copy.deepcopy(obj)
来源：http://hz.hysaishi.cn/gtneusiknj.html

PHP:  unserialize(serialize($obj));
来源：http://hz.smart0.xyz/gtktfemvnv.html

JS:   structuredClone(obj)
来源：http://hz.nwbrower.top/gtkkeodpbk.html

TS:   structuredClone(obj)
来源：http://hz.wangdashe.top/gtmgjzqbpv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.svipenyu.cn/gtheuvrcnt.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yongpay.top/gtxjnsjqft.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ywan-chungtsiang.top/gtxkwzqgzw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yj202588.top/gtekxuywyi.html

[K06] 解析 URL 查询串
来源：http://hz.fzhhl.top/gtrrpacmpa.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.chenjidiqi.icu/gtrsejpcnl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.tianlin.xyz/gtkumbqhco.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xuanzx.com/gtwyebnssv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ehwqpu.com/gtpcrobfue.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.dashuyun.cn/gtzxggxcmp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.redwolf501.top/gtvozmyzvw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.chenlongwang.top/gtqgigldvi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yangfankeji.com/gtuqgmffci.html

[K07] 进制转换
来源：http://hz.ppjwa.cn/gtgfpocoab.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.redwolf501.top/gturllkuej.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.gogol.net.cn/gtzicfifkh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hnqzz.top/gtkopzexrw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhaomingkeji.xyz/gtidfqfqqr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.chenjidiqi.icu/gtwjhmkmrj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.daria6918.cn/gtixufrizt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.dianchejie.cn/gtjnooygaq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.iojbl.cn/gthnqbxqtb.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.meibo888.top/gtfxywdeam.html

Py:   pickle.dumps(obj)
来源：http://hz.hongshengwenyu.top/gtifchfjnv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.xylfe.cn/gtoxptrukp.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.wangshuangyany.cn/gttubgrrsv.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yongpay.top/gtwkvufjrf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.iojbl.cn/gtsenxqgji.html

Go:   encoding/gob
来源：http://hz.tianlin.xyz/gtzcmgxjxx.html

Ruby: Marshal.dump(obj)
来源：http://hz.9152youxi.cn/gtlsdszqlu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.gaohongyu789.top/gtcuotgoga.html

================================================================================
来源：http://hz.tanke756.top/gtjbxorzjt.html

L. 网络请求
来源：http://hz.ehwqpu.com/gtyrnicwgf.html

================================================================================
来源：http://hz.xinyue.icu/gtmkxeslib.html

[L01] 发送 GET 请求
来源：http://hz.xuetiantiany.cn/gtsufgtqst.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jianghu66.top/gtunbnpmxl.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ehwqpu.com/gtkutuzegv.html

JS:   await fetch(url)
来源：http://hz.yonumen.top/gtzuxmnljp.html

TS:   await fetch(url)
来源：http://hz.redwolf501.top/gtmfdcqjzd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.gzhubu.top/gtrcmbmvia.html

Go:   resp, err := http.Get(url)
来源：http://hz.quarkkingdee.top/gtpfwrxijl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cdnleiting.top/gtnuzsrgkf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.daria6918.cn/gtosroidwz.html

[L02] 发送 POST JSON
来源：http://hz.guannengcc.top/gtsvlpkkyc.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ywan-chungtsiang.top/gtqzsbxdng.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.gzhubu.top/gtiudcqbqq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.chenlongwang.top/gtlyseqzqv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.pengpengdd.cyou/gtgmaadrfn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.xylfe.cn/gttlsjcwwn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.daxiang520.top/gtpbpzbvff.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jinqigfzy.top/gtiwohxvvi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.0kj1m.cn/gtvinltalw.html

[L03] 设置自定义请求头
来源：http://hz.guowangkeji.top/gtcsumxutr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.cheryme.top/gtodwibari.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.xuetiantiany.cn/gtczjkknna.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sweek.top/gttqhlmnwu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.smart0.xyz/gtifogqsfc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.feifeiyinyue.top/gtcnmjxcto.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.chenzaomai.com/gtzrtddrzr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.cheryme.top/gtsaurfvsk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.cdnleiting.top/gtmzqcozaj.html

[L04] 设置超时
来源：http://hz.quarkkingdee.top/gtrykixsnz.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jqgufenzy.top/gtbfdkrsam.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zhijiandao.cn/gtnxuevkvn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhongyouzk.top/gtrjjoxmtw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hnxiangtu.top/gtbggmhiiw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jinghuilouyu.cn/gtapsckwqo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zycfv.cn/gtpcalyawk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yvedp.cn/gtjgnjsozr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhixingplan.top/gtxfamsfir.html

[L05] 上传文件（multipart）
来源：http://hz.hysaishi.cn/gtgzlohpcu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zdqjudy.top/gtbefsmkrb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.fengsongda.top/gtdthjolwy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ppjwa.cn/gtsjziapgu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.gzhubu.top/gtscmwelgy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ybcxt.top/gtumtyyzsa.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yanxiufei.cn/gthdtrutru.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.fengsongda.top/gtbbdrouov.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.tian-w.cn/gtikboegzc.html

[L06] 解析响应为 JSON
来源：http://hz.nanxuanxn.top/gtmwxhbtoj.html

Py:   resp.json()
来源：http://hz.andypj.xyz/gtmunyoosp.html

PHP:  json_decode($body, true);
来源：http://hz.gaohongyu789.top/gtvppepcea.html

JS:   await resp.json()
来源：http://hz.ivvv.top/gtmvbbvfdv.html

TS:   await resp.json()
来源：http://hz.iojbl.cn/gtxixplkwf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.guowangkeji.top/gtsgqkkfem.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xziqi.cn/gtvsiaqxsi.html

Ruby: JSON.parse(resp.body)
来源：http://hz.wangshuangyany.cn/gtwrnisbrb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hnqzz.top/gtreiguign.html

[L07] 处理 HTTP 状态码
来源：http://hz.gogol.net.cn/gtgwjfchxf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhaomingkeji.xyz/gtepjvfjvm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yueranfly.top/gtcxnwnzfy.html

JS:   resp.ok;  resp.status
来源：http://hz.yueranfly.top/gtmgkxqoby.html

TS:   resp.ok;  resp.status
来源：http://hz.nwbrower.top/gtwirvjowd.html

Java: resp.statusCode()
来源：http://hz.jiagoushi.top/gtytocgogr.html

Go:   resp.StatusCode
来源：http://hz.ywan-chungtsiang.top/gtrjigqmji.html

Ruby: resp.code.to_i
来源：http://hz.havefunace.top/gttpjirkut.html

C#:   (int)resp.StatusCode
来源：http://hz.ydjk.org.cn/gtbrpwigqa.html

[L08] 并发请求多个地址
来源：http://hz.jinqigufen.top/gtqpmzupvf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zhengqikj.top/gtlswsdjbu.html

PHP:  curl_multi_init() 系列
来源：http://hz.xylfe.cn/gtruzqwkfa.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hywenlv.cn/gtffryipfr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.vqdsnc.cn/gtiudobhsp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.wangdashe.top/gtlpdtonhr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.cucudq.cn/gtgqffmwkq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.shanyushiyangkeji.top/gtwansvcer.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhaomingkeji.xyz/gtofrqgznp.html

================================================================================
来源：http://hz.cdnleiting.top/gtmnfgcamw.html

M. 命令行 / 进程 / 环境
来源：http://hz.haohaochexian.top/gtmpheoghx.html

================================================================================
来源：http://hz.kuanghao11.cn/gtnllgektb.html

[M01] 读取命令行参数
来源：http://hz.jinyuanbaomall.cn/gtpdkwmzmn.html

Py:   sys.argv[1:]
来源：http://hz.aibaodan.cn/gtuvenepbd.html

PHP:  $argv;  $argc;
来源：http://hz.ywan-chungtsiang.top/gtsywhjwsu.html

JS:   process.argv.slice(2)
来源：http://hz.ydjk.org.cn/gtblgulknk.html

TS:   process.argv.slice(2)
来源：http://hz.ivvv.top/gtxwnukqxl.html

Java: args 数组（main 方法参数）
来源：http://hz.redwolf501.top/gtehdssopw.html

Go:   os.Args[1:]
来源：http://hz.fengsongda.top/gtnujllemg.html

Ruby: ARGV
来源：http://hz.redwolf501.top/gtawvtuamu.html

C#:   args 数组（Main 方法参数）
来源：http://hz.snrcjt.cn/gtizdsrcct.html

[M02] 读取环境变量
来源：http://hz.snrcjt.cn/gtevhblwql.html

Py:   os.environ.get("HOME")
来源：http://hz.xingfuxueyuan.xyz/gtsgjbapqk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.nwbrower.top/gtjkpqkqnl.html

JS:   process.env.HOME
来源：http://hz.jqgufenzy.top/gtobpyyvwk.html

TS:   process.env.HOME
来源：http://hz.gogol.net.cn/gtwzyazclw.html

Java: System.getenv("HOME")
来源：http://hz.zhixingplan.top/gtlzkxxnna.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhixingplan.top/gtwvlqtdlw.html

Ruby: ENV["HOME"]
来源：http://hz.smart0.xyz/gtouegwxff.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.daria6918.cn/gtwahutjfe.html

[M03] 执行外部命令
来源：http://hz.yueranfly.top/gtxoanjonc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.meibo888.top/gtsiwgynco.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.smart0.xyz/gtdrhcxfuw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jlsjyb.cn/gtjollgpnu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhengqikj.top/gttddyyklg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhoulong.xyz/gtbmardbms.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.redwolf501.top/gtbeixvbeb.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jinqigfzy.top/gtlneftfgo.html

C#:   Process.Start("ls", "-l");
来源：http://hz.shanyushiyangtech.top/gtdyanabci.html

[M04] 获取当前工作目录
来源：http://hz.nanxuanxn.top/gtnavijxnt.html

Py:   os.getcwd()
来源：http://hz.xylfe.cn/gtuvyfxhwy.html

PHP:  getcwd();
来源：http://hz.shangyingyoupin.top/gtrpjvcsgs.html

JS:   process.cwd()
来源：http://hz.feifeiyinyue.top/gtwjheqbdn.html

TS:   process.cwd()
来源：http://hz.52xcode.cn/gtjweoczwj.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.wangshuangyany.cn/gtgquzvutp.html

Go:   os.Getwd()
来源：http://hz.shzxlz.cn/gtxlxtopxv.html

Ruby: Dir.pwd
来源：http://hz.0kj1m.cn/gtscgwhakd.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.snrcjt.cn/gtufcljrpk.html

[M05] 设置退出码
来源：http://hz.pengpengdd.cyou/gtvggptzzx.html

Py:   sys.exit(1)
来源：http://hz.jiagoushi.top/gtjvxvodur.html

PHP:  exit(1);
来源：http://hz.zhengqikj.top/gtjyyochyv.html

JS:   process.exit(1)
来源：http://hz.9152youxi.cn/gtojgadkyg.html

TS:   process.exit(1)
来源：http://hz.cqqwz.cn/gtpqxkdgxw.html

Java: System.exit(1)
来源：http://hz.smart0.xyz/gtndazzutj.html

Go:   os.Exit(1)
来源：http://hz.wangshuangyany.cn/gtjytvpqtp.html

Ruby: exit 1
来源：http://hz.vqdsnc.cn/gtlcothsda.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.dashuyun.cn/gtibbvltxf.html

[M06] 向标准错误输出
来源：http://hz.yangfankeji.com/gtdxmaqxxq.html

Py:   print("err", file=sys.stderr)
来源：http://hz.daria6918.cn/gtepkozuik.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.shuidangran.top/gtkzhouslb.html

JS:   console.error("err")
来源：http://hz.zhengqikj.top/gtnsfssaro.html

TS:   console.error("err")
来源：http://hz.yanxiufei.cn/gtmtxrxctj.html

Java: System.err.println("err")
来源：http://hz.sufxvd.cn/gtkgzkrstd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yj20258.top/gtmfxwmjrj.html

Ruby: warn "err"
来源：http://hz.tanke756.top/gtlqymxern.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yj20258.top/gtwwkdrrub.html

[M07] 判断是否为主入口
来源：http://hz.jinqigufen.top/gtxygdszxu.html

Py:   if __name__ == "__main__":
来源：http://hz.jqgufenzy.top/gtcxtyxpai.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shanyushiyangtech.top/gtycovdzul.html

JS:   require.main === module
来源：http://hz.daxiang520.top/gtvavqwhqd.html

TS:   require.main === module
来源：http://hz.hongshengwenyu.top/gtfhvjukgc.html

Java: public static void main(String[] args)
来源：http://hz.wangdashe.top/gtlpygygir.html

Go:   func main()
来源：http://hz.cdnleiting.top/gtcokhogay.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.snrcjt.cn/gtfbriaica.html

C#:   static void Main(string[] args)
来源：http://hz.xziqi.cn/gtleamyjyc.html

[M08] 获取系统与运行时信息
来源：http://hz.daxiang520.top/gtjuglsocl.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hammf.cn/gtfhjghynj.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.bjfxy.top/gtwmwowlow.html

JS:   process.platform;  process.version
来源：http://hz.daxiang520.top/gtazbnofjw.html

TS:   process.platform;  process.version
来源：http://hz.yanxiufei.cn/gtofhfeqrb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.ivvv.top/gtstrryhje.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.hammf.cn/gtyfcterpk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zycfv.cn/gtspggadzo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jqgufenzy.top/gtqubgkdkd.html

================================================================================
来源：http://hz.pengpengdd.cyou/gteesqlniv.html

N. 数据结构与算法
来源：http://hz.9152youxi.cn/gtgjgftkko.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtadgwuayf.html

[N01] 二分查找（有序数组）
来源：http://hz.sweek.top/gtvklklkst.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hnxiangtu.top/gtjssrbqly.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhixingplan.top/gtndwezoib.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hfpthk.cn/gtpndqxwjd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.dianchejie.cn/gtcyjvmyxf.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.9152youxi.cn/gtmxseyzmv.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gtjknroinc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.tianlin.xyz/gtdfwphdew.html


<!-- 参考信息 -->