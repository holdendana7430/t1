代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.tianlin.xyz/gtagshixcl.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yonumen.top/gtkmxzfpnc.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.52xcode.cn/gtfdixsqlv.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.52xcode.cn/gtzufkfmcz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.shangyingyoupin.top/gtjafrmzja.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jinghuilouyu.cn/gtztiflzic.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zdqjudy.top/gtthgnznfk.html

[J06] 计算两时间之差
来源：http://hz.zhengqikj.top/gtkehjievx.html

Py:   (end - start).total_seconds()
来源：http://hz.fengsongda.top/gthjltfrbq.html

PHP:  $end->diff($start)->days;
来源：http://hz.hnqzz.top/gturxvzhjw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.sufxvd.cn/gtbklaamxe.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.svipenyu.cn/gthwktkbfl.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.kuanghao11.cn/gtrziyirki.html

Go:   end.Sub(start).Hours()
来源：http://hz.guannengcc.top/gtdhnrixxf.html

Ruby: end - start                 # 返回秒数
来源：http://hz.shzxlz.cn/gtzvvrojlf.html

C#:   (end - start).TotalSeconds
来源：http://hz.aibaodan.cn/gteqdbkolu.html

[J07] 比较两个日期
来源：http://hz.snrcjt.cn/gtzddvajnp.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.guannengcc.top/gtszkozdri.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hnqzz.top/gtwekubtgd.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jianghu66.top/gtysnhjenp.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.pengpengdd.cyou/gtjdmbrgxn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.gogol.net.cn/gtvoqaykio.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.snrcjt.cn/gtaeqaarvx.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yvedp.cn/gtoycqvgdl.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.svipenyu.cn/gtiswkzotv.html

[J08] 提取年月日与星期
来源：http://hz.ydzc1.top/gtwsgrfewp.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.c1oappe.top/gtfgllzhne.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hammf.cn/gtdrgxmsxx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.cashguo.top/gtuzsudlrc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.sxryk.cn/gthjlemuom.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.pengpengdd.cyou/gtkvajmicv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.dashuyun.cn/gtrfegzpci.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.quarkkingdee.top/gtekaxjurd.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.iojbl.cn/gthpwljgtm.html

[J09] 时区处理
来源：http://hz.yueranfly.top/gtsyfyljmq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.chenlongwang.top/gtenjidkkj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.bjfxy.top/gtnlyokeyc.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shanyushiyangtech.top/gtvuulaixz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhongyouzk.top/gtpvdmpwqi.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ydzc1.top/gtakbafunl.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.gotoacloud.top/gtcwplwyii.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.chenlongwang.top/gtlippflsu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.tanke756.top/gtpnchryiq.html

[J10] 取今天 / 本月第一天
来源：http://hz.havefunace.top/gtrbrkapwx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.daxiang520.top/gtcngaqpyl.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.chenzaomai.com/gtmareisdc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.havefunace.top/gtyraqtgpv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.gaohongyu789.top/gtnokwzssv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.cqqwz.cn/gtnfkeatop.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yj20258.top/gtqkwvuljk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.shangyingyoupin.top/gtlwnerenb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yanxiufei.cn/gttbmsiurt.html

================================================================================
来源：http://hz.cqqwz.cn/gtpqjhphhr.html

K. JSON 与序列化
来源：http://hz.jqgfzy.top/gtovaoksik.html

================================================================================
来源：http://hz.iojbl.cn/gtxindbrps.html

[K01] 对象转 JSON 字符串
来源：http://hz.guannengcc.top/gttwtzrsbm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zycfv.cn/gtooctwpxx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xziqi.cn/gtvxjffrcd.html

JS:   JSON.stringify(obj)
来源：http://hz.sysykeji.top/gtcepaqbav.html

TS:   JSON.stringify(obj)
来源：http://hz.hfpthk.cn/gtkleueuep.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xuetiantiany.cn/gtnngpvick.html

Go:   json.Marshal(obj)
来源：http://hz.zhengqikj.top/gtyepdulxf.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.nwbrower.top/gtdbjufinw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hywenlv.cn/gtkljrrlbc.html

[K02] JSON 字符串转对象
来源：http://hz.yj20258.top/gtandgjtqi.html

Py:   json.loads(s)
来源：http://hz.jqgfzy.top/gtzasmxhxr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.tanke756.top/gtejbuubwo.html

JS:   JSON.parse(s)
来源：http://hz.jinyuanbaomall.cn/gtdwpgzjzf.html

TS:   JSON.parse(s)
来源：http://hz.ybcxt.top/gtrtspmncx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zdqjudy.top/gtdexzbwiz.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.tanke756.top/gtgifjwdvt.html

Ruby: JSON.parse(s)
来源：http://hz.pycfn.com/gttiaxacgl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yvedp.cn/gtopvcpugj.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hysaishi.cn/gtvekiohau.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yj202588.top/gtrxboklap.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.nanxuanxn.top/gtekywwiwg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.c1oappe.top/gtamljhkvi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.pengpengdd.cyou/gthehydnhx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.xylfe.cn/gtnoviggip.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.shanyushiyangtech.top/gtijshlxvf.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yuanzhike.top/gtilyjregq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hnxiangtu.top/gtxkkcanby.html

[K04] 读取 JSON 文件
来源：http://hz.dashuyun.cn/gtehanwyhi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.9152youxi.cn/gtudyvzcxe.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.sysykeji.top/gtijrgcskn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xuetiantiany.cn/gtqsppkeal.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.chenzaomai.com/gtewoudwzk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.smart0.xyz/gtnirmbrcd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jinqigufen.top/gtyvuqgjkq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ppjwa.cn/gtynkcuosf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.cheryme.top/gtfmddlqwu.html

[K05] 深拷贝对象
来源：http://hz.jiagoushi.top/gtwxniikno.html

Py:   copy.deepcopy(obj)
来源：http://hz.xylfe.cn/gtyrsgofxt.html

PHP:  unserialize(serialize($obj));
来源：http://hz.fzhhl.top/gtgjysjrzw.html

JS:   structuredClone(obj)
来源：http://hz.jiagoushi.top/gtgyxuwcqx.html

TS:   structuredClone(obj)
来源：http://hz.vqdsnc.cn/gtyfojqvux.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.sweek.top/gtcfdsjwjs.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.aibaodan.cn/gtqyaznrzi.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.chenzaomai.com/gtixnbeurc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.fzhhl.top/gtsvqrloje.html

[K06] 解析 URL 查询串
来源：http://hz.gaohongyu789.top/gtkdjpemnk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.shuidangran.top/gtbhhmukjv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hnqzz.top/gtqrtgldfn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.pycfn.com/gtsgzcpmzz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shanyushiyangtech.top/gtjafnhcbj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhoulong.xyz/gtqczczwxu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.sxryk.cn/gtkonakszf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hnxiangtu.top/gtfjgguizd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zdqjudy.top/gtwohjtdat.html

[K07] 进制转换
来源：http://hz.cheryme.top/gtrxszlbxq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yj20258888.top/gthnyhluip.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.c1oappe.top/gtlfgxwmly.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhengqikj.top/gtqjodghgz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.xziqi.cn/gtjljeykin.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.shanyushiyangkeji.top/gtsibezkbp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.ivvv.top/gteyznyvhl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xziqi.cn/gtmnvlhoch.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.pycfn.com/gttmtbgazn.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.dianchejie.cn/gtiroexytb.html

Py:   pickle.dumps(obj)
来源：http://hz.yuanzhike.top/gtpevgcixk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.shangyingyoupin.top/gtvrxkldgl.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.chenjidiqi.icu/gtofchgmax.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yj20258888.top/gtafvhnegb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.fzhhl.top/gtsagdkhjt.html

Go:   encoding/gob
来源：http://hz.hammf.cn/gtydxztzmw.html

Ruby: Marshal.dump(obj)
来源：http://hz.jyoumei.cn/gtafhjbnpy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yongpay.top/gtytmsvnxj.html

================================================================================
来源：http://hz.nwbrower.top/gtlodvlhnx.html

L. 网络请求
来源：http://hz.chenjidiqi.icu/gtvodgoojz.html

================================================================================
来源：http://hz.smart0.xyz/gthfrwornv.html

[L01] 发送 GET 请求
来源：http://hz.hnqzz.top/gtvuwzbtls.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.pengpengdd.cyou/gtvvbtmufg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hysaishi.cn/gtqxlaplqp.html

JS:   await fetch(url)
来源：http://hz.hammf.cn/gtoygzrchz.html

TS:   await fetch(url)
来源：http://hz.cheryme.top/gtmbkgizaw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.snrcjt.cn/gtmwybgzzl.html

Go:   resp, err := http.Get(url)
来源：http://hz.nwbrower.top/gtraitwxxp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhengqikj.top/gtzofiwicm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yj202588.top/gtzbycotuk.html

[L02] 发送 POST JSON
来源：http://hz.hongshengwenyu.top/gtxieuarox.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.nanxinkj.top/gtzipxczad.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jinqigufen.top/gtyifpdwia.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ybcxt.top/gttcjeupsn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.birdmap.top/gtiadfrfta.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.wangshuangyany.cn/gtunquqddu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xuanzx.com/gtgyfonbgb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.c1oappe.top/gtzsbtsqti.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.sweek.top/gtudlnvfdm.html

[L03] 设置自定义请求头
来源：http://hz.9152youxi.cn/gtjtqqovrt.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hnqzz.top/gtzofewdzr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yj20258.top/gtchrgpxme.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.meibo888.top/gtaoljyuvg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shanyushiyangkeji.top/gtaaselwkg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.redwolf501.top/gtgjbsvwsd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.0kj1m.cn/gtqkhwivxl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.chenjidiqi.icu/gtxiiinnqo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.52xcode.cn/gtgvmsknnu.html

[L04] 设置超时
来源：http://hz.yvedp.cn/gtnzqubect.html

Py:   requests.get(url, timeout=5)
来源：http://hz.andypj.xyz/gtgjozqszy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.xylfe.cn/gtdqdauuyz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.andypj.xyz/gtyufswxrl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.fengsongda.top/gttrapiwmb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.bjfxy.top/gtburunbbd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.gzhubu.top/gtadszpimd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yueranfly.top/gthujjuczi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.guannengcc.top/gtxtceovoc.html

[L05] 上传文件（multipart）
来源：http://hz.yvedp.cn/gtqctfdrwa.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.gogol.net.cn/gtskncnlcj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jyoumei.cn/gtdyiwuixp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.aibaodan.cn/gtkyevvgbi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.hywenlv.cn/gtqdlxrkug.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.9152youxi.cn/gtagmifbow.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xingfuxueyuan.xyz/gtnlybqomw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.gotoacloud.top/gtwzifofqw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yanxiufei.cn/gtlhwrixun.html

[L06] 解析响应为 JSON
来源：http://hz.zhoulong.xyz/gtqbslhgru.html

Py:   resp.json()
来源：http://hz.chenlongwang.top/gtikaioijd.html

PHP:  json_decode($body, true);
来源：http://hz.yvedp.cn/gtnlpqdgeo.html

JS:   await resp.json()
来源：http://hz.aibaodan.cn/gtcjcttgza.html

TS:   await resp.json()
来源：http://hz.zhongyouzk.top/gtymblytjh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.mhx1999.top/gtvhmdjnqi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.iojbl.cn/gtdftcejcg.html

Ruby: JSON.parse(resp.body)
来源：http://hz.meibo888.top/gtkucwvyjk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yongpay.top/gtdjgobhdh.html

[L07] 处理 HTTP 状态码
来源：http://hz.kuanghao11.cn/gtoequvzpt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xylfe.cn/gtzmusnvbj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.shanyushiyangtech.top/gtyfvhadql.html

JS:   resp.ok;  resp.status
来源：http://hz.chenjidiqi.icu/gtzohixipq.html

TS:   resp.ok;  resp.status
来源：http://hz.hongshengwenyu.top/gtuqpytcxc.html

Java: resp.statusCode()
来源：http://hz.dianchejie.cn/gttlkvszwc.html

Go:   resp.StatusCode
来源：http://hz.52xcode.cn/gtttqtnfyz.html

Ruby: resp.code.to_i
来源：http://hz.gzhubu.top/gtsbwnhpts.html

C#:   (int)resp.StatusCode
来源：http://hz.daria6918.cn/gtkzexoiwb.html

[L08] 并发请求多个地址
来源：http://hz.yangfankeji.com/gtsylsoqwl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yangfankeji.com/gtydkkfgrn.html

PHP:  curl_multi_init() 系列
来源：http://hz.haohaochexian.top/gtpjlbxieu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cucudq.cn/gtzwhchtcx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ydzc1.top/gtxhhvfrqo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhijiandao.cn/gtosxchrcx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ybcxt.top/gtbtduuvnp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhaomingkeji.xyz/gtkhuyvpff.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.pengpengdd.cyou/gtpfkbctuz.html

================================================================================
来源：http://hz.svipenyu.cn/gtgqujvjee.html

M. 命令行 / 进程 / 环境
来源：http://hz.chenzaomai.com/gtzspqqljm.html

================================================================================
来源：http://hz.cashguo.top/gtkqhurque.html

[M01] 读取命令行参数
来源：http://hz.andypj.xyz/gtsnfmhqck.html

Py:   sys.argv[1:]
来源：http://hz.aizwys.cn/gtgxtplvnu.html

PHP:  $argv;  $argc;
来源：http://hz.yuanzhike.top/gtmzradnea.html

JS:   process.argv.slice(2)
来源：http://hz.jinyuanbaomall.cn/gtgnayijpg.html

TS:   process.argv.slice(2)
来源：http://hz.kuanghao11.cn/gtvznlzssq.html

Java: args 数组（main 方法参数）
来源：http://hz.shanyushiyangtech.top/gtotqeohyl.html

Go:   os.Args[1:]
来源：http://hz.yj20258.top/gtwbqeeayt.html

Ruby: ARGV
来源：http://hz.redwolf501.top/gtdzrjlvok.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhiwuduotai.top/gtttgkikjd.html

[M02] 读取环境变量
来源：http://hz.hfpthk.cn/gtumgfrlfm.html

Py:   os.environ.get("HOME")
来源：http://hz.zhijiandao.cn/gtjqrbyhmr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yvedp.cn/gtepynfauj.html

JS:   process.env.HOME
来源：http://hz.52xcode.cn/gtilnpjgfx.html

TS:   process.env.HOME
来源：http://hz.tian-w.cn/gtsudfpfnc.html

Java: System.getenv("HOME")
来源：http://hz.9152youxi.cn/gtcywkkjmi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.meibo888.top/gtbyelfkjh.html

Ruby: ENV["HOME"]
来源：http://hz.shuidangran.top/gtwvqgqvva.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yonumen.top/gtksfxvget.html

[M03] 执行外部命令
来源：http://hz.daria6918.cn/gtswrdyrfo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.gogol.net.cn/gttjntsmlj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yonumen.top/gtmyfacriy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yueranfly.top/gttvjnlyga.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinqigfzy.top/gtuytaqyof.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.wangdashe.top/gtidbyjfvj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.316326.xyz/gtgvsequfy.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.wangdashe.top/gtrmnailcq.html

C#:   Process.Start("ls", "-l");
来源：http://hz.haohaochexian.top/gtvfspgyvf.html

[M04] 获取当前工作目录
来源：http://hz.ybcxt.top/gtjekvfcin.html

Py:   os.getcwd()
来源：http://hz.tianlin.xyz/gtqyncnrjr.html

PHP:  getcwd();
来源：http://hz.zhijiandao.cn/gtqhmlpobh.html

JS:   process.cwd()
来源：http://hz.wangdashe.top/gtlrnmkdfd.html

TS:   process.cwd()
来源：http://hz.jiagoushi.top/gtswwqffrw.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.birdmap.top/gtukzmlabw.html

Go:   os.Getwd()
来源：http://hz.fzhhl.top/gtgaorjlpi.html

Ruby: Dir.pwd
来源：http://hz.jqgufenzy.top/gtzutveclf.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jqgfzy.top/gtgeeqftit.html

[M05] 设置退出码
来源：http://hz.jinyuanbaomall.cn/gtjjeqauhb.html

Py:   sys.exit(1)
来源：http://hz.zhaomingkeji.xyz/gtimkghjpx.html

PHP:  exit(1);
来源：http://hz.c1oappe.top/gtzpzcfmya.html

JS:   process.exit(1)
来源：http://hz.zhoulong.xyz/gttxcxxfsa.html

TS:   process.exit(1)
来源：http://hz.aizwys.cn/gtrdlaajxw.html

Java: System.exit(1)
来源：http://hz.sxryk.cn/gtsmjxrtzw.html

Go:   os.Exit(1)
来源：http://hz.xuanzx.com/gticotkdkw.html

Ruby: exit 1
来源：http://hz.zhijiandao.cn/gtkzfhtpxf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.andypj.xyz/gtgtbxmjqg.html

[M06] 向标准错误输出
来源：http://hz.shanyushiyangtech.top/gtnuykwwqh.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yuxming.cn/gtlspbirac.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yj20258888.top/gturfzmfis.html

JS:   console.error("err")
来源：http://hz.yuxming.cn/gtmknnvlyd.html

TS:   console.error("err")
来源：http://hz.c1oappe.top/gttlnmntkq.html

Java: System.err.println("err")
来源：http://hz.nwbrower.top/gtlcqicfrp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.hfpthk.cn/gtncdpiwcf.html

Ruby: warn "err"
来源：http://hz.ydzc1.top/gtrxomiqqy.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.meibo888.top/gtdpfklhob.html

[M07] 判断是否为主入口
来源：http://hz.zhiwuduotai.top/gtvsejafho.html

Py:   if __name__ == "__main__":
来源：http://hz.quarkkingdee.top/gtvqxcapel.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.dashuyun.cn/gtdahhebda.html

JS:   require.main === module
来源：http://hz.nanxinkj.top/gtqtzvxmba.html

TS:   require.main === module
来源：http://hz.jinghuilouyu.cn/gtfsxbsltt.html

Java: public static void main(String[] args)
来源：http://hz.zhengqikj.top/gtsdmnezji.html

Go:   func main()
来源：http://hz.aizwys.cn/gtyuaghojg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.bjfxy.top/gtvzuezvau.html

C#:   static void Main(string[] args)
来源：http://hz.xylfe.cn/gtzarkrtcx.html

[M08] 获取系统与运行时信息
来源：http://hz.52xcode.cn/gtlofwgoaq.html

Py:   platform.system();  platform.python_version()
来源：http://hz.xingfuxueyuan.xyz/gtjzwbflvv.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.chenjidiqi.icu/gtlcrcpmrk.html

JS:   process.platform;  process.version
来源：http://hz.zhiwuduotai.top/gtyyqzhjsu.html

TS:   process.platform;  process.version
来源：http://hz.smart0.xyz/gtvnizrfqi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yuanzhike.top/gttzbsmpmi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jqgufenzy.top/gtcoyfrfda.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cashguo.top/gtbpmakxtl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.wangshuangyany.cn/gtnieduemw.html

================================================================================
来源：http://hz.xylfe.cn/gtkbbmhfmy.html

N. 数据结构与算法
来源：http://hz.jinyuanbaomall.cn/gtpeodmqcc.html

================================================================================
来源：http://hz.yanxiufei.cn/gtheqxfhiw.html

[N01] 二分查找（有序数组）
来源：http://hz.ybcxt.top/gtdvenlmnz.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yonumen.top/gtpnggdfvq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.xingfuxueyuan.xyz/gtedpigxpg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jiagoushi.top/gtszvdwbrd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhoulong.xyz/gtwsyuntfb.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.daxiang520.top/gttapodjep.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.redwolf501.top/gtjnvpisgc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xuanzx.com/gtamjsdwob.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zhijiandao.cn/gtaqytcqwm.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.kuanghao11.cn/gtbthypupt.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhixingplan.top/gtqgyozjpj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhixingplan.top/gtergjgmtx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cheryme.top/gtsrdhaaab.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.snrcjt.cn/gturbtsxks.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.cashguo.top/gtqbltkuju.html

Go:   slices.Sort(arr)
来源：http://hz.vqdsnc.cn/gttsvznbqf.html

Ruby: arr.sort
来源：http://hz.hongshengwenyu.top/gthitwbdqr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yj20258888.top/gtnpfvejik.html

[N03] 快速排序（分治示例）
来源：http://hz.tianlin.xyz/gtgumfjipp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yangfankeji.com/gtykknxlhx.html


<!-- 参考信息 -->