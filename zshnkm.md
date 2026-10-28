代发 wailian999

[J03] 字符串解析为日期
来源：http://hz.snrcjt.cn/gtbufdkrdf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.kuanghao11.cn/gtosuxqtvt.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jqgufenzy.top/gttbzyxbkh.html

JS:   new Date("2024-01-02")
来源：http://hz.feifeiyinyue.top/gtbjajfnpu.html

TS:   new Date("2024-01-02")
来源：http://hz.wangdashe.top/gtqvhqtlsv.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xuanzx.com/gtvwlzxxjq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.chenjidiqi.icu/gticqxspri.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ybcxt.top/gtotbhekcs.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.fzhhl.top/gtlbozugav.html

[J04] 时间戳与日期互转
来源：http://hz.jiagoushi.top/gtdmljoavn.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yj202588.top/gtwsvduzon.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhaomingkeji.xyz/gtgcrmoyze.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jinghuilouyu.cn/gtisrbshey.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yvedp.cn/gtqfidrkfz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.nanxuanxn.top/gtayfjpmbr.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.shzxlz.cn/gtwlplkfyh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.shuidangran.top/gtnxdxpnnu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zycfv.cn/gttcwqzsoz.html

[J05] 时间加减（加 7 天）
来源：http://hz.wangdashe.top/gtlbjdbkqz.html

Py:   now + timedelta(days=7)
来源：http://hz.sufxvd.cn/gtodlwsbtz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yangfankeji.com/gtrfxwpeob.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tanke756.top/gtlpqofbdr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinyuanbaomall.cn/gtzsdokwvs.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yueranfly.top/gtjretzppm.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jinghuilouyu.cn/gthydpkmcu.html

Ruby: Time.now + 7 * 86400
来源：http://hz.cqqwz.cn/gtpuiibseb.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xziqi.cn/gtfmpfqkda.html

[J06] 计算两时间之差
来源：http://hz.fzhhl.top/gtadzmtyvf.html

Py:   (end - start).total_seconds()
来源：http://hz.yonumen.top/gtedgkuvgl.html

PHP:  $end->diff($start)->days;
来源：http://hz.ydjk.org.cn/gtgmazfqhu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ehwqpu.com/gtijnyegje.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.52xcode.cn/gtmhuvjflr.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yuanzhike.top/gtcxerixph.html

Go:   end.Sub(start).Hours()
来源：http://hz.svipenyu.cn/gtlvczclvk.html

Ruby: end - start                 # 返回秒数
来源：http://hz.nwbrower.top/gtdqglgidm.html

C#:   (end - start).TotalSeconds
来源：http://hz.sweek.top/gtmtwxagfy.html

[J07] 比较两个日期
来源：http://hz.zhiwuduotai.top/gtwisifxmk.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xuetiantiany.cn/gtmehiszhv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.wangshuangyany.cn/gtsueuzfei.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.tianlin.xyz/gtdjmzvdzp.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.quarkkingdee.top/gtyhpnvdjq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhaomingkeji.xyz/gtdaostysr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.wangshuangyany.cn/gtffelklfg.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jinyuanbaomall.cn/gtzlalgnoa.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jiagoushi.top/gtxhxdfsju.html

[J08] 提取年月日与星期
来源：http://hz.wangdashe.top/gtuavogybv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.havefunace.top/gtjbsmdyts.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jqgufenzy.top/gtqklmqqwv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hywenlv.cn/gthrplpojq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yuanzhike.top/gtbngwnnkj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.dianchejie.cn/gtidwvatlf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.gogol.net.cn/gtkxwbhgap.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.tian-w.cn/gtunnsgtdy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.cqqwz.cn/gthbqidmhc.html

[J09] 时区处理
来源：http://hz.daxiang520.top/gtopkxqzno.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.gzhubu.top/gtifykjtns.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hysaishi.cn/gthzpyznbg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tianlin.xyz/gtlfyxgpjc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yanxiufei.cn/gtwjpsaukn.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jqgfzy.top/gtmfnyjzwa.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.gaohongyu789.top/gtentaokwl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.kuanghao11.cn/gtxubroays.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ehwqpu.com/gtmgbtsfyz.html

[J10] 取今天 / 本月第一天
来源：http://hz.quarkkingdee.top/gtmxwbzyoi.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jqgufenzy.top/gtkwqtbzme.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jqgfzy.top/gtlaottjvq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jiagoushi.top/gtbnjxdyqk.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.tian-w.cn/gtryeqgkvg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.xuetiantiany.cn/gtjzeotsje.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.haohaochexian.top/gtgrfdngdm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.316326.xyz/gtfizakalx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.cheryme.top/gtzgwomkfm.html

================================================================================
来源：http://hz.fzhhl.top/gtbkqafyss.html

K. JSON 与序列化
来源：http://hz.hnxiangtu.top/gtusouqwug.html

================================================================================
来源：http://hz.ehwqpu.com/gtmxtdpsbv.html

[K01] 对象转 JSON 字符串
来源：http://hz.jinqigfzy.top/gtqgohpwnu.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shanyushiyangkeji.top/gtorbltfnh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.meibo888.top/gtrsajpefb.html

JS:   JSON.stringify(obj)
来源：http://hz.hysaishi.cn/gtckglmetv.html

TS:   JSON.stringify(obj)
来源：http://hz.daxiang520.top/gtcnjsgkql.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.wangshuangyany.cn/gtoxisocnx.html

Go:   json.Marshal(obj)
来源：http://hz.ppjwa.cn/gtflgrekib.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.ppjwa.cn/gtivncgqwh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhengqikj.top/gtmulkxuow.html

[K02] JSON 字符串转对象
来源：http://hz.fengsongda.top/gtdmrzlbto.html

Py:   json.loads(s)
来源：http://hz.yj20258888.top/gtqetxsivp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cqqwz.cn/gtzbaxqvkx.html

JS:   JSON.parse(s)
来源：http://hz.sweek.top/gtdxqvwgwe.html

TS:   JSON.parse(s)
来源：http://hz.shzxlz.cn/gtghbtszrh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.snrcjt.cn/gtsxknrblo.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yanxiufei.cn/gtghgusefo.html

Ruby: JSON.parse(s)
来源：http://hz.hysaishi.cn/gtzhmfgaac.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.316326.xyz/gtthnidaak.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhongyouzk.top/gtucfjsbih.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhaomingkeji.xyz/gtbvrjkusx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jinyuanbaomall.cn/gtaakupvjs.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.fzhhl.top/gtewgoaybo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cucudq.cn/gtpsudwojh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hfpthk.cn/gtkuqyukcc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.shangyingyoupin.top/gtmavxfwsg.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.svipenyu.cn/gtreqqfkqt.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ywan-chungtsiang.top/gtswaamubc.html

[K04] 读取 JSON 文件
来源：http://hz.mhx1999.top/gthlmmtkru.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.quarkkingdee.top/gtogvopvzj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yj202588.top/gtgtwvpfui.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinyuanbaomall.cn/gtqioomngh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhengqikj.top/gtxlsgakuk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yonumen.top/gtoilhdpbu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yueranfly.top/gtayipogfv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jqgufenzy.top/gtgmrfuwfc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.0kj1m.cn/gthlgzbnvk.html

[K05] 深拷贝对象
来源：http://hz.cucudq.cn/gtiykhfpej.html

Py:   copy.deepcopy(obj)
来源：http://hz.nanxinkj.top/gtjyeftsax.html

PHP:  unserialize(serialize($obj));
来源：http://hz.xziqi.cn/gtnxrdwzot.html

JS:   structuredClone(obj)
来源：http://hz.zycfv.cn/gtwsgjwibt.html

TS:   structuredClone(obj)
来源：http://hz.jyoumei.cn/gtscuhsgjn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jlsjyb.cn/gtivjqaszl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.cqqwz.cn/gtldycjieg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.chenlongwang.top/gtugekjnpe.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.gaohongyu789.top/gtkudisixu.html

[K06] 解析 URL 查询串
来源：http://hz.jqgfzy.top/gtptuvdlqu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhongyouzk.top/gtlqtujpol.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhaomingkeji.xyz/gtgavxhatr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shanyushiyangtech.top/gtcpldakuf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cucudq.cn/gtoiqljhby.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yvedp.cn/gtajnunlmp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhixingplan.top/gtshcskzpv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yj20258.top/gthwilklfa.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.sufxvd.cn/gtzazpwvco.html

[K07] 进制转换
来源：http://hz.ydzc1.top/gteydapsbt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.aizwys.cn/gtutbbshrj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.chenlongwang.top/gtphgbkloy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.guannengcc.top/gtldfobdru.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yueranfly.top/gtjggywxsk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xylfe.cn/gtcmltsedm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.haohaochexian.top/gtgzrdchnt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.bjfxy.top/gtbxhumnhd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yonumen.top/gtcxveyzgi.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.dianchejie.cn/gtcfigvted.html

Py:   pickle.dumps(obj)
来源：http://hz.gaohongyu789.top/gtbbswqldw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hysaishi.cn/gtehbobzsw.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.0kj1m.cn/gtprbxtazj.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.shanyushiyangkeji.top/gtsdresbkr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hammf.cn/gtjspcanng.html

Go:   encoding/gob
来源：http://hz.nanxuanxn.top/gtsitgtace.html

Ruby: Marshal.dump(obj)
来源：http://hz.jqgufenzy.top/gtkagrsiht.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ehwqpu.com/gtcewsgyat.html

================================================================================
来源：http://hz.sufxvd.cn/gtxdnjeark.html

L. 网络请求
来源：http://hz.zdqjudy.top/gtxrezvtuw.html

================================================================================
来源：http://hz.jyoumei.cn/gtrrjgzlon.html

[L01] 发送 GET 请求
来源：http://hz.gogol.net.cn/gtamttzjps.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.svipenyu.cn/gtjudotnrt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.meibo888.top/gtqjomhcto.html

JS:   await fetch(url)
来源：http://hz.nanxuanxn.top/gtqwwypcmx.html

TS:   await fetch(url)
来源：http://hz.xuanzx.com/gtdveltbsz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.sweek.top/gtobxjzaoc.html

Go:   resp, err := http.Get(url)
来源：http://hz.hnxiangtu.top/gtjpwxhzft.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yvedp.cn/gtlxxttdsy.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.dianchejie.cn/gtcmpgizyz.html

[L02] 发送 POST JSON
来源：http://hz.ehwqpu.com/gtlhzvphod.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jinqigfzy.top/gtaczkzyfj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.cashguo.top/gtrsfxrtxd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xinyue.icu/gtwemplffm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhoulong.xyz/gtqczmvqkm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.c1oappe.top/gtqeezgkdj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yonumen.top/gtrwypmgcn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.daxiang520.top/gtxdfklrgd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zdqjudy.top/gtxmmjdpju.html

[L03] 设置自定义请求头
来源：http://hz.cucudq.cn/gtmhsdycqo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhaomingkeji.xyz/gtzydwurdr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.tanke756.top/gtafzocbrv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhongyouzk.top/gtfkvgclsd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.aibaodan.cn/gthhsavjpb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.shzxlz.cn/gtejhshfmn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.andypj.xyz/gtibmregte.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yonumen.top/gtdtwvpeit.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yonumen.top/gtvxxtljno.html

[L04] 设置超时
来源：http://hz.ehwqpu.com/gthdvgnkez.html

Py:   requests.get(url, timeout=5)
来源：http://hz.meibo888.top/gtpiihjgfs.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.daxiang520.top/gtzmxduiwr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.haohaochexian.top/gtdkkufrxo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj202588.top/gtfiwhycml.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.meibo888.top/gtjdulvfox.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.guowangkeji.top/gtcpinuxdk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hfpthk.cn/gtkjhrmiic.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.mhx1999.top/gtthspfdbj.html

[L05] 上传文件（multipart）
来源：http://hz.havefunace.top/gtujjyjxgv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jlsjyb.cn/gtxgcwvkjm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.hammf.cn/gtifbopxhl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yangfankeji.com/gtbkrdwdnz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yanxiufei.cn/gtcjinjtdy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.fzhhl.top/gtbzirvylj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ydjk.org.cn/gtzgaybrjd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.sufxvd.cn/gtzcxnhlyn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.tian-w.cn/gtdnfnlzfq.html

[L06] 解析响应为 JSON
来源：http://hz.guannengcc.top/gtidkrnmmt.html

Py:   resp.json()
来源：http://hz.iojbl.cn/gtakyfzcir.html

PHP:  json_decode($body, true);
来源：http://hz.yuxming.cn/gtygcrvcji.html

JS:   await resp.json()
来源：http://hz.redwolf501.top/gtwtqgupyf.html

TS:   await resp.json()
来源：http://hz.yvedp.cn/gtywsmprol.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.haohaochexian.top/gtlxumorco.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.chenlongwang.top/gtcijfedef.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ppjwa.cn/gtjddqmxom.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.52xcode.cn/gtlvxjnqqe.html

[L07] 处理 HTTP 状态码
来源：http://hz.tianlin.xyz/gtiianfsjc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hammf.cn/gtbywlyffj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhongyouzk.top/gtmjwvcvoz.html

JS:   resp.ok;  resp.status
来源：http://hz.zhijiandao.cn/gtshdnonhc.html

TS:   resp.ok;  resp.status
来源：http://hz.hnxiangtu.top/gtcdauxcno.html

Java: resp.statusCode()
来源：http://hz.zhijiandao.cn/gtdytlfhya.html

Go:   resp.StatusCode
来源：http://hz.wangdashe.top/gtjyhygsav.html

Ruby: resp.code.to_i
来源：http://hz.havefunace.top/gtqiozhjjf.html

C#:   (int)resp.StatusCode
来源：http://hz.fzhhl.top/gtomqlvjsn.html

[L08] 并发请求多个地址
来源：http://hz.jinyuanbaomall.cn/gttmnnqmel.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.cqqwz.cn/gtiguotmhx.html

PHP:  curl_multi_init() 系列
来源：http://hz.smart0.xyz/gtqwmgkesr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gotoacloud.top/gtryjuzczs.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenzaomai.com/gthwwernce.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jinghuilouyu.cn/gtritpnwwi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.sufxvd.cn/gtylrdrbru.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhengqikj.top/gtvqnrpjtm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.guannengcc.top/gtejajidin.html

================================================================================
来源：http://hz.quarkkingdee.top/gtmlfffzuq.html

M. 命令行 / 进程 / 环境
来源：http://hz.0kj1m.cn/gtsikksaws.html

================================================================================
来源：http://hz.9152youxi.cn/gtfmytlgrj.html

[M01] 读取命令行参数
来源：http://hz.andypj.xyz/gthxwytydl.html

Py:   sys.argv[1:]
来源：http://hz.yanxiufei.cn/gtkwgewcfe.html

PHP:  $argv;  $argc;
来源：http://hz.fengsongda.top/gtzedclget.html

JS:   process.argv.slice(2)
来源：http://hz.hongshengwenyu.top/gtssrzgfzp.html

TS:   process.argv.slice(2)
来源：http://hz.jyoumei.cn/gtklzieoho.html

Java: args 数组（main 方法参数）
来源：http://hz.hfpthk.cn/gtgfbywdlf.html

Go:   os.Args[1:]
来源：http://hz.andypj.xyz/gtuepklyur.html

Ruby: ARGV
来源：http://hz.ivvv.top/gtbbhjrmny.html

C#:   args 数组（Main 方法参数）
来源：http://hz.shanyushiyangkeji.top/gtxibgfmfa.html

[M02] 读取环境变量
来源：http://hz.c1oappe.top/gtcimqnvfu.html

Py:   os.environ.get("HOME")
来源：http://hz.shzxlz.cn/gtawhmsaui.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ybcxt.top/gtarsikwnx.html

JS:   process.env.HOME
来源：http://hz.sysykeji.top/gtzaaxjzjq.html

TS:   process.env.HOME
来源：http://hz.ywan-chungtsiang.top/gtfmjewvxe.html

Java: System.getenv("HOME")
来源：http://hz.c1oappe.top/gtyairpkxb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.ppjwa.cn/gtqfaqeloy.html

Ruby: ENV["HOME"]
来源：http://hz.sufxvd.cn/gtbiagvmuf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xylfe.cn/gtpdvcrwuw.html

[M03] 执行外部命令
来源：http://hz.jqgfzy.top/gtohflcpvg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yongpay.top/gtvafgrenc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.mhx1999.top/gtharionul.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhoulong.xyz/gtiahtrgal.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.gaohongyu789.top/gtvzsmmdcr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.sysykeji.top/gtkbqrnqxi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jqgufenzy.top/gttgemrvyg.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.vqdsnc.cn/gttdqmjwve.html

C#:   Process.Start("ls", "-l");
来源：http://hz.nanxuanxn.top/gtgjjlhmep.html

[M04] 获取当前工作目录
来源：http://hz.shangyingyoupin.top/gtbhdjlunm.html

Py:   os.getcwd()
来源：http://hz.dashuyun.cn/gtvlnnpdbe.html

PHP:  getcwd();
来源：http://hz.wangshuangyany.cn/gtucogmups.html

JS:   process.cwd()
来源：http://hz.yvedp.cn/gtqrazaomv.html

TS:   process.cwd()
来源：http://hz.yuanzhike.top/gtlmppaxxv.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.sufxvd.cn/gtxoznygvr.html

Go:   os.Getwd()
来源：http://hz.dashuyun.cn/gtiotctcxg.html

Ruby: Dir.pwd
来源：http://hz.hammf.cn/gtcaqniwrd.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.havefunace.top/gtgbfzmbuf.html

[M05] 设置退出码
来源：http://hz.zhaomingkeji.xyz/gtmimvekac.html

Py:   sys.exit(1)
来源：http://hz.0kj1m.cn/gtetdzpdij.html

PHP:  exit(1);
来源：http://hz.hongshengwenyu.top/gtombnyuof.html

JS:   process.exit(1)
来源：http://hz.yj20258.top/gtayoivihy.html

TS:   process.exit(1)
来源：http://hz.hammf.cn/gtysekufmr.html

Java: System.exit(1)
来源：http://hz.hongshengwenyu.top/gtpneswzxe.html

Go:   os.Exit(1)
来源：http://hz.ywan-chungtsiang.top/gtlqfqjxjo.html

Ruby: exit 1
来源：http://hz.redwolf501.top/gthnzzdild.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.xylfe.cn/gtclynsjyr.html

[M06] 向标准错误输出
来源：http://hz.gaohongyu789.top/gttmvmouvm.html

Py:   print("err", file=sys.stderr)
来源：http://hz.kuanghao11.cn/gtbmdkqjtj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.shanyushiyangtech.top/gtbcdxgdrd.html

JS:   console.error("err")
来源：http://hz.316326.xyz/gtpjyltosw.html

TS:   console.error("err")
来源：http://hz.mhx1999.top/gtdwvtbnqq.html

Java: System.err.println("err")
来源：http://hz.xuanzx.com/gtwzwevuhs.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.kuanghao11.cn/gtxmakxfqg.html

Ruby: warn "err"
来源：http://hz.sweek.top/gtgltxdvxa.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.smart0.xyz/gtuzfzussa.html

[M07] 判断是否为主入口
来源：http://hz.yueranfly.top/gtderzpqlj.html

Py:   if __name__ == "__main__":
来源：http://hz.52xcode.cn/gtjysdhvsh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.kuanghao11.cn/gtgddsxhnd.html

JS:   require.main === module
来源：http://hz.guannengcc.top/gtmevcjkzg.html

TS:   require.main === module
来源：http://hz.ywan-chungtsiang.top/gtocwcwbce.html

Java: public static void main(String[] args)
来源：http://hz.yj20258.top/gtqollrfly.html

Go:   func main()
来源：http://hz.ywan-chungtsiang.top/gtftofzxmq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.vqdsnc.cn/gtirrdcbya.html

C#:   static void Main(string[] args)
来源：http://hz.sufxvd.cn/gtzgzektyu.html

[M08] 获取系统与运行时信息
来源：http://hz.tian-w.cn/gttwzivoyz.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhijiandao.cn/gtxogkbtqh.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhoulong.xyz/gtpjzceygx.html

JS:   process.platform;  process.version
来源：http://hz.hongshengwenyu.top/gtlethypwm.html

TS:   process.platform;  process.version
来源：http://hz.xuanzx.com/gtctxhvyis.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yvedp.cn/gtbqvcfpsx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.gotoacloud.top/gtqailjplj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.mhx1999.top/gtnxpofyfp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.dianchejie.cn/gtgfabaqct.html

================================================================================
来源：http://hz.yvedp.cn/gtsotsyxob.html

N. 数据结构与算法
来源：http://hz.316326.xyz/gtvaqvbavh.html

================================================================================
来源：http://hz.tanke756.top/gtgidbkrda.html


<!-- 参考信息 -->