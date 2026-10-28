代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yongpay.top/gtwmsuipwl.html

[J04] 时间戳与日期互转
来源：http://hz.fengsongda.top/gtfoclnzym.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.sysykeji.top/gtgotyqpal.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.nanxinkj.top/gtbnedmtjs.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.pengpengdd.cyou/gtanfcogzw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hnqzz.top/gtbjyxngmq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.havefunace.top/gtaazmxzjn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.xuetiantiany.cn/gtyurguxfb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.svipenyu.cn/gtptvnjuij.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.wangshuangyany.cn/gttqqtajic.html

[J05] 时间加减（加 7 天）
来源：http://hz.ybcxt.top/gtwkhjpyfm.html

Py:   now + timedelta(days=7)
来源：http://hz.52xcode.cn/gtmdgiopfl.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.nanxuanxn.top/gtyswzvlku.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhijiandao.cn/gtnuefjobb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shanyushiyangkeji.top/gtnxpwyitp.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.cdnleiting.top/gtdtvawtlz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.daxiang520.top/gtpidiflcq.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hywenlv.cn/gttxsuhwfe.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.nwbrower.top/gtypyoxixo.html

[J06] 计算两时间之差
来源：http://hz.jinqigfzy.top/gtsvibjwdo.html

Py:   (end - start).total_seconds()
来源：http://hz.haohaochexian.top/gtuepqxnky.html

PHP:  $end->diff($start)->days;
来源：http://hz.hfpthk.cn/gtessoxeco.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ppjwa.cn/gtifuiedvn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ybcxt.top/gtxhdntrhy.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jqgufenzy.top/gtxrkrlqih.html

Go:   end.Sub(start).Hours()
来源：http://hz.quarkkingdee.top/gtbjxdanbd.html

Ruby: end - start                 # 返回秒数
来源：http://hz.gogol.net.cn/gtlvqgjwoo.html

C#:   (end - start).TotalSeconds
来源：http://hz.hywenlv.cn/gtkzekboes.html

[J07] 比较两个日期
来源：http://hz.hongshengwenyu.top/gtrtefcexf.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yongpay.top/gttzkyargu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.birdmap.top/gtnqsxuvkf.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.pycfn.com/gtdgptezjc.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yanxiufei.cn/gtlnnhjsgf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yvedp.cn/gtbdrfrqfb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.svipenyu.cn/gtrldvspsh.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hnqzz.top/gtrqhlsdyb.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yueranfly.top/gtxeoqlrnh.html

[J08] 提取年月日与星期
来源：http://hz.aibaodan.cn/gtthkzqxao.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.daxiang520.top/gtgcanpmou.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhengqikj.top/gtynprufno.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shanyushiyangkeji.top/gtrdrsjibj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ehwqpu.com/gtojlzufcm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hywenlv.cn/gtxgeathtp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.haohaochexian.top/gtnpnyqolb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhijiandao.cn/gtekdwwopn.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.cqqwz.cn/gtarevzwek.html

[J09] 时区处理
来源：http://hz.meibo888.top/gtfxoiwzyr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.aizwys.cn/gtmpqvgnxv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.c1oappe.top/gtecmktvtg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.bjfxy.top/gtebqrewkg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ppjwa.cn/gtljurahgm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.snrcjt.cn/gtkpivflvt.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.andypj.xyz/gtmwquhmhc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.feifeiyinyue.top/gtbozeahse.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.dianchejie.cn/gthrhtrffa.html

[J10] 取今天 / 本月第一天
来源：http://hz.bjfxy.top/gthifycsem.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhengqikj.top/gtrwutkdwf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.9152youxi.cn/gtrgbdtmqn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.mhx1999.top/gtollhopwp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hammf.cn/gtktsigixc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.aibaodan.cn/gtqywrhzln.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.sxryk.cn/gtqqybnile.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hnqzz.top/gtfwkowdta.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.shzxlz.cn/gtxpuigoll.html

================================================================================
来源：http://hz.sysykeji.top/gtjkbwtwsy.html

K. JSON 与序列化
来源：http://hz.aibaodan.cn/gteyhakswc.html

================================================================================
来源：http://hz.quarkkingdee.top/gthrgxyhuw.html

[K01] 对象转 JSON 字符串
来源：http://hz.meibo888.top/gtlqcgekob.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.daxiang520.top/gtdfzrimtn.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.shangyingyoupin.top/gtzdmwfeiu.html

JS:   JSON.stringify(obj)
来源：http://hz.aizwys.cn/gtbidwnmob.html

TS:   JSON.stringify(obj)
来源：http://hz.hysaishi.cn/gtzafbejdn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.vqdsnc.cn/gtaxyilxzu.html

Go:   json.Marshal(obj)
来源：http://hz.xuetiantiany.cn/gtblwpnrtk.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yj20258888.top/gtdjfmdvhp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.shanyushiyangkeji.top/gtujloztdx.html

[K02] JSON 字符串转对象
来源：http://hz.redwolf501.top/gtkhthbzjl.html

Py:   json.loads(s)
来源：http://hz.316326.xyz/gtzlfbudoj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhaomingkeji.xyz/gtkgzirasu.html

JS:   JSON.parse(s)
来源：http://hz.snrcjt.cn/gtrnbgtgzb.html

TS:   JSON.parse(s)
来源：http://hz.ydjk.org.cn/gtbizactjn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.haohaochexian.top/gtzisbxegk.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhiwuduotai.top/gtkfccqrge.html

Ruby: JSON.parse(s)
来源：http://hz.havefunace.top/gtprrecfec.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.redwolf501.top/gtfdqtyrsj.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zycfv.cn/gtgmzkktzm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.nanxuanxn.top/gtzcfjhiwy.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.daxiang520.top/gtenvexfbn.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj20258888.top/gtytbcqhpt.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hongshengwenyu.top/gtypuahewc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.bjfxy.top/gthokiukkj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xuetiantiany.cn/gturneuixa.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.cdnleiting.top/gtqhmnyrsi.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.pycfn.com/gtrlntqkal.html

[K04] 读取 JSON 文件
来源：http://hz.hywenlv.cn/gtenzcofzx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.andypj.xyz/gtwopvfcrq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.havefunace.top/gtvyzldvdh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.redwolf501.top/gtbtrmvmcn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.9152youxi.cn/gtimerxjjc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yueranfly.top/gtxepbquwr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ybcxt.top/gtjgtygtpj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhijiandao.cn/gtmjwqyolx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.xingfuxueyuan.xyz/gtglibxadt.html

[K05] 深拷贝对象
来源：http://hz.cqqwz.cn/gtuuapakui.html

Py:   copy.deepcopy(obj)
来源：http://hz.9152youxi.cn/gtxekroxfa.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hammf.cn/gtmfsoqkxk.html

JS:   structuredClone(obj)
来源：http://hz.ydzc1.top/gtlpifzzhy.html

TS:   structuredClone(obj)
来源：http://hz.cheryme.top/gtfplrrqry.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yvedp.cn/gtniknjnzf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.tian-w.cn/gtlbuswmmd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhengqikj.top/gtsqximckp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.xuetiantiany.cn/gtorzxhyic.html

[K06] 解析 URL 查询串
来源：http://hz.hywenlv.cn/gtwmnndbgg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.daxiang520.top/gtqazatcwn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.ybcxt.top/gttxtkrjrv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yangfankeji.com/gtlexziqin.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ydjk.org.cn/gtgpsbjxbb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yonumen.top/gtxdgmnnty.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.0kj1m.cn/gturghfydm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hnxiangtu.top/gtxyltfxbd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yuanzhike.top/gteemfkhbt.html

[K07] 进制转换
来源：http://hz.yvedp.cn/gtrvzinnva.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.guowangkeji.top/gtzqqmhgwx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.wangdashe.top/gthmwtrvnp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.sxryk.cn/gtkqntnlag.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.aibaodan.cn/gtywfvcrbn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.svipenyu.cn/gtalmqynho.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.daria6918.cn/gtowlztbyv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.kuanghao11.cn/gtquphspjj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zdqjudy.top/gtamrrnfai.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jiagoushi.top/gtcjgfwowi.html

Py:   pickle.dumps(obj)
来源：http://hz.xylfe.cn/gtofwvhzgf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jinqigfzy.top/gtqbyttdid.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.feifeiyinyue.top/gtfxrsnywj.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hongshengwenyu.top/gtnhfwtpvt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.kuanghao11.cn/gtaiwddtkr.html

Go:   encoding/gob
来源：http://hz.jiagoushi.top/gtsdzewioa.html

Ruby: Marshal.dump(obj)
来源：http://hz.xuetiantiany.cn/gtxtcvbsed.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.chenlongwang.top/gtdgorcpgq.html

================================================================================
来源：http://hz.tanke756.top/gtjgwvxfob.html

L. 网络请求
来源：http://hz.316326.xyz/gtesnpybev.html

================================================================================
来源：http://hz.yanxiufei.cn/gtngnfjpqj.html

[L01] 发送 GET 请求
来源：http://hz.jqgufenzy.top/gtedwaqcrp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.sysykeji.top/gtkwloeujz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yvedp.cn/gtwwksdlhs.html

JS:   await fetch(url)
来源：http://hz.zhijiandao.cn/gtxphwyhxm.html

TS:   await fetch(url)
来源：http://hz.svipenyu.cn/gtduxzzthr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yonumen.top/gtbivaxtqv.html

Go:   resp, err := http.Get(url)
来源：http://hz.yj20258.top/gtdaxiexri.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.chenjidiqi.icu/gtpcdwcoai.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zhiwuduotai.top/gtqhxrvkak.html

[L02] 发送 POST JSON
来源：http://hz.xylfe.cn/gtquxpuvsd.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.0kj1m.cn/gtstowajkx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xinyue.icu/gtdexccqis.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.kuanghao11.cn/gtshsjhgfd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gaohongyu789.top/gtvptlhddv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yueranfly.top/gtksztlued.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.meibo888.top/gtcspscjgi.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yongpay.top/gtmylrunru.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yongpay.top/gtctvcapau.html

[L03] 设置自定义请求头
来源：http://hz.tian-w.cn/gtyitvphvw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.daria6918.cn/gtaxkvmxsa.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.9152youxi.cn/gtaixgvgge.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sysykeji.top/gtxuaekent.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sufxvd.cn/gtbxqpbuxw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.fengsongda.top/gtlvulqknx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.wangshuangyany.cn/gtgabxbwmi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hfpthk.cn/gtqxbaqrem.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jinqigfzy.top/gtgbbzqxgk.html

[L04] 设置超时
来源：http://hz.zhongyouzk.top/gtgguijubj.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jinghuilouyu.cn/gtaqjylwlc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.sysykeji.top/gtozwzhpdo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zdqjudy.top/gtmugwmedk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xziqi.cn/gtefuoigyz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jinghuilouyu.cn/gtvjrgqeil.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.bjfxy.top/gtuuweeklz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.tianlin.xyz/gtuwthztmu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.0kj1m.cn/gthugdmtro.html

[L05] 上传文件（multipart）
来源：http://hz.ydzc1.top/gtemmmgpsp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yj202588.top/gtwnfhdsel.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.quarkkingdee.top/gtgpzcdrxx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zdqjudy.top/gtpczurhhy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jiagoushi.top/gthzaprwdm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.nanxinkj.top/gtwymlnvpr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhoulong.xyz/gthrhcicvc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.feifeiyinyue.top/gtrslzmwue.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jinyuanbaomall.cn/gtzkeobbzq.html

[L06] 解析响应为 JSON
来源：http://hz.yuxming.cn/gtucejrjzk.html

Py:   resp.json()
来源：http://hz.smart0.xyz/gtjtpawqjh.html

PHP:  json_decode($body, true);
来源：http://hz.316326.xyz/gtupdcypaw.html

JS:   await resp.json()
来源：http://hz.hfpthk.cn/gtqmytbahk.html

TS:   await resp.json()
来源：http://hz.zycfv.cn/gtetdvdcuk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yanxiufei.cn/gthkbhpwry.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jinqigfzy.top/gtuhudmzrl.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ppjwa.cn/gtjkgscnfy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhongyouzk.top/gtqbbmfepf.html

[L07] 处理 HTTP 状态码
来源：http://hz.cashguo.top/gtyblrxlkf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.haohaochexian.top/gtkmvslixo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.xylfe.cn/gtxcevobvw.html

JS:   resp.ok;  resp.status
来源：http://hz.redwolf501.top/gtjzonfyqz.html

TS:   resp.ok;  resp.status
来源：http://hz.yanxiufei.cn/gtbxkbrsha.html

Java: resp.statusCode()
来源：http://hz.chenlongwang.top/gtbjallmdg.html

Go:   resp.StatusCode
来源：http://hz.c1oappe.top/gtdknijzyy.html

Ruby: resp.code.to_i
来源：http://hz.ehwqpu.com/gtmrxnwlfz.html

C#:   (int)resp.StatusCode
来源：http://hz.zhoulong.xyz/gtgtrmwpzz.html

[L08] 并发请求多个地址
来源：http://hz.zhaomingkeji.xyz/gtexwyjsjm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.cdnleiting.top/gtksanwbtj.html

PHP:  curl_multi_init() 系列
来源：http://hz.andypj.xyz/gtbxzdkvde.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.wangshuangyany.cn/gtmoscrjpf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xylfe.cn/gtyilfnjez.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.c1oappe.top/gtpyxogrjo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yj20258.top/gtvmjjtzhq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.bjfxy.top/gtdtecunhf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.pengpengdd.cyou/gtdolrbfuw.html

================================================================================
来源：http://hz.zycfv.cn/gtxvcpqibd.html

M. 命令行 / 进程 / 环境
来源：http://hz.ybcxt.top/gtrodyjcpc.html

================================================================================
来源：http://hz.9152youxi.cn/gtpjfombxe.html

[M01] 读取命令行参数
来源：http://hz.yonumen.top/gtknhkbpsk.html

Py:   sys.argv[1:]
来源：http://hz.cheryme.top/gtruaypzfn.html

PHP:  $argv;  $argc;
来源：http://hz.guowangkeji.top/gtnqaylbcb.html

JS:   process.argv.slice(2)
来源：http://hz.shzxlz.cn/gtrgpkbdqu.html

TS:   process.argv.slice(2)
来源：http://hz.pycfn.com/gtfxfvlofx.html

Java: args 数组（main 方法参数）
来源：http://hz.sweek.top/gteoxiltrj.html

Go:   os.Args[1:]
来源：http://hz.fzhhl.top/gtmrfymkxc.html

Ruby: ARGV
来源：http://hz.zycfv.cn/gthgtxuhyh.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yanxiufei.cn/gtxqdpwfbj.html

[M02] 读取环境变量
来源：http://hz.ppjwa.cn/gtnfhjajxb.html

Py:   os.environ.get("HOME")
来源：http://hz.kuanghao11.cn/gtanrqyyxh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.dianchejie.cn/gtwmgokofo.html

JS:   process.env.HOME
来源：http://hz.ehwqpu.com/gtbnmqqzjs.html

TS:   process.env.HOME
来源：http://hz.guannengcc.top/gtqgeicbvt.html

Java: System.getenv("HOME")
来源：http://hz.nwbrower.top/gthtzikevx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.birdmap.top/gtxpyobiif.html

Ruby: ENV["HOME"]
来源：http://hz.xuanzx.com/gtphsoxgmq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.gogol.net.cn/gtbdrgblhe.html

[M03] 执行外部命令
来源：http://hz.dianchejie.cn/gtffmqxhbu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.svipenyu.cn/gtxmiqqhyg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.nanxuanxn.top/gtylxizjbf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hfpthk.cn/gtnbvttcdq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.smart0.xyz/gtdumwjoew.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.wangshuangyany.cn/gtxbmwsqyl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.aizwys.cn/gtxupjwppx.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhiwuduotai.top/gtnpciczzo.html

C#:   Process.Start("ls", "-l");
来源：http://hz.pengpengdd.cyou/gtjdpwrzxe.html

[M04] 获取当前工作目录
来源：http://hz.andypj.xyz/gtgkeavumm.html

Py:   os.getcwd()
来源：http://hz.cucudq.cn/gtbwivqxkl.html

PHP:  getcwd();
来源：http://hz.hnxiangtu.top/gtnpnjiriy.html

JS:   process.cwd()
来源：http://hz.nwbrower.top/gtypnseqla.html

TS:   process.cwd()
来源：http://hz.sysykeji.top/gtnmakjekn.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ybcxt.top/gtswfnbrln.html

Go:   os.Getwd()
来源：http://hz.tanke756.top/gtrcjvcngp.html

Ruby: Dir.pwd
来源：http://hz.jyoumei.cn/gtpzpniuke.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ehwqpu.com/gtntdujnxa.html

[M05] 设置退出码
来源：http://hz.ivvv.top/gtppwbiuqn.html

Py:   sys.exit(1)
来源：http://hz.yongpay.top/gtybviglnq.html

PHP:  exit(1);
来源：http://hz.xinyue.icu/gtkaexyyfr.html

JS:   process.exit(1)
来源：http://hz.yj202588.top/gtykhebdbu.html

TS:   process.exit(1)
来源：http://hz.jlsjyb.cn/gtzavjscno.html

Java: System.exit(1)
来源：http://hz.chenjidiqi.icu/gtuoqjodcs.html

Go:   os.Exit(1)
来源：http://hz.jqgufenzy.top/gtqfqsvorf.html

Ruby: exit 1
来源：http://hz.xinyue.icu/gtjpyksgym.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.xingfuxueyuan.xyz/gtjxowpdbu.html

[M06] 向标准错误输出
来源：http://hz.yj202588.top/gtlkmasvkz.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ybcxt.top/gtpjnbkkef.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yueranfly.top/gtmwdtdiqv.html

JS:   console.error("err")
来源：http://hz.yj20258.top/gtmqduqbhv.html

TS:   console.error("err")
来源：http://hz.guowangkeji.top/gtzifjnvax.html

Java: System.err.println("err")
来源：http://hz.chenjidiqi.icu/gttwnhmbhz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.hfpthk.cn/gttvpujpgc.html

Ruby: warn "err"
来源：http://hz.xinyue.icu/gteroagsno.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yanxiufei.cn/gtlpnrvaug.html

[M07] 判断是否为主入口
来源：http://hz.zhijiandao.cn/gtciypskpb.html

Py:   if __name__ == "__main__":
来源：http://hz.ydzc1.top/gtmtlxpajo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.52xcode.cn/gtisfuwxfy.html

JS:   require.main === module
来源：http://hz.daria6918.cn/gttqaigbkp.html

TS:   require.main === module
来源：http://hz.yvedp.cn/gtvgvxsguj.html

Java: public static void main(String[] args)
来源：http://hz.sysykeji.top/gtyxcfdjbq.html

Go:   func main()
来源：http://hz.yueranfly.top/gtvxoslvuh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhaomingkeji.xyz/gtoeyoidit.html

C#:   static void Main(string[] args)
来源：http://hz.9152youxi.cn/gtejsskkwc.html

[M08] 获取系统与运行时信息
来源：http://hz.0kj1m.cn/gtibnqlfwx.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yongpay.top/gtclbogthe.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.snrcjt.cn/gtxpbvekvd.html

JS:   process.platform;  process.version
来源：http://hz.fengsongda.top/gtcjwayaww.html

TS:   process.platform;  process.version
来源：http://hz.hysaishi.cn/gtuwlprmrq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.aizwys.cn/gtptiqxwbk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.smart0.xyz/gtjjcnvfgv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.xuetiantiany.cn/gtbhpljyji.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.sxryk.cn/gtehafcxjg.html

================================================================================
来源：http://hz.yuxming.cn/gtdmgpxlxw.html

N. 数据结构与算法
来源：http://hz.hammf.cn/gtxbicvszn.html

================================================================================
来源：http://hz.hnqzz.top/gtxjidwcwx.html

[N01] 二分查找（有序数组）
来源：http://hz.yvedp.cn/gtmstttlmu.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.gotoacloud.top/gtswgucvfd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.xylfe.cn/gtwbxzeztj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hammf.cn/gtadhdiegi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jianghu66.top/gtlvxvbbxq.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.andypj.xyz/gttbbqquez.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhongyouzk.top/gtpeqtvtzw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.nanxuanxn.top/gtinfmchsh.html


<!-- 参考信息 -->