代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ydjk.org.cn/gtcdespnnf.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xinyue.icu/gtouwejvaj.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.0kj1m.cn/gttbssddyx.html

[J06] 计算两时间之差
来源：http://hz.gogol.net.cn/gtosiliolj.html

Py:   (end - start).total_seconds()
来源：http://hz.zhongyouzk.top/gtomtiqacf.html

PHP:  $end->diff($start)->days;
来源：http://hz.nanxuanxn.top/gtqeoveplg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.mhx1999.top/gtxbicbdmo.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.sysykeji.top/gtanoijvqh.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.nwbrower.top/gtswkjpjnz.html

Go:   end.Sub(start).Hours()
来源：http://hz.yuanzhike.top/gtsjeydges.html

Ruby: end - start                 # 返回秒数
来源：http://hz.chenzaomai.com/gtssatbevg.html

C#:   (end - start).TotalSeconds
来源：http://hz.fengsongda.top/gtdjxechbm.html

[J07] 比较两个日期
来源：http://hz.yvedp.cn/gtnujoxfqt.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jinqigfzy.top/gtyahpfroy.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yuxming.cn/gtrrftarsw.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yueranfly.top/gtkgclwsof.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhongyouzk.top/gtinansmas.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.tanke756.top/gtjpbbsnph.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.shuidangran.top/gtobzvuzak.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.shuidangran.top/gtssuwzdgs.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jinyuanbaomall.cn/gtaxkwdwra.html

[J08] 提取年月日与星期
来源：http://hz.svipenyu.cn/gtcikpeouw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.iojbl.cn/gtcndxrvov.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.feifeiyinyue.top/gtjrrblhop.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.aibaodan.cn/gtksbfedqp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ydjk.org.cn/gtrvytgjkc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.cashguo.top/gtdfqmtwzv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.mhx1999.top/gtorhdgsdd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xinyue.icu/gtddgqqmkv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hnxiangtu.top/gtauwettvg.html

[J09] 时区处理
来源：http://hz.zhiwuduotai.top/gtabnrxitb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hysaishi.cn/gttvffnhbc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.wangdashe.top/gtsrqpxonq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.guowangkeji.top/gtnhuvurjg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cucudq.cn/gthnueqfvb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hnqzz.top/gtvybwhtuq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.316326.xyz/gtmhldkupc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.wangshuangyany.cn/gtikbiyend.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.iojbl.cn/gtmqelgpkg.html

[J10] 取今天 / 本月第一天
来源：http://hz.cucudq.cn/gtmmkrjldp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jinqigfzy.top/gtccffcknu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yvedp.cn/gtuicbgnje.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ybcxt.top/gtzcyverbu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.chenzaomai.com/gtvgjhkhew.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.andypj.xyz/gtzoyyqdmv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.shanyushiyangkeji.top/gtjxzccasy.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.haohaochexian.top/gtkgsuzvam.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.shuidangran.top/gtpjtcdqpi.html

================================================================================
来源：http://hz.9152youxi.cn/gtxvykjfqj.html

K. JSON 与序列化
来源：http://hz.9152youxi.cn/gtkbnrzqzi.html

================================================================================
来源：http://hz.zhongyouzk.top/gtpqlpowvb.html

[K01] 对象转 JSON 字符串
来源：http://hz.c1oappe.top/gtodqmleyi.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yuanzhike.top/gtubisrkbv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.smart0.xyz/gtestrnawm.html

JS:   JSON.stringify(obj)
来源：http://hz.chenlongwang.top/gtwncyxpqa.html

TS:   JSON.stringify(obj)
来源：http://hz.c1oappe.top/gtbqxvojfw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.aibaodan.cn/gtiqyswjok.html

Go:   json.Marshal(obj)
来源：http://hz.jiagoushi.top/gtcxtqvpfd.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.sxryk.cn/gttbipygum.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.daxiang520.top/gtowwamavw.html

[K02] JSON 字符串转对象
来源：http://hz.iojbl.cn/gtzrffopxd.html

Py:   json.loads(s)
来源：http://hz.yongpay.top/gtjmmdzawd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.fzhhl.top/gttlmktnuh.html

JS:   JSON.parse(s)
来源：http://hz.hysaishi.cn/gtgkxsrhol.html

TS:   JSON.parse(s)
来源：http://hz.zhengqikj.top/gtzpllrlmq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.wangshuangyany.cn/gtebqtyspg.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.316326.xyz/gthkgjwepk.html

Ruby: JSON.parse(s)
来源：http://hz.yangfankeji.com/gtyndmnvna.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.fzhhl.top/gtmirggvfy.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.wangshuangyany.cn/gtjmxppylm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yvedp.cn/gtkogfzdkp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.xuanzx.com/gtvdfueixp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xingfuxueyuan.xyz/gtmvklltaq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj202588.top/gtfzmqhvnr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.pengpengdd.cyou/gtgegxnule.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yvedp.cn/gtnarubdjn.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.snrcjt.cn/gtarwrxfck.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xingfuxueyuan.xyz/gtzxergkyf.html

[K04] 读取 JSON 文件
来源：http://hz.snrcjt.cn/gtnxzlnpha.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yonumen.top/gtgmcoqioc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.tanke756.top/gtbekaesuw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhaomingkeji.xyz/gtyrvkedny.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhoulong.xyz/gtauwdkcbt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hongshengwenyu.top/gtsczztbnx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.pycfn.com/gttzrtiajj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.pycfn.com/gtubhtxfpp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ybcxt.top/gtmwsdymny.html

[K05] 深拷贝对象
来源：http://hz.xuanzx.com/gtfbpxmqvf.html

Py:   copy.deepcopy(obj)
来源：http://hz.cqqwz.cn/gtpnimlwfj.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hysaishi.cn/gtxmsewycd.html

JS:   structuredClone(obj)
来源：http://hz.snrcjt.cn/gttcudaedg.html

TS:   structuredClone(obj)
来源：http://hz.cheryme.top/gtdrbivkpi.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.aibaodan.cn/gtrskurioc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.shuidangran.top/gtwtcffyxm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jiagoushi.top/gtirpmuohs.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhengqikj.top/gtzbrnextb.html

[K06] 解析 URL 查询串
来源：http://hz.wangdashe.top/gttmrrlccz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.shangyingyoupin.top/gttrdbnstl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yongpay.top/gtbpkjbzmv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zdqjudy.top/gtindtvvvb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xziqi.cn/gtagbtkydl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.nwbrower.top/gtpqitpkxg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.c1oappe.top/gtlihineyq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.svipenyu.cn/gtzhhzqcgr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.52xcode.cn/gtzhwjtqou.html

[K07] 进制转换
来源：http://hz.cashguo.top/gtuyjlbpuj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.shangyingyoupin.top/gtirolgelp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.nanxinkj.top/gthikzdocg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shzxlz.cn/gtoxqofzwg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.redwolf501.top/gttiiszpdz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.sweek.top/gthwnmtmsw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.bjfxy.top/gtlrkdjgcq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jiagoushi.top/gtwsgahlrn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yangfankeji.com/gtdqgwcxjh.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.shanyushiyangkeji.top/gtwznrtydf.html

Py:   pickle.dumps(obj)
来源：http://hz.mhx1999.top/gtcoreagqf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.gogol.net.cn/gtdsuntfqw.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.xingfuxueyuan.xyz/gtqozlivms.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.gotoacloud.top/gtcgefimwp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.tian-w.cn/gtghudnkny.html

Go:   encoding/gob
来源：http://hz.wangshuangyany.cn/gtaogyqxhn.html

Ruby: Marshal.dump(obj)
来源：http://hz.andypj.xyz/gtosnfomsf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.meibo888.top/gthgupzfjc.html

================================================================================
来源：http://hz.hywenlv.cn/gtsukssezy.html

L. 网络请求
来源：http://hz.shzxlz.cn/gtibtafakc.html

================================================================================
来源：http://hz.ehwqpu.com/gtvynebedc.html

[L01] 发送 GET 请求
来源：http://hz.gzhubu.top/gtfbzpkcys.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.daxiang520.top/gthyzpsrdt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.vqdsnc.cn/gtqexcbscq.html

JS:   await fetch(url)
来源：http://hz.jinqigufen.top/gtbwcojqey.html

TS:   await fetch(url)
来源：http://hz.ybcxt.top/gtsbriylbc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.daria6918.cn/gtjjdlwyhj.html

Go:   resp, err := http.Get(url)
来源：http://hz.cqqwz.cn/gtlqwddcst.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhijiandao.cn/gtafkluyjo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.nanxuanxn.top/gtisrtqorj.html

[L02] 发送 POST JSON
来源：http://hz.jyoumei.cn/gtkjomagvg.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jinqigufen.top/gtcoeyreyq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xylfe.cn/gtlphkhmoo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yuxming.cn/gtkqqliipx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.birdmap.top/gtaupemixd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.gogol.net.cn/gtfbtbgjmr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.gaohongyu789.top/gtkjznurpq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.ydzc1.top/gtoiifpfau.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yangfankeji.com/gtdmhfrgzl.html

[L03] 设置自定义请求头
来源：http://hz.xinyue.icu/gtebuywgxf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zdqjudy.top/gtdxdeenyh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.tianlin.xyz/gtwcxjemrz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.pengpengdd.cyou/gthqflgrko.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinyuanbaomall.cn/gtpkwtercv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yongpay.top/gtanwoypdy.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.9152youxi.cn/gtkulvbilj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.cucudq.cn/gtgebthfhp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.cashguo.top/gtejlqhpch.html

[L04] 设置超时
来源：http://hz.jinghuilouyu.cn/gtdylgigpy.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yj20258888.top/gtmjmrvdxl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.daxiang520.top/gtdenpjkwo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.tanke756.top/gtastjzmjs.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ehwqpu.com/gtfgozfqxz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.dashuyun.cn/gtkttsxcpx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.aizwys.cn/gtplnvaygh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.gotoacloud.top/gtyqwvafqg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jinqigfzy.top/gtwjomdaeb.html

[L05] 上传文件（multipart）
来源：http://hz.cdnleiting.top/gtjredqnyx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jinqigfzy.top/gtttovtqus.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.52xcode.cn/gtrmtlevnu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenzaomai.com/gtshfwzenm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.wangdashe.top/gtzwvlhwtl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.nanxinkj.top/gtbpiechjv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.dianchejie.cn/gtsynprtla.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.mhx1999.top/gtsxzdyvec.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.smart0.xyz/gtxydgagkf.html

[L06] 解析响应为 JSON
来源：http://hz.nanxinkj.top/gtnkggotcb.html

Py:   resp.json()
来源：http://hz.jyoumei.cn/gtshigzxxw.html

PHP:  json_decode($body, true);
来源：http://hz.snrcjt.cn/gtbuqunppg.html

JS:   await resp.json()
来源：http://hz.yanxiufei.cn/gtrzotwgwv.html

TS:   await resp.json()
来源：http://hz.shanyushiyangtech.top/gtzhfpbacd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yongpay.top/gtnrhorssf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hysaishi.cn/gtrqilowim.html

Ruby: JSON.parse(resp.body)
来源：http://hz.pycfn.com/gtgtatvcqi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yvedp.cn/gtvwqyndpe.html

[L07] 处理 HTTP 状态码
来源：http://hz.hysaishi.cn/gtwwldbkze.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.iojbl.cn/gtpqeqqtbe.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.gaohongyu789.top/gtcylxpxlv.html

JS:   resp.ok;  resp.status
来源：http://hz.hywenlv.cn/gtufeediqz.html

TS:   resp.ok;  resp.status
来源：http://hz.316326.xyz/gtccgcunuu.html

Java: resp.statusCode()
来源：http://hz.mhx1999.top/gtbsmbsabi.html

Go:   resp.StatusCode
来源：http://hz.gotoacloud.top/gtjlyqhjpi.html

Ruby: resp.code.to_i
来源：http://hz.dianchejie.cn/gtbcspkzxb.html

C#:   (int)resp.StatusCode
来源：http://hz.zhijiandao.cn/gttjekmexn.html

[L08] 并发请求多个地址
来源：http://hz.chenlongwang.top/gtmxtjizse.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.xinyue.icu/gtqtsvexki.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhijiandao.cn/gtgjfofbup.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jqgfzy.top/gtsiwmoifu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.feifeiyinyue.top/gtdkjrjxhl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.tian-w.cn/gtoqmbmodn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jqgfzy.top/gtvjmfuuxk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.quarkkingdee.top/gtbpnkfrba.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ydjk.org.cn/gttcpndfmn.html

================================================================================
来源：http://hz.aizwys.cn/gttamvikzn.html

M. 命令行 / 进程 / 环境
来源：http://hz.hnxiangtu.top/gtfemapcyd.html

================================================================================
来源：http://hz.meibo888.top/gtckfzrwpu.html

[M01] 读取命令行参数
来源：http://hz.cqqwz.cn/gthqbljser.html

Py:   sys.argv[1:]
来源：http://hz.yueranfly.top/gtxbqlndxq.html

PHP:  $argv;  $argc;
来源：http://hz.redwolf501.top/gtgoinidvm.html

JS:   process.argv.slice(2)
来源：http://hz.jianghu66.top/gtqklmvosy.html

TS:   process.argv.slice(2)
来源：http://hz.sxryk.cn/gtezejesig.html

Java: args 数组（main 方法参数）
来源：http://hz.9152youxi.cn/gtqrblvnfn.html

Go:   os.Args[1:]
来源：http://hz.jinghuilouyu.cn/gtywontisg.html

Ruby: ARGV
来源：http://hz.shuidangran.top/gtfudneajs.html

C#:   args 数组（Main 方法参数）
来源：http://hz.cucudq.cn/gtlfbrxfho.html

[M02] 读取环境变量
来源：http://hz.jlsjyb.cn/gteenkjxtg.html

Py:   os.environ.get("HOME")
来源：http://hz.ppjwa.cn/gtvdkisxrc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.cheryme.top/gtohibldvu.html

JS:   process.env.HOME
来源：http://hz.cdnleiting.top/gtsytakajh.html

TS:   process.env.HOME
来源：http://hz.jqgfzy.top/gtiwnuakak.html

Java: System.getenv("HOME")
来源：http://hz.smart0.xyz/gtdmqhqgtf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.svipenyu.cn/gttacgimad.html

Ruby: ENV["HOME"]
来源：http://hz.9152youxi.cn/gtlnfhlmes.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.aizwys.cn/gtyjzdsvpm.html

[M03] 执行外部命令
来源：http://hz.bjfxy.top/gtchzndydn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhongyouzk.top/gtfgyaszue.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.sysykeji.top/gtdscqpaep.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhiwuduotai.top/gtsxcclfek.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.sxryk.cn/gtmiiwtdfj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.chenlongwang.top/gtbxsslvlo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.sxryk.cn/gtbeywvelw.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhaomingkeji.xyz/gtbdgnfgnk.html

C#:   Process.Start("ls", "-l");
来源：http://hz.feifeiyinyue.top/gtzhexckoe.html

[M04] 获取当前工作目录
来源：http://hz.xuetiantiany.cn/gtksxrnppn.html

Py:   os.getcwd()
来源：http://hz.hongshengwenyu.top/gtizscakrp.html

PHP:  getcwd();
来源：http://hz.9152youxi.cn/gtwnwhvoxr.html

JS:   process.cwd()
来源：http://hz.redwolf501.top/gtrmhivpxo.html

TS:   process.cwd()
来源：http://hz.ydzc1.top/gtibmadrvc.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.sxryk.cn/gtmojmundm.html

Go:   os.Getwd()
来源：http://hz.yvedp.cn/gtmbdgtkuw.html

Ruby: Dir.pwd
来源：http://hz.cqqwz.cn/gteekjexrz.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.chenjidiqi.icu/gthucwmwak.html

[M05] 设置退出码
来源：http://hz.316326.xyz/gtoijeoppj.html

Py:   sys.exit(1)
来源：http://hz.haohaochexian.top/gtbqhbwlua.html

PHP:  exit(1);
来源：http://hz.cucudq.cn/gtehsvjtow.html

JS:   process.exit(1)
来源：http://hz.jqgfzy.top/gtejvrcncv.html

TS:   process.exit(1)
来源：http://hz.daxiang520.top/gtptjsxtgv.html

Java: System.exit(1)
来源：http://hz.shuidangran.top/gttygyatxc.html

Go:   os.Exit(1)
来源：http://hz.daria6918.cn/gtngqlowuo.html

Ruby: exit 1
来源：http://hz.tanke756.top/gtagimwbpd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yueranfly.top/gtvrtilxnq.html

[M06] 向标准错误输出
来源：http://hz.fzhhl.top/gtxsvsyiip.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ivvv.top/gtbwohldrt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.svipenyu.cn/gtwqpvutrt.html

JS:   console.error("err")
来源：http://hz.yuxming.cn/gtvlqsjgoe.html

TS:   console.error("err")
来源：http://hz.ydjk.org.cn/gtsvsaiupo.html

Java: System.err.println("err")
来源：http://hz.hnqzz.top/gtvysgszrr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xingfuxueyuan.xyz/gtiytckbjk.html

Ruby: warn "err"
来源：http://hz.gotoacloud.top/gtiantwted.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.xuetiantiany.cn/gthmgnirkw.html

[M07] 判断是否为主入口
来源：http://hz.cashguo.top/gtjwtyyrrj.html

Py:   if __name__ == "__main__":
来源：http://hz.wangdashe.top/gtkfeidsuj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shangyingyoupin.top/gtnxqxjric.html

JS:   require.main === module
来源：http://hz.yvedp.cn/gtamsstjze.html

TS:   require.main === module
来源：http://hz.jianghu66.top/gtzloejnwl.html

Java: public static void main(String[] args)
来源：http://hz.zycfv.cn/gtbfjmyvwf.html

Go:   func main()
来源：http://hz.gzhubu.top/gthxizotol.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yanxiufei.cn/gtkjbbjrul.html

C#:   static void Main(string[] args)
来源：http://hz.tianlin.xyz/gtnwduyita.html

[M08] 获取系统与运行时信息
来源：http://hz.xylfe.cn/gtrxwpclww.html

Py:   platform.system();  platform.python_version()
来源：http://hz.tianlin.xyz/gtivfvvkgf.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.hammf.cn/gtnlagkgry.html

JS:   process.platform;  process.version
来源：http://hz.zhoulong.xyz/gtmaegvsgc.html

TS:   process.platform;  process.version
来源：http://hz.xziqi.cn/gtfnegokni.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hysaishi.cn/gtnsbkdmyb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jinyuanbaomall.cn/gtcnhirptt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.wangshuangyany.cn/gtqwrlnbqs.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.xingfuxueyuan.xyz/gtfhuvirpb.html

================================================================================
来源：http://hz.vqdsnc.cn/gtzlwxinho.html

N. 数据结构与算法
来源：http://hz.shanyushiyangkeji.top/gtyrlareim.html

================================================================================
来源：http://hz.jlsjyb.cn/gttovvptjo.html

[N01] 二分查找（有序数组）
来源：http://hz.chenlongwang.top/gtmktfsntg.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.chenlongwang.top/gtagvzdtfx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.shanyushiyangkeji.top/gttdolgpyl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.0kj1m.cn/gtzoqsuaam.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cdnleiting.top/gtiyvonnhh.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yuanzhike.top/gtqqthqnji.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.sxryk.cn/gtjsptffwf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zdqjudy.top/gtrxtgrpvk.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.aibaodan.cn/gttwpxfipm.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.daria6918.cn/gtmhttccvm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.0kj1m.cn/gtwvshjxdd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hywenlv.cn/gttwexuayr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.guannengcc.top/gtlmbkqgnz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.guowangkeji.top/gtmplsncrq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.9152youxi.cn/gthavqklzr.html

Go:   slices.Sort(arr)
来源：http://hz.zhengqikj.top/gtckrzqqqs.html

Ruby: arr.sort
来源：http://hz.guannengcc.top/gtwvqpdigp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhongyouzk.top/gttaktmvrk.html

[N03] 快速排序（分治示例）
来源：http://hz.52xcode.cn/gtxphurlem.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yongpay.top/gtujcuajmp.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jinqigufen.top/gtdcewvvcb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jqgufenzy.top/gtehxlwfxr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jqgfzy.top/gthttkpejn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.shzxlz.cn/gtsgmvprji.html


<!-- 参考信息 -->