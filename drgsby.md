代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.cdnleiting.top/gttumodgyu.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.pycfn.com/gthnnlrdty.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.chenzaomai.com/gtsvbpcswp.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.xinyue.icu/gtwyqkjjsg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xingfuxueyuan.xyz/gtexojxuuk.html

Ruby: Time.now + 7 * 86400
来源：http://hz.wangshuangyany.cn/gtaltnhpag.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.gzhubu.top/gtbxahrqbb.html

[J06] 计算两时间之差
来源：http://hz.ybcxt.top/gtdbysgdnt.html

Py:   (end - start).total_seconds()
来源：http://hz.ydzc1.top/gtzbfbnbmo.html

PHP:  $end->diff($start)->days;
来源：http://hz.xuetiantiany.cn/gtobpdvkjm.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhongyouzk.top/gtnnyvxxmx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.cheryme.top/gtsphftndg.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yanxiufei.cn/gtptzjfbfh.html

Go:   end.Sub(start).Hours()
来源：http://hz.shangyingyoupin.top/gtkkdzctsk.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zhijiandao.cn/gtecxvjsao.html

C#:   (end - start).TotalSeconds
来源：http://hz.vqdsnc.cn/gtgutnbdrg.html

[J07] 比较两个日期
来源：http://hz.yj202588.top/gtgcblfjbm.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.gaohongyu789.top/gtxqsjdged.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.snrcjt.cn/gtxaghbbnc.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.cdnleiting.top/gtcotwfboh.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jqgufenzy.top/gtjkoyaqdm.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ppjwa.cn/gtsilvhtmx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.xylfe.cn/gtiflomzbz.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.guannengcc.top/gtnqayrdpm.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.birdmap.top/gtsdnvfmtg.html

[J08] 提取年月日与星期
来源：http://hz.andypj.xyz/gtxvpjjuzn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.shanyushiyangkeji.top/gtgkgonlip.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.dianchejie.cn/gtbgojxbkz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shanyushiyangkeji.top/gtxmiebgxj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shuidangran.top/gtdfhmxbxg.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhoulong.xyz/gtkmaanrsm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.pycfn.com/gtllbskyem.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.snrcjt.cn/gtxonapcwt.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.chenjidiqi.icu/gtcbrgxrvk.html

[J09] 时区处理
来源：http://hz.guowangkeji.top/gtakzuwefx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yongpay.top/gtxesjthqm.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.cqqwz.cn/gtefzsbhwe.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yuanzhike.top/gtlimhvzzz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jqgufenzy.top/gtimauogkj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hammf.cn/gtdcnmwila.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.0kj1m.cn/gttdgduopv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.cqqwz.cn/gtbggwjgmh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shanyushiyangkeji.top/gtomuafnku.html

[J10] 取今天 / 本月第一天
来源：http://hz.svipenyu.cn/gteokdwgdj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.daxiang520.top/gtgvxuswgz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.snrcjt.cn/gtfcknktsh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.vqdsnc.cn/gtdfeapdjy.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.quarkkingdee.top/gtvdkjnaqs.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.hnqzz.top/gtrihpcqcv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.cashguo.top/gtondsvxiw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.tian-w.cn/gtkeupsclq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.tanke756.top/gtxkthxwio.html

================================================================================
来源：http://hz.xuanzx.com/gtxeietmog.html

K. JSON 与序列化
来源：http://hz.jiagoushi.top/gtniesrtba.html

================================================================================
来源：http://hz.yuxming.cn/gtmivkjyjb.html

[K01] 对象转 JSON 字符串
来源：http://hz.nanxinkj.top/gtuaifgyku.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.cdnleiting.top/gtmricxics.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.cucudq.cn/gtxkyjllrg.html

JS:   JSON.stringify(obj)
来源：http://hz.wangshuangyany.cn/gtmvsgmuvn.html

TS:   JSON.stringify(obj)
来源：http://hz.daxiang520.top/gtamukoaoy.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jinqigfzy.top/gtrpbjcaez.html

Go:   json.Marshal(obj)
来源：http://hz.smart0.xyz/gttosotkgf.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shzxlz.cn/gtnzohayev.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.svipenyu.cn/gtncmhsrhk.html

[K02] JSON 字符串转对象
来源：http://hz.cheryme.top/gtpedkjqhy.html

Py:   json.loads(s)
来源：http://hz.jiagoushi.top/gtrxsluvly.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.c1oappe.top/gtrtehqeqb.html

JS:   JSON.parse(s)
来源：http://hz.ydzc1.top/gttlsfaxix.html

TS:   JSON.parse(s)
来源：http://hz.chenzaomai.com/gtgpdeatvu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.cheryme.top/gtvitmnrqi.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hywenlv.cn/gtqomghylq.html

Ruby: JSON.parse(s)
来源：http://hz.aizwys.cn/gtgtkeuian.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.shzxlz.cn/gtnhwfcdia.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zycfv.cn/gtxwrajdxi.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zycfv.cn/gtuovrmadm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jianghu66.top/gttgqaaopd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.pycfn.com/gtpcjbojkn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhixingplan.top/gtzxkkjbia.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.pengpengdd.cyou/gtjsdnfqff.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.shzxlz.cn/gtxcucgkre.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zdqjudy.top/gtcqgamikd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.dashuyun.cn/gtbhwrrksq.html

[K04] 读取 JSON 文件
来源：http://hz.ydzc1.top/gtxhqszxeh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ehwqpu.com/gtjsxmiqmp.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yj20258.top/gtpfwcnqeu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhongyouzk.top/gtzognslhd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ppjwa.cn/gtyozqvywj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.gzhubu.top/gtypqkgvqj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yongpay.top/gtqhpcouni.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hongshengwenyu.top/gtzuuvamkh.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ywan-chungtsiang.top/gtfyvhtuos.html

[K05] 深拷贝对象
来源：http://hz.haohaochexian.top/gtvkviocis.html

Py:   copy.deepcopy(obj)
来源：http://hz.jinghuilouyu.cn/gtmcxbidju.html

PHP:  unserialize(serialize($obj));
来源：http://hz.nanxuanxn.top/gtfkncdbae.html

JS:   structuredClone(obj)
来源：http://hz.nwbrower.top/gtmqlvtnyx.html

TS:   structuredClone(obj)
来源：http://hz.jlsjyb.cn/gtygmspqzy.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jinqigfzy.top/gtvqdgtifv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.haohaochexian.top/gtmybmjiwm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jqgufenzy.top/gtxhkqsgwl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hammf.cn/gtmnqmyjoa.html

[K06] 解析 URL 查询串
来源：http://hz.chenlongwang.top/gtmdrnakpc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jiagoushi.top/gtrisgeftb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jqgufenzy.top/gtwikiopys.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.iojbl.cn/gtckorlbrw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.52xcode.cn/gtwrkquuxh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.andypj.xyz/gtzwvmgqvx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.aizwys.cn/gtmrzfsiom.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.aizwys.cn/gtzjvlwcyv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.daria6918.cn/gtktxyvhyj.html

[K07] 进制转换
来源：http://hz.cashguo.top/gtxkbqcnuj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ydzc1.top/gtbvrbznrd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.sysykeji.top/gtooqziquu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hywenlv.cn/gtqktkbpuh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.cheryme.top/gtsbqimkot.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yvedp.cn/gtmqvgbism.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jinqigfzy.top/gtpckfhksm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.svipenyu.cn/gtyslduzje.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.wangdashe.top/gtqbmkgfbo.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.nanxuanxn.top/gthyvlcbwj.html

Py:   pickle.dumps(obj)
来源：http://hz.nwbrower.top/gtkyuwmrsc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yj20258.top/gtdoxwgknc.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jqgfzy.top/gtuazzwsys.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ywan-chungtsiang.top/gtojyauxcr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.xylfe.cn/gtxjysujzn.html

Go:   encoding/gob
来源：http://hz.gotoacloud.top/gtvweudpsu.html

Ruby: Marshal.dump(obj)
来源：http://hz.shzxlz.cn/gtzggrtxov.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xinyue.icu/gtwhoeuvib.html

================================================================================
来源：http://hz.yonumen.top/gtkdbsaaqq.html

L. 网络请求
来源：http://hz.zdqjudy.top/gtorfiiipl.html

================================================================================
来源：http://hz.birdmap.top/gtelsudwhh.html

[L01] 发送 GET 请求
来源：http://hz.redwolf501.top/gtifllwazx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jqgufenzy.top/gtqqzkzjwb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yanxiufei.cn/gtyrengttz.html

JS:   await fetch(url)
来源：http://hz.jinghuilouyu.cn/gtwcpwmviw.html

TS:   await fetch(url)
来源：http://hz.yvedp.cn/gtuupsmyhr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yueranfly.top/gthrotglgk.html

Go:   resp, err := http.Get(url)
来源：http://hz.aibaodan.cn/gtjbczvava.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cashguo.top/gtolqzzkkb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yuanzhike.top/gtjxxkgpcy.html

[L02] 发送 POST JSON
来源：http://hz.yj20258888.top/gtjqjodwtx.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.guowangkeji.top/gtovtpmylf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.fengsongda.top/gtjjbvwwgf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xinyue.icu/gtlzyyniur.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhijiandao.cn/gtoxnmvxbl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ivvv.top/gttwsbdpap.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jqgfzy.top/gtazvsaelq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.tanke756.top/gtjnkkjwov.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zhaomingkeji.xyz/gtxxlohkip.html

[L03] 设置自定义请求头
来源：http://hz.cheryme.top/gtrqqukysm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.tianlin.xyz/gtwfzrhcvh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.sufxvd.cn/gtzlithxse.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj20258888.top/gtbnrbrxaw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.bjfxy.top/gtaytogkbo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.kuanghao11.cn/gtrbizpbpw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.wangshuangyany.cn/gtpqoethbd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.sweek.top/gturflvooo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zdqjudy.top/gtrqkqjbru.html

[L04] 设置超时
来源：http://hz.jinqigfzy.top/gtzduufsze.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yongpay.top/gtmogxkzjm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zhiwuduotai.top/gtgfcmbbfc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ydzc1.top/gtovvmbmkz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj20258888.top/gtcyctarur.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.tanke756.top/gtmclybjzk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.gogol.net.cn/gtuimrjphx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hywenlv.cn/gtjrhycdiq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yonumen.top/gtrsapgkye.html

[L05] 上传文件（multipart）
来源：http://hz.yvedp.cn/gtajyrjznu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhixingplan.top/gtsqhrvwch.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.52xcode.cn/gtvltedxga.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.meibo888.top/gtpnrkfrgs.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jyoumei.cn/gtryrxaxyc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xylfe.cn/gtsirclzfd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.svipenyu.cn/gtapbwlncc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.hywenlv.cn/gtzesuqtyd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zdqjudy.top/gtedxqbhmu.html

[L06] 解析响应为 JSON
来源：http://hz.ydzc1.top/gtopnindzs.html

Py:   resp.json()
来源：http://hz.nwbrower.top/gtxtzceasv.html

PHP:  json_decode($body, true);
来源：http://hz.hysaishi.cn/gtzmgjhroi.html

JS:   await resp.json()
来源：http://hz.fzhhl.top/gttubsgqcc.html

TS:   await resp.json()
来源：http://hz.yj20258888.top/gthrkjjrqi.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yj20258888.top/gtpqzvfnwz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.ydjk.org.cn/gtigfgofhp.html

Ruby: JSON.parse(resp.body)
来源：http://hz.chenlongwang.top/gtprmgxaxo.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.quarkkingdee.top/gtmaydzwjt.html

[L07] 处理 HTTP 状态码
来源：http://hz.shangyingyoupin.top/gtpzqfditl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hongshengwenyu.top/gtndgqhgfq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.gotoacloud.top/gtlstutwbx.html

JS:   resp.ok;  resp.status
来源：http://hz.nwbrower.top/gthbmlsrwt.html

TS:   resp.ok;  resp.status
来源：http://hz.ydjk.org.cn/gthvsamqru.html

Java: resp.statusCode()
来源：http://hz.tanke756.top/gtzmbehezf.html

Go:   resp.StatusCode
来源：http://hz.andypj.xyz/gthrwyohqf.html

Ruby: resp.code.to_i
来源：http://hz.ybcxt.top/gtvnhrpwrp.html

C#:   (int)resp.StatusCode
来源：http://hz.hammf.cn/gtxziballq.html

[L08] 并发请求多个地址
来源：http://hz.sysykeji.top/gtaahkwflh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jqgfzy.top/gtohnqjzaw.html

PHP:  curl_multi_init() 系列
来源：http://hz.shangyingyoupin.top/gtpcbunqzh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cqqwz.cn/gtkztdromy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cheryme.top/gtmdvyqjcj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yj202588.top/gtbrflrzuk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.sxryk.cn/gtpicagmpv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.xziqi.cn/gtuoanyutu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ybcxt.top/gtfkpnphbv.html

================================================================================
来源：http://hz.wangdashe.top/gtmakcrjsx.html

M. 命令行 / 进程 / 环境
来源：http://hz.kuanghao11.cn/gthcsqjmbd.html

================================================================================
来源：http://hz.xuanzx.com/gtmidhjvbi.html

[M01] 读取命令行参数
来源：http://hz.feifeiyinyue.top/gtwexpyxdp.html

Py:   sys.argv[1:]
来源：http://hz.nanxuanxn.top/gtupmwcdan.html

PHP:  $argv;  $argc;
来源：http://hz.yueranfly.top/gtrufufrfe.html

JS:   process.argv.slice(2)
来源：http://hz.9152youxi.cn/gtmlkibtlv.html

TS:   process.argv.slice(2)
来源：http://hz.mhx1999.top/gtgazbqyaq.html

Java: args 数组（main 方法参数）
来源：http://hz.hnxiangtu.top/gtuluwybtv.html

Go:   os.Args[1:]
来源：http://hz.sxryk.cn/gtblqnmvjn.html

Ruby: ARGV
来源：http://hz.redwolf501.top/gtalurefri.html

C#:   args 数组（Main 方法参数）
来源：http://hz.tian-w.cn/gtyvxmdcsl.html

[M02] 读取环境变量
来源：http://hz.aizwys.cn/gtlcbepgas.html

Py:   os.environ.get("HOME")
来源：http://hz.chenjidiqi.icu/gtgxzroepl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ywan-chungtsiang.top/gtexsfbofx.html

JS:   process.env.HOME
来源：http://hz.snrcjt.cn/gtwxsgqrzp.html

TS:   process.env.HOME
来源：http://hz.shuidangran.top/gtbkajkscr.html

Java: System.getenv("HOME")
来源：http://hz.andypj.xyz/gtmnyzejfe.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.ivvv.top/gtrfmrpiqv.html

Ruby: ENV["HOME"]
来源：http://hz.zycfv.cn/gtgkssvbch.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hfpthk.cn/gtolvpmrpc.html

[M03] 执行外部命令
来源：http://hz.sufxvd.cn/gtoljgsnfd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jianghu66.top/gtovuqftnv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jyoumei.cn/gtfjzrncmp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.snrcjt.cn/gtzqmdlcrg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.guowangkeji.top/gtngpudhsa.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhoulong.xyz/gtexbfvqdv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jiagoushi.top/gtcnrilmkq.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.sysykeji.top/gtahbiysfd.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yj202588.top/gtbxrtgizu.html

[M04] 获取当前工作目录
来源：http://hz.shanyushiyangkeji.top/gtvlwglkcu.html

Py:   os.getcwd()
来源：http://hz.haohaochexian.top/gtfhoxjqyv.html

PHP:  getcwd();
来源：http://hz.shanyushiyangtech.top/gtpuvdvvdm.html

JS:   process.cwd()
来源：http://hz.52xcode.cn/gtokwpfwav.html

TS:   process.cwd()
来源：http://hz.shangyingyoupin.top/gtowmdklkq.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ydjk.org.cn/gtpvjieyfe.html

Go:   os.Getwd()
来源：http://hz.wangdashe.top/gtzinsdsqp.html

Ruby: Dir.pwd
来源：http://hz.meibo888.top/gtjqmwigyq.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.fengsongda.top/gtzuiyfmvj.html

[M05] 设置退出码
来源：http://hz.zhongyouzk.top/gtfltepubf.html

Py:   sys.exit(1)
来源：http://hz.mhx1999.top/gtitfumsxq.html

PHP:  exit(1);
来源：http://hz.nanxinkj.top/gtvnhfviyv.html

JS:   process.exit(1)
来源：http://hz.aizwys.cn/gtperekmpw.html

TS:   process.exit(1)
来源：http://hz.tianlin.xyz/gtnzkmnysg.html

Java: System.exit(1)
来源：http://hz.jyoumei.cn/gtemqrvadp.html

Go:   os.Exit(1)
来源：http://hz.meibo888.top/gtgakbtpgm.html

Ruby: exit 1
来源：http://hz.0kj1m.cn/gtuasobmih.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.andypj.xyz/gtekpdyeyk.html

[M06] 向标准错误输出
来源：http://hz.tianlin.xyz/gtvdyhfkzp.html

Py:   print("err", file=sys.stderr)
来源：http://hz.cucudq.cn/gtzrvneenq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.gzhubu.top/gtealphlee.html

JS:   console.error("err")
来源：http://hz.pycfn.com/gtbitkjcpt.html

TS:   console.error("err")
来源：http://hz.hnqzz.top/gtyvvnbbnv.html

Java: System.err.println("err")
来源：http://hz.0kj1m.cn/gtqahjsuhi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.shangyingyoupin.top/gtjudakrgv.html

Ruby: warn "err"
来源：http://hz.c1oappe.top/gtzavifbvh.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.nwbrower.top/gtpwdwayuq.html

[M07] 判断是否为主入口
来源：http://hz.tian-w.cn/gteinohfok.html

Py:   if __name__ == "__main__":
来源：http://hz.guowangkeji.top/gtjtmdbfmo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.daxiang520.top/gtfsrpestv.html

JS:   require.main === module
来源：http://hz.svipenyu.cn/gthwdcdaah.html

TS:   require.main === module
来源：http://hz.hywenlv.cn/gtmutmodfx.html

Java: public static void main(String[] args)
来源：http://hz.ppjwa.cn/gtemgyklml.html

Go:   func main()
来源：http://hz.0kj1m.cn/gtvixjidrc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.aibaodan.cn/gtvpmblrmi.html

C#:   static void Main(string[] args)
来源：http://hz.iojbl.cn/gttqnnbnta.html

[M08] 获取系统与运行时信息
来源：http://hz.jinghuilouyu.cn/gtyljqmmmr.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jqgufenzy.top/gtdgqurykq.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ivvv.top/gtyvigmkif.html

JS:   process.platform;  process.version
来源：http://hz.tianlin.xyz/gtppbfyunf.html

TS:   process.platform;  process.version
来源：http://hz.xinyue.icu/gtymkovwcr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.ybcxt.top/gtvwlghwyu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xingfuxueyuan.xyz/gtrprnnfcu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.smart0.xyz/gtigztwdpb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.wangdashe.top/gtwkiqhfxr.html

================================================================================
来源：http://hz.yuxming.cn/gtdajlmtoe.html

N. 数据结构与算法
来源：http://hz.yueranfly.top/gtpnzusyum.html

================================================================================
来源：http://hz.jianghu66.top/gtvtifvrln.html

[N01] 二分查找（有序数组）
来源：http://hz.yj202588.top/gtktehatzz.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jiagoushi.top/gtyctymtjn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.chenjidiqi.icu/gtakhsjtsq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yongpay.top/gtjfauqcqu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.snrcjt.cn/gtjhvzpoce.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.gzhubu.top/gttyccuryz.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yonumen.top/gtzkijqvfr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.shanyushiyangtech.top/gtlxyubsjq.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jinyuanbaomall.cn/gtvhcizjvx.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ppjwa.cn/gtdraqhuko.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jqgfzy.top/gtedhjsgrh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhijiandao.cn/gtoenbhzin.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.daria6918.cn/gtniromnyn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xziqi.cn/gtsrnatchn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hysaishi.cn/gtjawgekoz.html

Go:   slices.Sort(arr)
来源：http://hz.andypj.xyz/gtquickwpa.html

Ruby: arr.sort
来源：http://hz.xziqi.cn/gthhcskuus.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.wangshuangyany.cn/gtgfmjvjqm.html

[N03] 快速排序（分治示例）
来源：http://hz.9152youxi.cn/gtgqjbbwel.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.aizwys.cn/gtybcvnnbd.html


<!-- 参考信息 -->