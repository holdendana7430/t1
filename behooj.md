代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yuanzhike.top/gtyzpoumbk.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yueranfly.top/gtcaceoyjj.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jlsjyb.cn/gtzmyiaeoy.html

[J06] 计算两时间之差
来源：http://hz.hfpthk.cn/gtoyribcps.html

Py:   (end - start).total_seconds()
来源：http://hz.svipenyu.cn/gtsvhsjjmu.html

PHP:  $end->diff($start)->days;
来源：http://hz.yuxming.cn/gthggatnme.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hongshengwenyu.top/gtmkwgboca.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhongyouzk.top/gtpuqipull.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.sweek.top/gtjwuuzosh.html

Go:   end.Sub(start).Hours()
来源：http://hz.nanxinkj.top/gtajievdgc.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jyoumei.cn/gtowyjbpgq.html

C#:   (end - start).TotalSeconds
来源：http://hz.fengsongda.top/gtxppnhefx.html

[J07] 比较两个日期
来源：http://hz.zhongyouzk.top/gtdfndgdxf.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yangfankeji.com/gtaywywikf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhongyouzk.top/gtxvafrgic.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.nanxuanxn.top/gtcjnfpzku.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.nanxinkj.top/gtskvwffuj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.sysykeji.top/gtlnxybmll.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jyoumei.cn/gtrrncrujp.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jlsjyb.cn/gtxocbkcqw.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.xuanzx.com/gtmcmcdzrm.html

[J08] 提取年月日与星期
来源：http://hz.birdmap.top/gtpgakeamr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.nanxuanxn.top/gtdshzbqdh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jiagoushi.top/gtccexfflm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinyuanbaomall.cn/gthuycdsei.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ydjk.org.cn/gtpktmvcww.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yvedp.cn/gtkkxgvatm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.snrcjt.cn/gtzhrbaaww.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.gaohongyu789.top/gtzextwmnp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yanxiufei.cn/gtijbpubag.html

[J09] 时区处理
来源：http://hz.chenlongwang.top/gtfbnxwieq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cashguo.top/gtwvivsaup.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.fengsongda.top/gtcknirbcs.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.feifeiyinyue.top/gtbjgmkgkd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hongshengwenyu.top/gtkzwwehdq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xylfe.cn/gtysyisfmf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.sufxvd.cn/gttmvhofds.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.shanyushiyangtech.top/gtauegkhio.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jinyuanbaomall.cn/gtbyapnvbq.html

[J10] 取今天 / 本月第一天
来源：http://hz.hnxiangtu.top/gtsprlcmiv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.andypj.xyz/gtphdluoyg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.fzhhl.top/gthbbmwpnb.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yj20258888.top/gtqhzcssmr.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cdnleiting.top/gtquotllvy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jinyuanbaomall.cn/gtvvnkpbub.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.pengpengdd.cyou/gtlejaozwc.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.dianchejie.cn/gtbjqpnnbx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.havefunace.top/gtduowczkq.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtlcvstetr.html

K. JSON 与序列化
来源：http://hz.yj20258888.top/gtglleuqdd.html

================================================================================
来源：http://hz.bjfxy.top/gtutodiogr.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhoulong.xyz/gtjxaklvfk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hfpthk.cn/gtokwqjwbx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yj20258888.top/gtijzonfiy.html

JS:   JSON.stringify(obj)
来源：http://hz.pengpengdd.cyou/gtlpzukpey.html

TS:   JSON.stringify(obj)
来源：http://hz.xuanzx.com/gtezyjjbrc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.guannengcc.top/gtujkswmoc.html

Go:   json.Marshal(obj)
来源：http://hz.tianlin.xyz/gtaghxgeoc.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.sweek.top/gtkzysvgzx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.cdnleiting.top/gtiiniueiz.html

[K02] JSON 字符串转对象
来源：http://hz.nanxinkj.top/gtgmcrtsbm.html

Py:   json.loads(s)
来源：http://hz.redwolf501.top/gteadbaxqj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.chenlongwang.top/gtclvyxuoi.html

JS:   JSON.parse(s)
来源：http://hz.cqqwz.cn/gtbkdlotjl.html

TS:   JSON.parse(s)
来源：http://hz.tian-w.cn/gtwxziqozl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zdqjudy.top/gtdykwjigc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.sxryk.cn/gtimnseuow.html

Ruby: JSON.parse(s)
来源：http://hz.shanyushiyangkeji.top/gtrxcgfvzr.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.shanyushiyangtech.top/gtcdchmbur.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.mhx1999.top/gthikxdipv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhaomingkeji.xyz/gtdmhhbprd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.chenjidiqi.icu/gttfvsdjcz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.fengsongda.top/gtrhleqkjo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.wangshuangyany.cn/gtwmkrtvin.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.tian-w.cn/gtmdgezwlt.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yj20258.top/gtnjqmrkgq.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.cucudq.cn/gtkpdyyfcl.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ybcxt.top/gtgijovshv.html

[K04] 读取 JSON 文件
来源：http://hz.yonumen.top/gtofvclnah.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.nanxinkj.top/gtrklljgbo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.iojbl.cn/gtzrijepso.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.nwbrower.top/gtxzffqveb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hnxiangtu.top/gtiaohcpkk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jinyuanbaomall.cn/gtcmrllbyl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhiwuduotai.top/gtlrxgvmlj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.sweek.top/gtdkykrnbe.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yongpay.top/gtjltkjybx.html

[K05] 深拷贝对象
来源：http://hz.haohaochexian.top/gtnswjqknw.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhaomingkeji.xyz/gtucrcigcu.html

PHP:  unserialize(serialize($obj));
来源：http://hz.shanyushiyangkeji.top/gtelqnlanq.html

JS:   structuredClone(obj)
来源：http://hz.ydzc1.top/gtzfgpztor.html

TS:   structuredClone(obj)
来源：http://hz.ppjwa.cn/gtsjvykgdg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhoulong.xyz/gtayonmand.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jiagoushi.top/gtznpjhwno.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jinghuilouyu.cn/gttnxfgtel.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.pycfn.com/gtmcxuexql.html

[K06] 解析 URL 查询串
来源：http://hz.c1oappe.top/gthccrnaxk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yongpay.top/gtqgllbdiz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.nanxuanxn.top/gtyjjblmaz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yonumen.top/gttkymlziv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nanxinkj.top/gtgqosavsi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.xziqi.cn/gtkmywsugo.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.shangyingyoupin.top/gtdsqbcwjb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.snrcjt.cn/gtmpciagyu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.316326.xyz/gtqmlaohtt.html

[K07] 进制转换
来源：http://hz.jyoumei.cn/gtojvpkqoz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.daxiang520.top/gtdadfbgpq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ydzc1.top/gtaftganaa.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.guowangkeji.top/gtspjxbkzt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhaomingkeji.xyz/gttawppygh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yangfankeji.com/gtvrnwbzky.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.sufxvd.cn/gtntokqhpj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.wangshuangyany.cn/gtqporhnnc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yj20258.top/gtlqlkqtkf.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yuanzhike.top/gtecokueis.html

Py:   pickle.dumps(obj)
来源：http://hz.316326.xyz/gtwaacqsbk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.shzxlz.cn/gtugeenkmp.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ivvv.top/gtmzhumjqs.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yj20258888.top/gtvodnabwo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhaomingkeji.xyz/gthousucax.html

Go:   encoding/gob
来源：http://hz.nanxinkj.top/gtkxprzrtp.html

Ruby: Marshal.dump(obj)
来源：http://hz.jqgufenzy.top/gtrzojchnj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.wangdashe.top/gtkwpfqmxx.html

================================================================================
来源：http://hz.zhixingplan.top/gtzdpnqqej.html

L. 网络请求
来源：http://hz.gzhubu.top/gtoawsxigc.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtzbmklzai.html

[L01] 发送 GET 请求
来源：http://hz.xingfuxueyuan.xyz/gtzgadopqd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.chenzaomai.com/gtvbhjayfg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.andypj.xyz/gtliaqsbct.html

JS:   await fetch(url)
来源：http://hz.zhongyouzk.top/gtsxjzalsp.html

TS:   await fetch(url)
来源：http://hz.gaohongyu789.top/gtfmtvtile.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ydjk.org.cn/gtvhvtpqbo.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhijiandao.cn/gtpbhxbbnt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.daxiang520.top/gtctapuqcg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zhixingplan.top/gtkhucjccw.html

[L02] 发送 POST JSON
来源：http://hz.wangdashe.top/gtzqdcoxby.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.xingfuxueyuan.xyz/gtliekymwx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hywenlv.cn/gtxsfomclx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xingfuxueyuan.xyz/gtlyqtjcaw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shanyushiyangkeji.top/gtctdkyhph.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yuxming.cn/gtwidntvxy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hfpthk.cn/gtkoopvmir.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yuanzhike.top/gtgpbhsobu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.pengpengdd.cyou/gtxrctoddb.html

[L03] 设置自定义请求头
来源：http://hz.ybcxt.top/gtslpgrayc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhiwuduotai.top/gtbnaflwte.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.snrcjt.cn/gtaxvkjdbb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.svipenyu.cn/gtfepptegz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.meibo888.top/gtpmcfwfda.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.c1oappe.top/gtkkxahcto.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.chenzaomai.com/gtmyzmzenu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.shanyushiyangkeji.top/gtzgvdeazj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hammf.cn/gtsrtkfjnu.html

[L04] 设置超时
来源：http://hz.wangshuangyany.cn/gtibemnzdn.html

Py:   requests.get(url, timeout=5)
来源：http://hz.shuidangran.top/gtpzdkifob.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.hammf.cn/gtusfyvmhn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gaohongyu789.top/gtztqtmhlk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ywan-chungtsiang.top/gtgidfrwqj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhijiandao.cn/gttbwlubqg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.chenzaomai.com/gtgfonkwzo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.tian-w.cn/gtgsdkrwkx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.shanyushiyangtech.top/gtuufhdjrd.html

[L05] 上传文件（multipart）
来源：http://hz.zdqjudy.top/gtkmydraez.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.cucudq.cn/gtxqyhnbrh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhaomingkeji.xyz/gtiooxqnve.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.cqqwz.cn/gtxqutwvfl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.316326.xyz/gtkrquohbi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.andypj.xyz/gtcuamjdmm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.shuidangran.top/gtccfvwohu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ehwqpu.com/gtmmkdvdwu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhaomingkeji.xyz/gthwrdfdkb.html

[L06] 解析响应为 JSON
来源：http://hz.jianghu66.top/gtiwpuzqqi.html

Py:   resp.json()
来源：http://hz.vqdsnc.cn/gttzauxdnj.html

PHP:  json_decode($body, true);
来源：http://hz.shuidangran.top/gtiudxlioi.html

JS:   await resp.json()
来源：http://hz.ydzc1.top/gtcenybdcn.html

TS:   await resp.json()
来源：http://hz.zhixingplan.top/gtavjtbboo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.havefunace.top/gtxjzizjvd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zhengqikj.top/gtgzbmcmkm.html

Ruby: JSON.parse(resp.body)
来源：http://hz.shanyushiyangkeji.top/gtbkomtdko.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jqgufenzy.top/gtvgabxhjk.html

[L07] 处理 HTTP 状态码
来源：http://hz.yangfankeji.com/gtcvmyirck.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xingfuxueyuan.xyz/gtwfhvydvk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.meibo888.top/gtvcwnwbxw.html

JS:   resp.ok;  resp.status
来源：http://hz.tanke756.top/gtgsmuibya.html

TS:   resp.ok;  resp.status
来源：http://hz.c1oappe.top/gtfymkkmxh.html

Java: resp.statusCode()
来源：http://hz.hammf.cn/gtzszwmnqt.html

Go:   resp.StatusCode
来源：http://hz.nwbrower.top/gtwfbuucdl.html

Ruby: resp.code.to_i
来源：http://hz.gogol.net.cn/gtbupqvqqj.html

C#:   (int)resp.StatusCode
来源：http://hz.cheryme.top/gtwewlxmns.html

[L08] 并发请求多个地址
来源：http://hz.smart0.xyz/gtcjaiepmq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hnqzz.top/gtvswveogq.html

PHP:  curl_multi_init() 系列
来源：http://hz.gzhubu.top/gttouzparf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ivvv.top/gtlfjmmcdx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinqigfzy.top/gtfaenwmau.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.iojbl.cn/gttlpvefqb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zdqjudy.top/gtfovikdqv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.aibaodan.cn/gtfpqfenuk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hysaishi.cn/gtrkbsdsjv.html

================================================================================
来源：http://hz.zhixingplan.top/gtywwkqygp.html

M. 命令行 / 进程 / 环境
来源：http://hz.yuanzhike.top/gtrndalulh.html

================================================================================
来源：http://hz.cheryme.top/gthismwsuy.html

[M01] 读取命令行参数
来源：http://hz.jqgfzy.top/gtwvpxqjrx.html

Py:   sys.argv[1:]
来源：http://hz.xuanzx.com/gtmahnpaox.html

PHP:  $argv;  $argc;
来源：http://hz.xingfuxueyuan.xyz/gthewvxadb.html

JS:   process.argv.slice(2)
来源：http://hz.ydjk.org.cn/gtzlyvbyud.html

TS:   process.argv.slice(2)
来源：http://hz.yongpay.top/gtpfaffgcn.html

Java: args 数组（main 方法参数）
来源：http://hz.9152youxi.cn/gtghmfyerk.html

Go:   os.Args[1:]
来源：http://hz.jlsjyb.cn/gtfwpdzxlx.html

Ruby: ARGV
来源：http://hz.jqgfzy.top/gticnxwsjs.html

C#:   args 数组（Main 方法参数）
来源：http://hz.quarkkingdee.top/gttxdrbola.html

[M02] 读取环境变量
来源：http://hz.chenzaomai.com/gtzuqitrln.html

Py:   os.environ.get("HOME")
来源：http://hz.guowangkeji.top/gtgwpidskq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.andypj.xyz/gtdjfjjrmu.html

JS:   process.env.HOME
来源：http://hz.gaohongyu789.top/gtqyflvvvk.html

TS:   process.env.HOME
来源：http://hz.hongshengwenyu.top/gttdbvwmzk.html

Java: System.getenv("HOME")
来源：http://hz.jinqigfzy.top/gtjuxpitqh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.cdnleiting.top/gtfkldvjcb.html

Ruby: ENV["HOME"]
来源：http://hz.316326.xyz/gtoszdmgcc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.meibo888.top/gtzwtssjbv.html

[M03] 执行外部命令
来源：http://hz.jqgfzy.top/gtfefloakn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ppjwa.cn/gtybbqfjvu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jinqigfzy.top/gtgbfesozj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.quarkkingdee.top/gthvkywdck.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zdqjudy.top/gtaqmhzieu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.nwbrower.top/gtgtzimjza.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ywan-chungtsiang.top/gtnzqobsxo.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.c1oappe.top/gtthvrgeth.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jinyuanbaomall.cn/gtvhhwkffy.html

[M04] 获取当前工作目录
来源：http://hz.zhijiandao.cn/gtggdobzlu.html

Py:   os.getcwd()
来源：http://hz.yj20258888.top/gtomfyqdws.html

PHP:  getcwd();
来源：http://hz.yonumen.top/gtegdcdlao.html

JS:   process.cwd()
来源：http://hz.ppjwa.cn/gtbxsrbieg.html

TS:   process.cwd()
来源：http://hz.jinghuilouyu.cn/gtmgzderli.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.meibo888.top/gtyvvvwoqz.html

Go:   os.Getwd()
来源：http://hz.nanxuanxn.top/gtqhxcifyj.html

Ruby: Dir.pwd
来源：http://hz.ywan-chungtsiang.top/gtehqryasv.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.gogol.net.cn/gthrywruhe.html

[M05] 设置退出码
来源：http://hz.bjfxy.top/gtdhforrmq.html

Py:   sys.exit(1)
来源：http://hz.jinyuanbaomall.cn/gtoioxsnyi.html

PHP:  exit(1);
来源：http://hz.xziqi.cn/gtsizvrkua.html

JS:   process.exit(1)
来源：http://hz.xuanzx.com/gtowgmzahx.html

TS:   process.exit(1)
来源：http://hz.zhijiandao.cn/gtqemlffdx.html

Java: System.exit(1)
来源：http://hz.cqqwz.cn/gtfdpzvdkv.html

Go:   os.Exit(1)
来源：http://hz.shuidangran.top/gtnmeqbayn.html

Ruby: exit 1
来源：http://hz.yongpay.top/gtqlcvafyc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.xziqi.cn/gtstxebloc.html

[M06] 向标准错误输出
来源：http://hz.dashuyun.cn/gtutucfqxj.html

Py:   print("err", file=sys.stderr)
来源：http://hz.0kj1m.cn/gtisjpuukq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.bjfxy.top/gthfxgkbng.html

JS:   console.error("err")
来源：http://hz.svipenyu.cn/gtqejowgyl.html

TS:   console.error("err")
来源：http://hz.jianghu66.top/gtvylmagkt.html

Java: System.err.println("err")
来源：http://hz.hywenlv.cn/gttqvhdaub.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.sweek.top/gteyovosgz.html

Ruby: warn "err"
来源：http://hz.shzxlz.cn/gtrfjbaylb.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.iojbl.cn/gtiyrvkpkl.html

[M07] 判断是否为主入口
来源：http://hz.yuxming.cn/gtwesfaaxx.html

Py:   if __name__ == "__main__":
来源：http://hz.cqqwz.cn/gtnirdeqhr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cucudq.cn/gtpezqypzn.html

JS:   require.main === module
来源：http://hz.quarkkingdee.top/gteoethrxm.html

TS:   require.main === module
来源：http://hz.cqqwz.cn/gtamnhibqb.html

Java: public static void main(String[] args)
来源：http://hz.yj202588.top/gtosqmcnzw.html

Go:   func main()
来源：http://hz.jinqigfzy.top/gtunbnvazj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhongyouzk.top/gtqchquiem.html

C#:   static void Main(string[] args)
来源：http://hz.ydzc1.top/gtpvvsolqs.html

[M08] 获取系统与运行时信息
来源：http://hz.haohaochexian.top/gtmmxswpmf.html

Py:   platform.system();  platform.python_version()
来源：http://hz.fengsongda.top/gtwmdkivys.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.hysaishi.cn/gtmftcoxhb.html

JS:   process.platform;  process.version
来源：http://hz.cdnleiting.top/gtinofzksr.html

TS:   process.platform;  process.version
来源：http://hz.tanke756.top/gtijeomtaq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jiagoushi.top/gtqhbgodil.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.meibo888.top/gtolsfxkav.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ydzc1.top/gtulbyjato.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.sxryk.cn/gtpzrpskma.html

================================================================================
来源：http://hz.jinqigfzy.top/gtuyzpbyuh.html

N. 数据结构与算法
来源：http://hz.yuanzhike.top/gtggrlfhec.html

================================================================================
来源：http://hz.yangfankeji.com/gtkvupwzpr.html

[N01] 二分查找（有序数组）
来源：http://hz.yj20258.top/gtrezlasdo.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.mhx1999.top/gtmaqmmcxa.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.shuidangran.top/gttvavyjzu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yongpay.top/gtoiuwyuuo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.9152youxi.cn/gtoznaavkq.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.sufxvd.cn/gtcewtpvyj.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.chenlongwang.top/gtfviupfer.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.svipenyu.cn/gtdsggyukb.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ybcxt.top/gtejuznpmu.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhiwuduotai.top/gtswddyrlb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cdnleiting.top/gtzbnvmumw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yangfankeji.com/gtheqkpwky.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hnxiangtu.top/gtqzpswtjq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hnqzz.top/gtkriixmxy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.nanxinkj.top/gtuygucawk.html

Go:   slices.Sort(arr)
来源：http://hz.xuetiantiany.cn/gttsqyoatl.html

Ruby: arr.sort
来源：http://hz.havefunace.top/gtvueoeiwy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ehwqpu.com/gtfoergbhd.html

[N03] 快速排序（分治示例）
来源：http://hz.sweek.top/gtqgehemwf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.chenlongwang.top/gtviggzwjo.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zdqjudy.top/gtzxygbroh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.chenzaomai.com/gtwzkkvrza.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.haohaochexian.top/gtiaiclcgu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jqgfzy.top/gtnworttnd.html


<!-- 参考信息 -->