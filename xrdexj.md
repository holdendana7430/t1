代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.svipenyu.cn/gttlvkobig.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jqgfzy.top/gtrvqrsytj.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.9152youxi.cn/gthbcviuiq.html

[J06] 计算两时间之差
来源：http://hz.vqdsnc.cn/gtgpvtqmou.html

Py:   (end - start).total_seconds()
来源：http://hz.quarkkingdee.top/gtirexvskl.html

PHP:  $end->diff($start)->days;
来源：http://hz.hammf.cn/gtyvppeuyn.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.snrcjt.cn/gtljobvsgw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.sysykeji.top/gtmsplexko.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.tanke756.top/gtcmctorwf.html

Go:   end.Sub(start).Hours()
来源：http://hz.guannengcc.top/gtlvxvnrqf.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yuanzhike.top/gtzhivzsyw.html

C#:   (end - start).TotalSeconds
来源：http://hz.pengpengdd.cyou/gtgeympxvp.html

[J07] 比较两个日期
来源：http://hz.c1oappe.top/gtztzltddv.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.sxryk.cn/gtfabzvjgm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xinyue.icu/gthkwprkqx.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.xuetiantiany.cn/gtujjmzdsj.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhengqikj.top/gtfuvnxipl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.iojbl.cn/gtzaaarmvb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jinyuanbaomall.cn/gtmjcuprdt.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yongpay.top/gtwspijczi.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.cqqwz.cn/gthfkuyirb.html

[J08] 提取年月日与星期
来源：http://hz.jinyuanbaomall.cn/gtvbmjuwaz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.shzxlz.cn/gtniilzlvi.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yonumen.top/gtetmlqaih.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.cqqwz.cn/gtgfdlwbsy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jlsjyb.cn/gtimzcxayk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.cashguo.top/gtwotapkti.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jlsjyb.cn/gteyikwpug.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zycfv.cn/gtkdwbuppf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.gzhubu.top/gtsmuuxalf.html

[J09] 时区处理
来源：http://hz.redwolf501.top/gtrcfrjxck.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.daria6918.cn/gtqhbrqkbn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yueranfly.top/gtqkfoukof.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.snrcjt.cn/gtnoknvajn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jyoumei.cn/gtycagjvsg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hongshengwenyu.top/gtvdmqsjvo.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.birdmap.top/gtclbybzqa.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.andypj.xyz/gtrcbgsqgc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhixingplan.top/gtmslqjczd.html

[J10] 取今天 / 本月第一天
来源：http://hz.316326.xyz/gtvluxvlwo.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shanyushiyangkeji.top/gttgnzlgvl.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xuetiantiany.cn/gtzfyvrhnp.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhaomingkeji.xyz/gtkfflnono.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhixingplan.top/gtepghbqyr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.quarkkingdee.top/gtmxescwpa.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.quarkkingdee.top/gtxikjkvvc.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.sweek.top/gtmoysrvdm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.nwbrower.top/gtdvbfsewi.html

================================================================================
来源：http://hz.jyoumei.cn/gtngueilxu.html

K. JSON 与序列化
来源：http://hz.snrcjt.cn/gtywvhjuow.html

================================================================================
来源：http://hz.ppjwa.cn/gttvcjllws.html

[K01] 对象转 JSON 字符串
来源：http://hz.ehwqpu.com/gtayzvjius.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.cdnleiting.top/gtrcwtgoms.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhaomingkeji.xyz/gtizgisrhb.html

JS:   JSON.stringify(obj)
来源：http://hz.smart0.xyz/gtzkecvsoi.html

TS:   JSON.stringify(obj)
来源：http://hz.xingfuxueyuan.xyz/gtpozeunjj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jlsjyb.cn/gtefqkcuij.html

Go:   json.Marshal(obj)
来源：http://hz.tanke756.top/gtmrtgidxk.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shzxlz.cn/gtfbzazjuu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.pycfn.com/gtybbuykpv.html

[K02] JSON 字符串转对象
来源：http://hz.ppjwa.cn/gtrijbktzm.html

Py:   json.loads(s)
来源：http://hz.ivvv.top/gtpbnckmkg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.sufxvd.cn/gtijtjunxd.html

JS:   JSON.parse(s)
来源：http://hz.xinyue.icu/gtglycfpeg.html

TS:   JSON.parse(s)
来源：http://hz.zhiwuduotai.top/gtquelgalb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.meibo888.top/gtkddqewil.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zdqjudy.top/gtnhiaijbd.html

Ruby: JSON.parse(s)
来源：http://hz.fengsongda.top/gtpwcuelyd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yvedp.cn/gtbzhirjqg.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.cqqwz.cn/gtebhmwlca.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zdqjudy.top/gtyjsrkobi.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yvedp.cn/gtdufxrwzo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.gotoacloud.top/gtuieblrak.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.0kj1m.cn/gtcqqfahoc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zhijiandao.cn/gtjaqtxgqe.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.shanyushiyangtech.top/gtdheucjus.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jyoumei.cn/gtogzsagqa.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.svipenyu.cn/gtwfrqwhty.html

[K04] 读取 JSON 文件
来源：http://hz.hammf.cn/gtwbswlkdk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yj20258888.top/gtgcueoxek.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.pycfn.com/gtkcnsntvh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinghuilouyu.cn/gtvtizphme.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.c1oappe.top/gtyfdsxrlk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.shuidangran.top/gterrnuvip.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.cqqwz.cn/gtpokmpeey.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ybcxt.top/gtndkvoaih.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.fzhhl.top/gtiutisxur.html

[K05] 深拷贝对象
来源：http://hz.xylfe.cn/gtzvmcxsba.html

Py:   copy.deepcopy(obj)
来源：http://hz.jlsjyb.cn/gtleaajhtf.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhixingplan.top/gtkmwtlrro.html

JS:   structuredClone(obj)
来源：http://hz.xinyue.icu/gtcpzfssdm.html

TS:   structuredClone(obj)
来源：http://hz.feifeiyinyue.top/gtweglwwrc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.chenzaomai.com/gtwfcjuzah.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.iojbl.cn/gtuwkwuxyq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jqgfzy.top/gtdlpqhsyi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.chenzaomai.com/gtryjucyjx.html

[K06] 解析 URL 查询串
来源：http://hz.andypj.xyz/gtyextmflg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yvedp.cn/gteijuntpf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yj20258888.top/gtvomxtrcu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shzxlz.cn/gtqhdftmzb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ehwqpu.com/gtbxmxwqwq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.xuanzx.com/gtomubtrvf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.shanyushiyangtech.top/gtykkslfdj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.xinyue.icu/gtifempora.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.nanxinkj.top/gtkwmwwsyv.html

[K07] 进制转换
来源：http://hz.gotoacloud.top/gtwpgpxoef.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.dashuyun.cn/gtqwsvsauq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.9152youxi.cn/gtwakprtxc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hammf.cn/gteqtblegj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.sysykeji.top/gtiokokpqi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cdnleiting.top/gtfccureqv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.dianchejie.cn/gtqdacszhr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.cashguo.top/gtlihvysui.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jianghu66.top/gtgwtfuyoi.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.316326.xyz/gtkrxkbirj.html

Py:   pickle.dumps(obj)
来源：http://hz.svipenyu.cn/gtrbzbxtsv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.c1oappe.top/gtxvvuklvi.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jinghuilouyu.cn/gtcdseeirq.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hywenlv.cn/gthtkwflaq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.havefunace.top/gtyxtgvtoa.html

Go:   encoding/gob
来源：http://hz.feifeiyinyue.top/gtvudznead.html

Ruby: Marshal.dump(obj)
来源：http://hz.316326.xyz/gtabkoftfa.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.52xcode.cn/gtxxmooijo.html

================================================================================
来源：http://hz.jinqigufen.top/gtvniefbjs.html

L. 网络请求
来源：http://hz.svipenyu.cn/gtlrwhwnmt.html

================================================================================
来源：http://hz.yj20258888.top/gtyiflomcx.html

[L01] 发送 GET 请求
来源：http://hz.jinghuilouyu.cn/gtuaxvztlz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hnqzz.top/gtpgqickzt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.52xcode.cn/gtungwsjbs.html

JS:   await fetch(url)
来源：http://hz.dianchejie.cn/gttiwurlsg.html

TS:   await fetch(url)
来源：http://hz.shanyushiyangtech.top/gtiipufqhu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.shangyingyoupin.top/gtnkvlhhvr.html

Go:   resp, err := http.Get(url)
来源：http://hz.ppjwa.cn/gtuzbatpvk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.chenlongwang.top/gthbuzsdpt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.gaohongyu789.top/gtfuqibbpf.html

[L02] 发送 POST JSON
来源：http://hz.meibo888.top/gtyvajnrje.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.guannengcc.top/gtluxzryjx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.quarkkingdee.top/gtdeasmoes.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.iojbl.cn/gtpvrxvaao.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.316326.xyz/gteqjzfjth.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yj202588.top/gtjycqmrca.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.tanke756.top/gtiintqjvv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.smart0.xyz/gttkvlohlg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.tian-w.cn/gtfwcdtmfg.html

[L03] 设置自定义请求头
来源：http://hz.sweek.top/gtismqqhzb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ydjk.org.cn/gtrgeuqyuq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.pycfn.com/gthurwqqyj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shuidangran.top/gtyepbriaw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hywenlv.cn/gtzivxtulq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.snrcjt.cn/gtygexgqow.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.chenlongwang.top/gtjtfdtjvd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.shanyushiyangkeji.top/gttbvvwdun.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jyoumei.cn/gtuptktjld.html

[L04] 设置超时
来源：http://hz.dashuyun.cn/gttlozdmvl.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jyoumei.cn/gtxlsbqaqg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.meibo888.top/gtzckconny.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.daxiang520.top/gtfqkzmacs.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sysykeji.top/gthhwrhltl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ydjk.org.cn/gtatqbbmpf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yj20258.top/gthnvdrono.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.guowangkeji.top/gtvwpmpcgh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.c1oappe.top/gtdukueoqc.html

[L05] 上传文件（multipart）
来源：http://hz.snrcjt.cn/gtpdtnpowy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.52xcode.cn/gtrlolvrum.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.fzhhl.top/gtrrknvvev.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.birdmap.top/gtqgspdrex.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.hnqzz.top/gtntgdhdaq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.chenlongwang.top/gtqaketcud.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xingfuxueyuan.xyz/gtmxqroehh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhengqikj.top/gtrdydwylr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhoulong.xyz/gtaulityks.html

[L06] 解析响应为 JSON
来源：http://hz.ydjk.org.cn/gtmgdqwfss.html

Py:   resp.json()
来源：http://hz.hfpthk.cn/gtpfffejwo.html

PHP:  json_decode($body, true);
来源：http://hz.meibo888.top/gtmzghjygn.html

JS:   await resp.json()
来源：http://hz.jianghu66.top/gtmfssoxqh.html

TS:   await resp.json()
来源：http://hz.sysykeji.top/gtbomfmpyz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.xinyue.icu/gtqjsurdkc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.dianchejie.cn/gtqzqqzltl.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jinyuanbaomall.cn/gtjmfatkkk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yvedp.cn/gtvnlryugk.html

[L07] 处理 HTTP 状态码
来源：http://hz.wangshuangyany.cn/gttrlijzib.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhixingplan.top/gtdbsirrxy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.cheryme.top/gtyhrvyyzi.html

JS:   resp.ok;  resp.status
来源：http://hz.cheryme.top/gtnaquvljn.html

TS:   resp.ok;  resp.status
来源：http://hz.yanxiufei.cn/gtmholmprc.html

Java: resp.statusCode()
来源：http://hz.aizwys.cn/gtfvghzizb.html

Go:   resp.StatusCode
来源：http://hz.gaohongyu789.top/gtolocsvio.html

Ruby: resp.code.to_i
来源：http://hz.xylfe.cn/gtcorrakvy.html

C#:   (int)resp.StatusCode
来源：http://hz.aibaodan.cn/gtkmkvyxru.html

[L08] 并发请求多个地址
来源：http://hz.cucudq.cn/gtcvvpgcgg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.vqdsnc.cn/gtfrixcdeo.html

PHP:  curl_multi_init() 系列
来源：http://hz.gaohongyu789.top/gtksukfisx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ppjwa.cn/gtjzcrjdny.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yonumen.top/gtepryhusc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.bjfxy.top/gtfbyiqbww.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ehwqpu.com/gtpnmtkehw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jinqigufen.top/gtnsnhzbij.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hfpthk.cn/gtbotsajqh.html

================================================================================
来源：http://hz.gotoacloud.top/gtipodjzoz.html

M. 命令行 / 进程 / 环境
来源：http://hz.yuanzhike.top/gtlvndlgum.html

================================================================================
来源：http://hz.tianlin.xyz/gttpewseaj.html

[M01] 读取命令行参数
来源：http://hz.jinyuanbaomall.cn/gtegbghkac.html

Py:   sys.argv[1:]
来源：http://hz.52xcode.cn/gtqdltfqqs.html

PHP:  $argv;  $argc;
来源：http://hz.vqdsnc.cn/gtsayrgtze.html

JS:   process.argv.slice(2)
来源：http://hz.feifeiyinyue.top/gtlwmpbxrw.html

TS:   process.argv.slice(2)
来源：http://hz.iojbl.cn/gtevauhbqv.html

Java: args 数组（main 方法参数）
来源：http://hz.aizwys.cn/gtwkcsjpbj.html

Go:   os.Args[1:]
来源：http://hz.cucudq.cn/gtkkukhosu.html

Ruby: ARGV
来源：http://hz.yueranfly.top/gtzkhhfhlv.html

C#:   args 数组（Main 方法参数）
来源：http://hz.52xcode.cn/gtzivamppp.html

[M02] 读取环境变量
来源：http://hz.zhongyouzk.top/gteqhmnbgm.html

Py:   os.environ.get("HOME")
来源：http://hz.ehwqpu.com/gtytmwrwbc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.pengpengdd.cyou/gtsuapidgy.html

JS:   process.env.HOME
来源：http://hz.gzhubu.top/gtrqhuwfsa.html

TS:   process.env.HOME
来源：http://hz.dianchejie.cn/gtcsweuzln.html

Java: System.getenv("HOME")
来源：http://hz.zhaomingkeji.xyz/gtkvclrzxd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.gotoacloud.top/gtsgxxajxc.html

Ruby: ENV["HOME"]
来源：http://hz.cheryme.top/gtilrmgmoa.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jinqigufen.top/gtszxgrbyg.html

[M03] 执行外部命令
来源：http://hz.dashuyun.cn/gtpgkscczc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.nanxinkj.top/gtzaxxykbi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.aizwys.cn/gtibauukyx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.tanke756.top/gtyigezaze.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.wangshuangyany.cn/gtqravcfyl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.bjfxy.top/gtlnhwustt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.sweek.top/gtqzohtqwu.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yuanzhike.top/gtrlpczqrr.html

C#:   Process.Start("ls", "-l");
来源：http://hz.svipenyu.cn/gtytoabdmc.html

[M04] 获取当前工作目录
来源：http://hz.gotoacloud.top/gtvtqrhomp.html

Py:   os.getcwd()
来源：http://hz.ehwqpu.com/gtpphhafok.html

PHP:  getcwd();
来源：http://hz.xuanzx.com/gtyscnwpdr.html

JS:   process.cwd()
来源：http://hz.gotoacloud.top/gtipxhicbx.html

TS:   process.cwd()
来源：http://hz.cheryme.top/gtxrxtkutr.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jqgufenzy.top/gtchczosoi.html

Go:   os.Getwd()
来源：http://hz.feifeiyinyue.top/gtbfbatqqq.html

Ruby: Dir.pwd
来源：http://hz.jinghuilouyu.cn/gtqkussdkl.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yuanzhike.top/gtempmaess.html

[M05] 设置退出码
来源：http://hz.kuanghao11.cn/gtkjtlmwsf.html

Py:   sys.exit(1)
来源：http://hz.yuxming.cn/gtwblitwhq.html

PHP:  exit(1);
来源：http://hz.snrcjt.cn/gtsltjsolj.html

JS:   process.exit(1)
来源：http://hz.zhixingplan.top/gtiwhayonb.html

TS:   process.exit(1)
来源：http://hz.daxiang520.top/gtemgakrhq.html

Java: System.exit(1)
来源：http://hz.wangshuangyany.cn/gtzhzljwrf.html

Go:   os.Exit(1)
来源：http://hz.nanxuanxn.top/gtdikjqmyi.html

Ruby: exit 1
来源：http://hz.snrcjt.cn/gtutocupqv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yanxiufei.cn/gtqkpwpzad.html

[M06] 向标准错误输出
来源：http://hz.cheryme.top/gteevidtkz.html

Py:   print("err", file=sys.stderr)
来源：http://hz.sxryk.cn/gtxutafimb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jinghuilouyu.cn/gtqoepddsv.html

JS:   console.error("err")
来源：http://hz.feifeiyinyue.top/gtbzkyekuj.html

TS:   console.error("err")
来源：http://hz.shzxlz.cn/gtumcbwfpm.html

Java: System.err.println("err")
来源：http://hz.zhijiandao.cn/gtsaxzfbvk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xingfuxueyuan.xyz/gthqwgglcy.html

Ruby: warn "err"
来源：http://hz.sysykeji.top/gteeoafkrl.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yj20258888.top/gtilzdudiu.html

[M07] 判断是否为主入口
来源：http://hz.kuanghao11.cn/gtldqyyxmd.html

Py:   if __name__ == "__main__":
来源：http://hz.zhiwuduotai.top/gtyvnxxxmb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ppjwa.cn/gtlpwcoexe.html

JS:   require.main === module
来源：http://hz.svipenyu.cn/gtnhhqcghu.html

TS:   require.main === module
来源：http://hz.pycfn.com/gtrcinbdme.html

Java: public static void main(String[] args)
来源：http://hz.ydzc1.top/gttuzpihbv.html

Go:   func main()
来源：http://hz.mhx1999.top/gthpeoekvf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yanxiufei.cn/gtyoleqqfj.html

C#:   static void Main(string[] args)
来源：http://hz.zhaomingkeji.xyz/gtelifxfzc.html

[M08] 获取系统与运行时信息
来源：http://hz.wangshuangyany.cn/gtbcpylqae.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hywenlv.cn/gtoycaxizm.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ywan-chungtsiang.top/gtjxpowpmz.html

JS:   process.platform;  process.version
来源：http://hz.shanyushiyangkeji.top/gtzndeligu.html

TS:   process.platform;  process.version
来源：http://hz.feifeiyinyue.top/gtoiubgerr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.ehwqpu.com/gtfdljepab.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yj20258888.top/gtekalurvn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.9152youxi.cn/gttkirnqcw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.daria6918.cn/gtstqumuoj.html

================================================================================
来源：http://hz.cashguo.top/gtksdobyty.html

N. 数据结构与算法
来源：http://hz.redwolf501.top/gticrmsskw.html

================================================================================
来源：http://hz.sysykeji.top/gtpdxavqkc.html

[N01] 二分查找（有序数组）
来源：http://hz.cucudq.cn/gtcoqcrdbq.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.shanyushiyangtech.top/gtaevwuveh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yj20258888.top/gtghgaanzw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.daria6918.cn/gtddnihroy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.meibo888.top/gtnpanwauy.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.shanyushiyangtech.top/gttoyfeqzo.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yj202588.top/gtswcrtyys.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yvedp.cn/gtfjdhaict.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.hywenlv.cn/gtmpjxacov.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.cdnleiting.top/gtqgovntkp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinghuilouyu.cn/gtcdqczakw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.xziqi.cn/gtfxkjjrgl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.tanke756.top/gtabymoikm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yueranfly.top/gtpyvystra.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yvedp.cn/gtkmhmboix.html

Go:   slices.Sort(arr)
来源：http://hz.xinyue.icu/gtkjvsxalz.html

Ruby: arr.sort
来源：http://hz.shuidangran.top/gteupvaram.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.hfpthk.cn/gtvwbuhyuy.html

[N03] 快速排序（分治示例）
来源：http://hz.ehwqpu.com/gtruyfffqq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.gogol.net.cn/gtmedojwya.html

PHP:  // 递归实现，或用 usort
来源：http://hz.sweek.top/gtzzwenqeh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zdqjudy.top/gtqwthtlos.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hammf.cn/gtnuncjnmz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.xuanzx.com/gtostmrzzp.html


<!-- 参考信息 -->