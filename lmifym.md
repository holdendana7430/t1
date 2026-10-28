代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hongshengwenyu.top/gtjmzuuhcq.html

[J04] 时间戳与日期互转
来源：http://hz.cashguo.top/gthgmtfgfn.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.tianlin.xyz/gtrfxomlmt.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhiwuduotai.top/gtmsukcgbz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.smart0.xyz/gtwceftcdu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.316326.xyz/gtesaovpvm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.smart0.xyz/gtxfjxpoqg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.sufxvd.cn/gtpnvwqyoz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ywan-chungtsiang.top/gtbsxhapmw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhengqikj.top/gthdgvbvvg.html

[J05] 时间加减（加 7 天）
来源：http://hz.shuidangran.top/gtdvkhdrza.html

Py:   now + timedelta(days=7)
来源：http://hz.gaohongyu789.top/gtzactmmca.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jyoumei.cn/gtvvaipfxj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.iojbl.cn/gtxrtjojil.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ydzc1.top/gtjfsjhozn.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.svipenyu.cn/gtrmifejje.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.andypj.xyz/gtpzjxzzen.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jinqigfzy.top/gtnumtychk.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xziqi.cn/gtfvhwwogg.html

[J06] 计算两时间之差
来源：http://hz.316326.xyz/gtxkapzdeh.html

Py:   (end - start).total_seconds()
来源：http://hz.jianghu66.top/gtyulcrodu.html

PHP:  $end->diff($start)->days;
来源：http://hz.nanxuanxn.top/gtskywsxum.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.shangyingyoupin.top/gtcxffmnos.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yanxiufei.cn/gtvlkvsxzk.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.9152youxi.cn/gtvgeovxdz.html

Go:   end.Sub(start).Hours()
来源：http://hz.52xcode.cn/gtzzgszlcs.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zhongyouzk.top/gthlbnqiei.html

C#:   (end - start).TotalSeconds
来源：http://hz.cucudq.cn/gtoptwcyhl.html

[J07] 比较两个日期
来源：http://hz.ehwqpu.com/gthsfkapcc.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.shangyingyoupin.top/gtwxpjkuat.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.havefunace.top/gttjfijtbu.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.cheryme.top/gtbsijnanu.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.chenjidiqi.icu/gtnbienpss.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.dashuyun.cn/gthgakvems.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.feifeiyinyue.top/gtwavojgju.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.pengpengdd.cyou/gtvdmgwkfc.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.shuidangran.top/gtpoxbgmgw.html

[J08] 提取年月日与星期
来源：http://hz.jlsjyb.cn/gtfevrevte.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ehwqpu.com/gtlvttdhft.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hongshengwenyu.top/gtxznhiyet.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.smart0.xyz/gtilgzwfym.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.wangdashe.top/gtnbiochdf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hfpthk.cn/gtehcmszcp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jiagoushi.top/gtwtdhjwri.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ybcxt.top/gtaiogtlhg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.quarkkingdee.top/gthacvotme.html

[J09] 时区处理
来源：http://hz.hnxiangtu.top/gtumovdzub.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shanyushiyangkeji.top/gtiunyhvlz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.tanke756.top/gtigpxcgoe.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ydjk.org.cn/gteyouhelw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gogol.net.cn/gtmmkxvese.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yvedp.cn/gtbqimhwew.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yueranfly.top/gtrtwamncu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.c1oappe.top/gtokreioph.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhongyouzk.top/gtdaesricd.html

[J10] 取今天 / 本月第一天
来源：http://hz.daxiang520.top/gtonxozlwg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.kuanghao11.cn/gtauzywvfq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.tian-w.cn/gtlzxxxnst.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.aibaodan.cn/gtehbhhpgs.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.svipenyu.cn/gtlblvpsud.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yongpay.top/gtqqadqzsn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jinqigufen.top/gtclembthu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.cdnleiting.top/gtpbzuvjep.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.hysaishi.cn/gthcarugyz.html

================================================================================
来源：http://hz.mhx1999.top/gtxtulmeuv.html

K. JSON 与序列化
来源：http://hz.sufxvd.cn/gtboycgmzv.html

================================================================================
来源：http://hz.cheryme.top/gtuqtpdkib.html

[K01] 对象转 JSON 字符串
来源：http://hz.svipenyu.cn/gtzlhrjhji.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.haohaochexian.top/gtvbemapub.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.meibo888.top/gthftkiztl.html

JS:   JSON.stringify(obj)
来源：http://hz.xziqi.cn/gtuxzxhtmt.html

TS:   JSON.stringify(obj)
来源：http://hz.gzhubu.top/gtrgpeqbab.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.daria6918.cn/gtbodlseko.html

Go:   json.Marshal(obj)
来源：http://hz.ivvv.top/gtzldgcvcb.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.gotoacloud.top/gtmfxzjgje.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.316326.xyz/gtfmqtrpnl.html

[K02] JSON 字符串转对象
来源：http://hz.tianlin.xyz/gtkpualzqr.html

Py:   json.loads(s)
来源：http://hz.chenlongwang.top/gtrcpquxuv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.iojbl.cn/gthglqxnlo.html

JS:   JSON.parse(s)
来源：http://hz.chenjidiqi.icu/gtnshwpswq.html

TS:   JSON.parse(s)
来源：http://hz.ydzc1.top/gttmtalxbw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hnxiangtu.top/gtuwaucoge.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.sysykeji.top/gtoltqoldz.html

Ruby: JSON.parse(s)
来源：http://hz.guowangkeji.top/gtpltogzgl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.mhx1999.top/gtfnqgugkg.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.guowangkeji.top/gtpebwevnb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.meibo888.top/gtaztiglrl.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.cheryme.top/gtluyowcib.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinyuanbaomall.cn/gtqqmkyawh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.ehwqpu.com/gtbxkuxqys.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hfpthk.cn/gteavxzwql.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yj20258.top/gtaoanmnkp.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.daria6918.cn/gtyqosxssz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cashguo.top/gtrnmtlmtt.html

[K04] 读取 JSON 文件
来源：http://hz.bjfxy.top/gtjwdliliv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.316326.xyz/gtlkxnyrmw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.guowangkeji.top/gtbpycbmqo.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jiagoushi.top/gtodgkjmtp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.chenjidiqi.icu/gtamuxcqoz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yuanzhike.top/gtpvwkahjs.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.aibaodan.cn/gtfyvvykwn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.shanyushiyangkeji.top/gtntusnrkx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.havefunace.top/gtsrebduul.html

[K05] 深拷贝对象
来源：http://hz.iojbl.cn/gtbwahsfjd.html

Py:   copy.deepcopy(obj)
来源：http://hz.vqdsnc.cn/gtgduredpf.html

PHP:  unserialize(serialize($obj));
来源：http://hz.xuetiantiany.cn/gtcfisiwzq.html

JS:   structuredClone(obj)
来源：http://hz.chenzaomai.com/gtytmrqjcd.html

TS:   structuredClone(obj)
来源：http://hz.kuanghao11.cn/gtiqmyhjen.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.nanxuanxn.top/gtwsuroois.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.nanxuanxn.top/gtgrlrxdez.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.aizwys.cn/gtonbjujsy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.fzhhl.top/gtxytfrqgf.html

[K06] 解析 URL 查询串
来源：http://hz.jinqigfzy.top/gttxtadejl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jiagoushi.top/gtqdnggpsa.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.quarkkingdee.top/gtiidrfhim.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gogol.net.cn/gtbszvwlac.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cqqwz.cn/gtspsbwmvo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.kuanghao11.cn/gtbtudsykv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.chenlongwang.top/gttyuhzoaf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hnqzz.top/gtgemygjad.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yuxming.cn/gtfttqvutx.html

[K07] 进制转换
来源：http://hz.xziqi.cn/gtihkqigsx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.fzhhl.top/gtiegatfra.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.feifeiyinyue.top/gtgrkuzcti.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.fzhhl.top/gtfwkswdmv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.gotoacloud.top/gtexgbjbxr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.dianchejie.cn/gtzjiegjho.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.sysykeji.top/gtgkhpsbpo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jyoumei.cn/gtvneelnts.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.nanxinkj.top/gtuivasqch.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yvedp.cn/gtzffmgjzq.html

Py:   pickle.dumps(obj)
来源：http://hz.kuanghao11.cn/gttvixgxzf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.birdmap.top/gtxdoguugc.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.havefunace.top/gtniycvusw.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jqgufenzy.top/gtjitacttw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.birdmap.top/gtksymazxe.html

Go:   encoding/gob
来源：http://hz.yonumen.top/gtibmozmgc.html

Ruby: Marshal.dump(obj)
来源：http://hz.hnqzz.top/gtuqpukzcb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.mhx1999.top/gtcmiijibb.html

================================================================================
来源：http://hz.cdnleiting.top/gtdkzamqoi.html

L. 网络请求
来源：http://hz.nanxinkj.top/gtnhdoqigg.html

================================================================================
来源：http://hz.jiagoushi.top/gtvkhltdqe.html

[L01] 发送 GET 请求
来源：http://hz.havefunace.top/gtyhyhezpt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.xylfe.cn/gtnijztkla.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.shanyushiyangkeji.top/gtetdqvdsn.html

JS:   await fetch(url)
来源：http://hz.jlsjyb.cn/gtfblldhgf.html

TS:   await fetch(url)
来源：http://hz.0kj1m.cn/gtpjagkrgq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.xuanzx.com/gtkeosnrky.html

Go:   resp, err := http.Get(url)
来源：http://hz.aibaodan.cn/gtvwdszixg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.haohaochexian.top/gtywzkfbnt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hysaishi.cn/gtuuamwbtw.html

[L02] 发送 POST JSON
来源：http://hz.cdnleiting.top/gttfepysax.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yj202588.top/gtuluwaemz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yongpay.top/gthoicjiql.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yongpay.top/gtwbmalyol.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.chenjidiqi.icu/gttvhpbubx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ivvv.top/gtwebmoxhv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ywan-chungtsiang.top/gtpyuxjhhp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.sweek.top/gtohqoaghu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.cashguo.top/gtgvedvqfo.html

[L03] 设置自定义请求头
来源：http://hz.ppjwa.cn/gtbsofhtcm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yj202588.top/gtgymnhlfz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.316326.xyz/gtsnmbtpcw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.dianchejie.cn/gtmovhlxhz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinqigufen.top/gtejxoyvfs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hywenlv.cn/gtgtrzqlvi.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.pengpengdd.cyou/gtvwhkrodn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.guowangkeji.top/gthkrwajoj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.gaohongyu789.top/gtyhosldcg.html

[L04] 设置超时
来源：http://hz.jinqigfzy.top/gtocievclu.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jyoumei.cn/gtqvsgewcp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.dashuyun.cn/gtxvgzamiv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xingfuxueyuan.xyz/gtvgxqxivj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhixingplan.top/gtcvrinprc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xinyue.icu/gtskzvvkfl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.sufxvd.cn/gtlluyhluf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zhaomingkeji.xyz/gttgreirml.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.wangdashe.top/gtverpjibz.html

[L05] 上传文件（multipart）
来源：http://hz.yangfankeji.com/gtetrwzeyg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.shuidangran.top/gthlwordrb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.cqqwz.cn/gtiwhezbpy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hnqzz.top/gtjjcpejtj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.9152youxi.cn/gtqiyfhgtk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.sysykeji.top/gtkjuvojvz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ppjwa.cn/gtckvlgtzu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.chenzaomai.com/gtxumvjuwr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.chenlongwang.top/gtibxgjuxs.html

[L06] 解析响应为 JSON
来源：http://hz.yvedp.cn/gtmfwwshjr.html

Py:   resp.json()
来源：http://hz.shangyingyoupin.top/gtrvpseqzx.html

PHP:  json_decode($body, true);
来源：http://hz.xuanzx.com/gtzqvklaoc.html

JS:   await resp.json()
来源：http://hz.svipenyu.cn/gtbvhfcjzj.html

TS:   await resp.json()
来源：http://hz.ivvv.top/gtuksnqflm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hammf.cn/gtsuokmjuz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yonumen.top/gtlsutdwuj.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jinghuilouyu.cn/gtrocrjijm.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.snrcjt.cn/gtcbdbfybt.html

[L07] 处理 HTTP 状态码
来源：http://hz.yongpay.top/gtjevqjcqp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xuanzx.com/gtilbqlrjs.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.iojbl.cn/gtfhysxubr.html

JS:   resp.ok;  resp.status
来源：http://hz.ydzc1.top/gtopjqogha.html

TS:   resp.ok;  resp.status
来源：http://hz.9152youxi.cn/gtnbmeemmk.html

Java: resp.statusCode()
来源：http://hz.yvedp.cn/gtnwpchhsj.html

Go:   resp.StatusCode
来源：http://hz.chenlongwang.top/gtnybdjpkn.html

Ruby: resp.code.to_i
来源：http://hz.chenzaomai.com/gtvxrxcjtg.html

C#:   (int)resp.StatusCode
来源：http://hz.0kj1m.cn/gtrsyxioqi.html

[L08] 并发请求多个地址
来源：http://hz.zycfv.cn/gtkrbyudpu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ydjk.org.cn/gttcjbojvj.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhaomingkeji.xyz/gtaicnuzov.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhijiandao.cn/gtotkhxubd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yvedp.cn/gtpcaaampf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.sxryk.cn/gtkgfmpnww.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhijiandao.cn/gtfolojyzq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.tanke756.top/gtlkxhudgl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.fengsongda.top/gtvyxfbrkb.html

================================================================================
来源：http://hz.xuanzx.com/gtxjldjxiy.html

M. 命令行 / 进程 / 环境
来源：http://hz.cashguo.top/gtyqyyidoq.html

================================================================================
来源：http://hz.xuanzx.com/gtvtxzakxi.html

[M01] 读取命令行参数
来源：http://hz.fzhhl.top/gtgehskskw.html

Py:   sys.argv[1:]
来源：http://hz.aizwys.cn/gtcvzvbeus.html

PHP:  $argv;  $argc;
来源：http://hz.aizwys.cn/gtoofirrii.html

JS:   process.argv.slice(2)
来源：http://hz.xylfe.cn/gtgnymcgdi.html

TS:   process.argv.slice(2)
来源：http://hz.zhengqikj.top/gtavbfmgga.html

Java: args 数组（main 方法参数）
来源：http://hz.gogol.net.cn/gtxonsdkcu.html

Go:   os.Args[1:]
来源：http://hz.gzhubu.top/gtvmipqfmz.html

Ruby: ARGV
来源：http://hz.gaohongyu789.top/gtldcteyms.html

C#:   args 数组（Main 方法参数）
来源：http://hz.iojbl.cn/gtoniyrcip.html

[M02] 读取环境变量
来源：http://hz.chenjidiqi.icu/gtzunftupl.html

Py:   os.environ.get("HOME")
来源：http://hz.nanxuanxn.top/gthzecadvf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zhixingplan.top/gtvuzuhrby.html

JS:   process.env.HOME
来源：http://hz.shuidangran.top/gtwvqxkkef.html

TS:   process.env.HOME
来源：http://hz.zhijiandao.cn/gtkuonkbdv.html

Java: System.getenv("HOME")
来源：http://hz.mhx1999.top/gtkdyeymez.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yj20258.top/gtxyhywpgc.html

Ruby: ENV["HOME"]
来源：http://hz.wangdashe.top/gtzqpotdko.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.gotoacloud.top/gtvcngrjtw.html

[M03] 执行外部命令
来源：http://hz.wangdashe.top/gtaktmjvin.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.shanyushiyangkeji.top/gthvxjnqfx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.xuanzx.com/gtzmvuqbuv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.redwolf501.top/gtwsqiixro.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.nwbrower.top/gtznrkgkdz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.quarkkingdee.top/gtwkdzmuse.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.aibaodan.cn/gtckakjwax.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shuidangran.top/gtxdnszsdy.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zycfv.cn/gtzfjnpymu.html

[M04] 获取当前工作目录
来源：http://hz.zhongyouzk.top/gtfekwdlum.html

Py:   os.getcwd()
来源：http://hz.cdnleiting.top/gtxdmhxxzx.html

PHP:  getcwd();
来源：http://hz.yanxiufei.cn/gtwvgbdfqa.html

JS:   process.cwd()
来源：http://hz.aizwys.cn/gtibzgyuru.html

TS:   process.cwd()
来源：http://hz.jqgfzy.top/gtodwcxltm.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.gaohongyu789.top/gtiwvhupyz.html

Go:   os.Getwd()
来源：http://hz.cucudq.cn/gtroserqxd.html

Ruby: Dir.pwd
来源：http://hz.yj20258888.top/gtlmfngtsi.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.havefunace.top/gtfcrzwany.html

[M05] 设置退出码
来源：http://hz.tianlin.xyz/gtmdkvlbch.html

Py:   sys.exit(1)
来源：http://hz.nanxinkj.top/gttgjydyoo.html

PHP:  exit(1);
来源：http://hz.jqgufenzy.top/gtqauttmxw.html

JS:   process.exit(1)
来源：http://hz.316326.xyz/gteyokbkdg.html

TS:   process.exit(1)
来源：http://hz.iojbl.cn/gtnpjdwyci.html

Java: System.exit(1)
来源：http://hz.yangfankeji.com/gtfbnsigrk.html

Go:   os.Exit(1)
来源：http://hz.zycfv.cn/gttrkdvsqc.html

Ruby: exit 1
来源：http://hz.jinqigfzy.top/gtjlqeyykk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.pengpengdd.cyou/gtmzicgyji.html

[M06] 向标准错误输出
来源：http://hz.wangdashe.top/gtbcscopcm.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jinyuanbaomall.cn/gtekshfvps.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.aizwys.cn/gtdnluoepp.html

JS:   console.error("err")
来源：http://hz.smart0.xyz/gtwhmdxlup.html

TS:   console.error("err")
来源：http://hz.snrcjt.cn/gteexyrbhs.html

Java: System.err.println("err")
来源：http://hz.c1oappe.top/gttpnfsrxk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yongpay.top/gtpznvdkoq.html

Ruby: warn "err"
来源：http://hz.cqqwz.cn/gtiflzlcip.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jqgufenzy.top/gtvoftgiah.html

[M07] 判断是否为主入口
来源：http://hz.sweek.top/gtpjitedzg.html

Py:   if __name__ == "__main__":
来源：http://hz.jinqigufen.top/gtwzvozswe.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xylfe.cn/gtfzcsetnx.html

JS:   require.main === module
来源：http://hz.cdnleiting.top/gtndqzotni.html

TS:   require.main === module
来源：http://hz.fengsongda.top/gtyvecessr.html

Java: public static void main(String[] args)
来源：http://hz.shanyushiyangkeji.top/gtvhmsmolf.html

Go:   func main()
来源：http://hz.316326.xyz/gtxsbmlppr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.pengpengdd.cyou/gthyglyavz.html

C#:   static void Main(string[] args)
来源：http://hz.vqdsnc.cn/gtuezrcvdi.html

[M08] 获取系统与运行时信息
来源：http://hz.feifeiyinyue.top/gtskmlumcb.html

Py:   platform.system();  platform.python_version()
来源：http://hz.aizwys.cn/gtevboyepl.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.havefunace.top/gtbwipjyfg.html

JS:   process.platform;  process.version
来源：http://hz.cucudq.cn/gtcxorbbxb.html

TS:   process.platform;  process.version
来源：http://hz.zhaomingkeji.xyz/gtsydbcgyz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.dashuyun.cn/gtekoyumgf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.andypj.xyz/gtgtdxmewi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.snrcjt.cn/gtefbelzlv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yonumen.top/gtzwqeqfdw.html

================================================================================
来源：http://hz.yuanzhike.top/gtcpcdinsl.html

N. 数据结构与算法
来源：http://hz.sufxvd.cn/gtmozgqfeq.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtqqaligpo.html

[N01] 二分查找（有序数组）
来源：http://hz.yuxming.cn/gtrcyzuojo.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.iojbl.cn/gtclwxlhwp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.sxryk.cn/gtnydbneyi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shanyushiyangkeji.top/gtmhzzxwue.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cqqwz.cn/gtcvcntzwm.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hnqzz.top/gtwgdfmwcr.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.gaohongyu789.top/gtptlzvmfp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.aizwys.cn/gtfxowcops.html


<!-- 参考信息 -->