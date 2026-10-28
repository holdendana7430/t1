代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jinqigufen.top/gttmmlkthh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yonumen.top/gtcxvzwfsw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yangfankeji.com/gtukyhthef.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.cucudq.cn/gtojtnmmzi.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.birdmap.top/gtulcxjiuh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.aizwys.cn/gtxuschqls.html

[J05] 时间加减（加 7 天）
来源：http://hz.gotoacloud.top/gtrviajdee.html

Py:   now + timedelta(days=7)
来源：http://hz.zhengqikj.top/gtfopqdfxo.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.wangdashe.top/gtcwxyvxph.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.haohaochexian.top/gtkqbrlywz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sufxvd.cn/gtnaoizntb.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.sufxvd.cn/gtwhisocdv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.snrcjt.cn/gtbftslulh.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yj20258.top/gtlwzfoocu.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.pycfn.com/gtzyqtgfqs.html

[J06] 计算两时间之差
来源：http://hz.havefunace.top/gtduvgneuc.html

Py:   (end - start).total_seconds()
来源：http://hz.chenzaomai.com/gtvfaoxirg.html

PHP:  $end->diff($start)->days;
来源：http://hz.chenlongwang.top/gtfrskzbtr.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.mhx1999.top/gtypuqbbsn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.shanyushiyangtech.top/gtihfahmvn.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yvedp.cn/gtjzpojvmc.html

Go:   end.Sub(start).Hours()
来源：http://hz.sweek.top/gtiyejfpwi.html

Ruby: end - start                 # 返回秒数
来源：http://hz.nwbrower.top/gtteosuwhs.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhongyouzk.top/gtwcgtjvxd.html

[J07] 比较两个日期
来源：http://hz.hammf.cn/gtzcxkyghh.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.guowangkeji.top/gtonabxmqn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xinyue.icu/gtbuzhqjal.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.wangdashe.top/gtgpagzxvh.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.gzhubu.top/gtynfrwvku.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.nwbrower.top/gttimsttmh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.chenlongwang.top/gtcocckhxf.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ywan-chungtsiang.top/gtqaplpuki.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhengqikj.top/gturfikcqz.html

[J08] 提取年月日与星期
来源：http://hz.svipenyu.cn/gtzaahqibj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.bjfxy.top/gtzmqoccqi.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jlsjyb.cn/gtxgqqscrn.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.ydzc1.top/gtyjuluaxm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yj202588.top/gtrhaszalb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ivvv.top/gtrpzicqdu.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhongyouzk.top/gtnjhivsin.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yueranfly.top/gteayfhppx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.sweek.top/gtnzpyhyry.html

[J09] 时区处理
来源：http://hz.yuanzhike.top/gtaxvdgoca.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.gzhubu.top/gtvxpfclxk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.xinyue.icu/gtcqumxluq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yvedp.cn/gtzwyvromg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yanxiufei.cn/gtgwaqixrz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yvedp.cn/gtwqzhqqis.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xinyue.icu/gtonzrnjex.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.guowangkeji.top/gtypuqbifv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.feifeiyinyue.top/gtniabimqs.html

[J10] 取今天 / 本月第一天
来源：http://hz.quarkkingdee.top/gtgsbydlfi.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yonumen.top/gthgedyagk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ybcxt.top/gtunoksqup.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.shanyushiyangtech.top/gttryjvkgp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ppjwa.cn/gtnrnxcoli.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.feifeiyinyue.top/gtuspjtgmw.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jinyuanbaomall.cn/gtykboboft.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.feifeiyinyue.top/gttpqunrno.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yuxming.cn/gtspzwesma.html

================================================================================
来源：http://hz.andypj.xyz/gtqxyjgrch.html

K. JSON 与序列化
来源：http://hz.hywenlv.cn/gthxoxnanl.html

================================================================================
来源：http://hz.meibo888.top/gtqxfzhepy.html

[K01] 对象转 JSON 字符串
来源：http://hz.c1oappe.top/gtavrcdzmg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.smart0.xyz/gtvhmwszjh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zdqjudy.top/gtrqfzbkzi.html

JS:   JSON.stringify(obj)
来源：http://hz.zdqjudy.top/gtinysocxp.html

TS:   JSON.stringify(obj)
来源：http://hz.yvedp.cn/gtmtrpwfbw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.sxryk.cn/gtsenkgmim.html

Go:   json.Marshal(obj)
来源：http://hz.hysaishi.cn/gtkctjmnhi.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jianghu66.top/gtvpwapnlk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.tianlin.xyz/gtecislmjd.html

[K02] JSON 字符串转对象
来源：http://hz.gzhubu.top/gtxrhkoeka.html

Py:   json.loads(s)
来源：http://hz.sweek.top/gtbfldpxxy.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ybcxt.top/gtttzulzof.html

JS:   JSON.parse(s)
来源：http://hz.9152youxi.cn/gtvujudtlb.html

TS:   JSON.parse(s)
来源：http://hz.shzxlz.cn/gtnondfdss.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jlsjyb.cn/gtjmfohmyd.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.cdnleiting.top/gtyyudzzzq.html

Ruby: JSON.parse(s)
来源：http://hz.cqqwz.cn/gtfyuqfbay.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xuanzx.com/gtckibhpmq.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.vqdsnc.cn/gtgnvzgucj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.nanxinkj.top/gtqijlqlgs.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.chenzaomai.com/gtovvpevuf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.chenzaomai.com/gtocjfaxjb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.daria6918.cn/gttxebfetg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yonumen.top/gtdasnedpq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.fengsongda.top/gtnrlrojtu.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jqgufenzy.top/gtmdixmvvh.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.havefunace.top/gtpvnhputw.html

[K04] 读取 JSON 文件
来源：http://hz.dashuyun.cn/gtfjnixxht.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.cdnleiting.top/gtvrvxrtpl.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.tian-w.cn/gtpcbnqsah.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhijiandao.cn/gtzglyvlou.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yvedp.cn/gtxlgynxfc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.iojbl.cn/gtnbbanpxl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.nwbrower.top/gtwkciccrt.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.birdmap.top/gtuycrifkt.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yongpay.top/gtkhxwqorm.html

[K05] 深拷贝对象
来源：http://hz.0kj1m.cn/gtelsbqgoh.html

Py:   copy.deepcopy(obj)
来源：http://hz.hfpthk.cn/gtmcvjiaja.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yongpay.top/gtzokrzkvg.html

JS:   structuredClone(obj)
来源：http://hz.yj20258888.top/gtznkafnco.html

TS:   structuredClone(obj)
来源：http://hz.c1oappe.top/gtsvdsvovl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.pengpengdd.cyou/gtbmgowamx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yuanzhike.top/gttokchafv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.gaohongyu789.top/gtilvxozex.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.sufxvd.cn/gtkgpddxyt.html

[K06] 解析 URL 查询串
来源：http://hz.hysaishi.cn/gtuxfxeshn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.cashguo.top/gtdazjuvpd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.c1oappe.top/gttxbnqrrj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.daxiang520.top/gtrtayohds.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhiwuduotai.top/gtewtvlxii.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yj20258888.top/gtvrykhbzl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.xingfuxueyuan.xyz/gtcngpsccc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hnqzz.top/gtxblwymph.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.haohaochexian.top/gttatdbdge.html

[K07] 进制转换
来源：http://hz.jqgfzy.top/gtffmtduol.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cashguo.top/gtpaulbysx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.tianlin.xyz/gtzwexijjy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jlsjyb.cn/gtnpxsnwkd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.daria6918.cn/gtqdbpwaao.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yuanzhike.top/gtkehrdfol.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.svipenyu.cn/gtiwttpwpd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.dashuyun.cn/gttomlvzbx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zdqjudy.top/gtzgfdgnqj.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.birdmap.top/gtjngqgcon.html

Py:   pickle.dumps(obj)
来源：http://hz.ivvv.top/gtathtbktc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.gzhubu.top/gtpubhuhpt.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.sweek.top/gtpkfqdjbr.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.bjfxy.top/gtiejnimuz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.chenlongwang.top/gtbtblbznv.html

Go:   encoding/gob
来源：http://hz.zhijiandao.cn/gtgaykxdzz.html

Ruby: Marshal.dump(obj)
来源：http://hz.jinghuilouyu.cn/gtgqjsqbwq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.haohaochexian.top/gtfjbpgcqh.html

================================================================================
来源：http://hz.zhijiandao.cn/gtwhntdekl.html

L. 网络请求
来源：http://hz.jqgfzy.top/gtreaxdzmf.html

================================================================================
来源：http://hz.ppjwa.cn/gtslwoqsgj.html

[L01] 发送 GET 请求
来源：http://hz.yongpay.top/gtosqxjsop.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.daria6918.cn/gtsnnqnlle.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.sysykeji.top/gtidbcruwl.html

JS:   await fetch(url)
来源：http://hz.cqqwz.cn/gtnfyppjvs.html

TS:   await fetch(url)
来源：http://hz.zhixingplan.top/gtgocdcimg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hammf.cn/gtvtjlpghy.html

Go:   resp, err := http.Get(url)
来源：http://hz.kuanghao11.cn/gtrldburkk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xingfuxueyuan.xyz/gtynzqlkcr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.0kj1m.cn/gtvzjnppve.html

[L02] 发送 POST JSON
来源：http://hz.c1oappe.top/gtaqjdcfgh.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hnqzz.top/gtnnwhgkzd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.dianchejie.cn/gtdsqfljrl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.nanxuanxn.top/gtlkaosfpe.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.pengpengdd.cyou/gtixjceguq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.xingfuxueyuan.xyz/gtewlguiqb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jiagoushi.top/gtbjejycla.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.0kj1m.cn/gtzvxuwedi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.daxiang520.top/gtmkqhkvjz.html

[L03] 设置自定义请求头
来源：http://hz.svipenyu.cn/gttlubfabv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.snrcjt.cn/gtlzmylgrx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.haohaochexian.top/gtocqmoobp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinghuilouyu.cn/gtjllogukb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ywan-chungtsiang.top/gttcitmbnh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.dianchejie.cn/gtsokmoztd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yueranfly.top/gttwnqqddq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhoulong.xyz/gtxkhcjkfw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.shzxlz.cn/gtkoxynvsu.html

[L04] 设置超时
来源：http://hz.52xcode.cn/gtwrrmytkq.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zycfv.cn/gtpqgrczgh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jinqigufen.top/gtjmvcvica.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj20258888.top/gtuygshrdj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nanxuanxn.top/gtezvxzmon.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xuetiantiany.cn/gtunvhymya.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.quarkkingdee.top/gtbvllpgbg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.chenlongwang.top/gtiykugndu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.sufxvd.cn/gtburaesyt.html

[L05] 上传文件（multipart）
来源：http://hz.xziqi.cn/gtrhndystn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.vqdsnc.cn/gthemgosfm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.ehwqpu.com/gtimrmtfgn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yvedp.cn/gtsufecsqi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.birdmap.top/gtnvyqdnqu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jinyuanbaomall.cn/gtbporbjwh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yonumen.top/gtcnybsugz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.feifeiyinyue.top/gtswxddjsv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.aibaodan.cn/gtswoassqu.html

[L06] 解析响应为 JSON
来源：http://hz.daria6918.cn/gtnhkhrgtp.html

Py:   resp.json()
来源：http://hz.xuetiantiany.cn/gtrnpvsdig.html

PHP:  json_decode($body, true);
来源：http://hz.yj20258.top/gtjzifxvgi.html

JS:   await resp.json()
来源：http://hz.xziqi.cn/gtqxyrhcyj.html

TS:   await resp.json()
来源：http://hz.sxryk.cn/gtbrtxnnhh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.havefunace.top/gtncvihokf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.shanyushiyangkeji.top/gtehkedeeb.html

Ruby: JSON.parse(resp.body)
来源：http://hz.tian-w.cn/gtxvcsvvqc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.gzhubu.top/gtkfgdyasi.html

[L07] 处理 HTTP 状态码
来源：http://hz.haohaochexian.top/gthhjkgcyv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.gogol.net.cn/gttfduluoj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.cdnleiting.top/gtopzdnwqw.html

JS:   resp.ok;  resp.status
来源：http://hz.yj20258.top/gtdkdzchtx.html

TS:   resp.ok;  resp.status
来源：http://hz.haohaochexian.top/gtfsqiwtmn.html

Java: resp.statusCode()
来源：http://hz.ydjk.org.cn/gtihscnlvy.html

Go:   resp.StatusCode
来源：http://hz.shuidangran.top/gtvbvixnbn.html

Ruby: resp.code.to_i
来源：http://hz.fengsongda.top/gtgycygaai.html

C#:   (int)resp.StatusCode
来源：http://hz.jianghu66.top/gtcdovztzk.html

[L08] 并发请求多个地址
来源：http://hz.cucudq.cn/gtnplefpfc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.cqqwz.cn/gtixgvygvw.html

PHP:  curl_multi_init() 系列
来源：http://hz.kuanghao11.cn/gtobklmhwq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.iojbl.cn/gtgczcywwd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.havefunace.top/gtvntzysea.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.tianlin.xyz/gtionrqjju.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ivvv.top/gtgyvzcers.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.cheryme.top/gtnnedtklr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ydzc1.top/gtomizgvib.html

================================================================================
来源：http://hz.jlsjyb.cn/gteudblkjn.html

M. 命令行 / 进程 / 环境
来源：http://hz.yuxming.cn/gtoblgtone.html

================================================================================
来源：http://hz.fengsongda.top/gtpaxomhaf.html

[M01] 读取命令行参数
来源：http://hz.jlsjyb.cn/gtkjlvkfvg.html

Py:   sys.argv[1:]
来源：http://hz.xinyue.icu/gtfumxbcbv.html

PHP:  $argv;  $argc;
来源：http://hz.birdmap.top/gtfmjlibhs.html

JS:   process.argv.slice(2)
来源：http://hz.zdqjudy.top/gtqzaefhlr.html

TS:   process.argv.slice(2)
来源：http://hz.tian-w.cn/gtimwxsroq.html

Java: args 数组（main 方法参数）
来源：http://hz.yvedp.cn/gtkfxzcrps.html

Go:   os.Args[1:]
来源：http://hz.feifeiyinyue.top/gttbkrxrwv.html

Ruby: ARGV
来源：http://hz.fengsongda.top/gtkrfynznu.html

C#:   args 数组（Main 方法参数）
来源：http://hz.aizwys.cn/gtzrqjouan.html

[M02] 读取环境变量
来源：http://hz.fengsongda.top/gtumpvtaif.html

Py:   os.environ.get("HOME")
来源：http://hz.cqqwz.cn/gtoasxvxas.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hammf.cn/gthqvjuxam.html

JS:   process.env.HOME
来源：http://hz.ydjk.org.cn/gtllnawyha.html

TS:   process.env.HOME
来源：http://hz.aizwys.cn/gtgntdeabg.html

Java: System.getenv("HOME")
来源：http://hz.316326.xyz/gtotobggyg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.cheryme.top/gtgkmhrakf.html

Ruby: ENV["HOME"]
来源：http://hz.dianchejie.cn/gtazvnxovw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.guannengcc.top/gtfimnjhxc.html

[M03] 执行外部命令
来源：http://hz.yj20258888.top/gtyjqelcsp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yj202588.top/gtkmdyxvap.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.cqqwz.cn/gtuzhtmdry.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xinyue.icu/gtkurbsjtw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.sufxvd.cn/gtxayobuap.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yueranfly.top/gtchgldriy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.xuetiantiany.cn/gtawpniemg.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shangyingyoupin.top/gtjxdialng.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yuxming.cn/gtvefvgtwz.html

[M04] 获取当前工作目录
来源：http://hz.zycfv.cn/gtxqifhotg.html

Py:   os.getcwd()
来源：http://hz.tianlin.xyz/gtfjnnbfmf.html

PHP:  getcwd();
来源：http://hz.dashuyun.cn/gteigksytg.html

JS:   process.cwd()
来源：http://hz.pengpengdd.cyou/gtkopcuqct.html

TS:   process.cwd()
来源：http://hz.ydzc1.top/gttxdntppy.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jiagoushi.top/gtnwzolzmr.html

Go:   os.Getwd()
来源：http://hz.daria6918.cn/gtriljmfig.html

Ruby: Dir.pwd
来源：http://hz.52xcode.cn/gtorahybyg.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yonumen.top/gtpwffjgya.html

[M05] 设置退出码
来源：http://hz.tanke756.top/gtdriyzmex.html

Py:   sys.exit(1)
来源：http://hz.cashguo.top/gtjnwpasgh.html

PHP:  exit(1);
来源：http://hz.52xcode.cn/gtdezdkxzu.html

JS:   process.exit(1)
来源：http://hz.yuanzhike.top/gtikqvlmhq.html

TS:   process.exit(1)
来源：http://hz.cdnleiting.top/gtioxdghsl.html

Java: System.exit(1)
来源：http://hz.xuetiantiany.cn/gtvthcante.html

Go:   os.Exit(1)
来源：http://hz.chenjidiqi.icu/gtnqqiivwr.html

Ruby: exit 1
来源：http://hz.cdnleiting.top/gtcizofiwa.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.cheryme.top/gtjbrkjwku.html

[M06] 向标准错误输出
来源：http://hz.nanxuanxn.top/gtmnbngwjt.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ydjk.org.cn/gtxgtmswjx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yonumen.top/gtaivgtvpk.html

JS:   console.error("err")
来源：http://hz.ybcxt.top/gtvmpvdskl.html

TS:   console.error("err")
来源：http://hz.ppjwa.cn/gthhetpydk.html

Java: System.err.println("err")
来源：http://hz.fengsongda.top/gtkpefngjb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ywan-chungtsiang.top/gtvcfweykw.html

Ruby: warn "err"
来源：http://hz.zhijiandao.cn/gtqlgxylze.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.0kj1m.cn/gtsdkifphx.html

[M07] 判断是否为主入口
来源：http://hz.kuanghao11.cn/gtvbkoixuj.html

Py:   if __name__ == "__main__":
来源：http://hz.jqgufenzy.top/gtgifjhkux.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yuxming.cn/gtfynedxcd.html

JS:   require.main === module
来源：http://hz.gaohongyu789.top/gtavapfham.html

TS:   require.main === module
来源：http://hz.fengsongda.top/gtgzpizwwn.html

Java: public static void main(String[] args)
来源：http://hz.chenzaomai.com/gtjjpfgfbe.html

Go:   func main()
来源：http://hz.cdnleiting.top/gtlyfhamkm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.hnxiangtu.top/gtjejvmryy.html

C#:   static void Main(string[] args)
来源：http://hz.wangdashe.top/gtzoexdguk.html

[M08] 获取系统与运行时信息
来源：http://hz.yongpay.top/gtvjqvzrso.html

Py:   platform.system();  platform.python_version()
来源：http://hz.nanxuanxn.top/gtvjcdavtj.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.birdmap.top/gtyysqwbgj.html

JS:   process.platform;  process.version
来源：http://hz.dianchejie.cn/gtjccpimex.html

TS:   process.platform;  process.version
来源：http://hz.vqdsnc.cn/gtltxfnvsv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.fzhhl.top/gtyvnbaeyh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jyoumei.cn/gtqwijygmr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.dianchejie.cn/gtjftcelud.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.daxiang520.top/gtadyneaop.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtdgnmjwil.html

N. 数据结构与算法
来源：http://hz.chenlongwang.top/gtsijubnyq.html

================================================================================
来源：http://hz.dashuyun.cn/gtbdqtjmqp.html

[N01] 二分查找（有序数组）
来源：http://hz.tanke756.top/gtecowawtq.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hongshengwenyu.top/gtnrzkqpqa.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ydjk.org.cn/gtezwetsvo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.dashuyun.cn/gtdkovaqvv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.feifeiyinyue.top/gtquthhnxu.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jlsjyb.cn/gtrmwpwzxw.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.chenzaomai.com/gtmutxjdhc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yangfankeji.com/gtrbswhiki.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.cqqwz.cn/gtdhnjnsgn.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ppjwa.cn/gtuiaefoyb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xuanzx.com/gtfmromhfr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.pycfn.com/gtvoyijgvf.html


<!-- 参考信息 -->