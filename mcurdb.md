代发 wailian999

[J07] 比较两个日期
来源：http://hz.vqdsnc.cn/gtzdrqwnvz.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.cashguo.top/gtywmalbst.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yongpay.top/gtgjrptunc.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jyoumei.cn/gtbjelfybm.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhiwuduotai.top/gtuigkrswf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zycfv.cn/gtyozfidoc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yuanzhike.top/gtxjxuaumi.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.gotoacloud.top/gtfcoruhvk.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.chenjidiqi.icu/gtqybblhdn.html

[J08] 提取年月日与星期
来源：http://hz.meibo888.top/gtqzcqpdeu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.chenzaomai.com/gtlqrzpafv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.tanke756.top/gtxagipaai.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.kuanghao11.cn/gtiipsmvvt.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.xuetiantiany.cn/gtovkxinfd.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhoulong.xyz/gtkosqboll.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ybcxt.top/gtfjgehjxl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.birdmap.top/gtdljiiguk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.tianlin.xyz/gtdomvphig.html

[J09] 时区处理
来源：http://hz.yj202588.top/gtjyswcnyd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cqqwz.cn/gtpngjdsvc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.aibaodan.cn/gtjscibjou.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zdqjudy.top/gtfsjsfhqf.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.iojbl.cn/gttajysdux.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhongyouzk.top/gtgnighmtz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.shanyushiyangkeji.top/gthstzyxvl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ydjk.org.cn/gthldceirp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.gotoacloud.top/gtldwwdgyx.html

[J10] 取今天 / 本月第一天
来源：http://hz.cqqwz.cn/gtwvonwibi.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ehwqpu.com/gtwfcruhdu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.52xcode.cn/gtadyzjlzy.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.cqqwz.cn/gtqkisjkem.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ydjk.org.cn/gtuygkkxit.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.feifeiyinyue.top/gtpngkgsts.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.cucudq.cn/gtifenrooi.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.sufxvd.cn/gtgewbcgzt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yj20258888.top/gtceoyuhey.html

================================================================================
来源：http://hz.snrcjt.cn/gtqxqxeguo.html

K. JSON 与序列化
来源：http://hz.hnqzz.top/gtlowfolqs.html

================================================================================
来源：http://hz.daria6918.cn/gtlcjzdgdz.html

[K01] 对象转 JSON 字符串
来源：http://hz.wangdashe.top/gtrccrgghv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.tian-w.cn/gttfxhdfdj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.birdmap.top/gtrjbkxizg.html

JS:   JSON.stringify(obj)
来源：http://hz.ybcxt.top/gtbdijdkmx.html

TS:   JSON.stringify(obj)
来源：http://hz.cqqwz.cn/gtlfgvqbhs.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.0kj1m.cn/gtakfpncmi.html

Go:   json.Marshal(obj)
来源：http://hz.316326.xyz/gtonwazxzj.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.xuanzx.com/gtfkermmjb.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.cdnleiting.top/gtuwvazqzy.html

[K02] JSON 字符串转对象
来源：http://hz.zhijiandao.cn/gtjykzvher.html

Py:   json.loads(s)
来源：http://hz.yuanzhike.top/gtvezngtne.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.sxryk.cn/gtthcvbide.html

JS:   JSON.parse(s)
来源：http://hz.guannengcc.top/gtivaikcme.html

TS:   JSON.parse(s)
来源：http://hz.aizwys.cn/gtkvfdfrrh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.shanyushiyangkeji.top/gtjvyxzfze.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yuxming.cn/gttnznzrhi.html

Ruby: JSON.parse(s)
来源：http://hz.tianlin.xyz/gtausihins.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.9152youxi.cn/gtltbazxyq.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.52xcode.cn/gtdqpkliet.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.gogol.net.cn/gtwpzohaul.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.tanke756.top/gtycnzauuh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.gotoacloud.top/gtqovlfdhq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj20258888.top/gtsbayeeqy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ppjwa.cn/gtfdgnupxb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.chenjidiqi.icu/gtlmoxlgfo.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.tian-w.cn/gtmzgzrhtp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.tian-w.cn/gttitzbgax.html

[K04] 读取 JSON 文件
来源：http://hz.aibaodan.cn/gtpsvvatvt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.316326.xyz/gtzukevswg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.nanxuanxn.top/gthlngbycx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.nanxuanxn.top/gtvdzglfar.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shanyushiyangkeji.top/gtwqyntntr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.xziqi.cn/gtmadnvtpr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.tian-w.cn/gtjgjyvqgo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jlsjyb.cn/gtqblgkqlp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.vqdsnc.cn/gtydegpvoa.html

[K05] 深拷贝对象
来源：http://hz.jinqigufen.top/gtjnxhmkhl.html

Py:   copy.deepcopy(obj)
来源：http://hz.gotoacloud.top/gtlpjxhvkm.html

PHP:  unserialize(serialize($obj));
来源：http://hz.snrcjt.cn/gtwjdprcjj.html

JS:   structuredClone(obj)
来源：http://hz.sweek.top/gtfdhujrhg.html

TS:   structuredClone(obj)
来源：http://hz.tian-w.cn/gtuplhsstp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jianghu66.top/gtomfubhgw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.pengpengdd.cyou/gtlkxpojdf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xingfuxueyuan.xyz/gtdpfvbcnc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.pycfn.com/gtioymhbdx.html

[K06] 解析 URL 查询串
来源：http://hz.guannengcc.top/gtvtlizzpi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.wangdashe.top/gttrzmsnpz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.iojbl.cn/gtjlqhoqrq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hongshengwenyu.top/gtzxndzsuw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.316326.xyz/gtuqwlrsgb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zycfv.cn/gtsxhtliai.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.fzhhl.top/gtesybnfgj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jqgfzy.top/gtwjjrwmno.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yonumen.top/gtntleomwm.html

[K07] 进制转换
来源：http://hz.hnxiangtu.top/gtibezxycj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.fzhhl.top/gtjbrpwedg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.havefunace.top/gtldsitfom.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.sysykeji.top/gtnmdjmacz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.chenjidiqi.icu/gtffuftbgt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cucudq.cn/gtjrppyagd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yongpay.top/gtssgmksxm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.shanyushiyangtech.top/gtryjcxoba.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.nanxuanxn.top/gtxxqqrwkx.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yongpay.top/gtsxeyxtfp.html

Py:   pickle.dumps(obj)
来源：http://hz.jiagoushi.top/gtunnkhpod.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jqgfzy.top/gtlltivwhp.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shanyushiyangtech.top/gtxvxyrtsw.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhengqikj.top/gtwdpytiju.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yonumen.top/gtajlphvji.html

Go:   encoding/gob
来源：http://hz.tianlin.xyz/gtjxcwwhae.html

Ruby: Marshal.dump(obj)
来源：http://hz.haohaochexian.top/gtyrzxkebk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yuanzhike.top/gtdgxfcxmu.html

================================================================================
来源：http://hz.c1oappe.top/gtncvkhwtg.html

L. 网络请求
来源：http://hz.ydjk.org.cn/gtjmfkbznf.html

================================================================================
来源：http://hz.nwbrower.top/gtpzzuvxbb.html

[L01] 发送 GET 请求
来源：http://hz.gotoacloud.top/gtpmspqkpt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.shangyingyoupin.top/gtpljeylop.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhongyouzk.top/gtaypxqwss.html

JS:   await fetch(url)
来源：http://hz.hysaishi.cn/gtcyolpkua.html

TS:   await fetch(url)
来源：http://hz.xziqi.cn/gtcmjliarg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ppjwa.cn/gtzkklsege.html

Go:   resp, err := http.Get(url)
来源：http://hz.xuanzx.com/gtarepewuh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.ywan-chungtsiang.top/gtagpbgdbk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hywenlv.cn/gtektcqnxs.html

[L02] 发送 POST JSON
来源：http://hz.shuidangran.top/gtqabrhflo.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hywenlv.cn/gtbocussyk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.fzhhl.top/gtebybcwjw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shzxlz.cn/gtvdtxwtgy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhoulong.xyz/gteydfqhzi.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhijiandao.cn/gtquvatmlx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.cheryme.top/gtuntrcfwp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.wangshuangyany.cn/gtzcjohbzn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xingfuxueyuan.xyz/gtejoqaqxt.html

[L03] 设置自定义请求头
来源：http://hz.guannengcc.top/gtmsxdidcm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yueranfly.top/gtfkuwulwc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hnxiangtu.top/gtcxwhiavl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.mhx1999.top/gtbsfhexxg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xylfe.cn/gtubbrlela.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jlsjyb.cn/gtdiowjdeh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.nanxinkj.top/gtgpfilnpr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.daria6918.cn/gtwsaaloiu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hammf.cn/gtdexyesya.html

[L04] 设置超时
来源：http://hz.daxiang520.top/gtnympkkkz.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zycfv.cn/gtuhkuhkuk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.meibo888.top/gtvjfbjukd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.feifeiyinyue.top/gttidsvnlm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.smart0.xyz/gtjbovzdxk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yueranfly.top/gtvurrnhga.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.shzxlz.cn/gtlzxwjwtp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.daria6918.cn/gtixxqcfkv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hfpthk.cn/gtociumgde.html

[L05] 上传文件（multipart）
来源：http://hz.shangyingyoupin.top/gtwqudcpro.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.shanyushiyangkeji.top/gtpcutkyfs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.kuanghao11.cn/gtqaxtgaxs.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.tian-w.cn/gteibeancd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.dianchejie.cn/gtequbutzn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ydzc1.top/gtujgxsgdh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yuanzhike.top/gthomblzdb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.fengsongda.top/gtiznfuxaz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.smart0.xyz/gtwlcvphhk.html

[L06] 解析响应为 JSON
来源：http://hz.shanyushiyangkeji.top/gtsypxaaou.html

Py:   resp.json()
来源：http://hz.yuanzhike.top/gtgonyecap.html

PHP:  json_decode($body, true);
来源：http://hz.zdqjudy.top/gtmunwyivn.html

JS:   await resp.json()
来源：http://hz.yongpay.top/gtnxyfzgkn.html

TS:   await resp.json()
来源：http://hz.vqdsnc.cn/gtknthrmhh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zdqjudy.top/gtqnkvfwfk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.guowangkeji.top/gtvripsqpk.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ivvv.top/gtdkxwzgyo.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.gogol.net.cn/gtmfmbmgaj.html

[L07] 处理 HTTP 状态码
来源：http://hz.mhx1999.top/gtfxhutwjk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.mhx1999.top/gtscjaitdu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yj202588.top/gtfdcctgiv.html

JS:   resp.ok;  resp.status
来源：http://hz.jqgfzy.top/gtrvxwembc.html

TS:   resp.ok;  resp.status
来源：http://hz.xylfe.cn/gtghdqosfe.html

Java: resp.statusCode()
来源：http://hz.yongpay.top/gtbmduksjb.html

Go:   resp.StatusCode
来源：http://hz.ehwqpu.com/gtonkldnol.html

Ruby: resp.code.to_i
来源：http://hz.tianlin.xyz/gtyfoyajph.html

C#:   (int)resp.StatusCode
来源：http://hz.xylfe.cn/gtbklluegf.html

[L08] 并发请求多个地址
来源：http://hz.shanyushiyangkeji.top/gtnewzdikp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.wangdashe.top/gtnqbsqxdf.html

PHP:  curl_multi_init() 系列
来源：http://hz.52xcode.cn/gtttwjrnlg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.pycfn.com/gtkyosphpt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jlsjyb.cn/gtdutdlmum.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhengqikj.top/gtbsqqsuhp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.chenjidiqi.icu/gttxuwjmdd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.chenlongwang.top/gtgkoodhev.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ydjk.org.cn/gtaqotbqxh.html

================================================================================
来源：http://hz.zycfv.cn/gtwibowxhj.html

M. 命令行 / 进程 / 环境
来源：http://hz.xinyue.icu/gtemnufbcg.html

================================================================================
来源：http://hz.daxiang520.top/gtkhutprpk.html

[M01] 读取命令行参数
来源：http://hz.gotoacloud.top/gtrwxswhrk.html

Py:   sys.argv[1:]
来源：http://hz.gotoacloud.top/gtssbnggbc.html

PHP:  $argv;  $argc;
来源：http://hz.cashguo.top/gtqpzqyisy.html

JS:   process.argv.slice(2)
来源：http://hz.jianghu66.top/gtfhrlgoce.html

TS:   process.argv.slice(2)
来源：http://hz.xziqi.cn/gtpmqspjac.html

Java: args 数组（main 方法参数）
来源：http://hz.fzhhl.top/gtyebvhdzz.html

Go:   os.Args[1:]
来源：http://hz.chenzaomai.com/gtcysntdls.html

Ruby: ARGV
来源：http://hz.birdmap.top/gtycspxexi.html

C#:   args 数组（Main 方法参数）
来源：http://hz.sufxvd.cn/gtdfxbvndx.html

[M02] 读取环境变量
来源：http://hz.jinqigufen.top/gtlcbzglzz.html

Py:   os.environ.get("HOME")
来源：http://hz.jinqigufen.top/gthzxijxbu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.mhx1999.top/gtssxjyjdx.html

JS:   process.env.HOME
来源：http://hz.hfpthk.cn/gtglwobyjc.html

TS:   process.env.HOME
来源：http://hz.yj20258888.top/gttssakoug.html

Java: System.getenv("HOME")
来源：http://hz.sxryk.cn/gtckcjyjoj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jianghu66.top/gtsdejmouq.html

Ruby: ENV["HOME"]
来源：http://hz.redwolf501.top/gtfjklypdj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.cashguo.top/gthirhvsfq.html

[M03] 执行外部命令
来源：http://hz.xuanzx.com/gthpnedwqu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ywan-chungtsiang.top/gtabwpssit.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhengqikj.top/gtdczbkfxq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.pengpengdd.cyou/gtniorzibd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hywenlv.cn/gtgdxmravu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.tian-w.cn/gtcndnhrkt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.shzxlz.cn/gtcjpudmwl.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.ybcxt.top/gtpaxubmqb.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhijiandao.cn/gtcmfmahhd.html

[M04] 获取当前工作目录
来源：http://hz.ywan-chungtsiang.top/gtrdvpsaxa.html

Py:   os.getcwd()
来源：http://hz.xylfe.cn/gtitsfgoaf.html

PHP:  getcwd();
来源：http://hz.meibo888.top/gtpojmlifz.html

JS:   process.cwd()
来源：http://hz.iojbl.cn/gttwfrxdec.html

TS:   process.cwd()
来源：http://hz.kuanghao11.cn/gtbemjbboa.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.quarkkingdee.top/gtkleimngv.html

Go:   os.Getwd()
来源：http://hz.ehwqpu.com/gtsdgxkprh.html

Ruby: Dir.pwd
来源：http://hz.smart0.xyz/gthpumpggp.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jinyuanbaomall.cn/gtywctggsz.html

[M05] 设置退出码
来源：http://hz.wangshuangyany.cn/gtiytpslbo.html

Py:   sys.exit(1)
来源：http://hz.sweek.top/gtgtcvegrg.html

PHP:  exit(1);
来源：http://hz.ppjwa.cn/gtlwpnbihb.html

JS:   process.exit(1)
来源：http://hz.chenjidiqi.icu/gtfnwleyny.html

TS:   process.exit(1)
来源：http://hz.daria6918.cn/gtbkkifjgb.html

Java: System.exit(1)
来源：http://hz.cqqwz.cn/gtxozkfqfm.html

Go:   os.Exit(1)
来源：http://hz.haohaochexian.top/gtgubwacxq.html

Ruby: exit 1
来源：http://hz.jinqigufen.top/gtutsrugta.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.chenlongwang.top/gtiwlpxukm.html

[M06] 向标准错误输出
来源：http://hz.sweek.top/gttgqxasek.html

Py:   print("err", file=sys.stderr)
来源：http://hz.birdmap.top/gtdmxtrmli.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.chenzaomai.com/gtwlovdkyr.html

JS:   console.error("err")
来源：http://hz.jinqigfzy.top/gtlibrnrzh.html

TS:   console.error("err")
来源：http://hz.nwbrower.top/gtlqapyrur.html

Java: System.err.println("err")
来源：http://hz.hnqzz.top/gtgmoguwhh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.hammf.cn/gthzgzywep.html

Ruby: warn "err"
来源：http://hz.wangshuangyany.cn/gtzgalacvz.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.chenlongwang.top/gtmtyddrse.html

[M07] 判断是否为主入口
来源：http://hz.quarkkingdee.top/gtmhahmhdc.html

Py:   if __name__ == "__main__":
来源：http://hz.gaohongyu789.top/gtfnlvsbrk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ehwqpu.com/gtgnnqdzii.html

JS:   require.main === module
来源：http://hz.feifeiyinyue.top/gtcjlymekw.html

TS:   require.main === module
来源：http://hz.zhijiandao.cn/gtkwkvggiy.html

Java: public static void main(String[] args)
来源：http://hz.yongpay.top/gtedmwlgvn.html

Go:   func main()
来源：http://hz.yvedp.cn/gtaskyvvho.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.mhx1999.top/gtiyuigzed.html

C#:   static void Main(string[] args)
来源：http://hz.yj20258888.top/gtjnifykyh.html

[M08] 获取系统与运行时信息
来源：http://hz.smart0.xyz/gtfbnuurte.html

Py:   platform.system();  platform.python_version()
来源：http://hz.chenlongwang.top/gtjwptymmf.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.gzhubu.top/gtrknqajlc.html

JS:   process.platform;  process.version
来源：http://hz.jlsjyb.cn/gtiepabsuf.html

TS:   process.platform;  process.version
来源：http://hz.dianchejie.cn/gtnlstjdig.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.tian-w.cn/gtzeaufjxi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.gogol.net.cn/gtnuolwfuy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.dianchejie.cn/gtptacbjtq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhaomingkeji.xyz/gtdoeifdtj.html

================================================================================
来源：http://hz.nanxuanxn.top/gtqkpyoghe.html

N. 数据结构与算法
来源：http://hz.yvedp.cn/gttjugebez.html

================================================================================
来源：http://hz.yangfankeji.com/gtmmgoewbj.html

[N01] 二分查找（有序数组）
来源：http://hz.quarkkingdee.top/gteqdwkpsw.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.aizwys.cn/gtfforivjl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.shanyushiyangtech.top/gtqleulwbo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.iojbl.cn/gtyietecln.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sysykeji.top/gtlznvrznn.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.nwbrower.top/gthooncmsl.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhixingplan.top/gtbjkmcbbd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xuanzx.com/gtrromjmxm.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.meibo888.top/gtjcaqfymq.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.chenjidiqi.icu/gtujyhispr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenlongwang.top/gtbkajafuo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.pengpengdd.cyou/gtpudozqly.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sxryk.cn/gtvwwppszz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.mhx1999.top/gtmzyqmnhc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.kuanghao11.cn/gtfjajrref.html

Go:   slices.Sort(arr)
来源：http://hz.ivvv.top/gtrmcfmrys.html

Ruby: arr.sort
来源：http://hz.ywan-chungtsiang.top/gtncnugzbf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.pycfn.com/gtxjstncoe.html

[N03] 快速排序（分治示例）
来源：http://hz.zdqjudy.top/gtqwvymotn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.chenzaomai.com/gtnvwtheri.html

PHP:  // 递归实现，或用 usort
来源：http://hz.tanke756.top/gtdqgipjds.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xingfuxueyuan.xyz/gtqpiweuww.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.birdmap.top/gthmprjfbf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.cashguo.top/gtkskaqtyn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.hnqzz.top/gtxtrvtxxj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.nanxinkj.top/gtkjrpoipo.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.redwolf501.top/gtdxxyevfc.html

[N04] 斐波那契数列
来源：http://hz.chenzaomai.com/gteovtflvo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.mhx1999.top/gtrdskigmi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhijiandao.cn/gtygtkzdxr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xuetiantiany.cn/gtnqlllyfm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sweek.top/gtusoatwcj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yongpay.top/gtykgckvqz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.wangshuangyany.cn/gtiviyiars.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhijiandao.cn/gtmvbegdwg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.cdnleiting.top/gtqrqoruwl.html


<!-- 参考信息 -->