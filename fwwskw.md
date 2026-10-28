代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.c1oappe.top/gtjcqjixci.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.shanyushiyangkeji.top/gtjevzdteh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hnqzz.top/gtmcounzfm.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.meibo888.top/gtuzbopdpn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.shanyushiyangtech.top/gtynfgkjwz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.smart0.xyz/gtlzbqrqqy.html

[J05] 时间加减（加 7 天）
来源：http://hz.meibo888.top/gtyixgbjle.html

Py:   now + timedelta(days=7)
来源：http://hz.ywan-chungtsiang.top/gtrohuwfwz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shangyingyoupin.top/gtlwnbuukq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hnxiangtu.top/gtlervarsn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.fengsongda.top/gtuuvnshmp.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.ywan-chungtsiang.top/gtpsreypuu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhixingplan.top/gtaiavsqnq.html

Ruby: Time.now + 7 * 86400
来源：http://hz.pengpengdd.cyou/gtgsooifvi.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.sweek.top/gtlfbgiyfi.html

[J06] 计算两时间之差
来源：http://hz.shuidangran.top/gtfpsopjck.html

Py:   (end - start).total_seconds()
来源：http://hz.316326.xyz/gtuzstkbbs.html

PHP:  $end->diff($start)->days;
来源：http://hz.jianghu66.top/gtqvzbtkjr.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ydzc1.top/gthdoflgts.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.birdmap.top/gtnhukusdm.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhongyouzk.top/gtdyfwqqoq.html

Go:   end.Sub(start).Hours()
来源：http://hz.nanxuanxn.top/gtocvtjxjz.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yj20258.top/gtxvdfamhc.html

C#:   (end - start).TotalSeconds
来源：http://hz.sxryk.cn/gthtcarbaj.html

[J07] 比较两个日期
来源：http://hz.cheryme.top/gtprmlirsd.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.dianchejie.cn/gtrsekjoxu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.shangyingyoupin.top/gtaucggfio.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258.top/gtbtpwerzh.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xylfe.cn/gtyhzposcm.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.tianlin.xyz/gtbdrwboir.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.nanxuanxn.top/gtvsqtkahm.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xuanzx.com/gtjxeiskdd.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yj202588.top/gtdtgmmddq.html

[J08] 提取年月日与星期
来源：http://hz.sysykeji.top/gtvhunbpkq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ivvv.top/gtqbpnsweb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xuanzx.com/gttixwxetp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.svipenyu.cn/gtevonwwda.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yj20258888.top/gtrtwdmstn.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yj20258.top/gtbgguxtdb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhongyouzk.top/gtjbfecrqd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.sxryk.cn/gtumaszkwo.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jinqigufen.top/gtawqdzfhq.html

[J09] 时区处理
来源：http://hz.sufxvd.cn/gtqxceyuir.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hfpthk.cn/gtlyqomlbn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ppjwa.cn/gtdqebwgcy.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gzhubu.top/gtaoevuzhl.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ybcxt.top/gtrvcygigr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.tanke756.top/gtrwuoixgj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.cdnleiting.top/gtsxpxzmiv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yj20258.top/gtiovuyuvh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.sufxvd.cn/gtkgmnnrds.html

[J10] 取今天 / 本月第一天
来源：http://hz.0kj1m.cn/gtcszqcwym.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.xingfuxueyuan.xyz/gtbrddpilx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ybcxt.top/gtaiwytjcs.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.feifeiyinyue.top/gtpwqngooc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cdnleiting.top/gtgozmfxpd.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jinghuilouyu.cn/gtytvigbpd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.sweek.top/gtasztdbvz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xuetiantiany.cn/gttutlkeff.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jyoumei.cn/gtmetoobwg.html

================================================================================
来源：http://hz.jinqigufen.top/gtwcuxmabj.html

K. JSON 与序列化
来源：http://hz.52xcode.cn/gtpnbtmawf.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtnjqdzlqn.html

[K01] 对象转 JSON 字符串
来源：http://hz.sxryk.cn/gtkdzgjucc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shuidangran.top/gtddwxfscq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.fengsongda.top/gtkjghtpje.html

JS:   JSON.stringify(obj)
来源：http://hz.9152youxi.cn/gtxjzdxqhb.html

TS:   JSON.stringify(obj)
来源：http://hz.guowangkeji.top/gtuwhrxxvw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.daxiang520.top/gtyjztakeh.html

Go:   json.Marshal(obj)
来源：http://hz.guowangkeji.top/gtaicnusne.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.snrcjt.cn/gtevwofgzp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jqgfzy.top/gtnxsthxxd.html

[K02] JSON 字符串转对象
来源：http://hz.jinqigufen.top/gtmnexowuv.html

Py:   json.loads(s)
来源：http://hz.haohaochexian.top/gtjmhrqyco.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jianghu66.top/gtpuolitvc.html

JS:   JSON.parse(s)
来源：http://hz.tanke756.top/gtgbdywiod.html

TS:   JSON.parse(s)
来源：http://hz.snrcjt.cn/gttpdcsebe.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zdqjudy.top/gtvligmzmo.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ppjwa.cn/gtrftqfyci.html

Ruby: JSON.parse(s)
来源：http://hz.yanxiufei.cn/gtebcqptsp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jianghu66.top/gtfrsdmley.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ivvv.top/gttbhvsomv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.gogol.net.cn/gtjtuowtal.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.nwbrower.top/gtufzsmuep.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ehwqpu.com/gtwjyoslsx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.nanxuanxn.top/gtwcpjzkij.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zhoulong.xyz/gtlrbsdhoj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yongpay.top/gtciklnxei.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.xuetiantiany.cn/gtjkssrwzn.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.mhx1999.top/gtmfvqcekg.html

[K04] 读取 JSON 文件
来源：http://hz.hysaishi.cn/gtkmmguwkx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.quarkkingdee.top/gtcgwoworh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jinyuanbaomall.cn/gtjkyyrntc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.daria6918.cn/gtwvjjlxxw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zycfv.cn/gtfvuqydpq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.meibo888.top/gtvdhpnubn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.mhx1999.top/gteekopqqj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jinqigfzy.top/gtoqmcndxu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.nanxinkj.top/gtmfmbtirp.html

[K05] 深拷贝对象
来源：http://hz.yongpay.top/gtqqoovbyi.html

Py:   copy.deepcopy(obj)
来源：http://hz.vqdsnc.cn/gtuqfmaagk.html

PHP:  unserialize(serialize($obj));
来源：http://hz.sufxvd.cn/gtydzagzif.html

JS:   structuredClone(obj)
来源：http://hz.snrcjt.cn/gtpwjautqt.html

TS:   structuredClone(obj)
来源：http://hz.cucudq.cn/gtsetiymkm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yanxiufei.cn/gtgzwixhbj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.cashguo.top/gtsjouuvwb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.cqqwz.cn/gtwgtpiguk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jqgfzy.top/gtafoxvmnf.html

[K06] 解析 URL 查询串
来源：http://hz.havefunace.top/gtcjoljeqh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.nanxuanxn.top/gtecyppbqj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jianghu66.top/gteukwjzwf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.havefunace.top/gtplweessk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.chenlongwang.top/gtkaszjzoh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jyoumei.cn/gtbbeaytto.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jqgfzy.top/gtipfspvff.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhoulong.xyz/gtczjznjeg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.daxiang520.top/gthfnvodwu.html

[K07] 进制转换
来源：http://hz.daxiang520.top/gtmhhnwdmy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.havefunace.top/gtyscourgj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hywenlv.cn/gtooukqusu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.chenzaomai.com/gtywxnqitm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.aizwys.cn/gtanlbcatv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.gaohongyu789.top/gthcjrnhod.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.vqdsnc.cn/gtcuzsppbq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.shanyushiyangkeji.top/gtzxssgxfv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.fzhhl.top/gturshlsgk.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ywan-chungtsiang.top/gttfnblbkm.html

Py:   pickle.dumps(obj)
来源：http://hz.zhijiandao.cn/gtxznzpnwn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.nanxuanxn.top/gtexmycnlm.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.daxiang520.top/gtrzsycyrp.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.smart0.xyz/gtigahprgc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yongpay.top/gtgcvliuiq.html

Go:   encoding/gob
来源：http://hz.zhengqikj.top/gtaphzuhxy.html

Ruby: Marshal.dump(obj)
来源：http://hz.wangdashe.top/gtiisgmbtw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yuxming.cn/gtrnrhpecv.html

================================================================================
来源：http://hz.fzhhl.top/gtlrkdflhv.html

L. 网络请求
来源：http://hz.quarkkingdee.top/gtjikofjnf.html

================================================================================
来源：http://hz.sysykeji.top/gtbbprzezb.html

[L01] 发送 GET 请求
来源：http://hz.gotoacloud.top/gtvemugfhx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jianghu66.top/gtxambvqcp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.xuetiantiany.cn/gtjhpylthh.html

JS:   await fetch(url)
来源：http://hz.ppjwa.cn/gtqvpuhbis.html

TS:   await fetch(url)
来源：http://hz.jqgufenzy.top/gtqfgeytag.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.xinyue.icu/gteputtyrv.html

Go:   resp, err := http.Get(url)
来源：http://hz.tianlin.xyz/gtlnkaprsh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cashguo.top/gtvfcicmtw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jqgufenzy.top/gtguoheeii.html

[L02] 发送 POST JSON
来源：http://hz.jinyuanbaomall.cn/gtucqkmffk.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jiagoushi.top/gtqkaqtccy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ehwqpu.com/gtuglhhdao.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hysaishi.cn/gteyjvhjoo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tanke756.top/gtmaayeyue.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hnqzz.top/gtkyrfbkgr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.52xcode.cn/gtwgmproxe.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yongpay.top/gtvdkbhcpl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.guowangkeji.top/gtaewjxvpv.html

[L03] 设置自定义请求头
来源：http://hz.feifeiyinyue.top/gtjdtyatwx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.guowangkeji.top/gtdupwpgwe.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ehwqpu.com/gtrymahgtd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.bjfxy.top/gtushvieju.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yvedp.cn/gttqlpyksq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.sysykeji.top/gtzycpmbhu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ydzc1.top/gtmkhnhowg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.shanyushiyangtech.top/gtukpycmxo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.0kj1m.cn/gtvikgbdrb.html

[L04] 设置超时
来源：http://hz.ehwqpu.com/gtujnyikig.html

Py:   requests.get(url, timeout=5)
来源：http://hz.aibaodan.cn/gtshxdboxc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.chenjidiqi.icu/gtdnperdtp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.vqdsnc.cn/gtnvslpwlb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hywenlv.cn/gtoktxuajl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.redwolf501.top/gtpwqzmszm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zhiwuduotai.top/gtomvlwfvd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.smart0.xyz/gtfdjvogwr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.mhx1999.top/gthxplznua.html

[L05] 上传文件（multipart）
来源：http://hz.zycfv.cn/gtkhqkjhlj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.cheryme.top/gtphssdchr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xuetiantiany.cn/gtqbppruqn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenzaomai.com/gtiplamqeh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.hfpthk.cn/gtqymtujoo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.sweek.top/gtwawtugox.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.sysykeji.top/gtrakswrfb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xuanzx.com/gtsnzwaida.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.smart0.xyz/gtcdpfdbkj.html

[L06] 解析响应为 JSON
来源：http://hz.hfpthk.cn/gtwrhcnchl.html

Py:   resp.json()
来源：http://hz.jinyuanbaomall.cn/gtwyciejnm.html

PHP:  json_decode($body, true);
来源：http://hz.zhengqikj.top/gtzklxbjkh.html

JS:   await resp.json()
来源：http://hz.hysaishi.cn/gtxmblzrnm.html

TS:   await resp.json()
来源：http://hz.jqgufenzy.top/gtkjoyefmo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.quarkkingdee.top/gtfzfmjurn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.shanyushiyangtech.top/gteoirdqeh.html

Ruby: JSON.parse(resp.body)
来源：http://hz.sxryk.cn/gtvwczivua.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ivvv.top/gtyytckypl.html

[L07] 处理 HTTP 状态码
来源：http://hz.sxryk.cn/gtskbbmckj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yueranfly.top/gtzycejdsd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.bjfxy.top/gtdcxxbess.html

JS:   resp.ok;  resp.status
来源：http://hz.zhixingplan.top/gtvzvsoode.html

TS:   resp.ok;  resp.status
来源：http://hz.feifeiyinyue.top/gtfnafuhji.html

Java: resp.statusCode()
来源：http://hz.wangdashe.top/gtlfcufwkt.html

Go:   resp.StatusCode
来源：http://hz.xingfuxueyuan.xyz/gtseofgymt.html

Ruby: resp.code.to_i
来源：http://hz.guannengcc.top/gtlbahexnp.html

C#:   (int)resp.StatusCode
来源：http://hz.ppjwa.cn/gtzwgawiqg.html

[L08] 并发请求多个地址
来源：http://hz.aizwys.cn/gtagbpvhgw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ydzc1.top/gtkwruoiqa.html

PHP:  curl_multi_init() 系列
来源：http://hz.jianghu66.top/gtlblchucl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.vqdsnc.cn/gtvvwmsiyg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.dashuyun.cn/gtaywqjzis.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hfpthk.cn/gtanpvbngj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ydzc1.top/gtcmorosoo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.shuidangran.top/gtpfsxemtw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hammf.cn/gtcwouasga.html

================================================================================
来源：http://hz.sweek.top/gtuvjjoyir.html

M. 命令行 / 进程 / 环境
来源：http://hz.ybcxt.top/gtiscnmdar.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtrqzqvqtk.html

[M01] 读取命令行参数
来源：http://hz.nanxuanxn.top/gtukycgzwg.html

Py:   sys.argv[1:]
来源：http://hz.gaohongyu789.top/gtkpchpvpo.html

PHP:  $argv;  $argc;
来源：http://hz.zhaomingkeji.xyz/gtyoukhcxe.html

JS:   process.argv.slice(2)
来源：http://hz.iojbl.cn/gtxdzbncjm.html

TS:   process.argv.slice(2)
来源：http://hz.chenzaomai.com/gtsiwhnybr.html

Java: args 数组（main 方法参数）
来源：http://hz.daria6918.cn/gtxjmcmdkz.html

Go:   os.Args[1:]
来源：http://hz.tian-w.cn/gtwbjpdurc.html

Ruby: ARGV
来源：http://hz.9152youxi.cn/gtgphohsoc.html

C#:   args 数组（Main 方法参数）
来源：http://hz.sxryk.cn/gtmbuxsdmy.html

[M02] 读取环境变量
来源：http://hz.nanxuanxn.top/gtkqtlcjxx.html

Py:   os.environ.get("HOME")
来源：http://hz.wangshuangyany.cn/gtvrqqulci.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.wangshuangyany.cn/gtnhbxdwnk.html

JS:   process.env.HOME
来源：http://hz.ehwqpu.com/gtrqitlkvi.html

TS:   process.env.HOME
来源：http://hz.gzhubu.top/gtaglvlios.html

Java: System.getenv("HOME")
来源：http://hz.yuxming.cn/gttwagjoeg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yonumen.top/gtnvompenq.html

Ruby: ENV["HOME"]
来源：http://hz.sufxvd.cn/gthmaspwjq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.kuanghao11.cn/gtpdfgjbga.html

[M03] 执行外部命令
来源：http://hz.ppjwa.cn/gtmrewfehj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.nanxuanxn.top/gtxxfdlzvf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.fzhhl.top/gtriymrtff.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ivvv.top/gtyqrmjiqq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yj20258888.top/gtkfuxjdfk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.chenlongwang.top/gtxeidcjrq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.smart0.xyz/gtipaotzrt.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shanyushiyangtech.top/gtlyjalgiy.html

C#:   Process.Start("ls", "-l");
来源：http://hz.0kj1m.cn/gtwmidrdfr.html

[M04] 获取当前工作目录
来源：http://hz.xuetiantiany.cn/gtsootescu.html

Py:   os.getcwd()
来源：http://hz.yuxming.cn/gtxqraayot.html

PHP:  getcwd();
来源：http://hz.sufxvd.cn/gtmsgrgnvq.html

JS:   process.cwd()
来源：http://hz.smart0.xyz/gtduhknbeq.html

TS:   process.cwd()
来源：http://hz.jqgufenzy.top/gtojvjchoq.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.nanxuanxn.top/gtnqxaqaui.html

Go:   os.Getwd()
来源：http://hz.hysaishi.cn/gtiraamypw.html

Ruby: Dir.pwd
来源：http://hz.nwbrower.top/gttpokmszv.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.shanyushiyangkeji.top/gtlrjoiimz.html

[M05] 设置退出码
来源：http://hz.9152youxi.cn/gtfirdobzv.html

Py:   sys.exit(1)
来源：http://hz.cucudq.cn/gtedkvdzuy.html

PHP:  exit(1);
来源：http://hz.sweek.top/gtygytyjbo.html

JS:   process.exit(1)
来源：http://hz.kuanghao11.cn/gttwqhdwib.html

TS:   process.exit(1)
来源：http://hz.hammf.cn/gtpxcnismp.html

Java: System.exit(1)
来源：http://hz.zhoulong.xyz/gtqzquxyiv.html

Go:   os.Exit(1)
来源：http://hz.daria6918.cn/gticylcduz.html

Ruby: exit 1
来源：http://hz.yuxming.cn/gtprugxbat.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.xuanzx.com/gtmemyjfsk.html

[M06] 向标准错误输出
来源：http://hz.pengpengdd.cyou/gtxzrdghuy.html

Py:   print("err", file=sys.stderr)
来源：http://hz.cashguo.top/gtunehjqvr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.vqdsnc.cn/gttabkosgr.html

JS:   console.error("err")
来源：http://hz.smart0.xyz/gtahafnfkg.html

TS:   console.error("err")
来源：http://hz.xinyue.icu/gtcjqjqhjr.html

Java: System.err.println("err")
来源：http://hz.zycfv.cn/gtdxwojnzp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.316326.xyz/gtrlvvtonc.html

Ruby: warn "err"
来源：http://hz.yuxming.cn/gtakhsiyai.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.cdnleiting.top/gtrnqkzyqk.html

[M07] 判断是否为主入口
来源：http://hz.gogol.net.cn/gtyriahgya.html

Py:   if __name__ == "__main__":
来源：http://hz.wangdashe.top/gtfmmecqgy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.hywenlv.cn/gtbhohijlx.html

JS:   require.main === module
来源：http://hz.mhx1999.top/gtqebrkqsn.html

TS:   require.main === module
来源：http://hz.fengsongda.top/gtmjohsoko.html

Java: public static void main(String[] args)
来源：http://hz.zdqjudy.top/gtfrmvgynj.html

Go:   func main()
来源：http://hz.bjfxy.top/gtvvodfbxt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.quarkkingdee.top/gtuayonyss.html

C#:   static void Main(string[] args)
来源：http://hz.snrcjt.cn/gthorlmulg.html

[M08] 获取系统与运行时信息
来源：http://hz.hnqzz.top/gtsievparq.html

Py:   platform.system();  platform.python_version()
来源：http://hz.svipenyu.cn/gtdvptvkrm.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.pycfn.com/gtaqdfriqz.html

JS:   process.platform;  process.version
来源：http://hz.xuanzx.com/gtrmmyguky.html

TS:   process.platform;  process.version
来源：http://hz.ywan-chungtsiang.top/gtmfvismdm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hongshengwenyu.top/gtlpbsbqma.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.ywan-chungtsiang.top/gtskxrxwnm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hongshengwenyu.top/gtqxyvneaq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.gaohongyu789.top/gtoowbktkk.html

================================================================================
来源：http://hz.yuxming.cn/gtfzoxialo.html

N. 数据结构与算法
来源：http://hz.chenzaomai.com/gtxozuqiaw.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtcegcfthn.html

[N01] 二分查找（有序数组）
来源：http://hz.cucudq.cn/gttbusyhol.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhixingplan.top/gtpkpzndim.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.cqqwz.cn/gtbujxcaru.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.chenjidiqi.icu/gtfquqneyp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.havefunace.top/gtsmzoixlq.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.birdmap.top/gtecklhtwm.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cheryme.top/gtdakzfavl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.quarkkingdee.top/gtkpokecvw.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jinqigufen.top/gtwljsdhht.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.xylfe.cn/gtvtbelpfi.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hysaishi.cn/gtibjjlhji.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.ydjk.org.cn/gtrkkufqsc.html


<!-- 参考信息 -->