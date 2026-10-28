代发 wailian999

[J03] 字符串解析为日期
来源：http://hz.yonumen.top/gtwvhiuycl.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.daxiang520.top/gtdexkjdkw.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jinqigfzy.top/gtpyjiusus.html

JS:   new Date("2024-01-02")
来源：http://hz.quarkkingdee.top/gtrzwlozjt.html

TS:   new Date("2024-01-02")
来源：http://hz.shuidangran.top/gtyuacspao.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.sysykeji.top/gtcftgiupg.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yanxiufei.cn/gttygmrqas.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhijiandao.cn/gtmzmzfcqj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.nwbrower.top/gtzcumyvit.html

[J04] 时间戳与日期互转
来源：http://hz.jyoumei.cn/gtbdifjlao.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yanxiufei.cn/gtqfgoumcu.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhongyouzk.top/gtkfwwuxuc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jinqigufen.top/gtjtfxjnjd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yangfankeji.com/gtckzdhrji.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.dianchejie.cn/gtyddvlxta.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.guowangkeji.top/gtxlnnxvrw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jianghu66.top/gthszxjrcj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhixingplan.top/gtlsdnvpge.html

[J05] 时间加减（加 7 天）
来源：http://hz.tian-w.cn/gthoznivbb.html

Py:   now + timedelta(days=7)
来源：http://hz.bjfxy.top/gtoksmaexy.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shuidangran.top/gtoicfuxvf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhiwuduotai.top/gtgzpmuuyd.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xylfe.cn/gtlaauzdoh.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jiagoushi.top/gtqsmuxjxx.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yonumen.top/gtjgwlnhcy.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jinqigfzy.top/gtrnlilrzf.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ywan-chungtsiang.top/gtenkzmlnt.html

[J06] 计算两时间之差
来源：http://hz.chenlongwang.top/gtwklmtsuh.html

Py:   (end - start).total_seconds()
来源：http://hz.hywenlv.cn/gtbvupyqfo.html

PHP:  $end->diff($start)->days;
来源：http://hz.cdnleiting.top/gtwfogtdiz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hnxiangtu.top/gtzbdegypt.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yuanzhike.top/gtcsurvqtz.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.dianchejie.cn/gtmqxqrjpm.html

Go:   end.Sub(start).Hours()
来源：http://hz.gotoacloud.top/gtxoilntil.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jianghu66.top/gtbdhsacws.html

C#:   (end - start).TotalSeconds
来源：http://hz.jinyuanbaomall.cn/gtryufrbyk.html

[J07] 比较两个日期
来源：http://hz.jlsjyb.cn/gtgvwhyngo.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ywan-chungtsiang.top/gtkbmhotec.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.shanyushiyangtech.top/gtjookhkwa.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.pengpengdd.cyou/gtlvjttiqv.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xuanzx.com/gtgdqlsmjz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ehwqpu.com/gtiekxpfso.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.chenjidiqi.icu/gttwqxvpvv.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ydzc1.top/gtuecfyzkp.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hnqzz.top/gtezpuedns.html

[J08] 提取年月日与星期
来源：http://hz.guowangkeji.top/gthkfwtgrj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.havefunace.top/gtgcgwoqod.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hongshengwenyu.top/gtixcedyem.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.xziqi.cn/gtneawhkyv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jlsjyb.cn/gtdjhvwbcg.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.xuetiantiany.cn/gtcncvegbm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.cucudq.cn/gtskhmbnfq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.aizwys.cn/gtkyninvha.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xziqi.cn/gtjdmtzkaf.html

[J09] 时区处理
来源：http://hz.9152youxi.cn/gtwyvoadhu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.gogol.net.cn/gtcetomgbu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.xylfe.cn/gtnxwylfmg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jlsjyb.cn/gthocbaywl.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.vqdsnc.cn/gthdmsuzyo.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xuanzx.com/gtodfajbfo.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.sufxvd.cn/gttvdndjff.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ehwqpu.com/gtnocoiyej.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.daria6918.cn/gtlqanjzpa.html

[J10] 取今天 / 本月第一天
来源：http://hz.sweek.top/gtbedfscaa.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.svipenyu.cn/gtnxirkdhf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yuxming.cn/gteyakjank.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.cucudq.cn/gtplpyvxkh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jiagoushi.top/gtmbsqrfys.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.dianchejie.cn/gtqnzmavxc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhongyouzk.top/gtifrtormm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhiwuduotai.top/gtlfphjfah.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.nanxinkj.top/gtjmvokfzp.html

================================================================================
来源：http://hz.dashuyun.cn/gtbhnhgcol.html

K. JSON 与序列化
来源：http://hz.jiagoushi.top/gtmajzpmkv.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtkcbcsrsu.html

[K01] 对象转 JSON 字符串
来源：http://hz.smart0.xyz/gtvleqeicp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ehwqpu.com/gthsdcokqr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jinghuilouyu.cn/gtzmntgjbx.html

JS:   JSON.stringify(obj)
来源：http://hz.wangshuangyany.cn/gtkztwnsss.html

TS:   JSON.stringify(obj)
来源：http://hz.pycfn.com/gtxisydkdg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.quarkkingdee.top/gtzoglbisf.html

Go:   json.Marshal(obj)
来源：http://hz.havefunace.top/gtdccejmdj.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jqgfzy.top/gtvsyoywih.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ydjk.org.cn/gthycdhtcs.html

[K02] JSON 字符串转对象
来源：http://hz.guannengcc.top/gtyxmrfatu.html

Py:   json.loads(s)
来源：http://hz.mhx1999.top/gtxyhojfle.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.nanxinkj.top/gtwwnoykuj.html

JS:   JSON.parse(s)
来源：http://hz.hammf.cn/gtsgypkmda.html

TS:   JSON.parse(s)
来源：http://hz.yuanzhike.top/gtfpymsazk.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.shuidangran.top/gtfqhhtest.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.cheryme.top/gtfsbwrozs.html

Ruby: JSON.parse(s)
来源：http://hz.pengpengdd.cyou/gtklblnvor.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhixingplan.top/gtgwnucygd.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jinqigufen.top/gtewnkkvxf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yuxming.cn/gtmomqaidd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.xylfe.cn/gtbbswejfq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.wangdashe.top/gtltyvlgdw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.feifeiyinyue.top/gtppbifnvf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yanxiufei.cn/gtbzinbbsg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhijiandao.cn/gtrxkzdhte.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.dashuyun.cn/gtlhezailm.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jiagoushi.top/gtltmnznso.html

[K04] 读取 JSON 文件
来源：http://hz.cashguo.top/gtqylzktxv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.nwbrower.top/gtqxsqlaji.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shanyushiyangkeji.top/gtcqkhddhv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.aibaodan.cn/gtvmcydeob.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.meibo888.top/gtrtrkfayn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.pengpengdd.cyou/gtouawjnrg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ehwqpu.com/gtdiyaialw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yuxming.cn/gtlxflqmsf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.52xcode.cn/gttyjejpcd.html

[K05] 深拷贝对象
来源：http://hz.jinyuanbaomall.cn/gtxwulueja.html

Py:   copy.deepcopy(obj)
来源：http://hz.jiagoushi.top/gtdeusqgxs.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yvedp.cn/gtwoouwsav.html

JS:   structuredClone(obj)
来源：http://hz.zhijiandao.cn/gtcptsfqgi.html

TS:   structuredClone(obj)
来源：http://hz.sufxvd.cn/gteavhlual.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.sufxvd.cn/gttaaygkpm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hongshengwenyu.top/gtbbbbifpa.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shanyushiyangtech.top/gtpbjgqhti.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.cucudq.cn/gtznhcctzq.html

[K06] 解析 URL 查询串
来源：http://hz.0kj1m.cn/gttsobqdpl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.iojbl.cn/gtwiflmdpd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.aibaodan.cn/gtsouwkijr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zycfv.cn/gtzvhulgdg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.dashuyun.cn/gtyrzosdid.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.aizwys.cn/gtnnaimlcr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.iojbl.cn/gtebuvxbka.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.birdmap.top/gtkkzemeyy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ppjwa.cn/gtpehvkopy.html

[K07] 进制转换
来源：http://hz.shuidangran.top/gtsldpdbbh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.bjfxy.top/gtmqicuygz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.nanxinkj.top/gtiafpwbjn.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yj20258.top/gturcwibdz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.gotoacloud.top/gtmvzbugkd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hfpthk.cn/gtuaqpcoks.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.svipenyu.cn/gtwmatrgbc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.gotoacloud.top/gtxerqfzte.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.chenzaomai.com/gtiofscdkn.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.nanxuanxn.top/gtabybrugl.html

Py:   pickle.dumps(obj)
来源：http://hz.mhx1999.top/gtlnxyfsjb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hywenlv.cn/gtfbcnpmoz.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.chenjidiqi.icu/gtczvausdp.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yvedp.cn/gthvcpftfe.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.feifeiyinyue.top/gtegyzwohy.html

Go:   encoding/gob
来源：http://hz.gaohongyu789.top/gttmcpzapc.html

Ruby: Marshal.dump(obj)
来源：http://hz.jinghuilouyu.cn/gtxnfaxbuc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhaomingkeji.xyz/gthuocmyfw.html

================================================================================
来源：http://hz.cqqwz.cn/gtfkxzubwn.html

L. 网络请求
来源：http://hz.zhiwuduotai.top/gtydpsbcfg.html

================================================================================
来源：http://hz.zhongyouzk.top/gtjpldcisu.html

[L01] 发送 GET 请求
来源：http://hz.yj202588.top/gtbzxmckui.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cqqwz.cn/gtdbduvnwv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.redwolf501.top/gtjitjjpnx.html

JS:   await fetch(url)
来源：http://hz.shanyushiyangkeji.top/gtcrbfugvd.html

TS:   await fetch(url)
来源：http://hz.daxiang520.top/gtprfjvxkn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zycfv.cn/gtksvnigyl.html

Go:   resp, err := http.Get(url)
来源：http://hz.aizwys.cn/gtpnqwobmj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.tianlin.xyz/gtopiuwrqi.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yj202588.top/gtvcehobdb.html

[L02] 发送 POST JSON
来源：http://hz.ehwqpu.com/gtlfdujjat.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.chenzaomai.com/gtdrxaxfsz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.andypj.xyz/gtklihoylt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinqigufen.top/gtyszfnctv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.chenzaomai.com/gtudobffwb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.sysykeji.top/gtbcrrobsq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.sysykeji.top/gtockujfme.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yonumen.top/gtsonaefzm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hysaishi.cn/gtxgtshahv.html

[L03] 设置自定义请求头
来源：http://hz.jlsjyb.cn/gtkbfuxoaz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.nwbrower.top/gtvbdomrky.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zhengqikj.top/gtpguflisk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xuanzx.com/gttqffsqgm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj202588.top/gtssxxavyk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.wangshuangyany.cn/gtvpsyffon.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jiagoushi.top/gtrmruwgjq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.tanke756.top/gteaeyaysh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhijiandao.cn/gtiwdzaanz.html

[L04] 设置超时
来源：http://hz.cheryme.top/gtbmqirhse.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cashguo.top/gtzcaffazx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.smart0.xyz/gtltcfiddt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhongyouzk.top/gthcrcxhxj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zdqjudy.top/gtxmhiqrbz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jinqigfzy.top/gtptqceswi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yvedp.cn/gtoojolrzk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.fengsongda.top/gtpuqbwfsu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.andypj.xyz/gtwvheutef.html

[L05] 上传文件（multipart）
来源：http://hz.zhongyouzk.top/gtglktmvmq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.xylfe.cn/gtslwntztf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.andypj.xyz/gttcjmwgap.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.sweek.top/gteetjzlet.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.cheryme.top/gtdnaoctkh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.9152youxi.cn/gtbkpspkza.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.c1oappe.top/gtglzueucn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jinqigfzy.top/gtcfksyckd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.daxiang520.top/gtnpzrzjhd.html

[L06] 解析响应为 JSON
来源：http://hz.daxiang520.top/gtlhpvwduq.html

Py:   resp.json()
来源：http://hz.jyoumei.cn/gticjqqbyn.html

PHP:  json_decode($body, true);
来源：http://hz.yuxming.cn/gtjltpwsfw.html

JS:   await resp.json()
来源：http://hz.ehwqpu.com/gtrjcrrbaa.html

TS:   await resp.json()
来源：http://hz.yj20258.top/gtjxtbsdre.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jinghuilouyu.cn/gtsefwyrcn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.sxryk.cn/gtxvnsnbse.html

Ruby: JSON.parse(resp.body)
来源：http://hz.hnqzz.top/gtwviokphi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.sxryk.cn/gtbhhsagwg.html

[L07] 处理 HTTP 状态码
来源：http://hz.meibo888.top/gtbddgkozl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hnxiangtu.top/gtcyrjwrku.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.xuetiantiany.cn/gtwfqjbmrh.html

JS:   resp.ok;  resp.status
来源：http://hz.jiagoushi.top/gtlzhjtmrx.html

TS:   resp.ok;  resp.status
来源：http://hz.jianghu66.top/gtuqrxlzus.html

Java: resp.statusCode()
来源：http://hz.yanxiufei.cn/gtissghdwm.html

Go:   resp.StatusCode
来源：http://hz.yj20258.top/gtwgwmcrkb.html

Ruby: resp.code.to_i
来源：http://hz.cucudq.cn/gtxqhgtnsk.html

C#:   (int)resp.StatusCode
来源：http://hz.fzhhl.top/gtmuqjqbir.html

[L08] 并发请求多个地址
来源：http://hz.yueranfly.top/gtljvyklxx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.tian-w.cn/gtmpdnpkkw.html

PHP:  curl_multi_init() 系列
来源：http://hz.sweek.top/gtqsrjjlbn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tianlin.xyz/gtrjoodbyf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.quarkkingdee.top/gtgcqtvunz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jinqigfzy.top/gtwaluznnn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jinyuanbaomall.cn/gtwnqcyizk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hnqzz.top/gtpxzqessi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.52xcode.cn/gtmcbnbobr.html

================================================================================
来源：http://hz.cucudq.cn/gtsvmcutww.html

M. 命令行 / 进程 / 环境
来源：http://hz.xinyue.icu/gtjmevhdhe.html

================================================================================
来源：http://hz.iojbl.cn/gtwxpjrzvl.html

[M01] 读取命令行参数
来源：http://hz.jinghuilouyu.cn/gtjyhhgpei.html

Py:   sys.argv[1:]
来源：http://hz.haohaochexian.top/gtrigvkhzd.html

PHP:  $argv;  $argc;
来源：http://hz.tanke756.top/gtznctxgnl.html

JS:   process.argv.slice(2)
来源：http://hz.haohaochexian.top/gtnvwanxdt.html

TS:   process.argv.slice(2)
来源：http://hz.svipenyu.cn/gtvtlhggwl.html

Java: args 数组（main 方法参数）
来源：http://hz.jiagoushi.top/gtuxatrlhq.html

Go:   os.Args[1:]
来源：http://hz.nanxinkj.top/gtommejczb.html

Ruby: ARGV
来源：http://hz.nanxinkj.top/gtiulamxkd.html

C#:   args 数组（Main 方法参数）
来源：http://hz.fengsongda.top/gtjxnhvges.html

[M02] 读取环境变量
来源：http://hz.guowangkeji.top/gtzepvoqhb.html

Py:   os.environ.get("HOME")
来源：http://hz.52xcode.cn/gtgjemfnrq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zhixingplan.top/gtfvymtgee.html

JS:   process.env.HOME
来源：http://hz.birdmap.top/gtqlophnar.html

TS:   process.env.HOME
来源：http://hz.yj202588.top/gtcrcdwtqr.html

Java: System.getenv("HOME")
来源：http://hz.tian-w.cn/gtnxbfsjlm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.xuetiantiany.cn/gtvecbfuwi.html

Ruby: ENV["HOME"]
来源：http://hz.yj20258.top/gtggbbthei.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.aizwys.cn/gtzautiuqj.html

[M03] 执行外部命令
来源：http://hz.cqqwz.cn/gtjugfcbkl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jinqigufen.top/gtnuqkkqqy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.dianchejie.cn/gtrrabgyzh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.nanxinkj.top/gtpjuqskho.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.pycfn.com/gtnjvssdol.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zycfv.cn/gtjpcwmzna.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.dianchejie.cn/gthddxknlw.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.cheryme.top/gtvegqawpp.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zdqjudy.top/gtkfelvvbg.html

[M04] 获取当前工作目录
来源：http://hz.hammf.cn/gtzcxswwyl.html

Py:   os.getcwd()
来源：http://hz.zhixingplan.top/gtprhpicyg.html

PHP:  getcwd();
来源：http://hz.hfpthk.cn/gtdmjkxaoh.html

JS:   process.cwd()
来源：http://hz.aizwys.cn/gtbbtcyjcv.html

TS:   process.cwd()
来源：http://hz.shuidangran.top/gttgequmpm.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.52xcode.cn/gtesiecbvc.html

Go:   os.Getwd()
来源：http://hz.aizwys.cn/gteuhmwxmb.html

Ruby: Dir.pwd
来源：http://hz.sysykeji.top/gtultpevpu.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.316326.xyz/gtvecwyanb.html

[M05] 设置退出码
来源：http://hz.nanxinkj.top/gtjzccjwzh.html

Py:   sys.exit(1)
来源：http://hz.tianlin.xyz/gtsxexpqyl.html

PHP:  exit(1);
来源：http://hz.shuidangran.top/gtjuzeauts.html

JS:   process.exit(1)
来源：http://hz.ybcxt.top/gtdgcgotyj.html

TS:   process.exit(1)
来源：http://hz.zdqjudy.top/gtnzadjsym.html

Java: System.exit(1)
来源：http://hz.jianghu66.top/gtgelunvrn.html

Go:   os.Exit(1)
来源：http://hz.vqdsnc.cn/gtoeuqdxfx.html

Ruby: exit 1
来源：http://hz.yangfankeji.com/gtqolwnvsb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.0kj1m.cn/gtghwcdhyf.html

[M06] 向标准错误输出
来源：http://hz.ppjwa.cn/gtzbnucfwz.html

Py:   print("err", file=sys.stderr)
来源：http://hz.fzhhl.top/gtyylwlobo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jqgufenzy.top/gtbbyqhrbj.html

JS:   console.error("err")
来源：http://hz.nanxinkj.top/gtehwmwhje.html

TS:   console.error("err")
来源：http://hz.yuanzhike.top/gteccbkarr.html

Java: System.err.println("err")
来源：http://hz.yangfankeji.com/gthrkcpzxi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.svipenyu.cn/gtordyyjer.html

Ruby: warn "err"
来源：http://hz.ydzc1.top/gtvywbbrni.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhengqikj.top/gtcgpeyshh.html

[M07] 判断是否为主入口
来源：http://hz.sweek.top/gthxbqwfsa.html

Py:   if __name__ == "__main__":
来源：http://hz.tianlin.xyz/gttzgctpnu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.svipenyu.cn/gtstpfvhns.html

JS:   require.main === module
来源：http://hz.yj20258.top/gtgmcwkvvv.html

TS:   require.main === module
来源：http://hz.shanyushiyangkeji.top/gtyebupfdk.html

Java: public static void main(String[] args)
来源：http://hz.guowangkeji.top/gtvjaofnsu.html

Go:   func main()
来源：http://hz.ywan-chungtsiang.top/gtqlkftgsm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.gzhubu.top/gtdqwouwmc.html

C#:   static void Main(string[] args)
来源：http://hz.shangyingyoupin.top/gtstdwefok.html

[M08] 获取系统与运行时信息
来源：http://hz.gaohongyu789.top/gtxipsurer.html

Py:   platform.system();  platform.python_version()
来源：http://hz.xuetiantiany.cn/gtgcguzuoi.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jqgufenzy.top/gtzebcefez.html

JS:   process.platform;  process.version
来源：http://hz.chenlongwang.top/gtxlzwpsly.html

TS:   process.platform;  process.version
来源：http://hz.ydzc1.top/gtauaopcpw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jinqigufen.top/gtufccomyt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.nanxuanxn.top/gtijheowjt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.daxiang520.top/gtpkpeyosl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yuxming.cn/gtnevqqafj.html

================================================================================
来源：http://hz.hysaishi.cn/gtuwgzaxtb.html

N. 数据结构与算法
来源：http://hz.sufxvd.cn/gtgvirujnb.html

================================================================================
来源：http://hz.sufxvd.cn/gtzgilnykw.html


<!-- 参考信息 -->