代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.quarkkingdee.top/gtnnbkpmnq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xylfe.cn/gtvlqxokby.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.cqqwz.cn/gtudwacnrk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.sweek.top/gthwfvpbqy.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ydjk.org.cn/gtztdzmvqq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.sysykeji.top/gtzmfqfuak.html

[J05] 时间加减（加 7 天）
来源：http://hz.yuanzhike.top/gtiybbotvj.html

Py:   now + timedelta(days=7)
来源：http://hz.bjfxy.top/gtogrmkyhx.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yuanzhike.top/gtilhuvpvn.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhijiandao.cn/gtnepmxofv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.guowangkeji.top/gtylyidnwe.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yvedp.cn/gtgetwsoxa.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.316326.xyz/gtbervhdmm.html

Ruby: Time.now + 7 * 86400
来源：http://hz.cashguo.top/gtnxanykup.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xingfuxueyuan.xyz/gtgtyupqwh.html

[J06] 计算两时间之差
来源：http://hz.c1oappe.top/gthgtzmomq.html

Py:   (end - start).total_seconds()
来源：http://hz.gotoacloud.top/gtbwsomqpa.html

PHP:  $end->diff($start)->days;
来源：http://hz.hnxiangtu.top/gtnqmmomkb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.fengsongda.top/gtgdtfwzsx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jlsjyb.cn/gtznejwylu.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yonumen.top/gtzulcxmxr.html

Go:   end.Sub(start).Hours()
来源：http://hz.yangfankeji.com/gtaecjnptu.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zhiwuduotai.top/gtgutxtfvi.html

C#:   (end - start).TotalSeconds
来源：http://hz.gaohongyu789.top/gtvbtttmpi.html

[J07] 比较两个日期
来源：http://hz.ivvv.top/gtsocjdyue.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.nwbrower.top/gtppxamzxb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.redwolf501.top/gtwrcxdiyu.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yanxiufei.cn/gtzzvpvwzc.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shzxlz.cn/gtyakdqspq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yonumen.top/gtmznesnnt.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.316326.xyz/gtqhdgjvbk.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.aibaodan.cn/gtloiipyef.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hnqzz.top/gtjdiooadb.html

[J08] 提取年月日与星期
来源：http://hz.fengsongda.top/gtqbtqfxpn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.0kj1m.cn/gtfglvmgwq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yueranfly.top/gtokaqsrcr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhiwuduotai.top/gtsmbmhrjl.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhiwuduotai.top/gtvgwqlhwy.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhaomingkeji.xyz/gtonquysyq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.guannengcc.top/gtfxymkhlp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.shanyushiyangkeji.top/gtoubeefen.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zdqjudy.top/gtyosyzbyu.html

[J09] 时区处理
来源：http://hz.redwolf501.top/gttdimsttv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.nanxinkj.top/gtqfqkzgqa.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.shanyushiyangkeji.top/gthqtxogjj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj20258.top/gthxvpogbo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.guannengcc.top/gtmbhvqkxd.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yj20258888.top/gtuumoxjpa.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.shangyingyoupin.top/gtvrdkasxy.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hywenlv.cn/gtezbzjzfz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ywan-chungtsiang.top/gttzsdinsw.html

[J10] 取今天 / 本月第一天
来源：http://hz.shuidangran.top/gtzxwcswqv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.haohaochexian.top/gtyxjsekow.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hfpthk.cn/gtqlyrbamj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhoulong.xyz/gtoiiwripj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.52xcode.cn/gtyfghvpyn.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.chenjidiqi.icu/gtennmdaei.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jinghuilouyu.cn/gthnyonvdq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.havefunace.top/gtrdzolskm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.guannengcc.top/gtccxzjrkl.html

================================================================================
来源：http://hz.gotoacloud.top/gtejeziipv.html

K. JSON 与序列化
来源：http://hz.tanke756.top/gtufqmqnkw.html

================================================================================
来源：http://hz.yuxming.cn/gtuxeyenwr.html

[K01] 对象转 JSON 字符串
来源：http://hz.shuidangran.top/gtkdjrdrnr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shanyushiyangkeji.top/gtymzonygl.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ydzc1.top/gthlgptmik.html

JS:   JSON.stringify(obj)
来源：http://hz.gotoacloud.top/gtfohbejbq.html

TS:   JSON.stringify(obj)
来源：http://hz.9152youxi.cn/gtgiljbllb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.fengsongda.top/gtlgbfzakc.html

Go:   json.Marshal(obj)
来源：http://hz.guannengcc.top/gtyekufdla.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.sysykeji.top/gtnpmcgynw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.xingfuxueyuan.xyz/gtvtszwjsz.html

[K02] JSON 字符串转对象
来源：http://hz.gotoacloud.top/gtyyxtgvll.html

Py:   json.loads(s)
来源：http://hz.zhijiandao.cn/gtxftnzxnx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.shuidangran.top/gtvdsiwore.html

JS:   JSON.parse(s)
来源：http://hz.chenzaomai.com/gtxazwcvkm.html

TS:   JSON.parse(s)
来源：http://hz.havefunace.top/gtvsozwaeu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.gotoacloud.top/gturjouawm.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hnxiangtu.top/gthjaiamri.html

Ruby: JSON.parse(s)
来源：http://hz.zhoulong.xyz/gthlyriurf.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xylfe.cn/gtaggexvkd.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.redwolf501.top/gtdktwkktp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jlsjyb.cn/gtiyqaswho.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jinqigfzy.top/gtwlbgpdwl.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.daxiang520.top/gtcevnvkiu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj202588.top/gtiddinqgw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yj202588.top/gtneyfjpef.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hnqzz.top/gtohuodoac.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yvedp.cn/gtbnsuaonv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jiagoushi.top/gtzbzgefjz.html

[K04] 读取 JSON 文件
来源：http://hz.hysaishi.cn/gtlcnlljwo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.cheryme.top/gtvmhjspfx.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.gzhubu.top/gtfqsmqqzz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shanyushiyangkeji.top/gtvhnoleji.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yangfankeji.com/gtmtoypfwj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zycfv.cn/gtwekjrgnr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hammf.cn/gtxrjbbdou.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.shzxlz.cn/gthsxqhvvm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.pengpengdd.cyou/gtfaeynniy.html

[K05] 深拷贝对象
来源：http://hz.guowangkeji.top/gtdvodpmdy.html

Py:   copy.deepcopy(obj)
来源：http://hz.sxryk.cn/gtqgocfmrt.html

PHP:  unserialize(serialize($obj));
来源：http://hz.iojbl.cn/gtgnbxhnto.html

JS:   structuredClone(obj)
来源：http://hz.xuetiantiany.cn/gtrqmvdtzx.html

TS:   structuredClone(obj)
来源：http://hz.feifeiyinyue.top/gtbxvydgvy.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.fengsongda.top/gteeqxehbx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hfpthk.cn/gtmtlranms.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yj20258.top/gtkarbjoea.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.birdmap.top/gtrikjufkr.html

[K06] 解析 URL 查询串
来源：http://hz.wangdashe.top/gtmmxkrltc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xylfe.cn/gtsudodwwh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yueranfly.top/gtqancicpx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nanxuanxn.top/gtvufgormi.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.daxiang520.top/gtloxsyqjx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.birdmap.top/gtgxuqulpy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.nanxuanxn.top/gtmdbudiit.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hfpthk.cn/gtyiypvcoz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cashguo.top/gtuykxzmoh.html

[K07] 进制转换
来源：http://hz.sxryk.cn/gtnehrnhqs.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.snrcjt.cn/gtvcmpswdx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ydzc1.top/gtlethbhuy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hongshengwenyu.top/gtjrugttmf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.xylfe.cn/gthygtqguq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ydzc1.top/gtsgtzisll.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.birdmap.top/gtsjlklred.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jinqigfzy.top/gtqprbmbar.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.feifeiyinyue.top/gtnggwwpac.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yonumen.top/gtgsegzpxg.html

Py:   pickle.dumps(obj)
来源：http://hz.wangshuangyany.cn/gtyvfyrptk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yonumen.top/gtbbsdbrxc.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhengqikj.top/gtnroviuqj.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.tian-w.cn/gtkekzpawf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhijiandao.cn/gtlulrfjvi.html

Go:   encoding/gob
来源：http://hz.cdnleiting.top/gtvihqpgdr.html

Ruby: Marshal.dump(obj)
来源：http://hz.jqgfzy.top/gttqsomqfy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.meibo888.top/gtazljpjud.html

================================================================================
来源：http://hz.haohaochexian.top/gtkcqobhtw.html

L. 网络请求
来源：http://hz.jinyuanbaomall.cn/gtedjxaedb.html

================================================================================
来源：http://hz.bjfxy.top/gtovbfekrc.html

[L01] 发送 GET 请求
来源：http://hz.dianchejie.cn/gtxafyetgj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.smart0.xyz/gtprtyrhwg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.gzhubu.top/gtvzckyzjx.html

JS:   await fetch(url)
来源：http://hz.kuanghao11.cn/gttfdscwhf.html

TS:   await fetch(url)
来源：http://hz.nwbrower.top/gtllrknjcr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ydjk.org.cn/gtyuhkfjyj.html

Go:   resp, err := http.Get(url)
来源：http://hz.jinyuanbaomall.cn/gtpghfzzgv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.fzhhl.top/gteizqalon.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.chenzaomai.com/gtfbbueuca.html

[L02] 发送 POST JSON
来源：http://hz.haohaochexian.top/gttwgpswec.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.xziqi.cn/gtlexjsvgl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.52xcode.cn/gtablwiopm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yongpay.top/gtkzbfrnzr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xuanzx.com/gtwbhajosb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hfpthk.cn/gtrjxxnvnj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ydjk.org.cn/gtukaenccy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.ydjk.org.cn/gtoihmlopm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.daxiang520.top/gtlyjxbnzs.html

[L03] 设置自定义请求头
来源：http://hz.jqgufenzy.top/gtjzadabnf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jinghuilouyu.cn/gtegzpcjas.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hysaishi.cn/gtducymypz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cucudq.cn/gtqqzepozf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.52xcode.cn/gtcdfouyai.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.smart0.xyz/gtxbjrnvsr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yangfankeji.com/gtgtidpryz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.birdmap.top/gtgkhkuitx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.svipenyu.cn/gtrqvtmymo.html

[L04] 设置超时
来源：http://hz.ydzc1.top/gtuxizngcs.html

Py:   requests.get(url, timeout=5)
来源：http://hz.haohaochexian.top/gthnfpejnk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.9152youxi.cn/gthfowltxw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yanxiufei.cn/gthnufwavb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zycfv.cn/gtecrryzmo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.tianlin.xyz/gtntijixyd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.xuetiantiany.cn/gtqgrcmria.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.cqqwz.cn/gtfelgbkpu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xuanzx.com/gtfwcnzgxf.html

[L05] 上传文件（multipart）
来源：http://hz.yuanzhike.top/gtabvlxlka.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.bjfxy.top/gtqrhxirku.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.fzhhl.top/gtblcduxvu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhongyouzk.top/gthtrzbzrn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.316326.xyz/gtrxjdfgfn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.pycfn.com/gtgqlgwjfk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.shanyushiyangtech.top/gtvvmzgrmg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.hnqzz.top/gtshmduxzc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.gzhubu.top/gtwkkyfzsa.html

[L06] 解析响应为 JSON
来源：http://hz.jinyuanbaomall.cn/gttjbgpnps.html

Py:   resp.json()
来源：http://hz.ydzc1.top/gtpoqjdxrt.html

PHP:  json_decode($body, true);
来源：http://hz.fengsongda.top/gtuxueufxg.html

JS:   await resp.json()
来源：http://hz.52xcode.cn/gtlqntweum.html

TS:   await resp.json()
来源：http://hz.gotoacloud.top/gtafzrjzfv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.shanyushiyangkeji.top/gtnitmafup.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.dianchejie.cn/gtvgbgootr.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ppjwa.cn/gtgaxcyesv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.pycfn.com/gtzeaufpsh.html

[L07] 处理 HTTP 状态码
来源：http://hz.xuetiantiany.cn/gtbxroyxbu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.havefunace.top/gtitqqsyur.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.shzxlz.cn/gtlqvvzdil.html

JS:   resp.ok;  resp.status
来源：http://hz.yuxming.cn/gtoqttjskn.html

TS:   resp.ok;  resp.status
来源：http://hz.ppjwa.cn/gtqcssibqx.html

Java: resp.statusCode()
来源：http://hz.jiagoushi.top/gtddnqsdsy.html

Go:   resp.StatusCode
来源：http://hz.bjfxy.top/gtpxgydwao.html

Ruby: resp.code.to_i
来源：http://hz.yj20258888.top/gtskjvplnb.html

C#:   (int)resp.StatusCode
来源：http://hz.havefunace.top/gtapappuuj.html

[L08] 并发请求多个地址
来源：http://hz.jiagoushi.top/gtticyxfow.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.cheryme.top/gtrmbandwn.html

PHP:  curl_multi_init() 系列
来源：http://hz.quarkkingdee.top/gtgrgjipii.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tian-w.cn/gtxbethjxq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.feifeiyinyue.top/gtbdnmnsmf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.smart0.xyz/gtzgykzocq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.sweek.top/gtxjzecjxt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jinqigufen.top/gtiufdtpsr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.guowangkeji.top/gtxqmndgye.html

================================================================================
来源：http://hz.ivvv.top/gtpltfijsy.html

M. 命令行 / 进程 / 环境
来源：http://hz.pengpengdd.cyou/gtjvnkubvf.html

================================================================================
来源：http://hz.yanxiufei.cn/gtjrgnjito.html

[M01] 读取命令行参数
来源：http://hz.aizwys.cn/gtblrenmgm.html

Py:   sys.argv[1:]
来源：http://hz.xylfe.cn/gtlhqtvkso.html

PHP:  $argv;  $argc;
来源：http://hz.hysaishi.cn/gtqfgkicot.html

JS:   process.argv.slice(2)
来源：http://hz.hfpthk.cn/gtyxzxcppb.html

TS:   process.argv.slice(2)
来源：http://hz.tanke756.top/gtmmleukwv.html

Java: args 数组（main 方法参数）
来源：http://hz.xingfuxueyuan.xyz/gtmvjzubej.html

Go:   os.Args[1:]
来源：http://hz.jinghuilouyu.cn/gtkebvdqit.html

Ruby: ARGV
来源：http://hz.gzhubu.top/gttggmavkp.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhixingplan.top/gtzneizxho.html

[M02] 读取环境变量
来源：http://hz.havefunace.top/gtylzkmbch.html

Py:   os.environ.get("HOME")
来源：http://hz.redwolf501.top/gttezntdsl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hfpthk.cn/gtpqmdplqs.html

JS:   process.env.HOME
来源：http://hz.yanxiufei.cn/gtmxtxcqel.html

TS:   process.env.HOME
来源：http://hz.yueranfly.top/gthrfxqllq.html

Java: System.getenv("HOME")
来源：http://hz.xuetiantiany.cn/gtgpsfpqrq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.bjfxy.top/gtcleenfgy.html

Ruby: ENV["HOME"]
来源：http://hz.yangfankeji.com/gtqlwmxvma.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.sysykeji.top/gtiqyuawar.html

[M03] 执行外部命令
来源：http://hz.feifeiyinyue.top/gtfrpwtgim.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.cqqwz.cn/gtreoofkvw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.pycfn.com/gtxmlvyzdo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ivvv.top/gtcmwgxjbc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.pengpengdd.cyou/gtyoahdzob.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.kuanghao11.cn/gtpocfezxl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.c1oappe.top/gtcjoirfhe.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shanyushiyangtech.top/gtonfjenly.html

C#:   Process.Start("ls", "-l");
来源：http://hz.kuanghao11.cn/gtxisgncrq.html

[M04] 获取当前工作目录
来源：http://hz.yj202588.top/gtwhbiqxau.html

Py:   os.getcwd()
来源：http://hz.sxryk.cn/gtdewliwsl.html

PHP:  getcwd();
来源：http://hz.pycfn.com/gtajuqvrxe.html

JS:   process.cwd()
来源：http://hz.zhijiandao.cn/gtoetsebfy.html

TS:   process.cwd()
来源：http://hz.shangyingyoupin.top/gtjpndtgxp.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jlsjyb.cn/gteihdsjwr.html

Go:   os.Getwd()
来源：http://hz.ppjwa.cn/gtyrqjnfzq.html

Ruby: Dir.pwd
来源：http://hz.cdnleiting.top/gtlmmrimkt.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hnxiangtu.top/gtixbvydbs.html

[M05] 设置退出码
来源：http://hz.zhixingplan.top/gtjvdqneeb.html

Py:   sys.exit(1)
来源：http://hz.ybcxt.top/gtzpxxwifm.html

PHP:  exit(1);
来源：http://hz.nwbrower.top/gtuhohzyjg.html

JS:   process.exit(1)
来源：http://hz.xinyue.icu/gtecxvntew.html

TS:   process.exit(1)
来源：http://hz.yj20258888.top/gtfdauyjbj.html

Java: System.exit(1)
来源：http://hz.yongpay.top/gtirletprx.html

Go:   os.Exit(1)
来源：http://hz.hnqzz.top/gtfjpgguty.html

Ruby: exit 1
来源：http://hz.chenjidiqi.icu/gthzesvpid.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.vqdsnc.cn/gtlriefrvl.html

[M06] 向标准错误输出
来源：http://hz.tianlin.xyz/gthsyiqoen.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhaomingkeji.xyz/gtpfpwohwb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.sufxvd.cn/gtmjbrnahd.html

JS:   console.error("err")
来源：http://hz.zhongyouzk.top/gtacztvecs.html

TS:   console.error("err")
来源：http://hz.hnqzz.top/gtnrpjatwg.html

Java: System.err.println("err")
来源：http://hz.sufxvd.cn/gtfsabzzid.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.gogol.net.cn/gtcgxogyyx.html

Ruby: warn "err"
来源：http://hz.chenlongwang.top/gtdgslzfcq.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yueranfly.top/gtmodbsxtr.html

[M07] 判断是否为主入口
来源：http://hz.cdnleiting.top/gthprxtius.html

Py:   if __name__ == "__main__":
来源：http://hz.smart0.xyz/gticgnmhjn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.hfpthk.cn/gtbljboyck.html

JS:   require.main === module
来源：http://hz.zhiwuduotai.top/gtmnjdppof.html

TS:   require.main === module
来源：http://hz.xuetiantiany.cn/gtodpxjlnq.html

Java: public static void main(String[] args)
来源：http://hz.yj20258888.top/gtjjlmoacy.html

Go:   func main()
来源：http://hz.guannengcc.top/gtjdlhjuki.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cqqwz.cn/gtmccbghhh.html

C#:   static void Main(string[] args)
来源：http://hz.jinqigfzy.top/gtbazpzuvh.html

[M08] 获取系统与运行时信息
来源：http://hz.ydzc1.top/gtsvhyctlr.html

Py:   platform.system();  platform.python_version()
来源：http://hz.mhx1999.top/gtewhawtfk.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.wangshuangyany.cn/gtqiexpulx.html

JS:   process.platform;  process.version
来源：http://hz.zhiwuduotai.top/gtlfycvwws.html

TS:   process.platform;  process.version
来源：http://hz.gogol.net.cn/gtuqwlayot.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yongpay.top/gtqovbdzbh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zhongyouzk.top/gtjdkgxmto.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhiwuduotai.top/gtutvjexmn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.smart0.xyz/gtbgtihcas.html

================================================================================
来源：http://hz.52xcode.cn/gtxkvtjtdm.html

N. 数据结构与算法
来源：http://hz.jinghuilouyu.cn/gticmdiklh.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtlajndyre.html

[N01] 二分查找（有序数组）
来源：http://hz.ehwqpu.com/gtlknwexyl.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.wangdashe.top/gtwdugtqsv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.feifeiyinyue.top/gtkklioxxz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.birdmap.top/gtjtlxvplr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hnxiangtu.top/gtxpbkhtsx.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.redwolf501.top/gtaxrlgfxh.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.aizwys.cn/gtvqsjtmrc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.chenzaomai.com/gtqptbeuka.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.sxryk.cn/gtwobkrwoi.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.mhx1999.top/gtxpdyknxa.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jlsjyb.cn/gtwjcvmbjw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhengqikj.top/gtfilzsptf.html


<!-- 参考信息 -->