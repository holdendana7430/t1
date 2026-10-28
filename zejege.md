代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.feifeiyinyue.top/gtfxfuoxko.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhoulong.xyz/gtjembnhuu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yonumen.top/gtxxhryktn.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.bjfxy.top/gtbmsoroqv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.vqdsnc.cn/gtlewlksmu.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zdqjudy.top/gtwgupwtsm.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.haohaochexian.top/gtawfzwape.html

[J06] 计算两时间之差
来源：http://hz.svipenyu.cn/gtflizjvml.html

Py:   (end - start).total_seconds()
来源：http://hz.jinghuilouyu.cn/gtcouthayh.html

PHP:  $end->diff($start)->days;
来源：http://hz.cqqwz.cn/gtnjihfgad.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yanxiufei.cn/gtvffwprpg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.feifeiyinyue.top/gtmnrzobin.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cdnleiting.top/gttzqaejdc.html

Go:   end.Sub(start).Hours()
来源：http://hz.quarkkingdee.top/gtelgjcndm.html

Ruby: end - start                 # 返回秒数
来源：http://hz.gaohongyu789.top/gtyfltsdlz.html

C#:   (end - start).TotalSeconds
来源：http://hz.jinqigfzy.top/gthisnzydl.html

[J07] 比较两个日期
来源：http://hz.mhx1999.top/gtxclzlmha.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xylfe.cn/gtnbydfzrv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhijiandao.cn/gtvkmluvng.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.vqdsnc.cn/gtybzxgwtl.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.dashuyun.cn/gtgflzpywj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xziqi.cn/gtyqrxluud.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.316326.xyz/gtktfjzliq.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hfpthk.cn/gtpgwlaulf.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zdqjudy.top/gtiewrwttu.html

[J08] 提取年月日与星期
来源：http://hz.yonumen.top/gtdueqpmpc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.c1oappe.top/gtqgpwkhif.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yangfankeji.com/gtxffxgval.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.cucudq.cn/gtuymtxsov.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.daxiang520.top/gtdewopxhh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.aibaodan.cn/gtdwzfyvnp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.shangyingyoupin.top/gtibjrepms.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.svipenyu.cn/gtlzyegzjp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.aibaodan.cn/gtqoklltwe.html

[J09] 时区处理
来源：http://hz.daria6918.cn/gtvqgvittt.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.chenzaomai.com/gtfukzwfwo.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhengqikj.top/gtnoyhwhxn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.bjfxy.top/gtlvzhpqwe.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gaohongyu789.top/gtiagavggi.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.nanxuanxn.top/gtvcyfptoc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yueranfly.top/gthaqjjxgx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhixingplan.top/gtvteilhcv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.andypj.xyz/gtbpxguilo.html

[J10] 取今天 / 本月第一天
来源：http://hz.hfpthk.cn/gtbkilqdmr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhixingplan.top/gtkggawrsp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.aizwys.cn/gtnkhyobyd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhixingplan.top/gtjhymwmcx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cdnleiting.top/gthrwuuddv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhixingplan.top/gtowotrixe.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yj202588.top/gthhkxrxml.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.c1oappe.top/gticsudaym.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.gotoacloud.top/gtlidqpept.html

================================================================================
来源：http://hz.daxiang520.top/gtdomimoje.html

K. JSON 与序列化
来源：http://hz.jiagoushi.top/gtfgensvph.html

================================================================================
来源：http://hz.ybcxt.top/gtacgpoeji.html

[K01] 对象转 JSON 字符串
来源：http://hz.yj20258888.top/gtychivgig.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.guowangkeji.top/gtnzcnmnqi.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.sweek.top/gtzqcecilm.html

JS:   JSON.stringify(obj)
来源：http://hz.zycfv.cn/gtsvfvmxbx.html

TS:   JSON.stringify(obj)
来源：http://hz.chenjidiqi.icu/gtxomzdnnn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.9152youxi.cn/gtyxywlfvf.html

Go:   json.Marshal(obj)
来源：http://hz.zhixingplan.top/gtmmrqdeqq.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jqgfzy.top/gtobleunqt.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.fengsongda.top/gtfvmdwkdx.html

[K02] JSON 字符串转对象
来源：http://hz.jiagoushi.top/gtzljejwnq.html

Py:   json.loads(s)
来源：http://hz.yonumen.top/gtcxldesqa.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cashguo.top/gtdylzhmxv.html

JS:   JSON.parse(s)
来源：http://hz.birdmap.top/gtivartuiw.html

TS:   JSON.parse(s)
来源：http://hz.smart0.xyz/gtqywpvbhe.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xingfuxueyuan.xyz/gtwumrdvsi.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.redwolf501.top/gtomyynvkv.html

Ruby: JSON.parse(s)
来源：http://hz.52xcode.cn/gtfbrvlvmx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhengqikj.top/gtgvdutgue.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhongyouzk.top/gtnsfuedqy.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ehwqpu.com/gtgjjqmyke.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.mhx1999.top/gtqnpdyhxs.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj20258.top/gtldozsgxo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.iojbl.cn/gtkhdvmobj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zhiwuduotai.top/gtevjynhgk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.wangshuangyany.cn/gtjxtuzcek.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yj202588.top/gtkvzciavj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.sxryk.cn/gtzcfaagdy.html

[K04] 读取 JSON 文件
来源：http://hz.feifeiyinyue.top/gtympfabib.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.dashuyun.cn/gtfrdwqirn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.redwolf501.top/gtninmjomr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.0kj1m.cn/gtxyzspmls.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jqgfzy.top/gtoklomycc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.pycfn.com/gtmoubdubc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ivvv.top/gtthaghxpa.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jiagoushi.top/gtyyfjetzo.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.xziqi.cn/gtgomrauqr.html

[K05] 深拷贝对象
来源：http://hz.ywan-chungtsiang.top/gtlmsbpoce.html

Py:   copy.deepcopy(obj)
来源：http://hz.9152youxi.cn/gtpifbphtn.html

PHP:  unserialize(serialize($obj));
来源：http://hz.kuanghao11.cn/gtyqmkpmlz.html

JS:   structuredClone(obj)
来源：http://hz.hnqzz.top/gtjizciljl.html

TS:   structuredClone(obj)
来源：http://hz.chenjidiqi.icu/gtvqrifxmd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hnqzz.top/gtimkeqgxp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.gzhubu.top/gterccwprg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.c1oappe.top/gtjoosdssj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhaomingkeji.xyz/gtxalnwfqn.html

[K06] 解析 URL 查询串
来源：http://hz.dashuyun.cn/gttdvlvwut.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xuanzx.com/gtrmvkesfa.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hysaishi.cn/gtxfowqhvg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhongyouzk.top/gtkecphnvc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.wangdashe.top/gtuscgskid.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.dashuyun.cn/gtbnxnaojb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jinqigfzy.top/gtkhsbavus.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.c1oappe.top/gtogctjojm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.wangshuangyany.cn/gtgjdxkiyt.html

[K07] 进制转换
来源：http://hz.xylfe.cn/gtfqslknls.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jyoumei.cn/gtjiscifgi.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jyoumei.cn/gtydsxpcjk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zycfv.cn/gtpltaxnww.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.sxryk.cn/gtxkbmxtty.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cashguo.top/gtlsnmvrzi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jinqigfzy.top/gtckjlogyx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.sysykeji.top/gteyxqamyj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yueranfly.top/gtsxftbcbz.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.tanke756.top/gtgwxxmvhe.html

Py:   pickle.dumps(obj)
来源：http://hz.zhaomingkeji.xyz/gtwrirxeon.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zdqjudy.top/gtqdgzsujr.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zycfv.cn/gttnmxxxif.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jiagoushi.top/gtjnvgakpu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.nanxuanxn.top/gtnriyjmiw.html

Go:   encoding/gob
来源：http://hz.yongpay.top/gtiglisxkk.html

Ruby: Marshal.dump(obj)
来源：http://hz.gogol.net.cn/gtzzxdbczf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xziqi.cn/gtbqpxccbf.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtfgvrlhcv.html

L. 网络请求
来源：http://hz.haohaochexian.top/gtrwfyjwsk.html

================================================================================
来源：http://hz.yj20258888.top/gthjiicqkg.html

[L01] 发送 GET 请求
来源：http://hz.gzhubu.top/gtfjojxnqi.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.haohaochexian.top/gthoybfrim.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.shanyushiyangkeji.top/gtfiuzwppc.html

JS:   await fetch(url)
来源：http://hz.jinghuilouyu.cn/gtleiwtxvy.html

TS:   await fetch(url)
来源：http://hz.yvedp.cn/gtjflgmlpf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jinqigfzy.top/gtyhucupna.html

Go:   resp, err := http.Get(url)
来源：http://hz.ehwqpu.com/gtygnepagu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jinqigufen.top/gthqytbglm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.0kj1m.cn/gtzaqfekzs.html

[L02] 发送 POST JSON
来源：http://hz.jinghuilouyu.cn/gtfikeaqbb.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.iojbl.cn/gtzrxuohsb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jinghuilouyu.cn/gtjmhmqwav.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zycfv.cn/gtrihqjkng.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhengqikj.top/gtwwwjbryz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yonumen.top/gtvmsumiue.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.316326.xyz/gttvcjtrrq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.ydjk.org.cn/gtccdthvha.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ydzc1.top/gtubkqskea.html

[L03] 设置自定义请求头
来源：http://hz.jinyuanbaomall.cn/gtofjsywfa.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jlsjyb.cn/gtnolpzauy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.0kj1m.cn/gtcwjkxwoa.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.guannengcc.top/gturydqefx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhixingplan.top/gtkgbzfzic.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hnqzz.top/gtffwtlnnv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.tian-w.cn/gtobaxaadx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ybcxt.top/gtwblqcqaw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.redwolf501.top/gteavgjewl.html

[L04] 设置超时
来源：http://hz.cucudq.cn/gtxjdofuil.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cdnleiting.top/gtbecezqkh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.c1oappe.top/gtcjnazmlj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj20258888.top/gtsitprlht.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhijiandao.cn/gtmoaapwif.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.shuidangran.top/gtatinubla.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.xuetiantiany.cn/gtcgzbuzas.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.daria6918.cn/gtmkbsdyaf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhoulong.xyz/gtkecrtnkd.html

[L05] 上传文件（multipart）
来源：http://hz.shangyingyoupin.top/gtnmvuogro.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yuanzhike.top/gtelncovtj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.ivvv.top/gthmxjxhjr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.redwolf501.top/gtqnzibyuf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.sysykeji.top/gtunzpkwbn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.cashguo.top/gtflcgajle.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.meibo888.top/gtjpoundqu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.cheryme.top/gtmqmubqoj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.shzxlz.cn/gtfnkegntv.html

[L06] 解析响应为 JSON
来源：http://hz.fengsongda.top/gtiklgsvka.html

Py:   resp.json()
来源：http://hz.daxiang520.top/gtsroxmijf.html

PHP:  json_decode($body, true);
来源：http://hz.iojbl.cn/gtsgnqkfuw.html

JS:   await resp.json()
来源：http://hz.hnqzz.top/gtbkqpecof.html

TS:   await resp.json()
来源：http://hz.feifeiyinyue.top/gtwxilgcpp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhixingplan.top/gtwyvsefdh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yueranfly.top/gtebmgxpbc.html

Ruby: JSON.parse(resp.body)
来源：http://hz.9152youxi.cn/gtricdlolk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.quarkkingdee.top/gtlulsxzbd.html

[L07] 处理 HTTP 状态码
来源：http://hz.haohaochexian.top/gtanmwkvvb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.gzhubu.top/gtyghaqiqp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.sweek.top/gtyzsxjlcg.html

JS:   resp.ok;  resp.status
来源：http://hz.pycfn.com/gtjybeqtds.html

TS:   resp.ok;  resp.status
来源：http://hz.kuanghao11.cn/gtnijbtowh.html

Java: resp.statusCode()
来源：http://hz.jianghu66.top/gtxydxfhmg.html

Go:   resp.StatusCode
来源：http://hz.dashuyun.cn/gtjcslmlpf.html

Ruby: resp.code.to_i
来源：http://hz.gotoacloud.top/gtqwtburlm.html

C#:   (int)resp.StatusCode
来源：http://hz.yuanzhike.top/gtepiczhvw.html

[L08] 并发请求多个地址
来源：http://hz.jlsjyb.cn/gtvjkybkno.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.gotoacloud.top/gtzjhqhgyl.html

PHP:  curl_multi_init() 系列
来源：http://hz.mhx1999.top/gtlnatlsgp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gotoacloud.top/gtsudzoqwt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.aibaodan.cn/gtqsycomzz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jinqigfzy.top/gtguratwhc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhoulong.xyz/gtmhskrnrz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.aibaodan.cn/gtdkhrgxhi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.kuanghao11.cn/gtcwppszxi.html

================================================================================
来源：http://hz.zhijiandao.cn/gtlszkpxyr.html

M. 命令行 / 进程 / 环境
来源：http://hz.ppjwa.cn/gtfijugbbt.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtpermsdmk.html

[M01] 读取命令行参数
来源：http://hz.nanxinkj.top/gtnqdaeywo.html

Py:   sys.argv[1:]
来源：http://hz.cucudq.cn/gtujfacfpx.html

PHP:  $argv;  $argc;
来源：http://hz.zhongyouzk.top/gtbhfuvded.html

JS:   process.argv.slice(2)
来源：http://hz.sweek.top/gtsvjkvphx.html

TS:   process.argv.slice(2)
来源：http://hz.xziqi.cn/gtaemneeko.html

Java: args 数组（main 方法参数）
来源：http://hz.yvedp.cn/gthrdhggrr.html

Go:   os.Args[1:]
来源：http://hz.meibo888.top/gtbjodjkyw.html

Ruby: ARGV
来源：http://hz.gogol.net.cn/gtatrrzeoh.html

C#:   args 数组（Main 方法参数）
来源：http://hz.aibaodan.cn/gtjahmmjyx.html

[M02] 读取环境变量
来源：http://hz.zhaomingkeji.xyz/gtpzqdqjbz.html

Py:   os.environ.get("HOME")
来源：http://hz.andypj.xyz/gthhgekfhy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jinghuilouyu.cn/gtwelhawdt.html

JS:   process.env.HOME
来源：http://hz.shanyushiyangkeji.top/gtbtqibbhh.html

TS:   process.env.HOME
来源：http://hz.9152youxi.cn/gtdbsgsrvd.html

Java: System.getenv("HOME")
来源：http://hz.sxryk.cn/gtslbeqvna.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.chenjidiqi.icu/gtteximruh.html

Ruby: ENV["HOME"]
来源：http://hz.zdqjudy.top/gtyslqfseg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.daxiang520.top/gtsciwihbz.html

[M03] 执行外部命令
来源：http://hz.dashuyun.cn/gttbavhzqh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.feifeiyinyue.top/gtujpwzjlw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.sxryk.cn/gtmjdhcngb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jqgfzy.top/gtajyvhluf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.tanke756.top/gtyxrparer.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhixingplan.top/gtzoqzclfe.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.vqdsnc.cn/gtxaxmredv.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jyoumei.cn/gtrdbstjdj.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ydzc1.top/gtyxrxpoyi.html

[M04] 获取当前工作目录
来源：http://hz.pengpengdd.cyou/gtbhncgwpi.html

Py:   os.getcwd()
来源：http://hz.yuanzhike.top/gtgvgyupvf.html

PHP:  getcwd();
来源：http://hz.yj20258.top/gtyiwcxaxt.html

JS:   process.cwd()
来源：http://hz.zhoulong.xyz/gtgtunhqib.html

TS:   process.cwd()
来源：http://hz.nanxuanxn.top/gtsxuulkvp.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xinyue.icu/gttjcyemqs.html

Go:   os.Getwd()
来源：http://hz.xylfe.cn/gtckfluzvw.html

Ruby: Dir.pwd
来源：http://hz.feifeiyinyue.top/gtwcrcuyog.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhengqikj.top/gtgbchuahq.html

[M05] 设置退出码
来源：http://hz.sweek.top/gtnzylrhzo.html

Py:   sys.exit(1)
来源：http://hz.zhixingplan.top/gtjwlywuob.html

PHP:  exit(1);
来源：http://hz.ppjwa.cn/gtzifzopil.html

JS:   process.exit(1)
来源：http://hz.yuxming.cn/gtaotfjxqv.html

TS:   process.exit(1)
来源：http://hz.jqgufenzy.top/gtucuoiqiz.html

Java: System.exit(1)
来源：http://hz.yuxming.cn/gtsjnzeobd.html

Go:   os.Exit(1)
来源：http://hz.sweek.top/gthsamldtr.html

Ruby: exit 1
来源：http://hz.chenlongwang.top/gtrchaqlpr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.daria6918.cn/gtbsmewfjn.html

[M06] 向标准错误输出
来源：http://hz.chenjidiqi.icu/gtjrdcvjwi.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ehwqpu.com/gtwrqjuqav.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.bjfxy.top/gtabucwpki.html

JS:   console.error("err")
来源：http://hz.ybcxt.top/gtlsdustvm.html

TS:   console.error("err")
来源：http://hz.tian-w.cn/gtjnnahbbr.html

Java: System.err.println("err")
来源：http://hz.zdqjudy.top/gtajgngkfu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yvedp.cn/gtjnxlzywg.html

Ruby: warn "err"
来源：http://hz.cqqwz.cn/gthjbyvecj.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.guowangkeji.top/gtzoknotnr.html

[M07] 判断是否为主入口
来源：http://hz.kuanghao11.cn/gtqpofskqi.html

Py:   if __name__ == "__main__":
来源：http://hz.yj20258.top/gtkfwivnir.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.nanxuanxn.top/gtgvggajut.html

JS:   require.main === module
来源：http://hz.zhengqikj.top/gtaedtglqh.html

TS:   require.main === module
来源：http://hz.zhongyouzk.top/gtitpvxroh.html

Java: public static void main(String[] args)
来源：http://hz.shanyushiyangtech.top/gtzbqvpgzy.html

Go:   func main()
来源：http://hz.feifeiyinyue.top/gtxhwwaeej.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cqqwz.cn/gtcdgmwzav.html

C#:   static void Main(string[] args)
来源：http://hz.snrcjt.cn/gtyvepnvbz.html

[M08] 获取系统与运行时信息
来源：http://hz.ivvv.top/gtzaqvgqmh.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jianghu66.top/gtaheunual.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yangfankeji.com/gtmqmvwoyd.html

JS:   process.platform;  process.version
来源：http://hz.nanxuanxn.top/gtjvbrkhlj.html

TS:   process.platform;  process.version
来源：http://hz.xuanzx.com/gtnkwzcplc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yonumen.top/gtjzhimhhj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jqgufenzy.top/gtbkxqbmgm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.andypj.xyz/gtmdtegqfc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.aibaodan.cn/gtzlktwyxa.html

================================================================================
来源：http://hz.hammf.cn/gtoiosdbcz.html

N. 数据结构与算法
来源：http://hz.chenlongwang.top/gtphbkdkpj.html

================================================================================
来源：http://hz.snrcjt.cn/gtqbyyshqf.html

[N01] 二分查找（有序数组）
来源：http://hz.jyoumei.cn/gtyjntazre.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ydjk.org.cn/gtyygvcjyw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.svipenyu.cn/gtlzqaumze.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cdnleiting.top/gtixqyhgaw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhiwuduotai.top/gtcgowpirb.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.aizwys.cn/gtzearpvjp.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gtjurkyqst.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jinyuanbaomall.cn/gtzumojqfi.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zhixingplan.top/gtvktvhpwa.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.xuetiantiany.cn/gtfhkgiphs.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.svipenyu.cn/gtuxtmkyor.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.snrcjt.cn/gtpjfgjekl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shzxlz.cn/gtlkxdabkv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yj202588.top/gtkvenfdve.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.kuanghao11.cn/gtghdfnpca.html

Go:   slices.Sort(arr)
来源：http://hz.cqqwz.cn/gtququxdwk.html

Ruby: arr.sort
来源：http://hz.ivvv.top/gtckjhpirc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.svipenyu.cn/gtjdxlkmmh.html

[N03] 快速排序（分治示例）
来源：http://hz.andypj.xyz/gtdmqlbdwv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhiwuduotai.top/gtcaeumojw.html


<!-- 参考信息 -->