代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.havefunace.top/gtbwdoaxlx.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jlsjyb.cn/gttkuvsauc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.redwolf501.top/gtfgvidykh.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhixingplan.top/gtvcqbxbjf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.nanxuanxn.top/gteafuvsqw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhaomingkeji.xyz/gtsxdrldtc.html

[J05] 时间加减（加 7 天）
来源：http://hz.tanke756.top/gtqzrtjpti.html

Py:   now + timedelta(days=7)
来源：http://hz.zhoulong.xyz/gtwosokdqz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jinyuanbaomall.cn/gtpouyvzpd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinqigufen.top/gtjtqapqoi.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.pengpengdd.cyou/gtawbiisxs.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.aibaodan.cn/gtcdwfxbfy.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.sufxvd.cn/gtvwlvhxzc.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jinghuilouyu.cn/gtqewcvgdm.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.shanyushiyangtech.top/gtiqkvicoy.html

[J06] 计算两时间之差
来源：http://hz.chenzaomai.com/gtewhmdafq.html

Py:   (end - start).total_seconds()
来源：http://hz.dashuyun.cn/gtthsctvjk.html

PHP:  $end->diff($start)->days;
来源：http://hz.xinyue.icu/gtwfkoggdz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.bjfxy.top/gtkcmfprwe.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.wangdashe.top/gtqcenqmdb.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.birdmap.top/gtclispmvl.html

Go:   end.Sub(start).Hours()
来源：http://hz.cheryme.top/gtxaalrjzq.html

Ruby: end - start                 # 返回秒数
来源：http://hz.cqqwz.cn/gtwwsmgizb.html

C#:   (end - start).TotalSeconds
来源：http://hz.sysykeji.top/gtxfmtdrrd.html

[J07] 比较两个日期
来源：http://hz.sweek.top/gtehbgoprj.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.gotoacloud.top/gtqoppylbn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ybcxt.top/gtyyxhltdw.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yueranfly.top/gthinxelfg.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.mhx1999.top/gtnjbalfii.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.tianlin.xyz/gtfgugfdcn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hammf.cn/gtsoeuivjo.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.guannengcc.top/gtilshepyt.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zdqjudy.top/gtsxvjtptw.html

[J08] 提取年月日与星期
来源：http://hz.kuanghao11.cn/gtjfqlvntr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.cashguo.top/gtodrmkgej.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.haohaochexian.top/gtrmxxhvdq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhaomingkeji.xyz/gtffcthzjt.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yonumen.top/gtxuhnyoup.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ywan-chungtsiang.top/gtpebycvvk.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ivvv.top/gtixaiviyv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zycfv.cn/gthbezhjqe.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jianghu66.top/gttnkfvpou.html

[J09] 时区处理
来源：http://hz.yj20258888.top/gtufrsuqny.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shanyushiyangtech.top/gtqnudsics.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.feifeiyinyue.top/gtbmydntiq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shanyushiyangkeji.top/gtatpwqzuh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ppjwa.cn/gtuibtlacq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zycfv.cn/gtdafnvpqi.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jyoumei.cn/gtwybkebtu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jlsjyb.cn/gtxppnrtzp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.cashguo.top/gteowqvvdx.html

[J10] 取今天 / 本月第一天
来源：http://hz.dashuyun.cn/gtwbdnsxzs.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhixingplan.top/gtrmugutqw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.iojbl.cn/gtnlqdamhx.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.aibaodan.cn/gthurtkugv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yj20258.top/gtbudeltcv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jinqigfzy.top/gtxdbslkmr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.316326.xyz/gtajjrnkaj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhiwuduotai.top/gtvdmdtikr.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.daria6918.cn/gtipvtzibt.html

================================================================================
来源：http://hz.yangfankeji.com/gtypuxmkmr.html

K. JSON 与序列化
来源：http://hz.sxryk.cn/gtrazruzca.html

================================================================================
来源：http://hz.zycfv.cn/gtbttnpfbr.html

[K01] 对象转 JSON 字符串
来源：http://hz.yongpay.top/gtbpfqevwe.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.nanxuanxn.top/gtyuyuqjya.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.tian-w.cn/gtfbxnxmbp.html

JS:   JSON.stringify(obj)
来源：http://hz.jiagoushi.top/gtuijizdsw.html

TS:   JSON.stringify(obj)
来源：http://hz.jqgfzy.top/gtbpkuonpj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.nwbrower.top/gtfdeqtifx.html

Go:   json.Marshal(obj)
来源：http://hz.zhongyouzk.top/gtllvpyarw.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jinqigfzy.top/gtcnvyrwhv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.316326.xyz/gtgnhhksfx.html

[K02] JSON 字符串转对象
来源：http://hz.0kj1m.cn/gtckypprsx.html

Py:   json.loads(s)
来源：http://hz.mhx1999.top/gtgqnflvvx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ivvv.top/gtangifkqk.html

JS:   JSON.parse(s)
来源：http://hz.chenlongwang.top/gtumcsjmza.html

TS:   JSON.parse(s)
来源：http://hz.yonumen.top/gtssdfbrbs.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.dashuyun.cn/gtidkolzdx.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.nanxinkj.top/gtxcbrfzpg.html

Ruby: JSON.parse(s)
来源：http://hz.xziqi.cn/gtvzhbmhtr.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jinyuanbaomall.cn/gtdjwtzokc.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yonumen.top/gttsyujoqp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yangfankeji.com/gttaxgbcqo.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhiwuduotai.top/gtlcxjgkjy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhaomingkeji.xyz/gtjwhpehxz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhongyouzk.top/gtswfiyjfj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ppjwa.cn/gtpowuznfy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.c1oappe.top/gttcygushh.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zdqjudy.top/gtzovowncp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.tanke756.top/gtzrpynhgw.html

[K04] 读取 JSON 文件
来源：http://hz.zhijiandao.cn/gtqktxywtx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.wangshuangyany.cn/gtngjjrhgt.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.xinyue.icu/gtgpzgqjli.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.nanxuanxn.top/gtotnvphqh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.dashuyun.cn/gtwcrrlzck.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.tian-w.cn/gtajrajmcv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xylfe.cn/gtqphborzr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.cqqwz.cn/gthhmledss.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jinqigufen.top/gtlubezycn.html

[K05] 深拷贝对象
来源：http://hz.cucudq.cn/gtwiuwljjs.html

Py:   copy.deepcopy(obj)
来源：http://hz.ydzc1.top/gtdbyzorsv.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhongyouzk.top/gtesptmbbx.html

JS:   structuredClone(obj)
来源：http://hz.sufxvd.cn/gtvxusktgx.html

TS:   structuredClone(obj)
来源：http://hz.yangfankeji.com/gteopiiwup.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhiwuduotai.top/gtvwzwmhmk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yueranfly.top/gtzutgrujd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yangfankeji.com/gtktokqkxp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.cdnleiting.top/gtogrtwuip.html

[K06] 解析 URL 查询串
来源：http://hz.ybcxt.top/gtcqgluemk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.chenjidiqi.icu/gtckovdnlk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.guannengcc.top/gtpzuhdbqz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.havefunace.top/gtxkplxqej.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj20258888.top/gtepygkjws.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.dianchejie.cn/gthngsryvr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jiagoushi.top/gtdoujlujd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.cucudq.cn/gtzdbrruzh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.snrcjt.cn/gtizoybtjj.html

[K07] 进制转换
来源：http://hz.meibo888.top/gtmrwrqucj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.shangyingyoupin.top/gttsvivluw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yueranfly.top/gtuwttcljh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhengqikj.top/gttouutwjw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.mhx1999.top/gthefertrg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.sysykeji.top/gtkendinef.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.iojbl.cn/gtyyjjiplu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.aizwys.cn/gtnrkxzjep.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hywenlv.cn/gtkkopbqri.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.hnxiangtu.top/gtcctgebgv.html

Py:   pickle.dumps(obj)
来源：http://hz.yanxiufei.cn/gtmpcizzri.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.wangdashe.top/gtctlbuqko.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hnxiangtu.top/gtgtrokxob.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yj20258.top/gtlslgqtyc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.smart0.xyz/gtbffncvcx.html

Go:   encoding/gob
来源：http://hz.kuanghao11.cn/gtrbjiubfy.html

Ruby: Marshal.dump(obj)
来源：http://hz.chenzaomai.com/gtayvaitna.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.316326.xyz/gtsrwpfdaa.html

================================================================================
来源：http://hz.ydzc1.top/gtogvxnqmi.html

L. 网络请求
来源：http://hz.iojbl.cn/gtewhhlyll.html

================================================================================
来源：http://hz.yvedp.cn/gtmgdrbuwc.html

[L01] 发送 GET 请求
来源：http://hz.jinyuanbaomall.cn/gtwfiexgcj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.smart0.xyz/gtulaoltog.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jqgfzy.top/gtlufttitm.html

JS:   await fetch(url)
来源：http://hz.guowangkeji.top/gtjliujetw.html

TS:   await fetch(url)
来源：http://hz.jinyuanbaomall.cn/gtzluipbky.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.vqdsnc.cn/gtytqafbkj.html

Go:   resp, err := http.Get(url)
来源：http://hz.ywan-chungtsiang.top/gtenulhykn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.c1oappe.top/gtuxpvqdfn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.bjfxy.top/gtritgvjjq.html

[L02] 发送 POST JSON
来源：http://hz.chenzaomai.com/gtqkqvrfrc.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.c1oappe.top/gtzehjsezc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xuetiantiany.cn/gtfrbckuvg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hysaishi.cn/gtlaojxliq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jiagoushi.top/gtbziejsve.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhaomingkeji.xyz/gtoyjmoguu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yuxming.cn/gtbfxgwbwv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jinyuanbaomall.cn/gtohnnpwxr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yj202588.top/gtxoqxgqfl.html

[L03] 设置自定义请求头
来源：http://hz.redwolf501.top/gtthlvoyhw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhoulong.xyz/gtexwlvyri.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.guannengcc.top/gtjcmcytxn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yongpay.top/gtpdjysyee.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cqqwz.cn/gtboatxyfq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ybcxt.top/gtamcwmfvq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.feifeiyinyue.top/gtypxpuqgh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.aizwys.cn/gtoqbicsvq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jyoumei.cn/gtqtuihrko.html

[L04] 设置超时
来源：http://hz.shuidangran.top/gtfgczyksv.html

Py:   requests.get(url, timeout=5)
来源：http://hz.mhx1999.top/gtmwmzdyyr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.sweek.top/gtgdtbtuhq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.daxiang520.top/gtegfnjpsl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yangfankeji.com/gtdxmbxbss.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ivvv.top/gtobaoivfl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ehwqpu.com/gtgqdcxjns.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.sysykeji.top/gtranexoft.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hnxiangtu.top/gtpijwgtzb.html

[L05] 上传文件（multipart）
来源：http://hz.ehwqpu.com/gtvootkiwj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.aizwys.cn/gteoatkemy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhijiandao.cn/gtuzhiaefr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jianghu66.top/gtglozrosi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.hywenlv.cn/gtpdhkmqbd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ywan-chungtsiang.top/gthjrmejun.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.chenlongwang.top/gtkefabiyw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jinqigfzy.top/gtfqjzjwpp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhijiandao.cn/gtczahddfs.html

[L06] 解析响应为 JSON
来源：http://hz.dianchejie.cn/gtrwlqfiae.html

Py:   resp.json()
来源：http://hz.jqgfzy.top/gtnkxhljjs.html

PHP:  json_decode($body, true);
来源：http://hz.wangdashe.top/gtmzdmdwqe.html

JS:   await resp.json()
来源：http://hz.yuanzhike.top/gtwjqujlnk.html

TS:   await resp.json()
来源：http://hz.haohaochexian.top/gtzhhvipfg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.daxiang520.top/gtbijbuxgo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.kuanghao11.cn/gtjtjbzmas.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yongpay.top/gtmniahduc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hnxiangtu.top/gtjtahcots.html

[L07] 处理 HTTP 状态码
来源：http://hz.feifeiyinyue.top/gtiojdfxme.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jiagoushi.top/gtcjdrbeog.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hongshengwenyu.top/gtdorhjjse.html

JS:   resp.ok;  resp.status
来源：http://hz.hfpthk.cn/gtkxlnxycq.html

TS:   resp.ok;  resp.status
来源：http://hz.yueranfly.top/gtiabdnrpu.html

Java: resp.statusCode()
来源：http://hz.jiagoushi.top/gtftwtiqsx.html

Go:   resp.StatusCode
来源：http://hz.zhaomingkeji.xyz/gtmdgmqnun.html

Ruby: resp.code.to_i
来源：http://hz.quarkkingdee.top/gtpraltrri.html

C#:   (int)resp.StatusCode
来源：http://hz.nwbrower.top/gtpqruzjqr.html

[L08] 并发请求多个地址
来源：http://hz.shangyingyoupin.top/gtsmhzqncm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hnqzz.top/gtqnynznvb.html

PHP:  curl_multi_init() 系列
来源：http://hz.52xcode.cn/gtcuxwndve.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nanxinkj.top/gtgxrbvmrx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.bjfxy.top/gtelvnlcvt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yuxming.cn/gtjaiuxzub.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhijiandao.cn/gtdqlcdhvu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zycfv.cn/gtzzbvwbik.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.0kj1m.cn/gthgekidmy.html

================================================================================
来源：http://hz.chenzaomai.com/gtbbqcgxjq.html

M. 命令行 / 进程 / 环境
来源：http://hz.bjfxy.top/gtodrggexi.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtescajujo.html

[M01] 读取命令行参数
来源：http://hz.chenlongwang.top/gtyrmdubcu.html

Py:   sys.argv[1:]
来源：http://hz.tian-w.cn/gtlcwhavpp.html

PHP:  $argv;  $argc;
来源：http://hz.zdqjudy.top/gtrjcbtjuj.html

JS:   process.argv.slice(2)
来源：http://hz.jinqigfzy.top/gtscesrxrf.html

TS:   process.argv.slice(2)
来源：http://hz.yvedp.cn/gtcyrwxqmd.html

Java: args 数组（main 方法参数）
来源：http://hz.yongpay.top/gtxoxoebkh.html

Go:   os.Args[1:]
来源：http://hz.ehwqpu.com/gtilrkkjeq.html

Ruby: ARGV
来源：http://hz.yueranfly.top/gtwhqogfin.html

C#:   args 数组（Main 方法参数）
来源：http://hz.xziqi.cn/gtprtbtyon.html

[M02] 读取环境变量
来源：http://hz.hnxiangtu.top/gtptooepbz.html

Py:   os.environ.get("HOME")
来源：http://hz.svipenyu.cn/gtxfmcrcub.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.havefunace.top/gtnnnexlyl.html

JS:   process.env.HOME
来源：http://hz.zhoulong.xyz/gtxsdvxxeu.html

TS:   process.env.HOME
来源：http://hz.bjfxy.top/gtatlvzaob.html

Java: System.getenv("HOME")
来源：http://hz.yangfankeji.com/gtcgziekwa.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jqgufenzy.top/gtetmswqdi.html

Ruby: ENV["HOME"]
来源：http://hz.gzhubu.top/gtrjjsgssh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhiwuduotai.top/gtyiextquu.html

[M03] 执行外部命令
来源：http://hz.shangyingyoupin.top/gtihyvdxvs.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jiagoushi.top/gtmugxicli.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hfpthk.cn/gtitpuhgva.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yvedp.cn/gtwvrrplft.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.aizwys.cn/gtlkwsowgu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.dashuyun.cn/gtsorznrkk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yj202588.top/gtiytzapiy.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yj20258888.top/gtugedhrfl.html

C#:   Process.Start("ls", "-l");
来源：http://hz.aizwys.cn/gtchxrwfli.html

[M04] 获取当前工作目录
来源：http://hz.fzhhl.top/gtpznmpvwg.html

Py:   os.getcwd()
来源：http://hz.meibo888.top/gtemniofnx.html

PHP:  getcwd();
来源：http://hz.tanke756.top/gtxmdwrjpa.html

JS:   process.cwd()
来源：http://hz.cashguo.top/gtolctakgt.html

TS:   process.cwd()
来源：http://hz.cdnleiting.top/gtapjyayey.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yj20258888.top/gtivzwmzwa.html

Go:   os.Getwd()
来源：http://hz.gotoacloud.top/gtaxqecakg.html

Ruby: Dir.pwd
来源：http://hz.bjfxy.top/gtkxddzfdl.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yonumen.top/gtlwxiwlvo.html

[M05] 设置退出码
来源：http://hz.ehwqpu.com/gthyrxkias.html

Py:   sys.exit(1)
来源：http://hz.bjfxy.top/gtskufxudz.html

PHP:  exit(1);
来源：http://hz.hongshengwenyu.top/gtqxvgnghn.html

JS:   process.exit(1)
来源：http://hz.ehwqpu.com/gtzvxlkfor.html

TS:   process.exit(1)
来源：http://hz.tanke756.top/gtngxlkcvl.html

Java: System.exit(1)
来源：http://hz.jinqigfzy.top/gtedkstciz.html

Go:   os.Exit(1)
来源：http://hz.sxryk.cn/gtlkqobfcj.html

Ruby: exit 1
来源：http://hz.hnxiangtu.top/gtcnvaohxx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zhengqikj.top/gtbjhgpoyr.html

[M06] 向标准错误输出
来源：http://hz.feifeiyinyue.top/gtdxbcvbdq.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhoulong.xyz/gtemovskwm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ivvv.top/gtsbzyqzhs.html

JS:   console.error("err")
来源：http://hz.chenzaomai.com/gtcfqoiqij.html

TS:   console.error("err")
来源：http://hz.mhx1999.top/gtuapqmjqb.html

Java: System.err.println("err")
来源：http://hz.yonumen.top/gtfiracvsp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.gotoacloud.top/gtghnlpcbo.html

Ruby: warn "err"
来源：http://hz.feifeiyinyue.top/gtoyulqgvx.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.daria6918.cn/gtzrhqfjem.html

[M07] 判断是否为主入口
来源：http://hz.zhijiandao.cn/gtxkisvkjb.html

Py:   if __name__ == "__main__":
来源：http://hz.yongpay.top/gtafhcyyhi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.guowangkeji.top/gtevhbsldw.html

JS:   require.main === module
来源：http://hz.havefunace.top/gtbtjurayq.html

TS:   require.main === module
来源：http://hz.sufxvd.cn/gtcougkyea.html

Java: public static void main(String[] args)
来源：http://hz.xylfe.cn/gtteblkfcd.html

Go:   func main()
来源：http://hz.yuxming.cn/gtlihmprcz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.nanxuanxn.top/gtkepylwlj.html

C#:   static void Main(string[] args)
来源：http://hz.jyoumei.cn/gtbdiifooy.html

[M08] 获取系统与运行时信息
来源：http://hz.cqqwz.cn/gtentmfkag.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yongpay.top/gttxsbbrbp.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.c1oappe.top/gtxlcjzlii.html

JS:   process.platform;  process.version
来源：http://hz.birdmap.top/gthayvjhsn.html

TS:   process.platform;  process.version
来源：http://hz.nanxinkj.top/gtnbwaoipk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhixingplan.top/gtdxbgmita.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.ydjk.org.cn/gtgdwtcvpx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.9152youxi.cn/gtukcobvxr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhijiandao.cn/gtqljxzxep.html

================================================================================
来源：http://hz.yj20258.top/gtkmpcvrgs.html

N. 数据结构与算法
来源：http://hz.jyoumei.cn/gtluaqtntr.html

================================================================================
来源：http://hz.xinyue.icu/gtuwrirgjs.html

[N01] 二分查找（有序数组）
来源：http://hz.meibo888.top/gtgfdyuaaf.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.sysykeji.top/gtfuluylrp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhixingplan.top/gtkodzcymm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.aizwys.cn/gteljrqfno.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yongpay.top/gtjpxcaget.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jqgfzy.top/gtlejqlpys.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.tian-w.cn/gtzfkmvtpw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.sufxvd.cn/gtlzdikhle.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.hysaishi.cn/gtnstlmpdy.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yj202588.top/gtqnoddgcc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shuidangran.top/gtlfxekebf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.wangshuangyany.cn/gtagatxtju.html


<!-- 参考信息 -->