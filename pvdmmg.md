代发 wailian999

Py:   (end - start).total_seconds()
来源：http://hz.zhongyouzk.top/gttljrfjhl.html

PHP:  $end->diff($start)->days;
来源：http://hz.nanxuanxn.top/gtlasglsax.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hysaishi.cn/gteoijcbug.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yuxming.cn/gtpqdcqoun.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cucudq.cn/gttbiffiym.html

Go:   end.Sub(start).Hours()
来源：http://hz.yongpay.top/gteoyerrji.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hnqzz.top/gtrogaktmy.html

C#:   (end - start).TotalSeconds
来源：http://hz.guannengcc.top/gtmekkzjph.html

[J07] 比较两个日期
来源：http://hz.yanxiufei.cn/gtaliqqnlz.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ybcxt.top/gtaxzubict.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.snrcjt.cn/gtiznkeavg.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.shangyingyoupin.top/gtsjoczktt.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jqgfzy.top/gtgixayiwr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xinyue.icu/gthpyxpbag.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.fengsongda.top/gttvbpxgql.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.shanyushiyangtech.top/gttdntpeke.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.gogol.net.cn/gtoomduoeg.html

[J08] 提取年月日与星期
来源：http://hz.ppjwa.cn/gtzeffykoo.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.tian-w.cn/gtjeuwqpwr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yanxiufei.cn/gtbxnyrlbh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yongpay.top/gtgdoauliy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shuidangran.top/gtqchzkcgw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.pycfn.com/gtvaclpndp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.xylfe.cn/gthynybtws.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.sufxvd.cn/gtwjodayox.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jinqigufen.top/gtwfxzubce.html

[J09] 时区处理
来源：http://hz.smart0.xyz/gtwmbuidaa.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.bjfxy.top/gtuihmfsvz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.snrcjt.cn/gtbkxnlcfn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hywenlv.cn/gtbxoeqcah.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.redwolf501.top/gtcxmhpavd.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.svipenyu.cn/gtmktsdvly.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhaomingkeji.xyz/gtnvwwoxer.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.dashuyun.cn/gtvkfoakky.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhengqikj.top/gtysllsreu.html

[J10] 取今天 / 本月第一天
来源：http://hz.ywan-chungtsiang.top/gtslhhdgym.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jianghu66.top/gtgzfakukc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zycfv.cn/gtbevxtakq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhoulong.xyz/gtzplxoyep.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yueranfly.top/gtocmdpngx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jqgufenzy.top/gtqzaauuvz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.gotoacloud.top/gtisxxgigu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jinghuilouyu.cn/gtfuzwfuwf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.c1oappe.top/gteohosgex.html

================================================================================
来源：http://hz.kuanghao11.cn/gtaeqhgmkx.html

K. JSON 与序列化
来源：http://hz.tanke756.top/gtklcqahqe.html

================================================================================
来源：http://hz.havefunace.top/gtatyuglql.html

[K01] 对象转 JSON 字符串
来源：http://hz.ydjk.org.cn/gtxuawobgu.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.nwbrower.top/gtngdwgpum.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xingfuxueyuan.xyz/gtbwazbcth.html

JS:   JSON.stringify(obj)
来源：http://hz.yuanzhike.top/gtotsjhgvr.html

TS:   JSON.stringify(obj)
来源：http://hz.jinqigfzy.top/gtgknamsbf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.kuanghao11.cn/gtreeudizt.html

Go:   json.Marshal(obj)
来源：http://hz.hongshengwenyu.top/gtcmhtagnz.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.0kj1m.cn/gttiijphth.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jinqigufen.top/gtljlqojlu.html

[K02] JSON 字符串转对象
来源：http://hz.0kj1m.cn/gtmtkzjzhq.html

Py:   json.loads(s)
来源：http://hz.ivvv.top/gtpmptkany.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.haohaochexian.top/gtxdlovjpk.html

JS:   JSON.parse(s)
来源：http://hz.kuanghao11.cn/gtagbdnzbd.html

TS:   JSON.parse(s)
来源：http://hz.gaohongyu789.top/gtcqclzivz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.fzhhl.top/gtxkenrhjv.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yangfankeji.com/gttwpklrxz.html

Ruby: JSON.parse(s)
来源：http://hz.sysykeji.top/gtmofwthwn.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xylfe.cn/gtgmoompmx.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ybcxt.top/gtscnvkxac.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.guannengcc.top/gtujzofksx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ppjwa.cn/gtkhckvhuj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ppjwa.cn/gtviyrkyiz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj20258.top/gtqfmbhult.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.havefunace.top/gtsgsyaobp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.iojbl.cn/gtrimhngex.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.aizwys.cn/gtlftrjvaj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.tian-w.cn/gtztpovrjs.html

[K04] 读取 JSON 文件
来源：http://hz.jinyuanbaomall.cn/gtvywhpjif.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jinghuilouyu.cn/gtravzzrcz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.wangshuangyany.cn/gtvrzesuyp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gotoacloud.top/gtuthwajgm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhengqikj.top/gtgarjsbvv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.xinyue.icu/gtuvastdjl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.pengpengdd.cyou/gtxhviyxmy.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ehwqpu.com/gtupkahfkg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.smart0.xyz/gtrejwvqay.html

[K05] 深拷贝对象
来源：http://hz.vqdsnc.cn/gtqmtioipa.html

Py:   copy.deepcopy(obj)
来源：http://hz.yj20258.top/gtasiejqdo.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cqqwz.cn/gtwbettpqe.html

JS:   structuredClone(obj)
来源：http://hz.316326.xyz/gtnzdgkhzb.html

TS:   structuredClone(obj)
来源：http://hz.pengpengdd.cyou/gtmvnapsvk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yj20258888.top/gtqusqvgrj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.tian-w.cn/gttulnwafu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yvedp.cn/gtfsyboepz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jqgfzy.top/gtjztytglu.html

[K06] 解析 URL 查询串
来源：http://hz.xuetiantiany.cn/gtfawnhczn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.wangshuangyany.cn/gtsiktkgkf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.svipenyu.cn/gtzzorzahf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinqigfzy.top/gtcemzbfip.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.guowangkeji.top/gtaqohyzsm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yonumen.top/gttxmnixqp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.vqdsnc.cn/gthvbcdrdu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yangfankeji.com/gtgqcaqate.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhaomingkeji.xyz/gtpvtabyvb.html

[K07] 进制转换
来源：http://hz.havefunace.top/gtidltreys.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jyoumei.cn/gtmghchfjp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.shuidangran.top/gteglqfjcp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yuanzhike.top/gtwdiqrdpe.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yuxming.cn/gtwmoyoeql.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hywenlv.cn/gteslyvxza.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.sysykeji.top/gttmnalhll.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ppjwa.cn/gtxquffnzf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.dianchejie.cn/gtwjnmojrc.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yuxming.cn/gtedusnscq.html

Py:   pickle.dumps(obj)
来源：http://hz.xingfuxueyuan.xyz/gtuhohmrbz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zhongyouzk.top/gtcslygnxw.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hammf.cn/gtaenffaux.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.9152youxi.cn/gtkshwhlze.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.aizwys.cn/gtrboenpil.html

Go:   encoding/gob
来源：http://hz.ydjk.org.cn/gtgimshxan.html

Ruby: Marshal.dump(obj)
来源：http://hz.jinqigufen.top/gtqqhawbzi.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xinyue.icu/gtouzvkaye.html

================================================================================
来源：http://hz.vqdsnc.cn/gtswbfloxl.html

L. 网络请求
来源：http://hz.shuidangran.top/gtmawphqch.html

================================================================================
来源：http://hz.aizwys.cn/gtcinzyeal.html

[L01] 发送 GET 请求
来源：http://hz.yonumen.top/gtecdfrdpi.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.tianlin.xyz/gtvfmnmddr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.xinyue.icu/gthjecrdih.html

JS:   await fetch(url)
来源：http://hz.havefunace.top/gtzxdjbsqz.html

TS:   await fetch(url)
来源：http://hz.yuanzhike.top/gtodslwdqj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yj202588.top/gtnkdlakgx.html

Go:   resp, err := http.Get(url)
来源：http://hz.cheryme.top/gtmltovenn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhaomingkeji.xyz/gtkemfighz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hywenlv.cn/gtypimbhll.html

[L02] 发送 POST JSON
来源：http://hz.zycfv.cn/gtymnvkgwr.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.dianchejie.cn/gtwxosbnby.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xziqi.cn/gtplnbqjyw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ywan-chungtsiang.top/gtnlwpqatb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yj20258.top/gtguchfikl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jinghuilouyu.cn/gtoslfhvrv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.cucudq.cn/gtjqjzouhf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.52xcode.cn/gtkpvoofjg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zhoulong.xyz/gtpwvinxjx.html

[L03] 设置自定义请求头
来源：http://hz.yuxming.cn/gtulcjtenv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xuanzx.com/gtbvifnyzj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.nwbrower.top/gtidoxhbiw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yanxiufei.cn/gtqzpdtzeu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj202588.top/gtkhnikumc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jinghuilouyu.cn/gtlnezojek.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.haohaochexian.top/gtzmasznyg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hnqzz.top/gtfkkjlprv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jlsjyb.cn/gtqvubcwyy.html

[L04] 设置超时
来源：http://hz.ywan-chungtsiang.top/gtuaueyiek.html

Py:   requests.get(url, timeout=5)
来源：http://hz.pycfn.com/gtvxmlaiqw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.hammf.cn/gtiuqfqgcd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nwbrower.top/gtccapvelq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.daria6918.cn/gtepyrdmgn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jinqigufen.top/gtoyvfecfl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.cucudq.cn/gthpbyfcte.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hongshengwenyu.top/gtdgdikvva.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.quarkkingdee.top/gtrtnrxybx.html

[L05] 上传文件（multipart）
来源：http://hz.iojbl.cn/gtxlntodio.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.aizwys.cn/gtyaywranc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhijiandao.cn/gthjufreix.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yueranfly.top/gtbcejhwhc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jqgufenzy.top/gtwyerbyiz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.guannengcc.top/gtstjdbubi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jqgfzy.top/gtfgsvmmvs.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ivvv.top/gtdhmnkxlj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.ydjk.org.cn/gtbspyuype.html

[L06] 解析响应为 JSON
来源：http://hz.ydjk.org.cn/gtudgulrza.html

Py:   resp.json()
来源：http://hz.tianlin.xyz/gthpmerqvs.html

PHP:  json_decode($body, true);
来源：http://hz.yongpay.top/gtofbdhqyk.html

JS:   await resp.json()
来源：http://hz.dashuyun.cn/gtlrdfdikf.html

TS:   await resp.json()
来源：http://hz.zhijiandao.cn/gtatybhkxy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yonumen.top/gtplftcydy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yj20258888.top/gtyfehmoqc.html

Ruby: JSON.parse(resp.body)
来源：http://hz.hywenlv.cn/gtjsjoqqpm.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jinyuanbaomall.cn/gtsnlsvxin.html

[L07] 处理 HTTP 状态码
来源：http://hz.shanyushiyangkeji.top/gtadabbixy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.chenzaomai.com/gtdlacjope.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.vqdsnc.cn/gtztjqwoqq.html

JS:   resp.ok;  resp.status
来源：http://hz.cdnleiting.top/gtmrglcucl.html

TS:   resp.ok;  resp.status
来源：http://hz.aizwys.cn/gttsyeyhrw.html

Java: resp.statusCode()
来源：http://hz.hysaishi.cn/gtrfjcqmga.html

Go:   resp.StatusCode
来源：http://hz.yvedp.cn/gtoahvhbyb.html

Ruby: resp.code.to_i
来源：http://hz.vqdsnc.cn/gtmqnnzpbd.html

C#:   (int)resp.StatusCode
来源：http://hz.jlsjyb.cn/gtillyvknl.html

[L08] 并发请求多个地址
来源：http://hz.zhiwuduotai.top/gtcsviukxd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hnqzz.top/gtmkjgbcmo.html

PHP:  curl_multi_init() 系列
来源：http://hz.fengsongda.top/gtmrhuuuyf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xingfuxueyuan.xyz/gtcjdpgmay.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jianghu66.top/gttsxcmjce.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yonumen.top/gtmynszguc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ehwqpu.com/gtnymxnhqq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.feifeiyinyue.top/gtlapxwhkq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ydzc1.top/gtmsuuqabp.html

================================================================================
来源：http://hz.sweek.top/gtxraczmvc.html

M. 命令行 / 进程 / 环境
来源：http://hz.redwolf501.top/gtqgffbfyp.html

================================================================================
来源：http://hz.redwolf501.top/gtidotomvs.html

[M01] 读取命令行参数
来源：http://hz.meibo888.top/gtsptdhpvg.html

Py:   sys.argv[1:]
来源：http://hz.cheryme.top/gtrzknzqvx.html

PHP:  $argv;  $argc;
来源：http://hz.ehwqpu.com/gtuqrpnnub.html

JS:   process.argv.slice(2)
来源：http://hz.sweek.top/gtnzrcvhld.html

TS:   process.argv.slice(2)
来源：http://hz.hnxiangtu.top/gtxwukhskc.html

Java: args 数组（main 方法参数）
来源：http://hz.cdnleiting.top/gtuctcgmwn.html

Go:   os.Args[1:]
来源：http://hz.nanxinkj.top/gtjxzznouv.html

Ruby: ARGV
来源：http://hz.feifeiyinyue.top/gtivzzyhbf.html

C#:   args 数组（Main 方法参数）
来源：http://hz.bjfxy.top/gtodiobqrt.html

[M02] 读取环境变量
来源：http://hz.yangfankeji.com/gtzaoujjjh.html

Py:   os.environ.get("HOME")
来源：http://hz.yongpay.top/gtqkkpwgvz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jlsjyb.cn/gtfnvaisfh.html

JS:   process.env.HOME
来源：http://hz.gogol.net.cn/gtfqgqvysv.html

TS:   process.env.HOME
来源：http://hz.feifeiyinyue.top/gtbentrqrx.html

Java: System.getenv("HOME")
来源：http://hz.zycfv.cn/gtscnxxbhp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.gogol.net.cn/gtrbtccuys.html

Ruby: ENV["HOME"]
来源：http://hz.chenlongwang.top/gtkpfuxghe.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jqgufenzy.top/gtncbhfxra.html

[M03] 执行外部命令
来源：http://hz.jqgufenzy.top/gtmyafivrd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.nwbrower.top/gthtqinazk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yuanzhike.top/gtomckltmn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.andypj.xyz/gtkixhnvhr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.cqqwz.cn/gtaxzmbbhe.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.pengpengdd.cyou/gtvafykvfl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hfpthk.cn/gtzzgfceyn.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.ydjk.org.cn/gtfovnheqm.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yanxiufei.cn/gtjbcfvbnj.html

[M04] 获取当前工作目录
来源：http://hz.dashuyun.cn/gtfubbntud.html

Py:   os.getcwd()
来源：http://hz.ehwqpu.com/gtywugpqfb.html

PHP:  getcwd();
来源：http://hz.pengpengdd.cyou/gttibanvii.html

JS:   process.cwd()
来源：http://hz.9152youxi.cn/gtgdcpdoan.html

TS:   process.cwd()
来源：http://hz.cheryme.top/gtzxupbhiz.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.tian-w.cn/gtvmegwnrr.html

Go:   os.Getwd()
来源：http://hz.feifeiyinyue.top/gtazocevcu.html

Ruby: Dir.pwd
来源：http://hz.ppjwa.cn/gtkkatyvnl.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.cashguo.top/gtpuybynis.html

[M05] 设置退出码
来源：http://hz.andypj.xyz/gtzwbbxaih.html

Py:   sys.exit(1)
来源：http://hz.xziqi.cn/gtvhfljyui.html

PHP:  exit(1);
来源：http://hz.daria6918.cn/gtdseqrzhg.html

JS:   process.exit(1)
来源：http://hz.daria6918.cn/gtebklojvd.html

TS:   process.exit(1)
来源：http://hz.hnqzz.top/gtqufqjkmp.html

Java: System.exit(1)
来源：http://hz.vqdsnc.cn/gtyonedczl.html

Go:   os.Exit(1)
来源：http://hz.yangfankeji.com/gtsjsqpfpn.html

Ruby: exit 1
来源：http://hz.hongshengwenyu.top/gtvlnwbqoh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jqgfzy.top/gttjiszhlw.html

[M06] 向标准错误输出
来源：http://hz.cqqwz.cn/gtwzqnsrxg.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xziqi.cn/gtwxejsjhe.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.sweek.top/gtxprcqiqk.html

JS:   console.error("err")
来源：http://hz.ywan-chungtsiang.top/gtjlcpkgdm.html

TS:   console.error("err")
来源：http://hz.c1oappe.top/gtcjsuqldo.html

Java: System.err.println("err")
来源：http://hz.yongpay.top/gtwxupezyu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.haohaochexian.top/gtorlkvxpp.html

Ruby: warn "err"
来源：http://hz.shanyushiyangkeji.top/gtclkyfpji.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.aibaodan.cn/gtteapewek.html

[M07] 判断是否为主入口
来源：http://hz.vqdsnc.cn/gttlpwqlil.html

Py:   if __name__ == "__main__":
来源：http://hz.aizwys.cn/gtvhrxquyu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.tian-w.cn/gthzjkyovx.html

JS:   require.main === module
来源：http://hz.cucudq.cn/gtpjvxwoke.html

TS:   require.main === module
来源：http://hz.xingfuxueyuan.xyz/gtkicfvykn.html

Java: public static void main(String[] args)
来源：http://hz.jyoumei.cn/gtobtrjawb.html

Go:   func main()
来源：http://hz.jinqigfzy.top/gtchqmlpgb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yj20258.top/gtbncnlnvv.html

C#:   static void Main(string[] args)
来源：http://hz.birdmap.top/gtsjtkzlxb.html

[M08] 获取系统与运行时信息
来源：http://hz.sweek.top/gtcdvtwffx.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hammf.cn/gturvpjjiy.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ywan-chungtsiang.top/gtnbndzoqk.html

JS:   process.platform;  process.version
来源：http://hz.meibo888.top/gtmjzevubu.html

TS:   process.platform;  process.version
来源：http://hz.yj202588.top/gtdxasnxcd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.tianlin.xyz/gthfynubvj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.shanyushiyangkeji.top/gtyxsterwe.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.vqdsnc.cn/gtsfpgqhqg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.pengpengdd.cyou/gtvwntfelx.html

================================================================================
来源：http://hz.jyoumei.cn/gtkwyqaost.html

N. 数据结构与算法
来源：http://hz.hammf.cn/gtqkvrcmam.html

================================================================================
来源：http://hz.yangfankeji.com/gtixrbniwr.html

[N01] 二分查找（有序数组）
来源：http://hz.cashguo.top/gtgufuurly.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.cashguo.top/gtcmezdxlp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.aibaodan.cn/gtxxhuehyz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yj20258888.top/gtrsgxkbid.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yangfankeji.com/gtbjipmjfu.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.guannengcc.top/gtwocwfaqn.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.shzxlz.cn/gtyoruitmk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.bjfxy.top/gteteuphwg.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ehwqpu.com/gtzgnschqt.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.mhx1999.top/gtjnigdobp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinyuanbaomall.cn/gtfjjglbth.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.gogol.net.cn/gtzooipcue.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.fengsongda.top/gtuqgfusyu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ivvv.top/gtkujldiid.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ppjwa.cn/gtrsmjutzj.html

Go:   slices.Sort(arr)
来源：http://hz.yuxming.cn/gtuppcpcwq.html

Ruby: arr.sort
来源：http://hz.ivvv.top/gtyawszwjn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.redwolf501.top/gtjrymmzns.html

[N03] 快速排序（分治示例）
来源：http://hz.hysaishi.cn/gttyxecytn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hywenlv.cn/gtenjttnev.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xziqi.cn/gtorzdtaug.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xuanzx.com/gteycaqsqs.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xuanzx.com/gtosjnlzjx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhongyouzk.top/gtqhnhxikx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.ywan-chungtsiang.top/gtbjjaixfk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.guannengcc.top/gtbpvsqmxf.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhongyouzk.top/gtlpygwlsq.html

[N04] 斐波那契数列
来源：http://hz.dianchejie.cn/gtjbxsykwu.html


<!-- 参考信息 -->