代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cashguo.top/gtwndvvcym.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yvedp.cn/gtfprjfhxw.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ydjk.org.cn/gtfxeigkar.html

[J06] 计算两时间之差
来源：http://hz.zycfv.cn/gtpssfbccj.html

Py:   (end - start).total_seconds()
来源：http://hz.redwolf501.top/gtqjbmqvqr.html

PHP:  $end->diff($start)->days;
来源：http://hz.gzhubu.top/gtkevjimsr.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.fengsongda.top/gtviyviwtl.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.cdnleiting.top/gtdpjalkan.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hnqzz.top/gtrfzhzrmw.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhengqikj.top/gtrftpnuyv.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ehwqpu.com/gtocwsiuvg.html

C#:   (end - start).TotalSeconds
来源：http://hz.ydzc1.top/gtrwylbyhr.html

[J07] 比较两个日期
来源：http://hz.zhixingplan.top/gtpjkhykll.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhongyouzk.top/gtnnenzpfy.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hongshengwenyu.top/gtrbahdbmr.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yj202588.top/gtojiapeug.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.sufxvd.cn/gtjkoeecly.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.snrcjt.cn/gtktvilzyi.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.shuidangran.top/gtzhfwqnmw.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ydjk.org.cn/gtfkkkuwdr.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.xinyue.icu/gtoxufeaic.html

[J08] 提取年月日与星期
来源：http://hz.sysykeji.top/gtedzkdifh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.shanyushiyangkeji.top/gtcnynimmk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.aizwys.cn/gtzfljxaau.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.pycfn.com/gtezsmubcr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.sufxvd.cn/gtgzkogvhi.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.meibo888.top/gtoylojfkc.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.shanyushiyangtech.top/gtbnqjiqvb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.mhx1999.top/gtbbvxddcu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.birdmap.top/gtwzdppbaw.html

[J09] 时区处理
来源：http://hz.zhijiandao.cn/gtcxdigynh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.kuanghao11.cn/gtaxmtzakd.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jinyuanbaomall.cn/gtneriqarg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hywenlv.cn/gtrsjvtbxo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.chenzaomai.com/gtsszpwgve.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.aibaodan.cn/gtwhpoedgx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.dashuyun.cn/gtkutnvscn.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.fengsongda.top/gtpnbblopr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.dashuyun.cn/gtqlenicxp.html

[J10] 取今天 / 本月第一天
来源：http://hz.meibo888.top/gtljluwxwp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.smart0.xyz/gtpnnaxgey.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xziqi.cn/gtlviyczke.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.cdnleiting.top/gtkjwrwyna.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhoulong.xyz/gtawttpiqd.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shzxlz.cn/gtieneynof.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhiwuduotai.top/gtmblhhalu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xziqi.cn/gtjrmxcvcr.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.kuanghao11.cn/gtqjnzaenu.html

================================================================================
来源：http://hz.jinqigufen.top/gtgzvfrbht.html

K. JSON 与序列化
来源：http://hz.cdnleiting.top/gtwsrofprl.html

================================================================================
来源：http://hz.mhx1999.top/gtudjvxxbu.html

[K01] 对象转 JSON 字符串
来源：http://hz.jinghuilouyu.cn/gtqwrcrluf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.guowangkeji.top/gtmguproje.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xinyue.icu/gtsiyhfuax.html

JS:   JSON.stringify(obj)
来源：http://hz.meibo888.top/gtimvqdavc.html

TS:   JSON.stringify(obj)
来源：http://hz.jinghuilouyu.cn/gtfdqchroc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.guannengcc.top/gtbllbkdno.html

Go:   json.Marshal(obj)
来源：http://hz.zhijiandao.cn/gtkoyicvmi.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yuanzhike.top/gtumpdywcm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.52xcode.cn/gtusalxqug.html

[K02] JSON 字符串转对象
来源：http://hz.sxryk.cn/gtnpxeesrk.html

Py:   json.loads(s)
来源：http://hz.ybcxt.top/gtewyhnrxk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.redwolf501.top/gtcaeyokfs.html

JS:   JSON.parse(s)
来源：http://hz.sxryk.cn/gtvtbbxlxe.html

TS:   JSON.parse(s)
来源：http://hz.ppjwa.cn/gtaswominv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.ywan-chungtsiang.top/gtudijhhpk.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.tanke756.top/gtlrgdvurf.html

Ruby: JSON.parse(s)
来源：http://hz.ydjk.org.cn/gtrfqarzoz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.dashuyun.cn/gtkrkfzdpf.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yangfankeji.com/gtpfojdevm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yonumen.top/gtpgthvseq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hnxiangtu.top/gthwpgmkra.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.c1oappe.top/gtlfhvyhth.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.gaohongyu789.top/gtqhikqofx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yvedp.cn/gtquadfgrr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.cdnleiting.top/gtxxdylxog.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.shzxlz.cn/gtwejlinck.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jianghu66.top/gtujwrrdwm.html

[K04] 读取 JSON 文件
来源：http://hz.daxiang520.top/gtkeoagsjq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ybcxt.top/gtgcyewzyo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.redwolf501.top/gtbioahamp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.quarkkingdee.top/gtosiuggth.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jianghu66.top/gteekiookk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.cdnleiting.top/gtshbxgare.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.daxiang520.top/gtudjlucvb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.guannengcc.top/gtdzjdxphv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.cucudq.cn/gtohzvrwec.html

[K05] 深拷贝对象
来源：http://hz.zhiwuduotai.top/gtyjybsdwf.html

Py:   copy.deepcopy(obj)
来源：http://hz.ybcxt.top/gtqixacdld.html

PHP:  unserialize(serialize($obj));
来源：http://hz.havefunace.top/gtizamcraw.html

JS:   structuredClone(obj)
来源：http://hz.yanxiufei.cn/gtbmzebuqb.html

TS:   structuredClone(obj)
来源：http://hz.shangyingyoupin.top/gtlgnkhgrn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.andypj.xyz/gttnzuerew.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xuanzx.com/gtvpsckitp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zdqjudy.top/gtmkprnccu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yvedp.cn/gtwifxztdv.html

[K06] 解析 URL 查询串
来源：http://hz.xinyue.icu/gtkqexyowm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.c1oappe.top/gtsgmpnbgq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hnxiangtu.top/gttalfyxml.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xinyue.icu/gtatlfcepg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yangfankeji.com/gtufwbsria.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.haohaochexian.top/gtawvdcsfh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.snrcjt.cn/gtzrruectt.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ehwqpu.com/gtdpmpdvxq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ppjwa.cn/gtrudzhjwi.html

[K07] 进制转换
来源：http://hz.tanke756.top/gtwuacuryz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yuanzhike.top/gtaheghqpy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jqgufenzy.top/gtbfmylzsc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.gaohongyu789.top/gtnerzdsbv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhoulong.xyz/gtkudcyyfw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xinyue.icu/gtxgcxhnjj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.gotoacloud.top/gtczqejpml.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zhixingplan.top/gtucgnttri.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hammf.cn/gtgnhgrlxe.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.fengsongda.top/gtthrmmdmr.html

Py:   pickle.dumps(obj)
来源：http://hz.52xcode.cn/gtfaqzpoqy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yj20258888.top/gtcjtlaevx.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.aibaodan.cn/gtgjlhuege.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ivvv.top/gtlcjnolar.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hnxiangtu.top/gtxikhvoit.html

Go:   encoding/gob
来源：http://hz.cqqwz.cn/gtgefycnbe.html

Ruby: Marshal.dump(obj)
来源：http://hz.snrcjt.cn/gtzavvwmij.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.cucudq.cn/gtgzlfnife.html

================================================================================
来源：http://hz.sufxvd.cn/gtwsxfzqdj.html

L. 网络请求
来源：http://hz.fzhhl.top/gtxrdwiigq.html

================================================================================
来源：http://hz.andypj.xyz/gtkqqiokin.html

[L01] 发送 GET 请求
来源：http://hz.shangyingyoupin.top/gtkdzngppy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.dashuyun.cn/gtenqpkkvq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.nanxinkj.top/gtcoehwhog.html

JS:   await fetch(url)
来源：http://hz.xuetiantiany.cn/gtfilttpmo.html

TS:   await fetch(url)
来源：http://hz.redwolf501.top/gtgypvvylc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhijiandao.cn/gtrytthebv.html

Go:   resp, err := http.Get(url)
来源：http://hz.nanxinkj.top/gtuoelwenc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhoulong.xyz/gtgxbmjujz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.haohaochexian.top/gtgcjkwcob.html

[L02] 发送 POST JSON
来源：http://hz.yuanzhike.top/gtceasptfp.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.xingfuxueyuan.xyz/gtklwhrqeh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yongpay.top/gttnpvdctc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yvedp.cn/gtzbaqbjjq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shangyingyoupin.top/gtcehoddfm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yonumen.top/gtqbssgbci.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.gaohongyu789.top/gtmrudzhfm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.chenjidiqi.icu/gtiezlqqbq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xylfe.cn/gtwlqywydg.html

[L03] 设置自定义请求头
来源：http://hz.ybcxt.top/gtgtgqzeom.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.quarkkingdee.top/gtatpzidug.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zhongyouzk.top/gtqpljinsk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.9152youxi.cn/gtkghdijmx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gotoacloud.top/gtlrhbsfyc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.sxryk.cn/gtefikbrpd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.iojbl.cn/gtejvxltvl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.redwolf501.top/gtbahgfskk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhiwuduotai.top/gtxmalkboo.html

[L04] 设置超时
来源：http://hz.zhoulong.xyz/gtwkhcpalh.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xinyue.icu/gtcndwaynx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.havefunace.top/gtfzuqnbnn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.snrcjt.cn/gtzjxyxmda.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hnqzz.top/gtuijxjfyc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zycfv.cn/gteuxwubks.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yj202588.top/gtfasxdavc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.dashuyun.cn/gtbsdvdgqq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jyoumei.cn/gtmvzflipe.html

[L05] 上传文件（multipart）
来源：http://hz.jqgfzy.top/gtexnhhylh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.xziqi.cn/gtibvcthny.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.guowangkeji.top/gtgjveddiq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.iojbl.cn/gtsaznocwn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhaomingkeji.xyz/gtukuphwyb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.sufxvd.cn/gtntqfvswh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.52xcode.cn/gtowzffugo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.sysykeji.top/gtdbrmrxet.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.ydjk.org.cn/gtusrrsfre.html

[L06] 解析响应为 JSON
来源：http://hz.xinyue.icu/gtdxwuvhat.html

Py:   resp.json()
来源：http://hz.hysaishi.cn/gtzhkykqmj.html

PHP:  json_decode($body, true);
来源：http://hz.hfpthk.cn/gtaarzotgz.html

JS:   await resp.json()
来源：http://hz.0kj1m.cn/gtcnjixyce.html

TS:   await resp.json()
来源：http://hz.shangyingyoupin.top/gtcfhrilvf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.quarkkingdee.top/gtxtfkkfub.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.ehwqpu.com/gtdctjqvyu.html

Ruby: JSON.parse(resp.body)
来源：http://hz.fengsongda.top/gtnmpvvttf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.xingfuxueyuan.xyz/gtfytralez.html

[L07] 处理 HTTP 状态码
来源：http://hz.guannengcc.top/gtgevsksvk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.pengpengdd.cyou/gtlvbmzyec.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yanxiufei.cn/gtpozqrdjo.html

JS:   resp.ok;  resp.status
来源：http://hz.9152youxi.cn/gtfeibdvkl.html

TS:   resp.ok;  resp.status
来源：http://hz.pycfn.com/gtephujjvr.html

Java: resp.statusCode()
来源：http://hz.fzhhl.top/gtbmrlpkuj.html

Go:   resp.StatusCode
来源：http://hz.xylfe.cn/gteeckliso.html

Ruby: resp.code.to_i
来源：http://hz.ivvv.top/gtletpfxwf.html

C#:   (int)resp.StatusCode
来源：http://hz.ydjk.org.cn/gtkmoufhhg.html

[L08] 并发请求多个地址
来源：http://hz.ivvv.top/gtzfqdyjcn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.tanke756.top/gtbvzwxdtl.html

PHP:  curl_multi_init() 系列
来源：http://hz.vqdsnc.cn/gtbcbdonuv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jqgfzy.top/gtsogirsvw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shanyushiyangtech.top/gtlsfqoyvf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhijiandao.cn/gtcvnojcyu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ydjk.org.cn/gtccsbmnuu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hnqzz.top/gtopxegrdn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.cucudq.cn/gttkatjgfi.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtuguclizm.html

M. 命令行 / 进程 / 环境
来源：http://hz.jqgfzy.top/gtoygfohkt.html

================================================================================
来源：http://hz.snrcjt.cn/gtpdmqauoz.html

[M01] 读取命令行参数
来源：http://hz.aibaodan.cn/gtxdjbkmkg.html

Py:   sys.argv[1:]
来源：http://hz.chenjidiqi.icu/gtgxrqjqlc.html

PHP:  $argv;  $argc;
来源：http://hz.yuxming.cn/gtkghrkked.html

JS:   process.argv.slice(2)
来源：http://hz.0kj1m.cn/gtkslkiayy.html

TS:   process.argv.slice(2)
来源：http://hz.shanyushiyangkeji.top/gtskoqtqfo.html

Java: args 数组（main 方法参数）
来源：http://hz.quarkkingdee.top/gtlqmknzir.html

Go:   os.Args[1:]
来源：http://hz.fzhhl.top/gtcmyhbjbk.html

Ruby: ARGV
来源：http://hz.wangshuangyany.cn/gtnddkfpou.html

C#:   args 数组（Main 方法参数）
来源：http://hz.cashguo.top/gtcwtsbqer.html

[M02] 读取环境变量
来源：http://hz.jlsjyb.cn/gttarjokpw.html

Py:   os.environ.get("HOME")
来源：http://hz.quarkkingdee.top/gtaszzeaiz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yongpay.top/gtgsqokpqy.html

JS:   process.env.HOME
来源：http://hz.zhixingplan.top/gtmkqastra.html

TS:   process.env.HOME
来源：http://hz.yueranfly.top/gteqcpsxbt.html

Java: System.getenv("HOME")
来源：http://hz.tianlin.xyz/gtowrsmegi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.guannengcc.top/gturoknkrm.html

Ruby: ENV["HOME"]
来源：http://hz.svipenyu.cn/gtlakoeyhv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhongyouzk.top/gtnlipimgo.html

[M03] 执行外部命令
来源：http://hz.jinghuilouyu.cn/gtsqoqvjyd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhijiandao.cn/gtxwfwizme.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.havefunace.top/gtaqsooezd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xziqi.cn/gtthhdhmib.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.wangshuangyany.cn/gtatwxsqqu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhiwuduotai.top/gtithxpgrz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.meibo888.top/gthqpiigdm.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.gaohongyu789.top/gtaaepvorf.html

C#:   Process.Start("ls", "-l");
来源：http://hz.tianlin.xyz/gtumygyeri.html

[M04] 获取当前工作目录
来源：http://hz.shanyushiyangtech.top/gtfwbxhcaj.html

Py:   os.getcwd()
来源：http://hz.dashuyun.cn/gtnvpjiozh.html

PHP:  getcwd();
来源：http://hz.jiagoushi.top/gthsbicpjm.html

JS:   process.cwd()
来源：http://hz.aibaodan.cn/gtsbjnesde.html

TS:   process.cwd()
来源：http://hz.ivvv.top/gtmqywrejb.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jinqigfzy.top/gtacxdblym.html

Go:   os.Getwd()
来源：http://hz.tianlin.xyz/gtgrolkbps.html

Ruby: Dir.pwd
来源：http://hz.daria6918.cn/gtvcbmpnna.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.andypj.xyz/gtxrnsxvxb.html

[M05] 设置退出码
来源：http://hz.sxryk.cn/gtmlfqhnxc.html

Py:   sys.exit(1)
来源：http://hz.316326.xyz/gtspmqzppg.html

PHP:  exit(1);
来源：http://hz.52xcode.cn/gthemnklkw.html

JS:   process.exit(1)
来源：http://hz.yuanzhike.top/gtjwfiumsv.html

TS:   process.exit(1)
来源：http://hz.wangshuangyany.cn/gtdfuamaiu.html

Java: System.exit(1)
来源：http://hz.yangfankeji.com/gtfsfetvxj.html

Go:   os.Exit(1)
来源：http://hz.shuidangran.top/gtpmjwrcyu.html

Ruby: exit 1
来源：http://hz.9152youxi.cn/gtmuiivjkl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.xinyue.icu/gtatamipjs.html

[M06] 向标准错误输出
来源：http://hz.gogol.net.cn/gtcdapdmfv.html

Py:   print("err", file=sys.stderr)
来源：http://hz.pycfn.com/gtmwfkgmas.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yuxming.cn/gtdugavykv.html

JS:   console.error("err")
来源：http://hz.zhixingplan.top/gtsnfhbmzh.html

TS:   console.error("err")
来源：http://hz.jiagoushi.top/gtysdkkryb.html

Java: System.err.println("err")
来源：http://hz.yj20258.top/gteverwisr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.tianlin.xyz/gtytaocypq.html

Ruby: warn "err"
来源：http://hz.aizwys.cn/gticvnsxkr.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.c1oappe.top/gtvkqbmbdk.html

[M07] 判断是否为主入口
来源：http://hz.iojbl.cn/gtbabgrqec.html

Py:   if __name__ == "__main__":
来源：http://hz.hnqzz.top/gtkekjogfc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yj202588.top/gtqaiprazn.html

JS:   require.main === module
来源：http://hz.hnqzz.top/gtlgowiffe.html

TS:   require.main === module
来源：http://hz.jinyuanbaomall.cn/gthomnsieu.html

Java: public static void main(String[] args)
来源：http://hz.bjfxy.top/gtqedsiyot.html

Go:   func main()
来源：http://hz.guowangkeji.top/gtckpissiu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.9152youxi.cn/gthmlgmvee.html

C#:   static void Main(string[] args)
来源：http://hz.zhoulong.xyz/gtnhsfrpqj.html

[M08] 获取系统与运行时信息
来源：http://hz.shangyingyoupin.top/gtfhohzxsk.html

Py:   platform.system();  platform.python_version()
来源：http://hz.xinyue.icu/gtjwddztuh.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.hfpthk.cn/gtbjasypfr.html

JS:   process.platform;  process.version
来源：http://hz.zhongyouzk.top/gtxwybgqbv.html

TS:   process.platform;  process.version
来源：http://hz.jlsjyb.cn/gtwxlwerkh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.shuidangran.top/gttauharzz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yongpay.top/gtetvjypoy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.feifeiyinyue.top/gtpmcvlnwa.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhengqikj.top/gtoasrvukz.html

================================================================================
来源：http://hz.c1oappe.top/gtlrhqzujl.html

N. 数据结构与算法
来源：http://hz.jinqigfzy.top/gtgfmasyqn.html

================================================================================
来源：http://hz.zhoulong.xyz/gthlvfvtzq.html

[N01] 二分查找（有序数组）
来源：http://hz.tianlin.xyz/gtbflqgslf.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.sxryk.cn/gtwdxlvvgk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.quarkkingdee.top/gtoiudmuma.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cucudq.cn/gtsuncnicc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.c1oappe.top/gtqicbdgqy.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jianghu66.top/gtauulpczb.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.tian-w.cn/gtuulsahtj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ehwqpu.com/gtblktkmhh.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.havefunace.top/gtqpynzwzn.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhaomingkeji.xyz/gtkdwhsblm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinqigfzy.top/gtbycznxmr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.sweek.top/gttlbsbmsb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zdqjudy.top/gtzornvcqk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhixingplan.top/gtwybkcayc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hongshengwenyu.top/gtxumekotx.html

Go:   slices.Sort(arr)
来源：http://hz.dianchejie.cn/gtmvvencux.html

Ruby: arr.sort
来源：http://hz.zhixingplan.top/gtmripymwd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.haohaochexian.top/gtzwpqgaec.html

[N03] 快速排序（分治示例）
来源：http://hz.iojbl.cn/gtsrafbbax.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ivvv.top/gtzgwyttwd.html

PHP:  // 递归实现，或用 usort
来源：http://hz.gzhubu.top/gthkznlrcs.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hammf.cn/gtjpnynpfy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cucudq.cn/gtnecdnaty.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yvedp.cn/gtiaeciopt.html


<!-- 参考信息 -->