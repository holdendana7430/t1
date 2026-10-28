代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.nwbrower.top/gtdykmmmec.html

Ruby: Time.now + 7 * 86400
来源：http://hz.aibaodan.cn/gtrtctwgkf.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jianghu66.top/gtlnefxjgz.html

[J06] 计算两时间之差
来源：http://hz.meibo888.top/gtfgdesfxx.html

Py:   (end - start).total_seconds()
来源：http://hz.yanxiufei.cn/gteghpfpqz.html

PHP:  $end->diff($start)->days;
来源：http://hz.meibo888.top/gtzeceboyo.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhaomingkeji.xyz/gtulktsbtc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.pycfn.com/gtsiwqqmjy.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.xuetiantiany.cn/gtuzmqxchx.html

Go:   end.Sub(start).Hours()
来源：http://hz.hongshengwenyu.top/gtqfjbfmdh.html

Ruby: end - start                 # 返回秒数
来源：http://hz.sxryk.cn/gtiebclzpz.html

C#:   (end - start).TotalSeconds
来源：http://hz.snrcjt.cn/gtvqhvcuqo.html

[J07] 比较两个日期
来源：http://hz.redwolf501.top/gtegiqzuqy.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.gogol.net.cn/gtavhlebkd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.mhx1999.top/gtgltwskxu.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.wangshuangyany.cn/gtkwdmbodu.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zycfv.cn/gtahbnxzmv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jqgfzy.top/gtzpvonqkb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hongshengwenyu.top/gtxoadceul.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xylfe.cn/gtlkbjjnbl.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.tian-w.cn/gtlnyywsfj.html

[J08] 提取年月日与星期
来源：http://hz.nanxuanxn.top/gtgubdwyrv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.xylfe.cn/gtakpilvfh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.vqdsnc.cn/gtdtysbwnu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.cucudq.cn/gthtvwloyy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.kuanghao11.cn/gtgkopoxur.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.kuanghao11.cn/gtwiafdtln.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jinqigfzy.top/gtkcnjzxub.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.gaohongyu789.top/gtpaemwzet.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ybcxt.top/gttgpotusp.html

[J09] 时区处理
来源：http://hz.bjfxy.top/gtvmnvaiwd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.tianlin.xyz/gtnvcujwpm.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.shanyushiyangkeji.top/gtdpequujt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj202588.top/gtgouqohpm.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinyuanbaomall.cn/gthwfbfofp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhoulong.xyz/gtcqnwxoqi.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.cashguo.top/gtfgxygjzo.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yuxming.cn/gtxapvugve.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shuidangran.top/gtseapiwmj.html

[J10] 取今天 / 本月第一天
来源：http://hz.jyoumei.cn/gtsuycxlrj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.guowangkeji.top/gtrdfbipfg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.shanyushiyangkeji.top/gtxfljgfgn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jinyuanbaomall.cn/gtstirohvc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhijiandao.cn/gtspcfbtuz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.cheryme.top/gtxkylcbfu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yj202588.top/gtmqrhupwk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hongshengwenyu.top/gtnwnoxaqi.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.shuidangran.top/gtswazgjhi.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtcubttkhr.html

K. JSON 与序列化
来源：http://hz.daria6918.cn/gtxjcpioax.html

================================================================================
来源：http://hz.andypj.xyz/gtmitwepcn.html

[K01] 对象转 JSON 字符串
来源：http://hz.quarkkingdee.top/gtiqzonazk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jyoumei.cn/gtabfshsil.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.wangshuangyany.cn/gtzahqwngq.html

JS:   JSON.stringify(obj)
来源：http://hz.shuidangran.top/gtnmmrwxcg.html

TS:   JSON.stringify(obj)
来源：http://hz.52xcode.cn/gtmhgvigbf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jinqigufen.top/gtztovoczz.html

Go:   json.Marshal(obj)
来源：http://hz.chenjidiqi.icu/gtyzcadgii.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.316326.xyz/gtcihgcmbl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.shuidangran.top/gtvglcgyqc.html

[K02] JSON 字符串转对象
来源：http://hz.ppjwa.cn/gtsrsrnoyj.html

Py:   json.loads(s)
来源：http://hz.haohaochexian.top/gtmarzoanb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jiagoushi.top/gtsehsrnvc.html

JS:   JSON.parse(s)
来源：http://hz.jinghuilouyu.cn/gtgrbrlfkj.html

TS:   JSON.parse(s)
来源：http://hz.tanke756.top/gteeaquhcs.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hysaishi.cn/gtxlditkcw.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhiwuduotai.top/gthcwjmtms.html

Ruby: JSON.parse(s)
来源：http://hz.yj20258.top/gtmunmughx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yongpay.top/gtvrdggqay.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.cheryme.top/gtpkgvsrbg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.cqqwz.cn/gtcsttroey.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.wangdashe.top/gtzsjntisn.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jqgufenzy.top/gtgdmqkbds.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.shzxlz.cn/gtpcudggvi.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.wangdashe.top/gtzludkeiu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yangfankeji.com/gtcciqvwrx.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ivvv.top/gtiqhpjjdy.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ydjk.org.cn/gtylxjyhoi.html

[K04] 读取 JSON 文件
来源：http://hz.zhongyouzk.top/gtqezlosjp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ydjk.org.cn/gthvrzsmdw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.aibaodan.cn/gtbvwesvaa.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.wangshuangyany.cn/gtdwhklifs.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zycfv.cn/gtvtpyuslx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.daxiang520.top/gthurzhklg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.mhx1999.top/gtxryjbkib.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.bjfxy.top/gtuoohtqbq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.daxiang520.top/gtgzgvoyky.html

[K05] 深拷贝对象
来源：http://hz.jiagoushi.top/gtzhramsfz.html

Py:   copy.deepcopy(obj)
来源：http://hz.dashuyun.cn/gticgggwzw.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hnxiangtu.top/gtmxwekpkl.html

JS:   structuredClone(obj)
来源：http://hz.sufxvd.cn/gtdjgvpomj.html

TS:   structuredClone(obj)
来源：http://hz.gzhubu.top/gtjkdetznh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hywenlv.cn/gtmcuemjlk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ywan-chungtsiang.top/gtnlctczag.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ydzc1.top/gtdewtwzrp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.shuidangran.top/gtkelwejwy.html

[K06] 解析 URL 查询串
来源：http://hz.ybcxt.top/gtwhrnsrcp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.shangyingyoupin.top/gtbowvbtgi.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xylfe.cn/gtprkwovzz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tian-w.cn/gtqxqgobwr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tian-w.cn/gtqhgduusj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhaomingkeji.xyz/gtaxvrvuzk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.guowangkeji.top/gtrqsjgwpw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jianghu66.top/gtflngbguu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.meibo888.top/gtichfmdwm.html

[K07] 进制转换
来源：http://hz.ydjk.org.cn/gtehifclsv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.fengsongda.top/gtsbjlyyzd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.tanke756.top/gtcupkgexn.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yueranfly.top/gtedqjdijq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhijiandao.cn/gtpcgalkkr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.dianchejie.cn/gtbcqeqjal.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xuetiantiany.cn/gtwgpvrsjx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xziqi.cn/gtsrvnujcr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jianghu66.top/gtqogcfvig.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.daria6918.cn/gtypeysgkd.html

Py:   pickle.dumps(obj)
来源：http://hz.xziqi.cn/gtphmeinne.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.sufxvd.cn/gtdcwlorkd.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhiwuduotai.top/gtxkbfjggo.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.chenzaomai.com/gtnhhgdocx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jyoumei.cn/gtufdulchv.html

Go:   encoding/gob
来源：http://hz.yueranfly.top/gtmshfgtir.html

Ruby: Marshal.dump(obj)
来源：http://hz.pycfn.com/gtuiicmcwj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.chenlongwang.top/gtyznxekln.html

================================================================================
来源：http://hz.jqgfzy.top/gtthdgcdzl.html

L. 网络请求
来源：http://hz.guowangkeji.top/gtlmfaxuqf.html

================================================================================
来源：http://hz.gogol.net.cn/gtbsieffrj.html

[L01] 发送 GET 请求
来源：http://hz.andypj.xyz/gtkyfurkke.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jqgfzy.top/gtihnegcwm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yongpay.top/gtoczmrijx.html

JS:   await fetch(url)
来源：http://hz.andypj.xyz/gtwtoebfyi.html

TS:   await fetch(url)
来源：http://hz.fengsongda.top/gtwdmxnjsv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.meibo888.top/gtoyqloirf.html

Go:   resp, err := http.Get(url)
来源：http://hz.zycfv.cn/gtwcngvjyc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.gogol.net.cn/gtreuldhzx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yj20258888.top/gtusvrgsja.html

[L02] 发送 POST JSON
来源：http://hz.9152youxi.cn/gtclapfcrt.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.shuidangran.top/gtwxnlbcfq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.aibaodan.cn/gtyukumxpo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xuanzx.com/gtbzwztzxj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yvedp.cn/gtgyaqvadg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yonumen.top/gtvjefujyo.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.9152youxi.cn/gtkupbheqx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.hammf.cn/gtvfvesbpj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.smart0.xyz/gtjzskhhsi.html

[L03] 设置自定义请求头
来源：http://hz.ydzc1.top/gtqzbvrlqr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.fzhhl.top/gtjctcmfng.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.meibo888.top/gtrzlxflzi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj20258.top/gtcfgatnag.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yangfankeji.com/gtsqizgmsn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.aibaodan.cn/gttcufjqhw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.cashguo.top/gtjmefjkqf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.gogol.net.cn/gtgcpcohlo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yanxiufei.cn/gtevdfebdq.html

[L04] 设置超时
来源：http://hz.yongpay.top/gtduskykhn.html

Py:   requests.get(url, timeout=5)
来源：http://hz.smart0.xyz/gtkconwzob.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zhixingplan.top/gthkkugakw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shuidangran.top/gtiusfazbz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinyuanbaomall.cn/gtlboxnayz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.cheryme.top/gtnmxpteke.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yueranfly.top/gtzjhcedzw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.aizwys.cn/gtmsmrwjws.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.9152youxi.cn/gtztgovsud.html

[L05] 上传文件（multipart）
来源：http://hz.xuetiantiany.cn/gtbwhazeuh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.ppjwa.cn/gtlsrjugwa.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.shuidangran.top/gtctfmrqwl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.daria6918.cn/gtgupvkvyf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ivvv.top/gtshcwjmig.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xylfe.cn/gtsxnlielj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.snrcjt.cn/gtrezpmudx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yanxiufei.cn/gtwduogwsb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yanxiufei.cn/gtljcdicbi.html

[L06] 解析响应为 JSON
来源：http://hz.chenjidiqi.icu/gtzmsatchd.html

Py:   resp.json()
来源：http://hz.sxryk.cn/gttvzuszfa.html

PHP:  json_decode($body, true);
来源：http://hz.shanyushiyangtech.top/gtwelmoipl.html

JS:   await resp.json()
来源：http://hz.yuxming.cn/gtmhqkznne.html

TS:   await resp.json()
来源：http://hz.daxiang520.top/gtayocdmxh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.sysykeji.top/gtbenabhly.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xuetiantiany.cn/gtcczblpgq.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jinghuilouyu.cn/gtdrycqtdo.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.vqdsnc.cn/gtgwmpydng.html

[L07] 处理 HTTP 状态码
来源：http://hz.meibo888.top/gtzjlzbidx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yvedp.cn/gtisgvfdta.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jqgufenzy.top/gtkhjblmsi.html

JS:   resp.ok;  resp.status
来源：http://hz.ivvv.top/gtwyadeocq.html

TS:   resp.ok;  resp.status
来源：http://hz.zhijiandao.cn/gtnqbeqpbk.html

Java: resp.statusCode()
来源：http://hz.iojbl.cn/gtyoucgxyc.html

Go:   resp.StatusCode
来源：http://hz.hywenlv.cn/gtnvvvfoou.html

Ruby: resp.code.to_i
来源：http://hz.zhaomingkeji.xyz/gtgkmrfylm.html

C#:   (int)resp.StatusCode
来源：http://hz.chenzaomai.com/gtdzgmzldr.html

[L08] 并发请求多个地址
来源：http://hz.gogol.net.cn/gtgwotfwbg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jyoumei.cn/gtoljdyujs.html

PHP:  curl_multi_init() 系列
来源：http://hz.ydjk.org.cn/gtcgpqyifr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zycfv.cn/gtcivfsxdp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yj202588.top/gtjbbqidzg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hnqzz.top/gtxhivfvsv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.shuidangran.top/gtjzrqljvc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hfpthk.cn/gtidqoecki.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.cashguo.top/gtxueegwpy.html

================================================================================
来源：http://hz.havefunace.top/gtzwlwoksk.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhijiandao.cn/gttdudtkmx.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gttaaabkwp.html

[M01] 读取命令行参数
来源：http://hz.ppjwa.cn/gtpwafwiyb.html

Py:   sys.argv[1:]
来源：http://hz.zhongyouzk.top/gtuxmvwrzz.html

PHP:  $argv;  $argc;
来源：http://hz.gotoacloud.top/gtbxpumrpw.html

JS:   process.argv.slice(2)
来源：http://hz.nanxuanxn.top/gtzpttrgkj.html

TS:   process.argv.slice(2)
来源：http://hz.ywan-chungtsiang.top/gtajgpgxsy.html

Java: args 数组（main 方法参数）
来源：http://hz.chenzaomai.com/gtjyoqgibu.html

Go:   os.Args[1:]
来源：http://hz.xinyue.icu/gtxfzdzrcw.html

Ruby: ARGV
来源：http://hz.chenlongwang.top/gtvhrtcave.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yj20258888.top/gtudjzcfja.html

[M02] 读取环境变量
来源：http://hz.xingfuxueyuan.xyz/gtlryevyzo.html

Py:   os.environ.get("HOME")
来源：http://hz.zhaomingkeji.xyz/gtxtrdktwg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hfpthk.cn/gtezdbjyou.html

JS:   process.env.HOME
来源：http://hz.jyoumei.cn/gtkhbldtge.html

TS:   process.env.HOME
来源：http://hz.daria6918.cn/gtkhrppsfn.html

Java: System.getenv("HOME")
来源：http://hz.hywenlv.cn/gtjrxfiwtg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yvedp.cn/gtkmixifjn.html

Ruby: ENV["HOME"]
来源：http://hz.wangdashe.top/gtpjwzbjak.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.daria6918.cn/gtcvwqjvea.html

[M03] 执行外部命令
来源：http://hz.zhongyouzk.top/gtkkrqbtyg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhijiandao.cn/gtsdwztwto.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.fzhhl.top/gtqwzisprq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jqgufenzy.top/gtysqwqkis.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jiagoushi.top/gtfbfztgdx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.nanxuanxn.top/gtmenbjmuo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ppjwa.cn/gtflrpggha.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.cashguo.top/gthpsobvxz.html

C#:   Process.Start("ls", "-l");
来源：http://hz.andypj.xyz/gtmyyndeim.html

[M04] 获取当前工作目录
来源：http://hz.hywenlv.cn/gtmlhbxrvr.html

Py:   os.getcwd()
来源：http://hz.pengpengdd.cyou/gtinknajov.html

PHP:  getcwd();
来源：http://hz.sysykeji.top/gtjglsuqzb.html

JS:   process.cwd()
来源：http://hz.ydjk.org.cn/gtxpjlvuoe.html

TS:   process.cwd()
来源：http://hz.cashguo.top/gtayodcpuo.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.iojbl.cn/gtbovsdokl.html

Go:   os.Getwd()
来源：http://hz.zycfv.cn/gtbwslqqfx.html

Ruby: Dir.pwd
来源：http://hz.zhaomingkeji.xyz/gtptwqfguz.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.feifeiyinyue.top/gtrlkcubsj.html

[M05] 设置退出码
来源：http://hz.chenlongwang.top/gtwieowifl.html

Py:   sys.exit(1)
来源：http://hz.gzhubu.top/gtljoudffo.html

PHP:  exit(1);
来源：http://hz.zdqjudy.top/gtclntyykg.html

JS:   process.exit(1)
来源：http://hz.zhengqikj.top/gtgotkmwrz.html

TS:   process.exit(1)
来源：http://hz.ydjk.org.cn/gtllisgzoe.html

Java: System.exit(1)
来源：http://hz.sweek.top/gtytnxongh.html

Go:   os.Exit(1)
来源：http://hz.gzhubu.top/gtpejzajjh.html

Ruby: exit 1
来源：http://hz.zhijiandao.cn/gtvheviwmr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.aibaodan.cn/gttelctgjt.html

[M06] 向标准错误输出
来源：http://hz.yonumen.top/gtdsoeucpp.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ppjwa.cn/gtxwhxrrim.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhiwuduotai.top/gtqxqfbilt.html

JS:   console.error("err")
来源：http://hz.yj20258.top/gtfzqifbxv.html

TS:   console.error("err")
来源：http://hz.xziqi.cn/gtobsencld.html

Java: System.err.println("err")
来源：http://hz.zhaomingkeji.xyz/gtynqohwfz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xziqi.cn/gtiyavhqli.html

Ruby: warn "err"
来源：http://hz.jqgufenzy.top/gtlszpdlas.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.havefunace.top/gthgcxgami.html

[M07] 判断是否为主入口
来源：http://hz.xylfe.cn/gtjnfjvrik.html

Py:   if __name__ == "__main__":
来源：http://hz.redwolf501.top/gtwuezdquc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.meibo888.top/gtgybxvkqq.html

JS:   require.main === module
来源：http://hz.cdnleiting.top/gtdiokungi.html

TS:   require.main === module
来源：http://hz.gogol.net.cn/gtdfytisqn.html

Java: public static void main(String[] args)
来源：http://hz.xingfuxueyuan.xyz/gtabddodeu.html

Go:   func main()
来源：http://hz.ehwqpu.com/gthzdabkot.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yueranfly.top/gtjwgtibqb.html

C#:   static void Main(string[] args)
来源：http://hz.316326.xyz/gtpysuryqr.html

[M08] 获取系统与运行时信息
来源：http://hz.shuidangran.top/gtkwdublou.html

Py:   platform.system();  platform.python_version()
来源：http://hz.svipenyu.cn/gtbgkzbpmo.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.fzhhl.top/gtzzpxngzo.html

JS:   process.platform;  process.version
来源：http://hz.9152youxi.cn/gtngpmffpq.html

TS:   process.platform;  process.version
来源：http://hz.xylfe.cn/gtryvkbzgs.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhijiandao.cn/gtcirytzrl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jinqigufen.top/gtfmobmdmh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.xuetiantiany.cn/gtrqzxyeed.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.sweek.top/gtoxccxvhl.html

================================================================================
来源：http://hz.aizwys.cn/gtdnzgpqzz.html

N. 数据结构与算法
来源：http://hz.hammf.cn/gtuvljgsnf.html

================================================================================
来源：http://hz.sxryk.cn/gtttqlvjji.html

[N01] 二分查找（有序数组）
来源：http://hz.guannengcc.top/gtpctphefu.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gtvdsjqctx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.guowangkeji.top/gtewqudrsx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ydjk.org.cn/gtnvipmula.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.nanxuanxn.top/gtnqvkaodu.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.redwolf501.top/gtlmubsitu.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.bjfxy.top/gteblpqjiz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.feifeiyinyue.top/gthylyrviv.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jinyuanbaomall.cn/gtximqigyj.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.redwolf501.top/gtpuckcesf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jqgfzy.top/gtutlcdrbs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.sweek.top/gttqmvmgzm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.mhx1999.top/gteojimzht.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shuidangran.top/gtbbzfgddf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.vqdsnc.cn/gthctukmuc.html

Go:   slices.Sort(arr)
来源：http://hz.aibaodan.cn/gtuzfevihi.html

Ruby: arr.sort
来源：http://hz.zhengqikj.top/gthjmjpoab.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.aizwys.cn/gtmkeylrfp.html

[N03] 快速排序（分治示例）
来源：http://hz.xuetiantiany.cn/gtrssmgvgc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xuanzx.com/gtuowugkze.html

PHP:  // 递归实现，或用 usort
来源：http://hz.cqqwz.cn/gthpbsojmu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yvedp.cn/gtscrhnxev.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.feifeiyinyue.top/gtwjvsokix.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinyuanbaomall.cn/gtfoptyetl.html


<!-- 参考信息 -->