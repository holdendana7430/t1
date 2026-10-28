代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ydzc1.top/gtsqjsgfyt.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.ywan-chungtsiang.top/gtrpyrgknd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zdqjudy.top/gtbmpydkks.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.shanyushiyangtech.top/gttkejihsw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.vqdsnc.cn/gtpnusoqwq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.0kj1m.cn/gttfonqhyf.html

[J05] 时间加减（加 7 天）
来源：http://hz.ppjwa.cn/gtxynuaxbv.html

Py:   now + timedelta(days=7)
来源：http://hz.sweek.top/gtcazcxrgg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ehwqpu.com/gtuwqdbrpo.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.pengpengdd.cyou/gtixkmklid.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhoulong.xyz/gtlearljbl.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.andypj.xyz/gtylibazlf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xinyue.icu/gtevbrnpys.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xziqi.cn/gtceunajov.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.hnxiangtu.top/gtuurtotdt.html

[J06] 计算两时间之差
来源：http://hz.shuidangran.top/gtcrnxsixp.html

Py:   (end - start).total_seconds()
来源：http://hz.hongshengwenyu.top/gttiuavsly.html

PHP:  $end->diff($start)->days;
来源：http://hz.yuanzhike.top/gtxwqfxquk.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhongyouzk.top/gtmhatkbya.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.xinyue.icu/gtmssobeek.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cashguo.top/gtcmxbdhyd.html

Go:   end.Sub(start).Hours()
来源：http://hz.wangdashe.top/gtdwtfxqti.html

Ruby: end - start                 # 返回秒数
来源：http://hz.chenzaomai.com/gtnaigkrcr.html

C#:   (end - start).TotalSeconds
来源：http://hz.cheryme.top/gtpdwbhpxy.html

[J07] 比较两个日期
来源：http://hz.tanke756.top/gtlriqqvai.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hnxiangtu.top/gtecjhrmpi.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.316326.xyz/gtpqpbuqqr.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.chenzaomai.com/gtynrxrlef.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.tanke756.top/gtjkyfaorz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xinyue.icu/gtoutoklkw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hnqzz.top/gtgftsccgs.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yongpay.top/gtbdymztfz.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.cdnleiting.top/gtknigkcho.html

[J08] 提取年月日与星期
来源：http://hz.c1oappe.top/gtqjxtsfke.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hywenlv.cn/gtpzmxrjfw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.daxiang520.top/gtwyolwduj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yanxiufei.cn/gtxkjuweas.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhiwuduotai.top/gtppatwcta.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.kuanghao11.cn/gtctqfaeqh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.sufxvd.cn/gtkeoggjln.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zdqjudy.top/gtrmdnhdfe.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.daria6918.cn/gtfcbryyux.html

[J09] 时区处理
来源：http://hz.sxryk.cn/gtvbzzzlmm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.daria6918.cn/gtzvylutlx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.shanyushiyangtech.top/gtxenoitdh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.0kj1m.cn/gtkyyqmvii.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhengqikj.top/gtvhwoxplg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jyoumei.cn/gtosotrmuj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.tanke756.top/gtqqdotxto.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.sweek.top/gtyxjyklkx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.dashuyun.cn/gtqhbrqtzb.html

[J10] 取今天 / 本月第一天
来源：http://hz.nanxuanxn.top/gtztkdwhij.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.xuanzx.com/gthlmiqelw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.sweek.top/gtzwpyhukg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zycfv.cn/gtkatwcghw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.chenjidiqi.icu/gtpjvrgynk.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.sweek.top/gtbhiiaupu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.shanyushiyangtech.top/gtdubzsfov.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.meibo888.top/gtpricbzfw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jiagoushi.top/gthsxxdvho.html

================================================================================
来源：http://hz.iojbl.cn/gtwlalthth.html

K. JSON 与序列化
来源：http://hz.gotoacloud.top/gtqylzhmvc.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtgaakuoxo.html

[K01] 对象转 JSON 字符串
来源：http://hz.yj20258888.top/gtlkprfnzm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jinghuilouyu.cn/gtialfmxey.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.shangyingyoupin.top/gtzhvqhqkx.html

JS:   JSON.stringify(obj)
来源：http://hz.zhiwuduotai.top/gtgrixnpbj.html

TS:   JSON.stringify(obj)
来源：http://hz.ydzc1.top/gtldwcngcz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhaomingkeji.xyz/gtyygyoddi.html

Go:   json.Marshal(obj)
来源：http://hz.sxryk.cn/gtonvuipji.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.guowangkeji.top/gtnvkgzsha.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hysaishi.cn/gtsqnvphvk.html

[K02] JSON 字符串转对象
来源：http://hz.smart0.xyz/gtoxyrayme.html

Py:   json.loads(s)
来源：http://hz.ehwqpu.com/gtxxseefzp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jyoumei.cn/gtbcybdzyz.html

JS:   JSON.parse(s)
来源：http://hz.hongshengwenyu.top/gtyvyizplg.html

TS:   JSON.parse(s)
来源：http://hz.jiagoushi.top/gttdjldgyt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.pycfn.com/gtohtsglfc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.pengpengdd.cyou/gtmucdzhrq.html

Ruby: JSON.parse(s)
来源：http://hz.52xcode.cn/gturltwbll.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.cdnleiting.top/gttafintko.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhengqikj.top/gtgjurxhhz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hnxiangtu.top/gtxtgxbdlh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.feifeiyinyue.top/gtqoecdojo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zycfv.cn/gtaiwdvkey.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.316326.xyz/gtsjjhxqtt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jinqigufen.top/gtfiiubgqn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yanxiufei.cn/gtaelbuczf.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jlsjyb.cn/gtwyldapie.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jyoumei.cn/gtiaiwgsnh.html

[K04] 读取 JSON 文件
来源：http://hz.snrcjt.cn/gtozpjhknc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.shanyushiyangkeji.top/gtbgvflfms.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ywan-chungtsiang.top/gtnzbddxdi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.tianlin.xyz/gtvkfhdzcz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hnqzz.top/gtxipxoocg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yanxiufei.cn/gtsqnkxypu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.guowangkeji.top/gtkryfbacr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.gaohongyu789.top/gtafcjesbp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.meibo888.top/gtxggqtbbg.html

[K05] 深拷贝对象
来源：http://hz.chenlongwang.top/gtbbeabmiy.html

Py:   copy.deepcopy(obj)
来源：http://hz.ybcxt.top/gtjzmfhfdx.html

PHP:  unserialize(serialize($obj));
来源：http://hz.feifeiyinyue.top/gtxjyljekp.html

JS:   structuredClone(obj)
来源：http://hz.iojbl.cn/gtmukdfmda.html

TS:   structuredClone(obj)
来源：http://hz.zhoulong.xyz/gttlvabdtf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.aibaodan.cn/gtdmexghgx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.cqqwz.cn/gthbquthlr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.gzhubu.top/gtohbtehot.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.316326.xyz/gtjxpfwjpo.html

[K06] 解析 URL 查询串
来源：http://hz.hfpthk.cn/gtrqobjubw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.aibaodan.cn/gtzehrevyq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yuxming.cn/gtmzgvinhz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.vqdsnc.cn/gtilsuokki.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cucudq.cn/gtodjhybiq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.9152youxi.cn/gtaqrxehbu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yonumen.top/gtbfuesiov.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zdqjudy.top/gtnglcxvjc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.hnxiangtu.top/gtjovqwyma.html

[K07] 进制转换
来源：http://hz.birdmap.top/gtxfqkofxi.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.xziqi.cn/gtgcovkczm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hywenlv.cn/gtzvszfzry.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.cqqwz.cn/gtimjygaav.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.sxryk.cn/gtczrsbiyy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.tanke756.top/gtrtqcqzhh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jinqigfzy.top/gtxbimtgnh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.chenzaomai.com/gtfcpftyso.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.gzhubu.top/gtwmjijjwz.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.hammf.cn/gtcgwldpnv.html

Py:   pickle.dumps(obj)
来源：http://hz.pycfn.com/gtbsndzpbj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.svipenyu.cn/gtrwulcgyz.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.xuetiantiany.cn/gtryftoxer.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.shanyushiyangkeji.top/gtkcaelqjy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ywan-chungtsiang.top/gtdgwcerrb.html

Go:   encoding/gob
来源：http://hz.gaohongyu789.top/gtplsdzfxl.html

Ruby: Marshal.dump(obj)
来源：http://hz.ivvv.top/gtvjdpggbi.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.quarkkingdee.top/gtykrwzcxu.html

================================================================================
来源：http://hz.cheryme.top/gtexxacktb.html

L. 网络请求
来源：http://hz.feifeiyinyue.top/gtykoqjwik.html

================================================================================
来源：http://hz.aibaodan.cn/gtuovguonz.html

[L01] 发送 GET 请求
来源：http://hz.hnqzz.top/gtbypkooge.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.wangshuangyany.cn/gtamroimth.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.gaohongyu789.top/gtvvyckxaa.html

JS:   await fetch(url)
来源：http://hz.ivvv.top/gtmzzasdmq.html

TS:   await fetch(url)
来源：http://hz.snrcjt.cn/gtaayomugq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhiwuduotai.top/gtxlnldewk.html

Go:   resp, err := http.Get(url)
来源：http://hz.feifeiyinyue.top/gteechhffh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jyoumei.cn/gtbpmuigdc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yvedp.cn/gtrgvkejgd.html

[L02] 发送 POST JSON
来源：http://hz.daria6918.cn/gtlqvwqrbr.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.cucudq.cn/gtgpsdqwsq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.sweek.top/gtnpuvdbfa.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.andypj.xyz/gtqejatore.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shzxlz.cn/gtirhejhzb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.sweek.top/gtyfddjink.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.chenzaomai.com/gtcfgovhpt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yj20258888.top/gtrtqnbbcc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hnxiangtu.top/gtqdpgvhky.html

[L03] 设置自定义请求头
来源：http://hz.dianchejie.cn/gtipcwykvc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ppjwa.cn/gtxmtvyebg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ivvv.top/gtccwjaztx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jyoumei.cn/gteymitawv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.tanke756.top/gtwgacwxmp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhijiandao.cn/gtrvjvsmsn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.sysykeji.top/gtjmertkwn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jiagoushi.top/gtmozrfjqf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.shuidangran.top/gtqlmfcawu.html

[L04] 设置超时
来源：http://hz.haohaochexian.top/gtwmeapasp.html

Py:   requests.get(url, timeout=5)
来源：http://hz.shuidangran.top/gtksnpterc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.fengsongda.top/gtztgnuzwb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.tianlin.xyz/gtianbummg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.wangdashe.top/gtpnlexqal.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.dianchejie.cn/gtqvysesur.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hongshengwenyu.top/gtktcuqaly.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.gotoacloud.top/gtjonammur.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jinqigfzy.top/gtmcigdgak.html

[L05] 上传文件（multipart）
来源：http://hz.svipenyu.cn/gtjfbqjtab.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.shangyingyoupin.top/gtjlxubmfa.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.tian-w.cn/gtjtvjefqx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hnxiangtu.top/gtwuarhtkj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ehwqpu.com/gtcdnhmfji.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.316326.xyz/gtktaegqlp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhijiandao.cn/gtfogvkqum.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jinghuilouyu.cn/gtrdjlofug.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.xuetiantiany.cn/gttwrepctm.html

[L06] 解析响应为 JSON
来源：http://hz.mhx1999.top/gtnbybvdgg.html

Py:   resp.json()
来源：http://hz.tianlin.xyz/gtriucnvqj.html

PHP:  json_decode($body, true);
来源：http://hz.feifeiyinyue.top/gttbdckcnu.html

JS:   await resp.json()
来源：http://hz.yanxiufei.cn/gthecxnzbb.html

TS:   await resp.json()
来源：http://hz.ydjk.org.cn/gtbgfqndjw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.pycfn.com/gtltdkacxg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.feifeiyinyue.top/gtxjavsbkm.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jyoumei.cn/gtdrqkabdv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.9152youxi.cn/gtvfaubuad.html

[L07] 处理 HTTP 状态码
来源：http://hz.redwolf501.top/gthtapjdde.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yonumen.top/gtgclkshdw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.tianlin.xyz/gtzektrcze.html

JS:   resp.ok;  resp.status
来源：http://hz.hongshengwenyu.top/gtmpemotem.html

TS:   resp.ok;  resp.status
来源：http://hz.yj20258888.top/gtkzdyxrqn.html

Java: resp.statusCode()
来源：http://hz.haohaochexian.top/gtoiwkymcg.html

Go:   resp.StatusCode
来源：http://hz.nwbrower.top/gttrgnwoox.html

Ruby: resp.code.to_i
来源：http://hz.bjfxy.top/gticfodfcc.html

C#:   (int)resp.StatusCode
来源：http://hz.wangdashe.top/gtbuaaehhy.html

[L08] 并发请求多个地址
来源：http://hz.zhoulong.xyz/gthifangvm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.vqdsnc.cn/gtxpoixlhy.html

PHP:  curl_multi_init() 系列
来源：http://hz.wangshuangyany.cn/gtlquuljet.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sysykeji.top/gtqbxnkste.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xziqi.cn/gtmisjnjak.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jinghuilouyu.cn/gtgrknnpkp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.kuanghao11.cn/gtjotitxdy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ivvv.top/gtqbbmruug.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.wangshuangyany.cn/gtituthozn.html

================================================================================
来源：http://hz.wangdashe.top/gthetrpsnk.html

M. 命令行 / 进程 / 环境
来源：http://hz.shanyushiyangtech.top/gtxsykxwog.html

================================================================================
来源：http://hz.jianghu66.top/gtkxlzvvqw.html

[M01] 读取命令行参数
来源：http://hz.zhoulong.xyz/gtwbcvqhwh.html

Py:   sys.argv[1:]
来源：http://hz.xziqi.cn/gtyaobevns.html

PHP:  $argv;  $argc;
来源：http://hz.jinghuilouyu.cn/gtvfbfhixz.html

JS:   process.argv.slice(2)
来源：http://hz.yuxming.cn/gtjyrnrehc.html

TS:   process.argv.slice(2)
来源：http://hz.52xcode.cn/gtmsetfnep.html

Java: args 数组（main 方法参数）
来源：http://hz.daxiang520.top/gturirfaru.html

Go:   os.Args[1:]
来源：http://hz.quarkkingdee.top/gtzwrouwes.html

Ruby: ARGV
来源：http://hz.fengsongda.top/gtfgfnjxgi.html

C#:   args 数组（Main 方法参数）
来源：http://hz.xziqi.cn/gtvftwovuh.html

[M02] 读取环境变量
来源：http://hz.xuanzx.com/gtpjcenbei.html

Py:   os.environ.get("HOME")
来源：http://hz.hammf.cn/gtjpspefzr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.sysykeji.top/gtyunjentm.html

JS:   process.env.HOME
来源：http://hz.xingfuxueyuan.xyz/gtdqlbinve.html

TS:   process.env.HOME
来源：http://hz.kuanghao11.cn/gtahxffxwf.html

Java: System.getenv("HOME")
来源：http://hz.chenzaomai.com/gtraopqhqb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.daxiang520.top/gtqqzqfbbp.html

Ruby: ENV["HOME"]
来源：http://hz.shanyushiyangtech.top/gtkhmrneqo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shanyushiyangtech.top/gtqbhtgatr.html

[M03] 执行外部命令
来源：http://hz.sweek.top/gtrlhrpidx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.quarkkingdee.top/gtxrmtulvi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.aizwys.cn/gtgetucwyh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.snrcjt.cn/gtkekwmvbu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xingfuxueyuan.xyz/gtiwzqfyns.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.9152youxi.cn/gtmechqnym.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.andypj.xyz/gtolwydvnj.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhoulong.xyz/gtxkspgfys.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jinqigfzy.top/gtxjjxlnjz.html

[M04] 获取当前工作目录
来源：http://hz.hywenlv.cn/gtirhiyjux.html

Py:   os.getcwd()
来源：http://hz.hongshengwenyu.top/gtrtbagmyg.html

PHP:  getcwd();
来源：http://hz.yongpay.top/gthrcybnvj.html

JS:   process.cwd()
来源：http://hz.jqgufenzy.top/gtwkgneqpe.html

TS:   process.cwd()
来源：http://hz.tianlin.xyz/gtlyritnpu.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.0kj1m.cn/gtidzyixen.html

Go:   os.Getwd()
来源：http://hz.wangdashe.top/gtjfibbbga.html

Ruby: Dir.pwd
来源：http://hz.xziqi.cn/gtehhkyimz.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhengqikj.top/gtwcclxjwa.html

[M05] 设置退出码
来源：http://hz.chenzaomai.com/gtgfsaiyzb.html

Py:   sys.exit(1)
来源：http://hz.nanxuanxn.top/gtgmyhicin.html

PHP:  exit(1);
来源：http://hz.redwolf501.top/gtdgeterkz.html

JS:   process.exit(1)
来源：http://hz.jyoumei.cn/gtxtayslmh.html

TS:   process.exit(1)
来源：http://hz.aizwys.cn/gtfokdzran.html

Java: System.exit(1)
来源：http://hz.birdmap.top/gthazqfupr.html

Go:   os.Exit(1)
来源：http://hz.ydzc1.top/gtcyikfamy.html

Ruby: exit 1
来源：http://hz.dashuyun.cn/gtkuglesrd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jinqigufen.top/gtifpgppvp.html

[M06] 向标准错误输出
来源：http://hz.ydjk.org.cn/gtqsjbnqgu.html

Py:   print("err", file=sys.stderr)
来源：http://hz.daxiang520.top/gtapyumrth.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jianghu66.top/gtnuzztoeg.html

JS:   console.error("err")
来源：http://hz.xingfuxueyuan.xyz/gtkozxqozx.html

TS:   console.error("err")
来源：http://hz.yuanzhike.top/gtblbgomrr.html

Java: System.err.println("err")
来源：http://hz.jinyuanbaomall.cn/gtmbldhtfu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.redwolf501.top/gtwimdwmeg.html

Ruby: warn "err"
来源：http://hz.cdnleiting.top/gtionmyger.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.tian-w.cn/gtlhkoynmc.html

[M07] 判断是否为主入口
来源：http://hz.yueranfly.top/gtpklexvvz.html

Py:   if __name__ == "__main__":
来源：http://hz.sufxvd.cn/gtairajiev.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xylfe.cn/gtuguetmtx.html

JS:   require.main === module
来源：http://hz.fengsongda.top/gtzbegtfae.html

TS:   require.main === module
来源：http://hz.zhongyouzk.top/gtlskzpfxz.html

Java: public static void main(String[] args)
来源：http://hz.sufxvd.cn/gtkcxzupkg.html

Go:   func main()
来源：http://hz.chenzaomai.com/gtatyxxmrz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cqqwz.cn/gtfgwffsbc.html

C#:   static void Main(string[] args)
来源：http://hz.316326.xyz/gtrassoulb.html

[M08] 获取系统与运行时信息
来源：http://hz.cucudq.cn/gtwpmkaxqp.html

Py:   platform.system();  platform.python_version()
来源：http://hz.redwolf501.top/gtqubvkzae.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhengqikj.top/gtynwxrlwg.html

JS:   process.platform;  process.version
来源：http://hz.cashguo.top/gtrunluogv.html

TS:   process.platform;  process.version
来源：http://hz.jinqigfzy.top/gtdhwcvlnr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.cashguo.top/gtalgtowgs.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.dashuyun.cn/gtgskbfahs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jinyuanbaomall.cn/gtkvvvignn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.redwolf501.top/gtffltjmsl.html

================================================================================
来源：http://hz.xylfe.cn/gtrwgaxhsg.html

N. 数据结构与算法
来源：http://hz.nanxinkj.top/gtgbybeyhb.html

================================================================================
来源：http://hz.jiagoushi.top/gtenfkkkox.html

[N01] 二分查找（有序数组）
来源：http://hz.ivvv.top/gtilhgyclb.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yvedp.cn/gtgysgljjl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.cheryme.top/gtjlccqdev.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.chenjidiqi.icu/gttkyslbgm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.chenlongwang.top/gtzktunfsx.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.sufxvd.cn/gttnlfieon.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jiagoushi.top/gtweimjmeq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yj202588.top/gtrzbogxho.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.gotoacloud.top/gtpzppjttj.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jqgfzy.top/gtrnywbnrm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhiwuduotai.top/gtiirvevye.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.shangyingyoupin.top/gtffdstftd.html


<!-- 参考信息 -->