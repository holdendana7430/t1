代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhijiandao.cn/gtocxydrno.html

JS:   new Date();  Date.now()
来源：http://hz.shangyingyoupin.top/gtyglsqbsu.html

TS:   new Date();  Date.now()
来源：http://hz.ydjk.org.cn/gtsegnjwyv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hfpthk.cn/gtjzahymbx.html

Go:   time.Now()
来源：http://hz.ivvv.top/gtdhkqxggo.html

Ruby: Time.now
来源：http://hz.xylfe.cn/gtijgauden.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.chenjidiqi.icu/gtzihdaefc.html

[J02] 格式化输出
来源：http://hz.tianlin.xyz/gtcwlpfbpb.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cashguo.top/gttbfrmjss.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.cheryme.top/gtqzalpont.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jyoumei.cn/gtnsqazlbv.html

TS:   d.toISOString()
来源：http://hz.jinqigufen.top/gtqvagyjec.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jlsjyb.cn/gtkdgbifqj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhoulong.xyz/gtbptftlej.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.dashuyun.cn/gtocpqpisr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.dianchejie.cn/gthqxbptaf.html

[J03] 字符串解析为日期
来源：http://hz.tianlin.xyz/gtuxebpnuo.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.sufxvd.cn/gtcnkifhcl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.nanxuanxn.top/gtcwzuhyoq.html

JS:   new Date("2024-01-02")
来源：http://hz.xuetiantiany.cn/gtyoepbxjr.html

TS:   new Date("2024-01-02")
来源：http://hz.cdnleiting.top/gtqsqoitpz.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hfpthk.cn/gtokwwthiw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jinghuilouyu.cn/gtpljvycap.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ybcxt.top/gtfukizgyn.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.fengsongda.top/gtdsyljbwf.html

[J04] 时间戳与日期互转
来源：http://hz.mhx1999.top/gtunvcaqiw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yj202588.top/gtatdqdiht.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.daxiang520.top/gtymbfweqs.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hfpthk.cn/gtspgnijvd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.fzhhl.top/gtipvmccrh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.meibo888.top/gtmuaxmhip.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.aibaodan.cn/gtilmuvgxi.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.gogol.net.cn/gtdtmhkbit.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yanxiufei.cn/gtiejyzlsf.html

[J05] 时间加减（加 7 天）
来源：http://hz.gotoacloud.top/gtctdscwkw.html

Py:   now + timedelta(days=7)
来源：http://hz.chenlongwang.top/gttihhopjp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yj20258.top/gtygfjnypo.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nwbrower.top/gtkzybykpc.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hongshengwenyu.top/gthexcqczu.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jinghuilouyu.cn/gthxkyqhht.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cashguo.top/gtewfguuez.html

Ruby: Time.now + 7 * 86400
来源：http://hz.sufxvd.cn/gtllrxvfyl.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.sweek.top/gtuazuucfo.html

[J06] 计算两时间之差
来源：http://hz.zhaomingkeji.xyz/gtbtrsfkxt.html

Py:   (end - start).total_seconds()
来源：http://hz.jianghu66.top/gtukpjvgnr.html

PHP:  $end->diff($start)->days;
来源：http://hz.316326.xyz/gteyxcsupx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.meibo888.top/gtfiwhbawk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yuanzhike.top/gtysfcufsm.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jianghu66.top/gtpkutcnlq.html

Go:   end.Sub(start).Hours()
来源：http://hz.shanyushiyangtech.top/gtlwpjctzk.html

Ruby: end - start                 # 返回秒数
来源：http://hz.xziqi.cn/gtretiqsyu.html

C#:   (end - start).TotalSeconds
来源：http://hz.vqdsnc.cn/gttowbkxdd.html

[J07] 比较两个日期
来源：http://hz.jinyuanbaomall.cn/gtilajrdik.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.svipenyu.cn/gtgsqbviht.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jqgfzy.top/gtyhwxjfso.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.pengpengdd.cyou/gtkdlzfabd.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ydzc1.top/gtaeepbkgs.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.shanyushiyangtech.top/gtcoiwpfra.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jyoumei.cn/gtgvgizntq.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.haohaochexian.top/gtmjcasycs.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.fengsongda.top/gtxemgcxhs.html

[J08] 提取年月日与星期
来源：http://hz.yongpay.top/gtccxtvkxu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.daria6918.cn/gtoozsenvx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yuxming.cn/gtvwasqnte.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.chenlongwang.top/gtqknfdsfr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.daria6918.cn/gttsuccpcc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yongpay.top/gtcodrvuks.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.cqqwz.cn/gtnrezpbue.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhoulong.xyz/gtprilvbwm.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.aibaodan.cn/gttvaipkrd.html

[J09] 时区处理
来源：http://hz.jinghuilouyu.cn/gtbuvqmgae.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.sweek.top/gtrohhjrje.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.chenjidiqi.icu/gtxkkeayij.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinqigfzy.top/gtqsitfugf.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cucudq.cn/gtztrjftfg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.chenjidiqi.icu/gtfcpgmlzs.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.cdnleiting.top/gthbrgtvle.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.dianchejie.cn/gtsnovsjzu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.meibo888.top/gtdnviwwue.html

[J10] 取今天 / 本月第一天
来源：http://hz.hywenlv.cn/gtzyzrrgfn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.kuanghao11.cn/gtnfuwjxrx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.haohaochexian.top/gtfrwbnohv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yuanzhike.top/gtxwauknda.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.xuetiantiany.cn/gtdacregpw.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.havefunace.top/gttpdanmpr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jinqigufen.top/gtgqwadluj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhiwuduotai.top/gtrevxrbjb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yueranfly.top/gtxizgyntm.html

================================================================================
来源：http://hz.zhongyouzk.top/gttvkkzscq.html

K. JSON 与序列化
来源：http://hz.zhiwuduotai.top/gtdmjknjts.html

================================================================================
来源：http://hz.jqgfzy.top/gtceooyrvu.html

[K01] 对象转 JSON 字符串
来源：http://hz.0kj1m.cn/gtbdtfmlvt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hnqzz.top/gttusqtuwl.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jqgufenzy.top/gtuqbbcsgc.html

JS:   JSON.stringify(obj)
来源：http://hz.jinqigufen.top/gthdnefmzn.html

TS:   JSON.stringify(obj)
来源：http://hz.cqqwz.cn/gtcoxsdgyr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xingfuxueyuan.xyz/gtnwjhfpnz.html

Go:   json.Marshal(obj)
来源：http://hz.jinyuanbaomall.cn/gthedvyhpm.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.xylfe.cn/gtpeagtogp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yonumen.top/gthyjhzntx.html

[K02] JSON 字符串转对象
来源：http://hz.chenlongwang.top/gtfgtokxoj.html

Py:   json.loads(s)
来源：http://hz.ywan-chungtsiang.top/gtpucehokk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.mhx1999.top/gtfwbpmnao.html

JS:   JSON.parse(s)
来源：http://hz.316326.xyz/gtkkeqjzzy.html

TS:   JSON.parse(s)
来源：http://hz.jinghuilouyu.cn/gttkzyxkfj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.svipenyu.cn/gtsretyafa.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.9152youxi.cn/gtddmivell.html

Ruby: JSON.parse(s)
来源：http://hz.zhixingplan.top/gtoetjvsnp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jyoumei.cn/gtofcmbvkb.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.vqdsnc.cn/gtuunbatcu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ybcxt.top/gtedvyazww.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhoulong.xyz/gtqibsrfcx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.smart0.xyz/gtzszingwr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xziqi.cn/gtlehjyiox.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.shuidangran.top/gtzcbtqdfn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.gzhubu.top/gtsehsdpxf.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.gotoacloud.top/gtzbpcaxco.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.shzxlz.cn/gtyfmreibj.html

[K04] 读取 JSON 文件
来源：http://hz.chenzaomai.com/gtmslxcvcd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.dashuyun.cn/gtxviwpanv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ppjwa.cn/gtelaosbcm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sxryk.cn/gtzpcxdwgg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinqigfzy.top/gttfykfurb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.xingfuxueyuan.xyz/gtbunlysnk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhoulong.xyz/gtpuqzhqri.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zycfv.cn/gtlhllczdi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ywan-chungtsiang.top/gtnjndyymj.html

[K05] 深拷贝对象
来源：http://hz.hnqzz.top/gtnkkdwfcx.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhongyouzk.top/gtnjmzuigw.html

PHP:  unserialize(serialize($obj));
来源：http://hz.vqdsnc.cn/gtrevcboje.html

JS:   structuredClone(obj)
来源：http://hz.havefunace.top/gtjwqkcgnl.html

TS:   structuredClone(obj)
来源：http://hz.birdmap.top/gtunigsumy.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xziqi.cn/gtzxqwtaza.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.vqdsnc.cn/gtfhgkuvzt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.gaohongyu789.top/gtinppbuos.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yuxming.cn/gtpizqqzbj.html

[K06] 解析 URL 查询串
来源：http://hz.0kj1m.cn/gtmajsvoak.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.daria6918.cn/gtgavxyyap.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.quarkkingdee.top/gtwlcclinr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj20258888.top/gtbohhwuhh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cheryme.top/gtcjflcqkn.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.fengsongda.top/gtwdxbpurz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jianghu66.top/gtvkftabwg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.smart0.xyz/gtwliidrsa.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yj20258888.top/gtactiyhfi.html

[K07] 进制转换
来源：http://hz.jqgufenzy.top/gteatoihyg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.dashuyun.cn/gtpoewbigu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.gotoacloud.top/gtpnmxswkf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jinyuanbaomall.cn/gtxaarwzaz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jyoumei.cn/gtbdcelqwb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhoulong.xyz/gtcgkbvifp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.pycfn.com/gtnpiggtov.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.kuanghao11.cn/gtfywlmyqr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.gzhubu.top/gtfgjhwuil.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.0kj1m.cn/gtyhmbtrzi.html

Py:   pickle.dumps(obj)
来源：http://hz.dashuyun.cn/gtrtneuxzi.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.vqdsnc.cn/gtvgxdwwqe.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.birdmap.top/gtucwmwhjg.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ybcxt.top/gttddergdl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhongyouzk.top/gthtnkxslo.html

Go:   encoding/gob
来源：http://hz.pengpengdd.cyou/gtsnnrrqwt.html

Ruby: Marshal.dump(obj)
来源：http://hz.hammf.cn/gthejxyjno.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.sxryk.cn/gtluwqtmrz.html

================================================================================
来源：http://hz.chenzaomai.com/gtvbofznbe.html

L. 网络请求
来源：http://hz.hammf.cn/gtokdiguwv.html

================================================================================
来源：http://hz.cqqwz.cn/gtieeiwgfn.html

[L01] 发送 GET 请求
来源：http://hz.jinyuanbaomall.cn/gtwngxdcok.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.andypj.xyz/gtpdeldnem.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.tianlin.xyz/gtthtncyzf.html

JS:   await fetch(url)
来源：http://hz.xuetiantiany.cn/gtcgatdhgf.html

TS:   await fetch(url)
来源：http://hz.shuidangran.top/gtciwjahvd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hnxiangtu.top/gtfwsfqlef.html

Go:   resp, err := http.Get(url)
来源：http://hz.cqqwz.cn/gtsalvgbbb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.daxiang520.top/gtnwrrjdxi.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.fzhhl.top/gtdetbeelu.html

[L02] 发送 POST JSON
来源：http://hz.aizwys.cn/gtilrllutk.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.cucudq.cn/gtzexdwidv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yvedp.cn/gtqsfwrqcm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shangyingyoupin.top/gtgabmqwrm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.birdmap.top/gtxtmdffao.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.guowangkeji.top/gtqzplaabd.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.316326.xyz/gtidjcusop.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhiwuduotai.top/gtffwsvhoa.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.iojbl.cn/gtogpbbxbp.html

[L03] 设置自定义请求头
来源：http://hz.jiagoushi.top/gtedigsopm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.mhx1999.top/gtzaqnrdsa.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zhiwuduotai.top/gttostdpdc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gaohongyu789.top/gtvzhsadnp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.chenzaomai.com/gtzihlhorz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.xylfe.cn/gteesdsoxx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.pengpengdd.cyou/gtygdboakt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jinqigufen.top/gtjsoybmwd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yangfankeji.com/gtkackhigi.html

[L04] 设置超时
来源：http://hz.mhx1999.top/gtcxxaauzb.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yj202588.top/gtggqejsnu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.wangshuangyany.cn/gteqopllfb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.52xcode.cn/gtpdghhqij.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shanyushiyangkeji.top/gtvjrkouww.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.redwolf501.top/gtzggakhnq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.shanyushiyangtech.top/gtpgtsidyz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hnqzz.top/gtdzoslgvd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xinyue.icu/gtqginctwr.html

[L05] 上传文件（multipart）
来源：http://hz.andypj.xyz/gtczvmsclm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.cashguo.top/gtcwxxxrql.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.c1oappe.top/gthtdougzi.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.gotoacloud.top/gtgkbebcnd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.sufxvd.cn/gtfccsjvsw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yvedp.cn/gtdnroobpv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.wangdashe.top/gtfmgsfqjd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yj202588.top/gtskwewfeo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yuxming.cn/gtnnltynit.html

[L06] 解析响应为 JSON
来源：http://hz.gogol.net.cn/gtgqderjjh.html

Py:   resp.json()
来源：http://hz.dashuyun.cn/gtqualepci.html

PHP:  json_decode($body, true);
来源：http://hz.yanxiufei.cn/gtyxydvpxt.html

JS:   await resp.json()
来源：http://hz.zycfv.cn/gteywxhhii.html

TS:   await resp.json()
来源：http://hz.redwolf501.top/gtzureawil.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.xinyue.icu/gtfpzqgmwn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hnxiangtu.top/gtpwpscprx.html

Ruby: JSON.parse(resp.body)
来源：http://hz.fengsongda.top/gtazbmauky.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.wangshuangyany.cn/gtzbkrzsie.html

[L07] 处理 HTTP 状态码
来源：http://hz.cqqwz.cn/gthqobwivt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.nanxuanxn.top/gtqzgpacql.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.dashuyun.cn/gtmkgaulkt.html

JS:   resp.ok;  resp.status
来源：http://hz.fzhhl.top/gtocsbaeqa.html

TS:   resp.ok;  resp.status
来源：http://hz.hnxiangtu.top/gtnytwndex.html

Java: resp.statusCode()
来源：http://hz.yongpay.top/gtpkatpvms.html

Go:   resp.StatusCode
来源：http://hz.tianlin.xyz/gtdjorgvtd.html

Ruby: resp.code.to_i
来源：http://hz.snrcjt.cn/gtdtgtlqll.html

C#:   (int)resp.StatusCode
来源：http://hz.redwolf501.top/gttrlyaewb.html

[L08] 并发请求多个地址
来源：http://hz.yongpay.top/gtxoszjfoj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jinqigufen.top/gtecwgddwn.html

PHP:  curl_multi_init() 系列
来源：http://hz.xinyue.icu/gtbrhiopvj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cucudq.cn/gtcoldxtpq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hysaishi.cn/gtwiqawfup.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ywan-chungtsiang.top/gtrazyuzlp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.sufxvd.cn/gtayvmpbrq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hywenlv.cn/gtlhpbdyql.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.gogol.net.cn/gtocopqqza.html

================================================================================
来源：http://hz.c1oappe.top/gtlksvpxet.html

M. 命令行 / 进程 / 环境
来源：http://hz.havefunace.top/gtrhbndsnq.html

================================================================================
来源：http://hz.zdqjudy.top/gtxwoxlkzs.html

[M01] 读取命令行参数
来源：http://hz.jlsjyb.cn/gtlmbyclmp.html

Py:   sys.argv[1:]
来源：http://hz.jinqigufen.top/gtzmntkoqc.html

PHP:  $argv;  $argc;
来源：http://hz.52xcode.cn/gtgozjefcx.html

JS:   process.argv.slice(2)
来源：http://hz.shuidangran.top/gttpheaeee.html

TS:   process.argv.slice(2)
来源：http://hz.cheryme.top/gtbokqrlvc.html

Java: args 数组（main 方法参数）
来源：http://hz.cqqwz.cn/gtcqpytpkx.html

Go:   os.Args[1:]
来源：http://hz.gotoacloud.top/gthxjnttaw.html

Ruby: ARGV
来源：http://hz.hammf.cn/gtmhnwbozh.html

C#:   args 数组（Main 方法参数）
来源：http://hz.pengpengdd.cyou/gtkeocjyec.html

[M02] 读取环境变量
来源：http://hz.daria6918.cn/gtsgwlotud.html

Py:   os.environ.get("HOME")
来源：http://hz.kuanghao11.cn/gtewkepeed.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.sysykeji.top/gtpzwbgxaf.html

JS:   process.env.HOME
来源：http://hz.kuanghao11.cn/gttlwxuqos.html

TS:   process.env.HOME
来源：http://hz.shanyushiyangkeji.top/gtaowsjvqt.html

Java: System.getenv("HOME")
来源：http://hz.shangyingyoupin.top/gtctomculx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jinqigufen.top/gtmkcisfxg.html

Ruby: ENV["HOME"]
来源：http://hz.ydzc1.top/gtsydgkjko.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hammf.cn/gtxhazetqd.html

[M03] 执行外部命令
来源：http://hz.316326.xyz/gtcviyhmvt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.redwolf501.top/gtcitqytif.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yj202588.top/gtspzpzagt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.aibaodan.cn/gtpujzjlhq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhiwuduotai.top/gtsnpdliqo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ywan-chungtsiang.top/gtlckywfog.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.gotoacloud.top/gtkuuzjnhw.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.chenzaomai.com/gtyqrlgubv.html

C#:   Process.Start("ls", "-l");
来源：http://hz.aizwys.cn/gttjgppvzl.html

[M04] 获取当前工作目录
来源：http://hz.ivvv.top/gtbcdhpyex.html

Py:   os.getcwd()
来源：http://hz.smart0.xyz/gtlzhejbsf.html

PHP:  getcwd();
来源：http://hz.xziqi.cn/gtsddzmole.html

JS:   process.cwd()
来源：http://hz.ppjwa.cn/gtfdycpgfz.html

TS:   process.cwd()
来源：http://hz.chenjidiqi.icu/gttocxiknw.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yueranfly.top/gtwwthzxlh.html

Go:   os.Getwd()
来源：http://hz.guannengcc.top/gttlsnadcg.html

Ruby: Dir.pwd
来源：http://hz.haohaochexian.top/gtqseebriv.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yuanzhike.top/gtsxjrkfur.html

[M05] 设置退出码
来源：http://hz.nanxinkj.top/gtizniodmw.html

Py:   sys.exit(1)
来源：http://hz.zhaomingkeji.xyz/gtscsflcut.html

PHP:  exit(1);
来源：http://hz.jianghu66.top/gtqwgdcfzg.html

JS:   process.exit(1)
来源：http://hz.316326.xyz/gtyvrpoxjw.html

TS:   process.exit(1)
来源：http://hz.jinyuanbaomall.cn/gtukotpkvy.html

Java: System.exit(1)
来源：http://hz.shanyushiyangtech.top/gtsbsxbzxc.html

Go:   os.Exit(1)
来源：http://hz.sufxvd.cn/gtiwufihwz.html

Ruby: exit 1
来源：http://hz.ehwqpu.com/gtbsnmzbaa.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yongpay.top/gtqmjhqhmp.html

[M06] 向标准错误输出
来源：http://hz.jinyuanbaomall.cn/gtgohydptr.html

Py:   print("err", file=sys.stderr)
来源：http://hz.gaohongyu789.top/gtlkiwjllh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.fzhhl.top/gtsxmyoxib.html

JS:   console.error("err")
来源：http://hz.chenjidiqi.icu/gtzcoizvsa.html

TS:   console.error("err")
来源：http://hz.jqgfzy.top/gtipyzsufr.html

Java: System.err.println("err")
来源：http://hz.dianchejie.cn/gturoaormo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xziqi.cn/gtdbbgklhl.html

Ruby: warn "err"
来源：http://hz.jinqigufen.top/gtjpeqozdm.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhijiandao.cn/gtyheoyyiv.html

[M07] 判断是否为主入口
来源：http://hz.gogol.net.cn/gtboqmzvmy.html

Py:   if __name__ == "__main__":
来源：http://hz.cdnleiting.top/gtvpmshpnm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.quarkkingdee.top/gtwmrfjvjn.html

JS:   require.main === module
来源：http://hz.zhiwuduotai.top/gtawxigxke.html

TS:   require.main === module
来源：http://hz.316326.xyz/gtscfmbbis.html


<!-- 参考信息 -->