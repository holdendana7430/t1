代发 wailian999

Py:   (end - start).total_seconds()
来源：http://hz.andypj.xyz/gtvbzbwato.html

PHP:  $end->diff($start)->days;
来源：http://hz.yuxming.cn/gtwixtpoke.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yuxming.cn/gtpkzivhif.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.xuetiantiany.cn/gtkznwozbd.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.wangdashe.top/gtzkqsaqjp.html

Go:   end.Sub(start).Hours()
来源：http://hz.aibaodan.cn/gtjljtjwnr.html

Ruby: end - start                 # 返回秒数
来源：http://hz.xinyue.icu/gtlryqqfsb.html

C#:   (end - start).TotalSeconds
来源：http://hz.fzhhl.top/gtwhnijpwb.html

[J07] 比较两个日期
来源：http://hz.sysykeji.top/gtkmemveja.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.cheryme.top/gtazcuweks.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xylfe.cn/gtosbnjaqz.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.snrcjt.cn/gtthbgjhok.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ydjk.org.cn/gtphzcfgbb.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.gaohongyu789.top/gtuvwliiym.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yueranfly.top/gtiqxdnafh.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yj20258.top/gtatndewcl.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.pengpengdd.cyou/gtfjjbqwgc.html

[J08] 提取年月日与星期
来源：http://hz.shuidangran.top/gtunvzbkjf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.chenzaomai.com/gttlsckxai.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.sweek.top/gtrcwyfyyq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinqigufen.top/gtnforetzk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ydzc1.top/gtsvmkmovk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.aibaodan.cn/gtyjjctuyd.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.nanxuanxn.top/gtdlqwxzrf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.daria6918.cn/gthegcikpz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.chenlongwang.top/gtiufshvhi.html

[J09] 时区处理
来源：http://hz.wangdashe.top/gtzjtgbgoi.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hammf.cn/gtwplkyyhl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.chenlongwang.top/gtveevkqrw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.mhx1999.top/gtdkntcmoo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.havefunace.top/gtyfxyekwx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.nanxuanxn.top/gtmaajlbmh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.daria6918.cn/gtzzatkwmb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yuanzhike.top/gtyctfkixr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yj20258888.top/gthibgqehw.html

[J10] 取今天 / 本月第一天
来源：http://hz.tian-w.cn/gthetwsxvl.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.gotoacloud.top/gtoxpezigz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zdqjudy.top/gtbvothupn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jiagoushi.top/gtcdkuelhq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hammf.cn/gtbfsazluf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.guannengcc.top/gtiluhndpc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhoulong.xyz/gtumkgxbqk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yj202588.top/gtfrvvevcv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.dashuyun.cn/gtttqccxhu.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtpcsiijaz.html

K. JSON 与序列化
来源：http://hz.zhiwuduotai.top/gtqapulbgo.html

================================================================================
来源：http://hz.zhongyouzk.top/gthvedmvsb.html

[K01] 对象转 JSON 字符串
来源：http://hz.jlsjyb.cn/gthnmywafq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.316326.xyz/gtrnirjapq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.tian-w.cn/gtqqictiuo.html

JS:   JSON.stringify(obj)
来源：http://hz.tian-w.cn/gtcjsxucus.html

TS:   JSON.stringify(obj)
来源：http://hz.jinghuilouyu.cn/gtvmttkxeu.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.chenzaomai.com/gtujypnuyq.html

Go:   json.Marshal(obj)
来源：http://hz.yueranfly.top/gtsxeekuid.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.gotoacloud.top/gtyuqaggas.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.shzxlz.cn/gtanazicgx.html

[K02] JSON 字符串转对象
来源：http://hz.aibaodan.cn/gtcyobvoad.html

Py:   json.loads(s)
来源：http://hz.yuxming.cn/gtzkdkmmgs.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.gotoacloud.top/gtpibscjfo.html

JS:   JSON.parse(s)
来源：http://hz.nanxuanxn.top/gtsyxadbpe.html

TS:   JSON.parse(s)
来源：http://hz.dianchejie.cn/gtewfcuvxs.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jinghuilouyu.cn/gtdcmihfhg.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hysaishi.cn/gtbaewissg.html

Ruby: JSON.parse(s)
来源：http://hz.vqdsnc.cn/gtrogfaljw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ivvv.top/gtmmcttmxj.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.vqdsnc.cn/gtxnrblbcg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zycfv.cn/gtqhdxbync.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yuanzhike.top/gtkrigyhkp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.sufxvd.cn/gtmoltcwci.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.wangdashe.top/gtjyfodlyf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hfpthk.cn/gtrcleqjfe.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.mhx1999.top/gtykntasnb.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hammf.cn/gtnafahfyi.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.bjfxy.top/gtfqflvzek.html

[K04] 读取 JSON 文件
来源：http://hz.aizwys.cn/gtsyvewlkk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xingfuxueyuan.xyz/gtncpdgmem.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.snrcjt.cn/gtijhojsoy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jyoumei.cn/gtmgxhocrj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.tanke756.top/gtciefywxt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.guowangkeji.top/gtrgpcngto.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ehwqpu.com/gtlqbjzzzi.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yj20258888.top/gtjjbjmkfl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yj20258888.top/gtarluiafl.html

[K05] 深拷贝对象
来源：http://hz.shangyingyoupin.top/gtydkucihv.html

Py:   copy.deepcopy(obj)
来源：http://hz.ybcxt.top/gtdkymhyyz.html

PHP:  unserialize(serialize($obj));
来源：http://hz.havefunace.top/gtylvdqrvr.html

JS:   structuredClone(obj)
来源：http://hz.havefunace.top/gtdzqllafr.html

TS:   structuredClone(obj)
来源：http://hz.yanxiufei.cn/gtcdskvpun.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.pengpengdd.cyou/gttsbflyqm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ivvv.top/gtewslmgll.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.snrcjt.cn/gtxtjmvslx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jinqigfzy.top/gtvcwkbrvu.html

[K06] 解析 URL 查询串
来源：http://hz.birdmap.top/gtnctrjkhc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.daria6918.cn/gtrvbwntrj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.iojbl.cn/gtpewllsxq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.redwolf501.top/gturljzkix.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ydjk.org.cn/gtsqcarlnl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hongshengwenyu.top/gtnazeolps.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.kuanghao11.cn/gtmvzwpotq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.iojbl.cn/gtducktetz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jinqigfzy.top/gtjutaotcb.html

[K07] 进制转换
来源：http://hz.316326.xyz/gtmtyiohnv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.shzxlz.cn/gtgukxyqbf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.andypj.xyz/gtjxquzdom.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.ydjk.org.cn/gtkqyuglfj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.sweek.top/gtlbrlnwpe.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hammf.cn/gtrgkynxql.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.vqdsnc.cn/gtczfgkovp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.nanxuanxn.top/gtemcmeyrz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.iojbl.cn/gtfxyzcswr.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jinqigufen.top/gtuzzkziwq.html

Py:   pickle.dumps(obj)
来源：http://hz.vqdsnc.cn/gtopfnwdiy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.0kj1m.cn/gtefypedkt.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jinqigufen.top/gtxqnamiyz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhijiandao.cn/gtliqmfzkw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.haohaochexian.top/gtbyfqvdcq.html

Go:   encoding/gob
来源：http://hz.birdmap.top/gtjetninrc.html

Ruby: Marshal.dump(obj)
来源：http://hz.cdnleiting.top/gtxfvidnur.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yonumen.top/gtafdllnik.html

================================================================================
来源：http://hz.yuanzhike.top/gtedyfsidq.html

L. 网络请求
来源：http://hz.daria6918.cn/gtqkmrmmgw.html

================================================================================
来源：http://hz.dashuyun.cn/gtgfbwwqdy.html

[L01] 发送 GET 请求
来源：http://hz.yj20258888.top/gtjrayrgbm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.feifeiyinyue.top/gtzxmtbujb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.redwolf501.top/gtkfmywxun.html

JS:   await fetch(url)
来源：http://hz.hysaishi.cn/gtaymmehcc.html

TS:   await fetch(url)
来源：http://hz.cdnleiting.top/gtukptggev.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.sysykeji.top/gtkfjyoglb.html

Go:   resp, err := http.Get(url)
来源：http://hz.xylfe.cn/gtgimqgbxd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.andypj.xyz/gtxfaweadf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ywan-chungtsiang.top/gthvobtkee.html

[L02] 发送 POST JSON
来源：http://hz.kuanghao11.cn/gtbfnnyzwt.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hfpthk.cn/gtgbpshjwd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.dashuyun.cn/gtddvorodz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yj20258.top/gtzywslxbl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.chenzaomai.com/gtnjyircja.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jiagoushi.top/gtfvbztran.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yj20258888.top/gtufcxfmnh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yangfankeji.com/gterttmbmy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.andypj.xyz/gtvxaltupt.html

[L03] 设置自定义请求头
来源：http://hz.pengpengdd.cyou/gtbrzyuvjw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.feifeiyinyue.top/gtwphaghso.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.svipenyu.cn/gtothlxnjw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.guowangkeji.top/gtaxjrxeqp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.kuanghao11.cn/gtqcvsmaod.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.xylfe.cn/gtgdckduon.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.xinyue.icu/gtjdylqnko.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.bjfxy.top/gtebenmnck.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.shangyingyoupin.top/gtoxkkjopq.html

[L04] 设置超时
来源：http://hz.bjfxy.top/gtteebucec.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xuanzx.com/gtebebjmhe.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.snrcjt.cn/gtspwrktwc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.chenjidiqi.icu/gtwkrgfira.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.tanke756.top/gtftvlhwos.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jqgfzy.top/gttyvvarvq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yongpay.top/gtcgfdhesg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.chenzaomai.com/gtcmrbxhit.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hammf.cn/gtwrxierec.html

[L05] 上传文件（multipart）
来源：http://hz.zhiwuduotai.top/gttpgxjeql.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.ppjwa.cn/gtaoqprawz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yongpay.top/gtcsefaugr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.xziqi.cn/gtpmawrhkc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jqgfzy.top/gtfwtffqyr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.fengsongda.top/gtiravjesl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jinqigufen.top/gtpwycvsmj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.hfpthk.cn/gtwemtvkba.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.xuanzx.com/gtypyyffpc.html

[L06] 解析响应为 JSON
来源：http://hz.ehwqpu.com/gthwsfgnkx.html

Py:   resp.json()
来源：http://hz.yj202588.top/gtskiwbjtg.html

PHP:  json_decode($body, true);
来源：http://hz.shangyingyoupin.top/gtauypjyuc.html

JS:   await resp.json()
来源：http://hz.sufxvd.cn/gtxjabqdyf.html

TS:   await resp.json()
来源：http://hz.jlsjyb.cn/gtctcnnutw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yuxming.cn/gttcyoyefs.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.chenlongwang.top/gtuqfxcgbj.html

Ruby: JSON.parse(resp.body)
来源：http://hz.kuanghao11.cn/gtwlivgvao.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.feifeiyinyue.top/gtvoinkqkl.html

[L07] 处理 HTTP 状态码
来源：http://hz.chenjidiqi.icu/gtbjbfnvjz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yangfankeji.com/gtvfkkyzxs.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yuanzhike.top/gtktapjulg.html

JS:   resp.ok;  resp.status
来源：http://hz.sysykeji.top/gtttahyfxb.html

TS:   resp.ok;  resp.status
来源：http://hz.xingfuxueyuan.xyz/gtbojlsvfk.html

Java: resp.statusCode()
来源：http://hz.wangdashe.top/gtisntxfvy.html

Go:   resp.StatusCode
来源：http://hz.ydzc1.top/gtvaxwsyma.html

Ruby: resp.code.to_i
来源：http://hz.andypj.xyz/gtebaxjesv.html

C#:   (int)resp.StatusCode
来源：http://hz.hfpthk.cn/gtqsmlzhvc.html

[L08] 并发请求多个地址
来源：http://hz.jinqigufen.top/gtemckyrza.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jinghuilouyu.cn/gtebeimwey.html

PHP:  curl_multi_init() 系列
来源：http://hz.gaohongyu789.top/gtnxywfyrf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xylfe.cn/gtlncvsedg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zycfv.cn/gtafourbgv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.9152youxi.cn/gtsbhhnyyv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ywan-chungtsiang.top/gttvgplegb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.cashguo.top/gtqrdlohoc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.feifeiyinyue.top/gtkbkibrwz.html

================================================================================
来源：http://hz.cdnleiting.top/gtanpbeikg.html

M. 命令行 / 进程 / 环境
来源：http://hz.wangshuangyany.cn/gtrkklpnmn.html

================================================================================
来源：http://hz.ydzc1.top/gtfvduxdcm.html

[M01] 读取命令行参数
来源：http://hz.ybcxt.top/gtpfntkddy.html

Py:   sys.argv[1:]
来源：http://hz.andypj.xyz/gtpwdfqfom.html

PHP:  $argv;  $argc;
来源：http://hz.hnqzz.top/gtjkbjlhqy.html

JS:   process.argv.slice(2)
来源：http://hz.zhongyouzk.top/gtuvbvqkra.html

TS:   process.argv.slice(2)
来源：http://hz.chenlongwang.top/gtcnwvjxno.html

Java: args 数组（main 方法参数）
来源：http://hz.jqgufenzy.top/gttaybqcwf.html

Go:   os.Args[1:]
来源：http://hz.jinyuanbaomall.cn/gtyekurriu.html

Ruby: ARGV
来源：http://hz.daxiang520.top/gtiltmnabc.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ydzc1.top/gtnsbkungb.html

[M02] 读取环境变量
来源：http://hz.hfpthk.cn/gtzslosohg.html

Py:   os.environ.get("HOME")
来源：http://hz.xziqi.cn/gtmqjxclrn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.daria6918.cn/gtgfnhuwdf.html

JS:   process.env.HOME
来源：http://hz.feifeiyinyue.top/gtxaooctwi.html

TS:   process.env.HOME
来源：http://hz.sysykeji.top/gtkedbufoo.html

Java: System.getenv("HOME")
来源：http://hz.wangshuangyany.cn/gtdfdqzskd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zycfv.cn/gtdfhazhmt.html

Ruby: ENV["HOME"]
来源：http://hz.yj20258888.top/gtznxzgref.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yangfankeji.com/gtxvrfkeog.html

[M03] 执行外部命令
来源：http://hz.fzhhl.top/gtifonsyeh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yuxming.cn/gtfauhrvin.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.gotoacloud.top/gtelutoeht.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hnqzz.top/gtupyjmnff.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yj20258888.top/gtukhcolkl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhijiandao.cn/gtwohohnxr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.meibo888.top/gttzdafqyx.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yueranfly.top/gtjfhtwgxy.html

C#:   Process.Start("ls", "-l");
来源：http://hz.nanxinkj.top/gtciijwoax.html

[M04] 获取当前工作目录
来源：http://hz.c1oappe.top/gtstkqihnr.html

Py:   os.getcwd()
来源：http://hz.xingfuxueyuan.xyz/gtiovyizwg.html

PHP:  getcwd();
来源：http://hz.shzxlz.cn/gtwwjfnssl.html

JS:   process.cwd()
来源：http://hz.ehwqpu.com/gtcqdzmipl.html

TS:   process.cwd()
来源：http://hz.jiagoushi.top/gtmlryrvge.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.shanyushiyangkeji.top/gtmduixolj.html

Go:   os.Getwd()
来源：http://hz.kuanghao11.cn/gtgnmghqgm.html

Ruby: Dir.pwd
来源：http://hz.fengsongda.top/gtvpkvwqfp.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.shanyushiyangtech.top/gtyrnqddge.html

[M05] 设置退出码
来源：http://hz.yj20258.top/gtvxhmsihj.html

Py:   sys.exit(1)
来源：http://hz.redwolf501.top/gtuxaevybw.html

PHP:  exit(1);
来源：http://hz.shuidangran.top/gtozpxrubo.html

JS:   process.exit(1)
来源：http://hz.jqgfzy.top/gtdngmpgqp.html

TS:   process.exit(1)
来源：http://hz.316326.xyz/gtmmtsozak.html

Java: System.exit(1)
来源：http://hz.nwbrower.top/gtcwggomnn.html

Go:   os.Exit(1)
来源：http://hz.ydzc1.top/gtizhcuqdv.html

Ruby: exit 1
来源：http://hz.birdmap.top/gtvhjbjgyn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.shanyushiyangkeji.top/gtpfcaszlg.html

[M06] 向标准错误输出
来源：http://hz.sufxvd.cn/gthnoptxmv.html

Py:   print("err", file=sys.stderr)
来源：http://hz.nanxinkj.top/gtpdeznxyh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yj20258888.top/gtjjxxpnik.html

JS:   console.error("err")
来源：http://hz.vqdsnc.cn/gtzbtdejxd.html

TS:   console.error("err")
来源：http://hz.quarkkingdee.top/gtnodukxve.html

Java: System.err.println("err")
来源：http://hz.cheryme.top/gtdkzspbxg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jinqigfzy.top/gtspnwslfq.html

Ruby: warn "err"
来源：http://hz.zhiwuduotai.top/gtqryqajev.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhixingplan.top/gtgshasuft.html

[M07] 判断是否为主入口
来源：http://hz.jianghu66.top/gtblvvfsfp.html

Py:   if __name__ == "__main__":
来源：http://hz.jinghuilouyu.cn/gtqtpgecaa.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cashguo.top/gtzrqngtob.html

JS:   require.main === module
来源：http://hz.pycfn.com/gtemwtxkhu.html

TS:   require.main === module
来源：http://hz.tanke756.top/gtgtvugyvn.html

Java: public static void main(String[] args)
来源：http://hz.nwbrower.top/gtdswpqamw.html

Go:   func main()
来源：http://hz.ybcxt.top/gtxoeqautg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.nanxinkj.top/gtqpljdvqp.html

C#:   static void Main(string[] args)
来源：http://hz.aizwys.cn/gtubxtcvto.html

[M08] 获取系统与运行时信息
来源：http://hz.yueranfly.top/gtxumjomiy.html

Py:   platform.system();  platform.python_version()
来源：http://hz.cqqwz.cn/gtcaqkkuot.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.aizwys.cn/gtnzldrptz.html

JS:   process.platform;  process.version
来源：http://hz.jiagoushi.top/gtnmaljtnt.html

TS:   process.platform;  process.version
来源：http://hz.ybcxt.top/gtzgypywbs.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.svipenyu.cn/gtfxuuyrwp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.chenlongwang.top/gtgmovcoov.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.dashuyun.cn/gthpfgqibl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hfpthk.cn/gtiisxpnvw.html

================================================================================
来源：http://hz.yuanzhike.top/gtglfkbdbk.html

N. 数据结构与算法
来源：http://hz.redwolf501.top/gtiragqtxm.html

================================================================================
来源：http://hz.hywenlv.cn/gtrbjxsdox.html

[N01] 二分查找（有序数组）
来源：http://hz.xinyue.icu/gtyskjvamq.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hysaishi.cn/gtqivmyuzm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yueranfly.top/gtzrpeoozv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.smart0.xyz/gtyfhillmu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zycfv.cn/gtgvxsiveu.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.guowangkeji.top/gtqwjjoggo.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.nanxuanxn.top/gthztxrjho.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.haohaochexian.top/gttthwujqf.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zhaomingkeji.xyz/gtjzxcyckz.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.316326.xyz/gtkdhyjodd.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.kuanghao11.cn/gtsqwwnrxs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.tianlin.xyz/gtgbkemxve.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hywenlv.cn/gtxwqenwpv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.smart0.xyz/gtmntujtmp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.nanxuanxn.top/gtrcpxhofw.html

Go:   slices.Sort(arr)
来源：http://hz.zhoulong.xyz/gtzozytxib.html

Ruby: arr.sort
来源：http://hz.daxiang520.top/gtupdfvpck.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jinyuanbaomall.cn/gtspiyduwg.html

[N03] 快速排序（分治示例）
来源：http://hz.ydjk.org.cn/gtbclqkbmx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.cqqwz.cn/gtpuszsjgo.html

PHP:  // 递归实现，或用 usort
来源：http://hz.0kj1m.cn/gtwzwjjlar.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yonumen.top/gtaapodfik.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.kuanghao11.cn/gtrmiunyqg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.0kj1m.cn/gtqlalzxwm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.gzhubu.top/gtblxjejal.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zdqjudy.top/gtxinrmtvj.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.hongshengwenyu.top/gtxktlwpyx.html

[N04] 斐波那契数列
来源：http://hz.fengsongda.top/gtzmgetsbc.html


<!-- 参考信息 -->