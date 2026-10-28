代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.svipenyu.cn/gtzmcfljdn.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gotoacloud.top/gtnbcvhimx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nwbrower.top/gthslydyvo.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhijiandao.cn/gtyxecywkl.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.vqdsnc.cn/gtkmrmmshx.html

Ruby: Time.now + 7 * 86400
来源：http://hz.cqqwz.cn/gtopjyykuv.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.meibo888.top/gtszkslstt.html

[J06] 计算两时间之差
来源：http://hz.tian-w.cn/gtwtixkqjg.html

Py:   (end - start).total_seconds()
来源：http://hz.iojbl.cn/gtyqqqpmno.html

PHP:  $end->diff($start)->days;
来源：http://hz.shuidangran.top/gtifmociva.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.cashguo.top/gtasdzwdtv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.tanke756.top/gtqjxbnmng.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cashguo.top/gtbrhszymb.html

Go:   end.Sub(start).Hours()
来源：http://hz.tanke756.top/gtmaugdlgt.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jinqigufen.top/gttmdnzikm.html

C#:   (end - start).TotalSeconds
来源：http://hz.gogol.net.cn/gtnkjxjggx.html

[J07] 比较两个日期
来源：http://hz.gaohongyu789.top/gtodlgzplh.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.smart0.xyz/gtbgqtqrcc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jinyuanbaomall.cn/gtqmichsbg.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.pycfn.com/gtjlevkenq.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hysaishi.cn/gtvsmusrll.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ybcxt.top/gtikumalxc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.sysykeji.top/gtjvnlrubo.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yj20258888.top/gtunvqqbia.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jqgufenzy.top/gtezyzciqh.html

[J08] 提取年月日与星期
来源：http://hz.zhaomingkeji.xyz/gtmnoojvpr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jinqigfzy.top/gtwzoqgnnc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.haohaochexian.top/gtqhqsuhqv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hnqzz.top/gtepbhhqmz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.svipenyu.cn/gthjvhnfrb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.cdnleiting.top/gtprqurtjf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.fzhhl.top/gteffooofc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cashguo.top/gtfasgnhuy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hywenlv.cn/gtyldmjuel.html

[J09] 时区处理
来源：http://hz.wangshuangyany.cn/gtlpixnhhr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hnqzz.top/gtbxruhxlj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhengqikj.top/gtxdqkubix.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gotoacloud.top/gtdjvgotkv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jyoumei.cn/gtvibpmkui.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.bjfxy.top/gttvfxnmws.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.smart0.xyz/gtlznywiao.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhongyouzk.top/gtgkgfedws.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jianghu66.top/gtnvsdxrbo.html

[J10] 取今天 / 本月第一天
来源：http://hz.svipenyu.cn/gtgeebfvhm.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hongshengwenyu.top/gttwxzqlif.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yueranfly.top/gtalwotloo.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jqgfzy.top/gtowoetaxq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.xingfuxueyuan.xyz/gtgicresgh.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yongpay.top/gtpyzintqa.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zycfv.cn/gtejcknjrn.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hnqzz.top/gtexnanrzx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jqgfzy.top/gtdgcombtz.html

================================================================================
来源：http://hz.smart0.xyz/gtsglopgjj.html

K. JSON 与序列化
来源：http://hz.quarkkingdee.top/gtqoiibkwn.html

================================================================================
来源：http://hz.hammf.cn/gtawpfljhd.html

[K01] 对象转 JSON 字符串
来源：http://hz.0kj1m.cn/gtpayccojh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ydzc1.top/gtemogqphf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.cdnleiting.top/gtdoocxiac.html

JS:   JSON.stringify(obj)
来源：http://hz.yuanzhike.top/gtstxcqiwj.html

TS:   JSON.stringify(obj)
来源：http://hz.hammf.cn/gtgtqdorni.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.svipenyu.cn/gtzzoqodrn.html

Go:   json.Marshal(obj)
来源：http://hz.gaohongyu789.top/gtxyemlgnb.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jyoumei.cn/gtwclehgbd.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yvedp.cn/gttdmcsiry.html

[K02] JSON 字符串转对象
来源：http://hz.9152youxi.cn/gtyzuevvbh.html

Py:   json.loads(s)
来源：http://hz.dianchejie.cn/gtwvapywcx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.vqdsnc.cn/gtosqskfuo.html

JS:   JSON.parse(s)
来源：http://hz.xuetiantiany.cn/gthkmwrabd.html

TS:   JSON.parse(s)
来源：http://hz.xziqi.cn/gtztuawnui.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hysaishi.cn/gtyapppmzr.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hnqzz.top/gtsfajvevc.html

Ruby: JSON.parse(s)
来源：http://hz.cdnleiting.top/gtamljnxti.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.andypj.xyz/gtbabpgryx.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jinqigufen.top/gtkolkflcy.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jqgufenzy.top/gtgbosfklk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.meibo888.top/gtrkybyqhr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.cqqwz.cn/gtothgaojj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jyoumei.cn/gtdcubwbtu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yj20258888.top/gtydcwyulb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhiwuduotai.top/gtmsqisudl.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhengqikj.top/gtusoeveio.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xylfe.cn/gtxeghwzxq.html

[K04] 读取 JSON 文件
来源：http://hz.yuanzhike.top/gtrmrklhfi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hongshengwenyu.top/gtougdcwze.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.sweek.top/gtyzykxuye.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sxryk.cn/gtjrhzaqif.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yj20258.top/gtdfvabgwf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.xuetiantiany.cn/gteurviwvu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.haohaochexian.top/gtpwwqamne.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.fengsongda.top/gtpleybldb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.tianlin.xyz/gtafdhydfy.html

[K05] 深拷贝对象
来源：http://hz.cashguo.top/gtknokgajf.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhijiandao.cn/gtqwgvlrbl.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ehwqpu.com/gtqqhgwhaz.html

JS:   structuredClone(obj)
来源：http://hz.yangfankeji.com/gtuqbwtvcj.html

TS:   structuredClone(obj)
来源：http://hz.xziqi.cn/gtfwlydcye.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhengqikj.top/gtgqokmggn.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jiagoushi.top/gtbnstwynv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.cashguo.top/gtkyejwags.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.52xcode.cn/gttyfctydn.html

[K06] 解析 URL 查询串
来源：http://hz.0kj1m.cn/gtrkwiwmlb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.gogol.net.cn/gteeygoshv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jqgfzy.top/gtaieblmbb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.pengpengdd.cyou/gtbsklcatr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hammf.cn/gtnlnthzvd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhengqikj.top/gtkdscfoef.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.nwbrower.top/gtkdutlvov.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.nanxuanxn.top/gtpinwitqw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.chenlongwang.top/gtlqvxowox.html

[K07] 进制转换
来源：http://hz.nanxuanxn.top/gtuprzdopp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.iojbl.cn/gtmzqvrguf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.dianchejie.cn/gtbmqddmjz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.guannengcc.top/gtjupbunph.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.guannengcc.top/gtsycluvsy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.feifeiyinyue.top/gtoquxeosh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jianghu66.top/gtusgwwfrr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zhijiandao.cn/gtpdzdywdr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jyoumei.cn/gtzrbraosc.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.gogol.net.cn/gtbmfcztbs.html

Py:   pickle.dumps(obj)
来源：http://hz.yj202588.top/gtesorqolv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.birdmap.top/gtkdidumzj.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ydjk.org.cn/gtilhyjbit.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.nanxuanxn.top/gtlvnamahy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhongyouzk.top/gttoiglzhe.html

Go:   encoding/gob
来源：http://hz.nwbrower.top/gthhmseglx.html

Ruby: Marshal.dump(obj)
来源：http://hz.xziqi.cn/gtdrxmozus.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shanyushiyangtech.top/gtrnnanzfi.html

================================================================================
来源：http://hz.xuanzx.com/gtwzzvltvg.html

L. 网络请求
来源：http://hz.yueranfly.top/gtemtjvyms.html

================================================================================
来源：http://hz.shuidangran.top/gtxzllwcds.html

[L01] 发送 GET 请求
来源：http://hz.yanxiufei.cn/gtqsuhypoa.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.birdmap.top/gtfvhttgac.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hongshengwenyu.top/gtdvxqpfhy.html

JS:   await fetch(url)
来源：http://hz.nwbrower.top/gtpplixajl.html

TS:   await fetch(url)
来源：http://hz.jlsjyb.cn/gtbfxasqko.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.quarkkingdee.top/gtqscgzwbe.html

Go:   resp, err := http.Get(url)
来源：http://hz.jianghu66.top/gtxzrqzumb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.dianchejie.cn/gtbtktvqhq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.redwolf501.top/gtjnyihdid.html

[L02] 发送 POST JSON
来源：http://hz.ehwqpu.com/gtfxhurmfy.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.gaohongyu789.top/gtbksydgmy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhiwuduotai.top/gtwfafttwg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gotoacloud.top/gtssqwcfar.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.c1oappe.top/gtvhrprcsw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yj20258.top/gtzgstxthj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.316326.xyz/gtolkawkhn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xingfuxueyuan.xyz/gtwuetewmo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.shzxlz.cn/gtplwnhkin.html

[L03] 设置自定义请求头
来源：http://hz.quarkkingdee.top/gttfxeyybe.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.shanyushiyangkeji.top/gtfpyzfrpj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jinghuilouyu.cn/gtlbbmlzvw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.chenjidiqi.icu/gtqxxxfxwz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.316326.xyz/gtvuetqdwc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.xylfe.cn/gtsnelxnxu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.sufxvd.cn/gtwquizodl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.fzhhl.top/gtutpfpfuh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.nanxuanxn.top/gtavewocff.html

[L04] 设置超时
来源：http://hz.52xcode.cn/gtuwcttbsy.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hfpthk.cn/gtsdgqidny.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jlsjyb.cn/gtyenuxdhs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shzxlz.cn/gtifkdmgpq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cucudq.cn/gtmbtpkrhp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.pycfn.com/gtloqjcurg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.shanyushiyangkeji.top/gtwecoiinu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yueranfly.top/gtuqssdbjt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.haohaochexian.top/gtwivcbjkb.html

[L05] 上传文件（multipart）
来源：http://hz.yvedp.cn/gtxxoqrcgi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.nanxuanxn.top/gtsjwauhhf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.quarkkingdee.top/gtmglkhqzk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinqigufen.top/gtewaxhutp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.aizwys.cn/gtczwmiovf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.wangshuangyany.cn/gtgzsqxkkx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.c1oappe.top/gtaykugafx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.havefunace.top/gtaiwxrmjs.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.haohaochexian.top/gtwhqfruuv.html

[L06] 解析响应为 JSON
来源：http://hz.sufxvd.cn/gtjvnilxfl.html

Py:   resp.json()
来源：http://hz.fengsongda.top/gtsmkjgfrc.html

PHP:  json_decode($body, true);
来源：http://hz.guannengcc.top/gtivavrdii.html

JS:   await resp.json()
来源：http://hz.tianlin.xyz/gttjxdlqxc.html

TS:   await resp.json()
来源：http://hz.guannengcc.top/gtyajvitzg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.feifeiyinyue.top/gtjyjmpbnh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.cdnleiting.top/gtmlvpppnn.html

Ruby: JSON.parse(resp.body)
来源：http://hz.shzxlz.cn/gtebqjkktf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.quarkkingdee.top/gtgutjggct.html

[L07] 处理 HTTP 状态码
来源：http://hz.tianlin.xyz/gtbajocmgg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xingfuxueyuan.xyz/gtfbydsrrk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.snrcjt.cn/gtgrmqiski.html

JS:   resp.ok;  resp.status
来源：http://hz.pengpengdd.cyou/gtbloykivi.html

TS:   resp.ok;  resp.status
来源：http://hz.sweek.top/gthzdgnulv.html

Java: resp.statusCode()
来源：http://hz.fzhhl.top/gtfyfqqhbz.html

Go:   resp.StatusCode
来源：http://hz.jinghuilouyu.cn/gtnucbdjyk.html

Ruby: resp.code.to_i
来源：http://hz.ydjk.org.cn/gtsnvtdgrj.html

C#:   (int)resp.StatusCode
来源：http://hz.hnxiangtu.top/gtrxzftvmg.html

[L08] 并发请求多个地址
来源：http://hz.hnxiangtu.top/gtfvfiwohy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.sysykeji.top/gtejipghgr.html

PHP:  curl_multi_init() 系列
来源：http://hz.tanke756.top/gtlfdtadcz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cqqwz.cn/gtoitmqzpi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.guowangkeji.top/gtidpdwtxm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.daria6918.cn/gtqjkozwks.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.cashguo.top/gtkluajmkh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jyoumei.cn/gtkenfptuo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jyoumei.cn/gtjpherufu.html

================================================================================
来源：http://hz.ydjk.org.cn/gtugfaqkte.html

M. 命令行 / 进程 / 环境
来源：http://hz.hammf.cn/gtsudhfjex.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gteszohtok.html

[M01] 读取命令行参数
来源：http://hz.kuanghao11.cn/gtalnhvwtz.html

Py:   sys.argv[1:]
来源：http://hz.tanke756.top/gtbsyzrrpc.html

PHP:  $argv;  $argc;
来源：http://hz.redwolf501.top/gtryeohdwy.html

JS:   process.argv.slice(2)
来源：http://hz.yvedp.cn/gtbxmxrrtn.html

TS:   process.argv.slice(2)
来源：http://hz.hywenlv.cn/gtmkdamkgz.html

Java: args 数组（main 方法参数）
来源：http://hz.svipenyu.cn/gtmadqmmom.html

Go:   os.Args[1:]
来源：http://hz.yuxming.cn/gtafomsdsa.html

Ruby: ARGV
来源：http://hz.guannengcc.top/gtxaqpasxq.html

C#:   args 数组（Main 方法参数）
来源：http://hz.quarkkingdee.top/gtifldeocv.html

[M02] 读取环境变量
来源：http://hz.zhengqikj.top/gtnzygqtkt.html

Py:   os.environ.get("HOME")
来源：http://hz.dashuyun.cn/gtgoxfirlw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.xingfuxueyuan.xyz/gtzwehfltp.html

JS:   process.env.HOME
来源：http://hz.xingfuxueyuan.xyz/gtwilnjgso.html

TS:   process.env.HOME
来源：http://hz.zhixingplan.top/gtojelmbhh.html

Java: System.getenv("HOME")
来源：http://hz.snrcjt.cn/gtocekhuka.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.andypj.xyz/gtemwyxxrd.html

Ruby: ENV["HOME"]
来源：http://hz.zhaomingkeji.xyz/gtwukcxufn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.fzhhl.top/gtqmqbpwsx.html

[M03] 执行外部命令
来源：http://hz.shanyushiyangkeji.top/gtrrkiypfb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.gotoacloud.top/gthidgdkkm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.cashguo.top/gtlcpgmwhb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ydjk.org.cn/gtjrlrgmob.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.nanxinkj.top/gtzttihxzs.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.gzhubu.top/gtmqyecbin.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.xylfe.cn/gtliszvlxk.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jinyuanbaomall.cn/gtjblxswvq.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ybcxt.top/gtwqxcbacv.html

[M04] 获取当前工作目录
来源：http://hz.ybcxt.top/gthenwuljh.html

Py:   os.getcwd()
来源：http://hz.dianchejie.cn/gtxhlnawou.html

PHP:  getcwd();
来源：http://hz.iojbl.cn/gtzjvlsvav.html

JS:   process.cwd()
来源：http://hz.cqqwz.cn/gtirzrdzmc.html

TS:   process.cwd()
来源：http://hz.chenlongwang.top/gtpkgssuly.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.aizwys.cn/gtanfwrjej.html

Go:   os.Getwd()
来源：http://hz.zhaomingkeji.xyz/gtsmelznew.html

Ruby: Dir.pwd
来源：http://hz.chenlongwang.top/gtzstiepid.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.gzhubu.top/gtdzgnvhne.html

[M05] 设置退出码
来源：http://hz.nanxuanxn.top/gthwjvrboi.html

Py:   sys.exit(1)
来源：http://hz.shanyushiyangkeji.top/gtcjwoqutn.html

PHP:  exit(1);
来源：http://hz.yj20258888.top/gtlccnhtnl.html

JS:   process.exit(1)
来源：http://hz.nanxuanxn.top/gtnplndhcw.html

TS:   process.exit(1)
来源：http://hz.haohaochexian.top/gtdgjsbqhn.html

Java: System.exit(1)
来源：http://hz.cucudq.cn/gtlwrvoxgr.html

Go:   os.Exit(1)
来源：http://hz.aibaodan.cn/gtgjsgbinx.html

Ruby: exit 1
来源：http://hz.9152youxi.cn/gttkaxhylq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jqgufenzy.top/gtxwkmplvh.html

[M06] 向标准错误输出
来源：http://hz.jinghuilouyu.cn/gtidyrisvd.html

Py:   print("err", file=sys.stderr)
来源：http://hz.aizwys.cn/gtdbbrorqx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zycfv.cn/gtpietgekq.html

JS:   console.error("err")
来源：http://hz.yj202588.top/gtmtflksta.html

TS:   console.error("err")
来源：http://hz.yj20258.top/gtthligxwu.html

Java: System.err.println("err")
来源：http://hz.meibo888.top/gtkcotvcag.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhiwuduotai.top/gttpormkxa.html

Ruby: warn "err"
来源：http://hz.zhengqikj.top/gtjlvspcto.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jyoumei.cn/gtzbutfnrf.html

[M07] 判断是否为主入口
来源：http://hz.haohaochexian.top/gtgyilekeh.html

Py:   if __name__ == "__main__":
来源：http://hz.hammf.cn/gtrwrwabjg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ybcxt.top/gtcioarkwe.html

JS:   require.main === module
来源：http://hz.hysaishi.cn/gtbxpposeu.html

TS:   require.main === module
来源：http://hz.zhengqikj.top/gtjdzrujhw.html

Java: public static void main(String[] args)
来源：http://hz.haohaochexian.top/gtmcfdzgvu.html

Go:   func main()
来源：http://hz.iojbl.cn/gtddhebreb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jinyuanbaomall.cn/gtrxlxyhzw.html

C#:   static void Main(string[] args)
来源：http://hz.xylfe.cn/gtslyqbocv.html

[M08] 获取系统与运行时信息
来源：http://hz.9152youxi.cn/gtgdmkokop.html

Py:   platform.system();  platform.python_version()
来源：http://hz.gotoacloud.top/gttpodfrdg.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.cdnleiting.top/gtueghmajy.html

JS:   process.platform;  process.version
来源：http://hz.hongshengwenyu.top/gtzbvefnnh.html

TS:   process.platform;  process.version
来源：http://hz.zycfv.cn/gtkgjmuqel.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.guannengcc.top/gtyqmjhaph.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xuetiantiany.cn/gtedvhwaim.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.xuanzx.com/gtzwlipkas.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhijiandao.cn/gttnjcwsgk.html

================================================================================
来源：http://hz.tian-w.cn/gtjmewvgtk.html

N. 数据结构与算法
来源：http://hz.guowangkeji.top/gtapnvlznj.html

================================================================================
来源：http://hz.chenzaomai.com/gtvakklzob.html

[N01] 二分查找（有序数组）
来源：http://hz.zhongyouzk.top/gthgmwduke.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yangfankeji.com/gtdnnxjapx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.xinyue.icu/gtzlyjykdx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.wangdashe.top/gtcmyvllhi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ppjwa.cn/gtwvblqgms.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.ppjwa.cn/gtmbrfekxs.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhixingplan.top/gtooadxpzy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jinghuilouyu.cn/gteshupuxw.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.fengsongda.top/gtpmhpeyjq.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yj20258.top/gtrfmiywhp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jianghu66.top/gtfhtdkuwa.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yonumen.top/gtlsrmhpsq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.fengsongda.top/gtbwulmcmu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shangyingyoupin.top/gtyragtmmp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.cqqwz.cn/gtvgeedgve.html

Go:   slices.Sort(arr)
来源：http://hz.jlsjyb.cn/gtbvlkqesk.html

Ruby: arr.sort
来源：http://hz.hammf.cn/gteblzjysf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jiagoushi.top/gtfhfhkthd.html

[N03] 快速排序（分治示例）
来源：http://hz.hammf.cn/gttnxyrqaj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.quarkkingdee.top/gtuomedqhe.html


<!-- 参考信息 -->