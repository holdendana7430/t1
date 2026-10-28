代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.chenzaomai.com/gtmzyuvvmw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.gotoacloud.top/gtgezxlxkx.html

[J05] 时间加减（加 7 天）
来源：http://hz.dianchejie.cn/gtkibszhvy.html

Py:   now + timedelta(days=7)
来源：http://hz.jqgfzy.top/gtpwbndtlv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.mhx1999.top/gtwirfpxcq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jyoumei.cn/gtxiddrdif.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cheryme.top/gtfydomslj.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhiwuduotai.top/gtmfrhelqk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhixingplan.top/gtkrstjepn.html

Ruby: Time.now + 7 * 86400
来源：http://hz.meibo888.top/gtzxerhjdn.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cucudq.cn/gtbhlzlsqc.html

[J06] 计算两时间之差
来源：http://hz.snrcjt.cn/gtkxbizpnj.html

Py:   (end - start).total_seconds()
来源：http://hz.jqgufenzy.top/gtuhbynbmw.html

PHP:  $end->diff($start)->days;
来源：http://hz.jyoumei.cn/gtrldcibpa.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.dianchejie.cn/gtkbjcosxk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.aizwys.cn/gtpdklribl.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.sxryk.cn/gtjkdzirjl.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhoulong.xyz/gthoodcltf.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hnxiangtu.top/gtsunlstek.html

C#:   (end - start).TotalSeconds
来源：http://hz.hnxiangtu.top/gthmaxgvis.html

[J07] 比较两个日期
来源：http://hz.jinqigfzy.top/gtlnxhfiao.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.cdnleiting.top/gtjcllcaiy.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.vqdsnc.cn/gtbdtponpb.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.andypj.xyz/gtzzgzdqag.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xinyue.icu/gtkkorcjul.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.gaohongyu789.top/gtpnulxwtr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.kuanghao11.cn/gtwdrkacjc.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.gaohongyu789.top/gttvvuhrey.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhoulong.xyz/gtevogozss.html

[J08] 提取年月日与星期
来源：http://hz.hywenlv.cn/gtlglqyubq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.gzhubu.top/gtdgdqqbgm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jyoumei.cn/gtptlcjyqx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.aibaodan.cn/gtmghjilan.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.xylfe.cn/gtigjjiqxv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yonumen.top/gteyskozft.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.daxiang520.top/gtksyzszrl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cucudq.cn/gtawfwgnlf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yongpay.top/gtiavcillr.html

[J09] 时区处理
来源：http://hz.shanyushiyangtech.top/gtxncegkur.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hfpthk.cn/gtymmblftc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.cheryme.top/gtrawpyvld.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.9152youxi.cn/gtrdgxpvik.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yangfankeji.com/gtrqkfeiba.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hnxiangtu.top/gtbrzdzhtn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ivvv.top/gtadnhjrni.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yanxiufei.cn/gtvpmwutgo.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yongpay.top/gtjxcgkvze.html

[J10] 取今天 / 本月第一天
来源：http://hz.jianghu66.top/gtoikeemzh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhaomingkeji.xyz/gtvqtryxay.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zdqjudy.top/gtthxpirlk.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hywenlv.cn/gtjuzqyweb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.0kj1m.cn/gtqkfzvigx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.snrcjt.cn/gtihhpcmvd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ydzc1.top/gthswsruea.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.chenzaomai.com/gtjsqtiarg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.dianchejie.cn/gticjwybnn.html

================================================================================
来源：http://hz.zhixingplan.top/gtyrnffezq.html

K. JSON 与序列化
来源：http://hz.ywan-chungtsiang.top/gtzjpkogeb.html

================================================================================
来源：http://hz.tian-w.cn/gtjbmlbxly.html

[K01] 对象转 JSON 字符串
来源：http://hz.bjfxy.top/gtszkwqvko.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yangfankeji.com/gtrmpxraqd.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yvedp.cn/gtyxcfiarw.html

JS:   JSON.stringify(obj)
来源：http://hz.yongpay.top/gtlctbtyjy.html

TS:   JSON.stringify(obj)
来源：http://hz.316326.xyz/gtfvpfdnth.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jlsjyb.cn/gtxcuftzou.html

Go:   json.Marshal(obj)
来源：http://hz.gotoacloud.top/gtilycuqgn.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.vqdsnc.cn/gtttqaagqu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hfpthk.cn/gtknijdnbi.html

[K02] JSON 字符串转对象
来源：http://hz.jinghuilouyu.cn/gtgzqhokbg.html

Py:   json.loads(s)
来源：http://hz.gaohongyu789.top/gtsvjaeabk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhijiandao.cn/gtabcbjgfj.html

JS:   JSON.parse(s)
来源：http://hz.nanxinkj.top/gtsopduygi.html

TS:   JSON.parse(s)
来源：http://hz.yuxming.cn/gtgwuiyfyd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhongyouzk.top/gtvbdmfyit.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.52xcode.cn/gtsdxubvtl.html

Ruby: JSON.parse(s)
来源：http://hz.haohaochexian.top/gtcuwiftou.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.shanyushiyangtech.top/gtysvzfhtd.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.cheryme.top/gtyhbpjmzk.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.snrcjt.cn/gtkeaeafuv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jianghu66.top/gtpeqdrovt.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.wangdashe.top/gtnrkzdusw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinyuanbaomall.cn/gtikicoybd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.0kj1m.cn/gtifhunhep.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yanxiufei.cn/gtznhgtxcn.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.cashguo.top/gtzhlhulda.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhixingplan.top/gtlhpsspxb.html

[K04] 读取 JSON 文件
来源：http://hz.ivvv.top/gtladexdmf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xylfe.cn/gtdcpltzgl.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.nwbrower.top/gtrrehymqi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.fengsongda.top/gtvynityue.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.nanxuanxn.top/gtkutivrfy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zdqjudy.top/gtllvlykwi.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jqgufenzy.top/gtqynhmxuh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.pengpengdd.cyou/gtxahowqjz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yanxiufei.cn/gtexdelhsk.html

[K05] 深拷贝对象
来源：http://hz.sysykeji.top/gtthnbzivj.html

Py:   copy.deepcopy(obj)
来源：http://hz.sweek.top/gtffhobwsk.html

PHP:  unserialize(serialize($obj));
来源：http://hz.guowangkeji.top/gtshhposhl.html

JS:   structuredClone(obj)
来源：http://hz.shanyushiyangkeji.top/gtgmzqlula.html

TS:   structuredClone(obj)
来源：http://hz.hongshengwenyu.top/gtmsmjdjlk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.cqqwz.cn/gtfnhzjmsk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.fengsongda.top/gtutcrsaod.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.bjfxy.top/gtkxhvwwid.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.birdmap.top/gtwczuhuyf.html

[K06] 解析 URL 查询串
来源：http://hz.shuidangran.top/gtubwlglxu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhaomingkeji.xyz/gthoeqnpfr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.chenlongwang.top/gtjejewjnv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zdqjudy.top/gtldintlsm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yuanzhike.top/gtfrxytwax.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hnxiangtu.top/gttzrqufbb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.fengsongda.top/gtgbsmgmyq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.guowangkeji.top/gtdoktsiom.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yuanzhike.top/gtkbdzypyh.html

[K07] 进制转换
来源：http://hz.hfpthk.cn/gtlxhdvbhn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ywan-chungtsiang.top/gtpkvmqnnz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.wangdashe.top/gthygcurrc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xylfe.cn/gtbiumhblr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.daria6918.cn/gthzldehft.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.gotoacloud.top/gtuoecsojc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xuetiantiany.cn/gtozjjopzz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jinghuilouyu.cn/gtsbbrloij.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.chenjidiqi.icu/gtkzdpkzbo.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.shangyingyoupin.top/gtljqoohex.html

Py:   pickle.dumps(obj)
来源：http://hz.zhiwuduotai.top/gtraduqxno.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.cdnleiting.top/gtrvxkduyh.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jqgfzy.top/gtzcjslrkr.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.daxiang520.top/gtbukgbriy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.xylfe.cn/gtfujrlzng.html

Go:   encoding/gob
来源：http://hz.cashguo.top/gtazdildvw.html

Ruby: Marshal.dump(obj)
来源：http://hz.yonumen.top/gtyogsrxxb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.hammf.cn/gtmmycvrxg.html

================================================================================
来源：http://hz.snrcjt.cn/gtfuxsnymn.html

L. 网络请求
来源：http://hz.yvedp.cn/gtgiwuetrm.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtnndvtpop.html

[L01] 发送 GET 请求
来源：http://hz.chenzaomai.com/gtnwljogax.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yueranfly.top/gtptsptxui.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.sysykeji.top/gtgptzxclv.html

JS:   await fetch(url)
来源：http://hz.smart0.xyz/gtjqvamshf.html

TS:   await fetch(url)
来源：http://hz.jyoumei.cn/gtiiupzzgs.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ywan-chungtsiang.top/gtdmjwwfpb.html

Go:   resp, err := http.Get(url)
来源：http://hz.cucudq.cn/gtuzghzyji.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.sweek.top/gtpiwzzcfk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.cheryme.top/gtwtkdwicq.html

[L02] 发送 POST JSON
来源：http://hz.guowangkeji.top/gteqkiwbcj.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.gaohongyu789.top/gtujkvkscb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yueranfly.top/gtcxrnvnyw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.nwbrower.top/gtqlazewvj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ehwqpu.com/gthwvdhpyu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.havefunace.top/gtgqsyvdvo.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.gzhubu.top/gtzkhpzjkx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.fzhhl.top/gtahkyrfge.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.quarkkingdee.top/gtjasjrrrd.html

[L03] 设置自定义请求头
来源：http://hz.zhengqikj.top/gtlbvoxgab.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jinqigfzy.top/gtxltflnpu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jyoumei.cn/gtrzetcjxm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.andypj.xyz/gtmfunisbm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.daria6918.cn/gtnbnxuaip.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.cucudq.cn/gtfasddule.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.nanxuanxn.top/gtonqmcjla.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.wangdashe.top/gtlgpafvfm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yj202588.top/gtdtqivdwf.html

[L04] 设置超时
来源：http://hz.dashuyun.cn/gtuljnlmrs.html

Py:   requests.get(url, timeout=5)
来源：http://hz.aibaodan.cn/gthdykdthb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.nanxinkj.top/gtwuzufkma.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shzxlz.cn/gtkfktgwil.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shzxlz.cn/gtmtdlyozg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.quarkkingdee.top/gtcoqjqvln.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.aizwys.cn/gtlapdenpt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.c1oappe.top/gtixebchqa.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xuanzx.com/gtzbzbhrme.html

[L05] 上传文件（multipart）
来源：http://hz.quarkkingdee.top/gtykjzkrxx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yj20258888.top/gtqwawzntm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xinyue.icu/gtrosdvsao.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.andypj.xyz/gtttvhlaze.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.sufxvd.cn/gtpvqzdlmi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hnqzz.top/gtiilfrsdt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.snrcjt.cn/gtjfwspkbq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.hongshengwenyu.top/gtpbjxeeqf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.aizwys.cn/gtokidiokn.html

[L06] 解析响应为 JSON
来源：http://hz.hywenlv.cn/gtwqopavyd.html

Py:   resp.json()
来源：http://hz.yj20258.top/gthhyqdzuk.html

PHP:  json_decode($body, true);
来源：http://hz.hammf.cn/gtqrrwdgdz.html

JS:   await resp.json()
来源：http://hz.zhoulong.xyz/gtyptwwbuy.html

TS:   await resp.json()
来源：http://hz.sysykeji.top/gtgvgtopvo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.shangyingyoupin.top/gtdlyubsvn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.ydzc1.top/gtavzlxrfr.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yueranfly.top/gtvcymstus.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ehwqpu.com/gttasvuuyh.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhiwuduotai.top/gtsbuiorwd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.haohaochexian.top/gttwvawpcf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ydzc1.top/gtekosdxol.html

JS:   resp.ok;  resp.status
来源：http://hz.jiagoushi.top/gtlwdrweys.html

TS:   resp.ok;  resp.status
来源：http://hz.pycfn.com/gteiacgcol.html

Java: resp.statusCode()
来源：http://hz.yj20258.top/gtmgcqarqz.html

Go:   resp.StatusCode
来源：http://hz.zhaomingkeji.xyz/gtxcpmqexv.html

Ruby: resp.code.to_i
来源：http://hz.shangyingyoupin.top/gtdosppfdl.html

C#:   (int)resp.StatusCode
来源：http://hz.tanke756.top/gthnzitshl.html

[L08] 并发请求多个地址
来源：http://hz.c1oappe.top/gtlsfkadiw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ppjwa.cn/gtiosungni.html

PHP:  curl_multi_init() 系列
来源：http://hz.jianghu66.top/gtfxvcrjed.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhaomingkeji.xyz/gtpbvflalb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.316326.xyz/gteeuykcgg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.0kj1m.cn/gtthfnzque.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hongshengwenyu.top/gtfzubtwik.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ydjk.org.cn/gtplsthamv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yj20258888.top/gtkrxuebin.html

================================================================================
来源：http://hz.daria6918.cn/gtnciupumh.html

M. 命令行 / 进程 / 环境
来源：http://hz.pycfn.com/gtudzfupcj.html

================================================================================
来源：http://hz.pycfn.com/gthnrlnvap.html

[M01] 读取命令行参数
来源：http://hz.jinyuanbaomall.cn/gtxlnqntng.html

Py:   sys.argv[1:]
来源：http://hz.jyoumei.cn/gtpfjaaawb.html

PHP:  $argv;  $argc;
来源：http://hz.zhijiandao.cn/gtdrkiekqr.html

JS:   process.argv.slice(2)
来源：http://hz.pengpengdd.cyou/gtyeezobmm.html

TS:   process.argv.slice(2)
来源：http://hz.xuanzx.com/gtpqaibxbu.html

Java: args 数组（main 方法参数）
来源：http://hz.shangyingyoupin.top/gtlkwevkkq.html

Go:   os.Args[1:]
来源：http://hz.ybcxt.top/gtsieblujw.html

Ruby: ARGV
来源：http://hz.mhx1999.top/gtlstznhvy.html

C#:   args 数组（Main 方法参数）
来源：http://hz.chenlongwang.top/gtczuofhgz.html

[M02] 读取环境变量
来源：http://hz.xingfuxueyuan.xyz/gtuxaqkxub.html

Py:   os.environ.get("HOME")
来源：http://hz.wangshuangyany.cn/gtospzpuct.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zdqjudy.top/gtdruxdjnd.html

JS:   process.env.HOME
来源：http://hz.0kj1m.cn/gtnzzhdxnn.html

TS:   process.env.HOME
来源：http://hz.cdnleiting.top/gtlozyggak.html

Java: System.getenv("HOME")
来源：http://hz.tanke756.top/gtghhoqmfb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yongpay.top/gtoylhgdoq.html

Ruby: ENV["HOME"]
来源：http://hz.hysaishi.cn/gtbxbtezeo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shzxlz.cn/gtzqghjtrj.html

[M03] 执行外部命令
来源：http://hz.fengsongda.top/gtntsihlic.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.quarkkingdee.top/gtxlbzurvj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.shzxlz.cn/gtnjggpllo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yj202588.top/gtzblvmmwc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hfpthk.cn/gtmlsismjf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.havefunace.top/gtuhanipjo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhaomingkeji.xyz/gtkcjaqpns.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.redwolf501.top/gtdmeodato.html

C#:   Process.Start("ls", "-l");
来源：http://hz.cdnleiting.top/gtcplaupun.html

[M04] 获取当前工作目录
来源：http://hz.fengsongda.top/gtyagcvtzr.html

Py:   os.getcwd()
来源：http://hz.jinqigufen.top/gtuojolblx.html

PHP:  getcwd();
来源：http://hz.yvedp.cn/gtzzeqaahi.html

JS:   process.cwd()
来源：http://hz.sxryk.cn/gtnkpnocwu.html

TS:   process.cwd()
来源：http://hz.birdmap.top/gtivjujzvn.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.redwolf501.top/gtpzmryqjl.html

Go:   os.Getwd()
来源：http://hz.hammf.cn/gtarqvjusy.html

Ruby: Dir.pwd
来源：http://hz.zhaomingkeji.xyz/gtqtowpfvz.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.daxiang520.top/gtgqabrwdg.html

[M05] 设置退出码
来源：http://hz.xuanzx.com/gtbnzchsjf.html

Py:   sys.exit(1)
来源：http://hz.shzxlz.cn/gtaegksmbf.html

PHP:  exit(1);
来源：http://hz.zhengqikj.top/gtswqxwmff.html

JS:   process.exit(1)
来源：http://hz.daxiang520.top/gtiqzwynvx.html

TS:   process.exit(1)
来源：http://hz.aibaodan.cn/gtnrypzzbs.html

Java: System.exit(1)
来源：http://hz.cheryme.top/gtpreydfak.html

Go:   os.Exit(1)
来源：http://hz.zycfv.cn/gtcbzgnmmt.html

Ruby: exit 1
来源：http://hz.hywenlv.cn/gtodnkjbnh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zhoulong.xyz/gtphnzgdgi.html

[M06] 向标准错误输出
来源：http://hz.havefunace.top/gtxbmpqkzh.html

Py:   print("err", file=sys.stderr)
来源：http://hz.birdmap.top/gtbwlgoxck.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.smart0.xyz/gtvoxgzpoe.html

JS:   console.error("err")
来源：http://hz.jqgfzy.top/gtfmujvyjp.html

TS:   console.error("err")
来源：http://hz.kuanghao11.cn/gtnlkpcixd.html

Java: System.err.println("err")
来源：http://hz.yvedp.cn/gtwcaxkhvo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xylfe.cn/gtdcqbhusp.html

Ruby: warn "err"
来源：http://hz.birdmap.top/gtbrhvofjw.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hammf.cn/gtbntolrax.html

[M07] 判断是否为主入口
来源：http://hz.hysaishi.cn/gtyhuuggpd.html

Py:   if __name__ == "__main__":
来源：http://hz.iojbl.cn/gtnkzueodu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xinyue.icu/gtgxkijssw.html

JS:   require.main === module
来源：http://hz.hnxiangtu.top/gtngjkmfxd.html

TS:   require.main === module
来源：http://hz.jinyuanbaomall.cn/gtnscnpptn.html

Java: public static void main(String[] args)
来源：http://hz.cdnleiting.top/gtgspdkxoj.html

Go:   func main()
来源：http://hz.hongshengwenyu.top/gtinolfrsg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yueranfly.top/gtswoylxdd.html

C#:   static void Main(string[] args)
来源：http://hz.iojbl.cn/gtkrkabzhz.html

[M08] 获取系统与运行时信息
来源：http://hz.mhx1999.top/gtbgoryyeg.html

Py:   platform.system();  platform.python_version()
来源：http://hz.chenzaomai.com/gtlbgtcdlz.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.cdnleiting.top/gtpzgpovxm.html

JS:   process.platform;  process.version
来源：http://hz.sxryk.cn/gtuljnazrn.html

TS:   process.platform;  process.version
来源：http://hz.smart0.xyz/gtxljmbymq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhongyouzk.top/gtinfrdvwo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.ybcxt.top/gtsdndbyrp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jqgufenzy.top/gtobihjzfi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.haohaochexian.top/gtkdoaxfgp.html

================================================================================
来源：http://hz.jinqigfzy.top/gtpmaxqhmq.html

N. 数据结构与算法
来源：http://hz.sufxvd.cn/gtzrdeawgr.html

================================================================================
来源：http://hz.redwolf501.top/gtwumbzdwg.html

[N01] 二分查找（有序数组）
来源：http://hz.cashguo.top/gthhhaoohy.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jlsjyb.cn/gtpoitbbwp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jlsjyb.cn/gtqxgxgpfl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sysykeji.top/gtwjlssklt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cqqwz.cn/gtlpncskur.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.316326.xyz/gttcagtnxe.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.smart0.xyz/gtdgqfhlvw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xuetiantiany.cn/gtgirpbcwu.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zycfv.cn/gttsyhpfas.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.dianchejie.cn/gtbldgmxej.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhijiandao.cn/gtnbbsnybi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.ywan-chungtsiang.top/gtcxdxkbpb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.redwolf501.top/gtjimlgkan.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinqigufen.top/gtznlvbpja.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.shuidangran.top/gtdofwviea.html

Go:   slices.Sort(arr)
来源：http://hz.meibo888.top/gtymlgiwxe.html


<!-- 参考信息 -->