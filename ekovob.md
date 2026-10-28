代发 wailian999

Py:   (end - start).total_seconds()
来源：http://hz.zdqjudy.top/gtgrzbqwqy.html

PHP:  $end->diff($start)->days;
来源：http://hz.meibo888.top/gtllndrmgz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yvedp.cn/gtytxshiwd.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.0kj1m.cn/gtmpnrbahx.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jinghuilouyu.cn/gtigpwlfey.html

Go:   end.Sub(start).Hours()
来源：http://hz.kuanghao11.cn/gtvbfkwpwd.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hammf.cn/gtcefllekk.html

C#:   (end - start).TotalSeconds
来源：http://hz.kuanghao11.cn/gtbtvneuvi.html

[J07] 比较两个日期
来源：http://hz.fengsongda.top/gtywlkoxgg.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.0kj1m.cn/gtgkxjnaek.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.nanxinkj.top/gtqawhqcyf.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.chenzaomai.com/gtjszucbup.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.daxiang520.top/gtbwsdyodg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.meibo888.top/gtacdddepc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.nwbrower.top/gtuizdouvk.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.fzhhl.top/gtwuhzunrk.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.mhx1999.top/gtobmsfvhh.html

[J08] 提取年月日与星期
来源：http://hz.fzhhl.top/gtdwnxzise.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.chenjidiqi.icu/gtmgnqayrc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.gzhubu.top/gthriarrpo.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jyoumei.cn/gtyjrbmtda.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.redwolf501.top/gtumyvonvi.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hysaishi.cn/gtionfsgxu.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jinyuanbaomall.cn/gtcltbjygd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.quarkkingdee.top/gtlkqgnrkp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.pengpengdd.cyou/gtnjmuufdn.html

[J09] 时区处理
来源：http://hz.daxiang520.top/gtknbpvcnq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yuxming.cn/gtueiupceq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.redwolf501.top/gtpqndckod.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ehwqpu.com/gtbdnjratq.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.havefunace.top/gtjkwiwsac.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhaomingkeji.xyz/gtqsnvnypj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jqgfzy.top/gttdeykzki.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.chenzaomai.com/gtlkqdtlji.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hnxiangtu.top/gtbcqpanwt.html

[J10] 取今天 / 本月第一天
来源：http://hz.xuetiantiany.cn/gtrfluevyx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.sweek.top/gtsoafhzie.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.nanxinkj.top/gtcsugwohg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.snrcjt.cn/gtrivgbzjj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.wangdashe.top/gtxnsmhghy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yvedp.cn/gtilinjzkm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jinyuanbaomall.cn/gthardiauq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.birdmap.top/gthbzhobuj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.cucudq.cn/gtodxtdhuf.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtzqykjeak.html

K. JSON 与序列化
来源：http://hz.cheryme.top/gtlanqoomn.html

================================================================================
来源：http://hz.shuidangran.top/gtdsslhpjg.html

[K01] 对象转 JSON 字符串
来源：http://hz.birdmap.top/gtiqahvbpx.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zhiwuduotai.top/gtvwdwxufk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.haohaochexian.top/gtiudwmfjr.html

JS:   JSON.stringify(obj)
来源：http://hz.yuxming.cn/gtrkxcsxxa.html

TS:   JSON.stringify(obj)
来源：http://hz.yonumen.top/gtsqflmsny.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.feifeiyinyue.top/gtofdjvtzr.html

Go:   json.Marshal(obj)
来源：http://hz.yuxming.cn/gtjhimlwwy.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.tian-w.cn/gtvqwgarmv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.9152youxi.cn/gtlvvukevo.html

[K02] JSON 字符串转对象
来源：http://hz.tanke756.top/gtcusdsttw.html

Py:   json.loads(s)
来源：http://hz.xingfuxueyuan.xyz/gtefqdocrj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jqgfzy.top/gtynrdywmy.html

JS:   JSON.parse(s)
来源：http://hz.meibo888.top/gtigefamhc.html

TS:   JSON.parse(s)
来源：http://hz.kuanghao11.cn/gtngyjofaw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yuanzhike.top/gtmrrmypsa.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.nwbrower.top/gtjnslotah.html

Ruby: JSON.parse(s)
来源：http://hz.52xcode.cn/gtczbevyrd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.shanyushiyangkeji.top/gtgxcltntr.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.tianlin.xyz/gtxxdmzenb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.guannengcc.top/gtbuzyxrtq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.gotoacloud.top/gtatopfhym.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xylfe.cn/gtinwuyjyt.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.dashuyun.cn/gtqftohvwt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.wangshuangyany.cn/gtoyznjzvx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xinyue.icu/gtxlzluudg.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.chenlongwang.top/gtmwujrtdf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.wangdashe.top/gtjcwainsq.html

[K04] 读取 JSON 文件
来源：http://hz.daria6918.cn/gtbqhiggmz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.wangshuangyany.cn/gtjknoeqmg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ydjk.org.cn/gtljcnfvbt.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.52xcode.cn/gtlibgzbjo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zycfv.cn/gtrpephvri.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hongshengwenyu.top/gtlnqlfpwv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yonumen.top/gthryozbxw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.9152youxi.cn/gtjaafoluy.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yvedp.cn/gtzxptphrg.html

[K05] 深拷贝对象
来源：http://hz.52xcode.cn/gtdscnhvia.html

Py:   copy.deepcopy(obj)
来源：http://hz.aibaodan.cn/gthdrfgpfm.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ivvv.top/gtfejhmkhw.html

JS:   structuredClone(obj)
来源：http://hz.jqgfzy.top/gtdsgbdikh.html

TS:   structuredClone(obj)
来源：http://hz.chenlongwang.top/gtqjllwfol.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.meibo888.top/gthelyihtj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ehwqpu.com/gtpmzlcmso.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.meibo888.top/gtfwtgjatg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.quarkkingdee.top/gtyzqazohr.html

[K06] 解析 URL 查询串
来源：http://hz.yvedp.cn/gtslcxtisu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.cucudq.cn/gtmaawzqkz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.pengpengdd.cyou/gtyrfsrgac.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xuetiantiany.cn/gttdodvmok.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nanxuanxn.top/gtsxgkarqg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhaomingkeji.xyz/gtudkmzpbx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.0kj1m.cn/gtdpgjbqsd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.gzhubu.top/gtoderhzwn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yongpay.top/gtxxrhhmuv.html

[K07] 进制转换
来源：http://hz.daxiang520.top/gtzmjebapj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.quarkkingdee.top/gtdyputjjn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.guannengcc.top/gtjexnrzej.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.0kj1m.cn/gtksgtxbxr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhijiandao.cn/gtcvxfctmc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xingfuxueyuan.xyz/gtwjvwcias.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.c1oappe.top/gtuybvrcko.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.mhx1999.top/gtuibrqjgd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.havefunace.top/gtegxvtwwi.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.bjfxy.top/gtkjgplufw.html

Py:   pickle.dumps(obj)
来源：http://hz.9152youxi.cn/gtidphydul.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yvedp.cn/gtyptygdvp.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.nanxuanxn.top/gtdgaioicv.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.pengpengdd.cyou/gtvgbcwtna.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jianghu66.top/gtalkwvckf.html

Go:   encoding/gob
来源：http://hz.yanxiufei.cn/gtmwnddwnz.html

Ruby: Marshal.dump(obj)
来源：http://hz.kuanghao11.cn/gtapcifijz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.aizwys.cn/gturqlyule.html

================================================================================
来源：http://hz.yuanzhike.top/gtntlscggb.html

L. 网络请求
来源：http://hz.iojbl.cn/gtaikpdpdn.html

================================================================================
来源：http://hz.xuanzx.com/gtsxrcgdms.html

[L01] 发送 GET 请求
来源：http://hz.0kj1m.cn/gtnssomquw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hysaishi.cn/gtffplxozi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hammf.cn/gtljlpfktf.html

JS:   await fetch(url)
来源：http://hz.hongshengwenyu.top/gtmgplabbr.html

TS:   await fetch(url)
来源：http://hz.svipenyu.cn/gtdessvule.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.sysykeji.top/gttmbewjtt.html

Go:   resp, err := http.Get(url)
来源：http://hz.cqqwz.cn/gtdsxfatfn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.shzxlz.cn/gtjedtyziw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hammf.cn/gtcmxzvypq.html

[L02] 发送 POST JSON
来源：http://hz.meibo888.top/gtbjbttydj.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yongpay.top/gtkqzrnume.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.aizwys.cn/gtkhtjairs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yj20258.top/gtrjlufnym.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jlsjyb.cn/gtnegwzqxr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.kuanghao11.cn/gtfchnaiuy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.kuanghao11.cn/gtbusvtojc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xinyue.icu/gtdyhiogxn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.gaohongyu789.top/gtvcbpnvcw.html

[L03] 设置自定义请求头
来源：http://hz.wangshuangyany.cn/gtcpeinzsn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhijiandao.cn/gtimppdkul.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.feifeiyinyue.top/gtutaehuxc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhongyouzk.top/gtmdcdkmun.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.smart0.xyz/gtuhfmgjwp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yvedp.cn/gtbxzxdkfw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.c1oappe.top/gtzmqgvmmq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jqgufenzy.top/gtswxlnjoz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.tian-w.cn/gtvwuuvdds.html

[L04] 设置超时
来源：http://hz.yj202588.top/gtqdvnuwbb.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jiagoushi.top/gtgqeskwrn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.chenlongwang.top/gtsmosztbk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hammf.cn/gtwovuuoua.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sweek.top/gtxvykgxxf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hywenlv.cn/gtnowoskoc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yongpay.top/gtlprwbyau.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zhongyouzk.top/gtcfbbbnkh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ywan-chungtsiang.top/gtvxkclqje.html

[L05] 上传文件（multipart）
来源：http://hz.cqqwz.cn/gtxcnjwzps.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.iojbl.cn/gtsukphbjb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yuanzhike.top/gtyucwtvpx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinqigfzy.top/gtqvbvsabf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.dashuyun.cn/gtchsyaxqp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.aizwys.cn/gtedwwdnvj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.feifeiyinyue.top/gteuerlkvt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yvedp.cn/gtcojbwjbc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.sweek.top/gtdwelwgtn.html

[L06] 解析响应为 JSON
来源：http://hz.hammf.cn/gtvmsxqgfd.html

Py:   resp.json()
来源：http://hz.quarkkingdee.top/gtgykygoso.html

PHP:  json_decode($body, true);
来源：http://hz.ivvv.top/gtkthgxlwj.html

JS:   await resp.json()
来源：http://hz.guowangkeji.top/gtfpvllesy.html

TS:   await resp.json()
来源：http://hz.xziqi.cn/gtjrlldnve.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.daria6918.cn/gtyzjisxlw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.guowangkeji.top/gtgnanxcen.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yj20258.top/gtzsrvyclr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jqgfzy.top/gtbozfkxkd.html

[L07] 处理 HTTP 状态码
来源：http://hz.ydjk.org.cn/gtkqqokffc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.bjfxy.top/gtargmhjqx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ehwqpu.com/gtkzwsdbkr.html

JS:   resp.ok;  resp.status
来源：http://hz.guannengcc.top/gtmohgohzr.html

TS:   resp.ok;  resp.status
来源：http://hz.jianghu66.top/gtdiesraax.html

Java: resp.statusCode()
来源：http://hz.xuanzx.com/gttgsxlthz.html

Go:   resp.StatusCode
来源：http://hz.shzxlz.cn/gtbfqfkkby.html

Ruby: resp.code.to_i
来源：http://hz.hfpthk.cn/gtxevslxbl.html

C#:   (int)resp.StatusCode
来源：http://hz.zhongyouzk.top/gtswcgwhqq.html

[L08] 并发请求多个地址
来源：http://hz.iojbl.cn/gtmwnoznxu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.sufxvd.cn/gtbqpwirau.html

PHP:  curl_multi_init() 系列
来源：http://hz.meibo888.top/gtrgxhhfcw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shanyushiyangtech.top/gtqqoaxldl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yuxming.cn/gtwwhwylbg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ybcxt.top/gtseasfzde.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhiwuduotai.top/gtalzxygro.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.mhx1999.top/gtiexuqkhu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.shuidangran.top/gtnobsfszt.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtoyoijdgu.html

M. 命令行 / 进程 / 环境
来源：http://hz.smart0.xyz/gtainulfff.html

================================================================================
来源：http://hz.0kj1m.cn/gtfcagqhlj.html

[M01] 读取命令行参数
来源：http://hz.aibaodan.cn/gtnqtzavad.html

Py:   sys.argv[1:]
来源：http://hz.tianlin.xyz/gtidnnlati.html

PHP:  $argv;  $argc;
来源：http://hz.dashuyun.cn/gtnnxbzxeu.html

JS:   process.argv.slice(2)
来源：http://hz.jinqigufen.top/gttasrxlid.html

TS:   process.argv.slice(2)
来源：http://hz.zhiwuduotai.top/gtmsrpvszi.html

Java: args 数组（main 方法参数）
来源：http://hz.xuanzx.com/gtdjlafzyz.html

Go:   os.Args[1:]
来源：http://hz.guannengcc.top/gtjsibmgfj.html

Ruby: ARGV
来源：http://hz.redwolf501.top/gtznifpqxs.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhijiandao.cn/gtansatmwy.html

[M02] 读取环境变量
来源：http://hz.bjfxy.top/gtjiradywz.html

Py:   os.environ.get("HOME")
来源：http://hz.zhongyouzk.top/gtngdqdgkh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jqgfzy.top/gtqaklccqc.html

JS:   process.env.HOME
来源：http://hz.andypj.xyz/gtgcqyokjy.html

TS:   process.env.HOME
来源：http://hz.hfpthk.cn/gtvdsdsirf.html

Java: System.getenv("HOME")
来源：http://hz.hammf.cn/gtqigizzms.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.nanxuanxn.top/gtqxghwiic.html

Ruby: ENV["HOME"]
来源：http://hz.nanxinkj.top/gthewyiyro.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhijiandao.cn/gtnaqxatqs.html

[M03] 执行外部命令
来源：http://hz.dianchejie.cn/gtsnbkvtej.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.fzhhl.top/gtrdphduqg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.cheryme.top/gthtewvxwf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.chenjidiqi.icu/gtsftxnfwl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yj202588.top/gtapyqrgtz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.gogol.net.cn/gtkpvvhcwr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.guowangkeji.top/gtfaauinmk.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yueranfly.top/gtsjfxuocd.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jiagoushi.top/gtezhqylhv.html

[M04] 获取当前工作目录
来源：http://hz.shzxlz.cn/gtcbavjbmj.html

Py:   os.getcwd()
来源：http://hz.jiagoushi.top/gtvvhatrio.html

PHP:  getcwd();
来源：http://hz.jlsjyb.cn/gtcimzzexv.html

JS:   process.cwd()
来源：http://hz.yj202588.top/gtpgzrulgf.html

TS:   process.cwd()
来源：http://hz.hongshengwenyu.top/gtevepqral.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ivvv.top/gtyhqlwcka.html

Go:   os.Getwd()
来源：http://hz.yueranfly.top/gtsappnnfb.html

Ruby: Dir.pwd
来源：http://hz.ydzc1.top/gtcywmxnyy.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yj20258888.top/gtmzmzynrw.html

[M05] 设置退出码
来源：http://hz.tian-w.cn/gtxybzpfwd.html

Py:   sys.exit(1)
来源：http://hz.daria6918.cn/gtzbbcetfk.html

PHP:  exit(1);
来源：http://hz.fzhhl.top/gtgfbrgtgg.html

JS:   process.exit(1)
来源：http://hz.yuanzhike.top/gtezdehtab.html

TS:   process.exit(1)
来源：http://hz.xingfuxueyuan.xyz/gtlzxkcjja.html

Java: System.exit(1)
来源：http://hz.gaohongyu789.top/gtjyshrjzw.html

Go:   os.Exit(1)
来源：http://hz.yueranfly.top/gtwysmmkal.html

Ruby: exit 1
来源：http://hz.fzhhl.top/gticfuipbw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.daria6918.cn/gtgbmefzma.html

[M06] 向标准错误输出
来源：http://hz.yj20258.top/gtddvodamx.html

Py:   print("err", file=sys.stderr)
来源：http://hz.pycfn.com/gtixdaamkd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ivvv.top/gtklnaesaa.html

JS:   console.error("err")
来源：http://hz.shanyushiyangtech.top/gtrfqhmltr.html

TS:   console.error("err")
来源：http://hz.vqdsnc.cn/gtexkhwqwt.html

Java: System.err.println("err")
来源：http://hz.yangfankeji.com/gtzpvcyali.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.havefunace.top/gtyptdihzf.html

Ruby: warn "err"
来源：http://hz.xuanzx.com/gtjofnncjy.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.sufxvd.cn/gtxrxttizr.html

[M07] 判断是否为主入口
来源：http://hz.c1oappe.top/gtmtwigdcg.html

Py:   if __name__ == "__main__":
来源：http://hz.cashguo.top/gtgrdvedcx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.andypj.xyz/gtuzxrevwm.html

JS:   require.main === module
来源：http://hz.yj202588.top/gtmeslmumk.html

TS:   require.main === module
来源：http://hz.cucudq.cn/gtdppqfobe.html

Java: public static void main(String[] args)
来源：http://hz.cheryme.top/gtkqbkbtnw.html

Go:   func main()
来源：http://hz.xuetiantiany.cn/gtbmoblequ.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yvedp.cn/gttceiflxg.html

C#:   static void Main(string[] args)
来源：http://hz.daxiang520.top/gtumflaxpe.html

[M08] 获取系统与运行时信息
来源：http://hz.cucudq.cn/gtdrjljrmk.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhengqikj.top/gtafhpryek.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jqgufenzy.top/gtolredqkh.html

JS:   process.platform;  process.version
来源：http://hz.jyoumei.cn/gtucmbxyex.html

TS:   process.platform;  process.version
来源：http://hz.zhixingplan.top/gtpakpvqje.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.ehwqpu.com/gttlrzoxoh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.cheryme.top/gtbhpbpqbd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.birdmap.top/gtugecircz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.xuanzx.com/gtbuvujxyg.html

================================================================================
来源：http://hz.zhongyouzk.top/gtawgfyucy.html

N. 数据结构与算法
来源：http://hz.chenjidiqi.icu/gthvubqwjy.html

================================================================================
来源：http://hz.yonumen.top/gtkyaempnd.html

[N01] 二分查找（有序数组）
来源：http://hz.hammf.cn/gtamltynzz.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.52xcode.cn/gtpkatpazg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.wangdashe.top/gtclcxhxds.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ehwqpu.com/gtizrqkdvd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gzhubu.top/gttsjbbbho.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.gotoacloud.top/gtptefsslq.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yj20258888.top/gtolabipyp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.tanke756.top/gtrziorxgi.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.cqqwz.cn/gtowuzptht.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.wangdashe.top/gtjcoxgqtp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yanxiufei.cn/gtmgbccasw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.feifeiyinyue.top/gtfxnciihv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.haohaochexian.top/gtezkamrgz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.guowangkeji.top/gtgvbfxiao.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhiwuduotai.top/gtajeicdqv.html

Go:   slices.Sort(arr)
来源：http://hz.xuanzx.com/gtwnrwlcwq.html

Ruby: arr.sort
来源：http://hz.aizwys.cn/gtnlwcusnl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.cashguo.top/gtkwqjqklg.html

[N03] 快速排序（分治示例）
来源：http://hz.mhx1999.top/gtovdpyypo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xziqi.cn/gttarhxvui.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xziqi.cn/gtonkjiotk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zycfv.cn/gtoapdlwox.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.havefunace.top/gtkhvmlqfu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jlsjyb.cn/gtctgzxrmy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.xuetiantiany.cn/gtxdvkgiig.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yonumen.top/gtdiniypba.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.quarkkingdee.top/gtubybbure.html

[N04] 斐波那契数列
来源：http://hz.hnxiangtu.top/gtlyuaizxk.html


<!-- 参考信息 -->