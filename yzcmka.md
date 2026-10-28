代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.gogol.net.cn/gttcafgzrl.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.316326.xyz/gtggvhxjxz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.aibaodan.cn/gtibusyolq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.fengsongda.top/gtrnkgpmye.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yangfankeji.com/gtwkypxisr.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.guannengcc.top/gttnviofeq.html

[J05] 时间加减（加 7 天）
来源：http://hz.52xcode.cn/gtqshomdof.html

Py:   now + timedelta(days=7)
来源：http://hz.jinghuilouyu.cn/gtuihgpjjb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.haohaochexian.top/gtjudponai.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.andypj.xyz/gttcsbbzus.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shanyushiyangkeji.top/gtpyyvypnh.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.nanxinkj.top/gtutgjqpxu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yj20258.top/gtndojftej.html

Ruby: Time.now + 7 * 86400
来源：http://hz.52xcode.cn/gtggqzpsfw.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xziqi.cn/gtlufwurws.html

[J06] 计算两时间之差
来源：http://hz.yj20258.top/gtqopazxnf.html

Py:   (end - start).total_seconds()
来源：http://hz.yueranfly.top/gtvuvkwfnz.html

PHP:  $end->diff($start)->days;
来源：http://hz.bjfxy.top/gtqignidfw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.tian-w.cn/gtwxkdamqq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.snrcjt.cn/gtyoyowilj.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jianghu66.top/gtqwdqaqzz.html

Go:   end.Sub(start).Hours()
来源：http://hz.bjfxy.top/gtqlsziihh.html

Ruby: end - start                 # 返回秒数
来源：http://hz.aizwys.cn/gtjeyvarhb.html

C#:   (end - start).TotalSeconds
来源：http://hz.hfpthk.cn/gthuahxjbd.html

[J07] 比较两个日期
来源：http://hz.daxiang520.top/gtgynfjdme.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.shuidangran.top/gthhmbmzwz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.nanxuanxn.top/gtrcxamfkb.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.feifeiyinyue.top/gthfffkfnr.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.pengpengdd.cyou/gtmoxgvtkg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ydjk.org.cn/gtgobanjtm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ydzc1.top/gtdowwuzug.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.daxiang520.top/gtalsodrlr.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.redwolf501.top/gteqsbqqkd.html

[J08] 提取年月日与星期
来源：http://hz.pengpengdd.cyou/gtcrgyxcgv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.shuidangran.top/gtamxgvneh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.dianchejie.cn/gtcsovnebr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yj20258.top/gtguvupviz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.bjfxy.top/gtelqnwoif.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.dashuyun.cn/gtjulqiwxe.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhixingplan.top/gtdszbeudv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.mhx1999.top/gtnhxtcgvm.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.shanyushiyangtech.top/gtratkizre.html

[J09] 时区处理
来源：http://hz.shanyushiyangkeji.top/gtafgqtamp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.chenzaomai.com/gtoezoymfv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhengqikj.top/gtspvztvhi.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.guannengcc.top/gtoftasocf.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yuanzhike.top/gtliyeblve.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.guannengcc.top/gthcwbmdvh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.shangyingyoupin.top/gtwjhzuquz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yonumen.top/gtvzrraicm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yj202588.top/gtyutztczs.html

[J10] 取今天 / 本月第一天
来源：http://hz.shzxlz.cn/gtncnxthxc.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhaomingkeji.xyz/gttpapkgjv.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.shzxlz.cn/gtedlhupoc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.guannengcc.top/gtuxubwxvd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.chenlongwang.top/gtjrvvucfj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.hammf.cn/gtqhbajbdm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.wangshuangyany.cn/gttvslcigv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ywan-chungtsiang.top/gtrzfnrunp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.cqqwz.cn/gtzupjubzz.html

================================================================================
来源：http://hz.vqdsnc.cn/gtjjohvoww.html

K. JSON 与序列化
来源：http://hz.xylfe.cn/gtrjipaxnw.html

================================================================================
来源：http://hz.aibaodan.cn/gtgmilhyjb.html

[K01] 对象转 JSON 字符串
来源：http://hz.svipenyu.cn/gtfnfvjbdc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.birdmap.top/gtfdrmhvlm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yonumen.top/gtxbyneldg.html

JS:   JSON.stringify(obj)
来源：http://hz.iojbl.cn/gtabyrzyvm.html

TS:   JSON.stringify(obj)
来源：http://hz.hnxiangtu.top/gtaspvojos.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.feifeiyinyue.top/gtfdnvaxib.html

Go:   json.Marshal(obj)
来源：http://hz.tanke756.top/gtjzangnbk.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hnxiangtu.top/gtjdofvukr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.0kj1m.cn/gtzfsxsqak.html

[K02] JSON 字符串转对象
来源：http://hz.shanyushiyangkeji.top/gtqswpyxps.html

Py:   json.loads(s)
来源：http://hz.zhoulong.xyz/gtpreucubv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hysaishi.cn/gtkmiluzjh.html

JS:   JSON.parse(s)
来源：http://hz.shanyushiyangtech.top/gtcyjzquhk.html

TS:   JSON.parse(s)
来源：http://hz.zhongyouzk.top/gtfnioajtj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhoulong.xyz/gtguioorbt.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.aizwys.cn/gtniuwakye.html

Ruby: JSON.parse(s)
来源：http://hz.svipenyu.cn/gtwslolrlz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.chenzaomai.com/gthmewyaml.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yj202588.top/gtaelvjmkz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhaomingkeji.xyz/gteadyjkvx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.xylfe.cn/gtyuhalgvx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinghuilouyu.cn/gtsedrhpmy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.dashuyun.cn/gtsobkhiwo.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.nanxinkj.top/gtbnmqpxeu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yongpay.top/gtjtpocbcn.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.chenzaomai.com/gtmjduznam.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.nanxuanxn.top/gtjsyukpos.html

[K04] 读取 JSON 文件
来源：http://hz.shanyushiyangtech.top/gtemqonlfv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zycfv.cn/gtrnivhphc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.fengsongda.top/gtfizppirq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.aibaodan.cn/gtsvktkrnm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.aibaodan.cn/gtedhdfzgg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.pengpengdd.cyou/gtsfltaipj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.gogol.net.cn/gtvzmfdamf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yuanzhike.top/gtkkyhaqnd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.smart0.xyz/gtkjcmnuqq.html

[K05] 深拷贝对象
来源：http://hz.gzhubu.top/gttpmdiedd.html

Py:   copy.deepcopy(obj)
来源：http://hz.ywan-chungtsiang.top/gtmozocref.html

PHP:  unserialize(serialize($obj));
来源：http://hz.shangyingyoupin.top/gtwanughob.html

JS:   structuredClone(obj)
来源：http://hz.gogol.net.cn/gthacmtjbe.html

TS:   structuredClone(obj)
来源：http://hz.quarkkingdee.top/gtbmzvncgb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.9152youxi.cn/gtlgfhwzgw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.shangyingyoupin.top/gtimayfudr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yangfankeji.com/gtqsetfrto.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.52xcode.cn/gtkyjywcoq.html

[K06] 解析 URL 查询串
来源：http://hz.316326.xyz/gtqxoqziie.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ivvv.top/gtxntekawn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yj202588.top/gttwovhngw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinqigufen.top/gtwlwtdllg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.aibaodan.cn/gtkhrnnubj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yvedp.cn/gtpoawvcgt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.svipenyu.cn/gtouugpihd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.andypj.xyz/gtorodtckb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.snrcjt.cn/gtkhspdlvg.html

[K07] 进制转换
来源：http://hz.meibo888.top/gtvxouvbwn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yueranfly.top/gtwpvswmye.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zdqjudy.top/gtarzylpvx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.tanke756.top/gtmrumcqgc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.xingfuxueyuan.xyz/gtzacnsyyv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.andypj.xyz/gteewdsiih.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jinghuilouyu.cn/gtkgxrjtjp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.feifeiyinyue.top/gtjkyfkrnq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.cqqwz.cn/gtpeoxpbku.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.pycfn.com/gttezguygl.html

Py:   pickle.dumps(obj)
来源：http://hz.hnqzz.top/gtvaascaom.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yuxming.cn/gtyzojgcwz.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.feifeiyinyue.top/gtvyijghnb.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.kuanghao11.cn/gtisyubvwz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.sweek.top/gtccsgvtbw.html

Go:   encoding/gob
来源：http://hz.chenlongwang.top/gtkapjuikn.html

Ruby: Marshal.dump(obj)
来源：http://hz.52xcode.cn/gtubvtuepn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jinqigufen.top/gtuoljfnog.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtkswufrhx.html

L. 网络请求
来源：http://hz.cdnleiting.top/gtywoyvxfv.html

================================================================================
来源：http://hz.haohaochexian.top/gtjcvarcca.html

[L01] 发送 GET 请求
来源：http://hz.wangshuangyany.cn/gtjvxoyixq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cucudq.cn/gtjkormbkd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.316326.xyz/gtwskmkwhu.html

JS:   await fetch(url)
来源：http://hz.yj202588.top/gtrwvblfix.html

TS:   await fetch(url)
来源：http://hz.zhengqikj.top/gtyoqmhvcp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhijiandao.cn/gttikifucs.html

Go:   resp, err := http.Get(url)
来源：http://hz.chenzaomai.com/gtrynhpnjx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.chenzaomai.com/gtfcphoaag.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yongpay.top/gtcuxfkcgl.html

[L02] 发送 POST JSON
来源：http://hz.haohaochexian.top/gtjoshgxmy.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhaomingkeji.xyz/gtfgqosmid.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zycfv.cn/gtlbyeuikl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhaomingkeji.xyz/gtsjstpmja.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shzxlz.cn/gtwegiljdd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhixingplan.top/gtluwtwspz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hfpthk.cn/gtahzchowt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.fzhhl.top/gtylvkyeia.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.bjfxy.top/gtzaodcoik.html

[L03] 设置自定义请求头
来源：http://hz.zhiwuduotai.top/gtgergaiby.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.iojbl.cn/gtgavaakdg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.aizwys.cn/gtsyhjqexf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.guannengcc.top/gtmbpikpwk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhaomingkeji.xyz/gthjhjalub.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.cucudq.cn/gtmpoezukt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jinqigufen.top/gteqomiioq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hammf.cn/gtjorvtiyh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yvedp.cn/gtqroiibiw.html

[L04] 设置超时
来源：http://hz.jinqigfzy.top/gttsqqjnsj.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cdnleiting.top/gtlezqwsrf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yuxming.cn/gtgrhcjvpy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yuanzhike.top/gtfqpqendz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.chenlongwang.top/gtxejofhbp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ivvv.top/gtawifltfj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.quarkkingdee.top/gtstinzoyr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.snrcjt.cn/gtdhnhwjut.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ppjwa.cn/gtjygafilk.html

[L05] 上传文件（multipart）
来源：http://hz.jlsjyb.cn/gtrachxaja.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.wangshuangyany.cn/gtwwuflidw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.tianlin.xyz/gtxchuvwfe.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.shuidangran.top/gtvrwxjbnf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.quarkkingdee.top/gtzngffcdv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.c1oappe.top/gtvcexxgqc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.tanke756.top/gtauuympsw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shangyingyoupin.top/gtqsshodwf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yonumen.top/gtsaadahnc.html

[L06] 解析响应为 JSON
来源：http://hz.feifeiyinyue.top/gtnyjaeima.html

Py:   resp.json()
来源：http://hz.guannengcc.top/gtjlzoeaxb.html

PHP:  json_decode($body, true);
来源：http://hz.yangfankeji.com/gtiixkuaie.html

JS:   await resp.json()
来源：http://hz.cashguo.top/gtijscdirs.html

TS:   await resp.json()
来源：http://hz.chenzaomai.com/gtfnihuvpf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.sxryk.cn/gtlogwantg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.feifeiyinyue.top/gtxlydozdz.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ppjwa.cn/gtrjnunqww.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.daria6918.cn/gtqxrfkmou.html

[L07] 处理 HTTP 状态码
来源：http://hz.mhx1999.top/gtrszeykmy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.cdnleiting.top/gthpnoaxfo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.andypj.xyz/gtikpfselz.html

JS:   resp.ok;  resp.status
来源：http://hz.redwolf501.top/gtmezwtdoo.html

TS:   resp.ok;  resp.status
来源：http://hz.dianchejie.cn/gtpaaasgtt.html

Java: resp.statusCode()
来源：http://hz.birdmap.top/gtqwpvqybe.html

Go:   resp.StatusCode
来源：http://hz.meibo888.top/gtastdgnmh.html

Ruby: resp.code.to_i
来源：http://hz.yj20258888.top/gtgwoceifp.html

C#:   (int)resp.StatusCode
来源：http://hz.ydzc1.top/gtlrhawzhg.html

[L08] 并发请求多个地址
来源：http://hz.xziqi.cn/gtdfgxpldp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jlsjyb.cn/gtskypfpoj.html

PHP:  curl_multi_init() 系列
来源：http://hz.ydzc1.top/gtkatvxeek.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yangfankeji.com/gtfppsnopc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gogol.net.cn/gtmholdyay.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.chenjidiqi.icu/gtoiwhsfur.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xylfe.cn/gtklhyneqw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.dianchejie.cn/gtgpacxuct.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhongyouzk.top/gtjxpzasgv.html

================================================================================
来源：http://hz.hnxiangtu.top/gtlzhugdaz.html

M. 命令行 / 进程 / 环境
来源：http://hz.wangdashe.top/gtbclxlsgd.html

================================================================================
来源：http://hz.aizwys.cn/gtyyqwvslw.html

[M01] 读取命令行参数
来源：http://hz.guannengcc.top/gttiieupgp.html

Py:   sys.argv[1:]
来源：http://hz.zdqjudy.top/gtpmsbgknv.html

PHP:  $argv;  $argc;
来源：http://hz.guowangkeji.top/gtfrllqqoh.html

JS:   process.argv.slice(2)
来源：http://hz.yuxming.cn/gtqrnaloco.html

TS:   process.argv.slice(2)
来源：http://hz.yangfankeji.com/gtwvyrelnk.html

Java: args 数组（main 方法参数）
来源：http://hz.zdqjudy.top/gtflqlwwcd.html

Go:   os.Args[1:]
来源：http://hz.ppjwa.cn/gtydszuabx.html

Ruby: ARGV
来源：http://hz.xingfuxueyuan.xyz/gtvovfiyhj.html

C#:   args 数组（Main 方法参数）
来源：http://hz.xuetiantiany.cn/gtpwvxryyj.html

[M02] 读取环境变量
来源：http://hz.ydzc1.top/gtsyvujjeb.html

Py:   os.environ.get("HOME")
来源：http://hz.yj202588.top/gtiftujnvy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jinghuilouyu.cn/gtyfjoebis.html

JS:   process.env.HOME
来源：http://hz.nanxinkj.top/gtncavgtsg.html

TS:   process.env.HOME
来源：http://hz.zhixingplan.top/gtredhyyjy.html

Java: System.getenv("HOME")
来源：http://hz.xziqi.cn/gtctszhzra.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jlsjyb.cn/gtvifpiarz.html

Ruby: ENV["HOME"]
来源：http://hz.ydjk.org.cn/gtkwsmvbye.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.smart0.xyz/gtuyigksdu.html

[M03] 执行外部命令
来源：http://hz.cdnleiting.top/gtxxvreyvx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.feifeiyinyue.top/gtbeelbdil.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hnqzz.top/gtxdwjdjil.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xuetiantiany.cn/gtvhfgccih.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.cdnleiting.top/gtvqdzqjxv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.havefunace.top/gttjvgkdlf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hysaishi.cn/gtxnbzvytc.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shuidangran.top/gtswxrezqw.html

C#:   Process.Start("ls", "-l");
来源：http://hz.shangyingyoupin.top/gtfprnydtc.html

[M04] 获取当前工作目录
来源：http://hz.0kj1m.cn/gtfnfkhvbt.html

Py:   os.getcwd()
来源：http://hz.sufxvd.cn/gtikfwosqm.html

PHP:  getcwd();
来源：http://hz.chenjidiqi.icu/gtgcytuark.html

JS:   process.cwd()
来源：http://hz.feifeiyinyue.top/gtwbqbcyrq.html

TS:   process.cwd()
来源：http://hz.316326.xyz/gtiurebtsn.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.chenzaomai.com/gtbmddzjqz.html

Go:   os.Getwd()
来源：http://hz.chenzaomai.com/gtnarpcmio.html

Ruby: Dir.pwd
来源：http://hz.chenzaomai.com/gtxtqfbqcm.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.0kj1m.cn/gtsgtfkxqs.html

[M05] 设置退出码
来源：http://hz.9152youxi.cn/gtcetgfwmn.html

Py:   sys.exit(1)
来源：http://hz.tanke756.top/gteegkjmim.html

PHP:  exit(1);
来源：http://hz.chenzaomai.com/gtadjjwwpo.html

JS:   process.exit(1)
来源：http://hz.zhaomingkeji.xyz/gtsvhqxpgq.html

TS:   process.exit(1)
来源：http://hz.yongpay.top/gtrligczto.html

Java: System.exit(1)
来源：http://hz.9152youxi.cn/gtbdmdmgau.html

Go:   os.Exit(1)
来源：http://hz.9152youxi.cn/gtkymtqwxt.html

Ruby: exit 1
来源：http://hz.shuidangran.top/gttttezejy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jinqigfzy.top/gtfgbmfblb.html

[M06] 向标准错误输出
来源：http://hz.yangfankeji.com/gtdwnmyimq.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ppjwa.cn/gtyuolgkff.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.shzxlz.cn/gtvktxzqop.html

JS:   console.error("err")
来源：http://hz.gogol.net.cn/gthokbdvbx.html

TS:   console.error("err")
来源：http://hz.meibo888.top/gthakncxew.html

Java: System.err.println("err")
来源：http://hz.gaohongyu789.top/gtytkijfmh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.hfpthk.cn/gtxgmhfcwm.html

Ruby: warn "err"
来源：http://hz.nwbrower.top/gtedhoqvgn.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.316326.xyz/gtoqbpdwqy.html

[M07] 判断是否为主入口
来源：http://hz.yj20258.top/gtgbakarvs.html

Py:   if __name__ == "__main__":
来源：http://hz.yuxming.cn/gtfbudwnct.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.hfpthk.cn/gtwyvvovup.html

JS:   require.main === module
来源：http://hz.zhongyouzk.top/gtszgkujkm.html

TS:   require.main === module
来源：http://hz.ywan-chungtsiang.top/gtuxcwccub.html

Java: public static void main(String[] args)
来源：http://hz.yuanzhike.top/gtensgsiph.html

Go:   func main()
来源：http://hz.sufxvd.cn/gtlnoennvt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cashguo.top/gtavrxfpps.html

C#:   static void Main(string[] args)
来源：http://hz.shangyingyoupin.top/gtgpsydtqx.html

[M08] 获取系统与运行时信息
来源：http://hz.zhijiandao.cn/gtgfbwrnkx.html

Py:   platform.system();  platform.python_version()
来源：http://hz.xinyue.icu/gtbihanazq.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.meibo888.top/gtitciwqvl.html

JS:   process.platform;  process.version
来源：http://hz.aibaodan.cn/gtyscjzfoc.html

TS:   process.platform;  process.version
来源：http://hz.daxiang520.top/gtmfxjedla.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hongshengwenyu.top/gtcaqvgtht.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.shzxlz.cn/gtvlazpykf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.chenjidiqi.icu/gtbeeghapq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.vqdsnc.cn/gtjmebufod.html

================================================================================
来源：http://hz.gzhubu.top/gtazssppyv.html

N. 数据结构与算法
来源：http://hz.gogol.net.cn/gtclaygztv.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtcklvefpv.html

[N01] 二分查找（有序数组）
来源：http://hz.birdmap.top/gtndqjuhvh.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hnqzz.top/gtekwyuyse.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.cqqwz.cn/gtycxbyekr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gaohongyu789.top/gtdnxebijg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.haohaochexian.top/gtzumghmvy.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.fzhhl.top/gtpejuahpj.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.dashuyun.cn/gtgcvdzcol.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.chenjidiqi.icu/gtynybmhyd.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.sufxvd.cn/gtoukedsrn.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.cqqwz.cn/gtaegswkif.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.quarkkingdee.top/gtihdlftbr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.cheryme.top/gttmllfoex.html


<!-- 参考信息 -->