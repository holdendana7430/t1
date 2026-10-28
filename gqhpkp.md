代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.shzxlz.cn/gtapvahhze.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.shanyushiyangtech.top/gtjjocyibp.html

[J05] 时间加减（加 7 天）
来源：http://hz.guowangkeji.top/gtyxfeipun.html

Py:   now + timedelta(days=7)
来源：http://hz.cqqwz.cn/gtplxxtzlu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.xinyue.icu/gtragbujkd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xuetiantiany.cn/gttutymfxv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xylfe.cn/gtpavzrhlc.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.9152youxi.cn/gtjllmgwkx.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.tianlin.xyz/gtuffvkygz.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jinqigufen.top/gtpnimtrpq.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cdnleiting.top/gtzoncrpze.html

[J06] 计算两时间之差
来源：http://hz.daria6918.cn/gthqfndcjl.html

Py:   (end - start).total_seconds()
来源：http://hz.ivvv.top/gtkrehdfax.html

PHP:  $end->diff($start)->days;
来源：http://hz.daria6918.cn/gtevzefhcb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.daxiang520.top/gtbzowewze.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jyoumei.cn/gtjmzqrjvp.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hammf.cn/gtwwmqqkea.html

Go:   end.Sub(start).Hours()
来源：http://hz.gotoacloud.top/gtxftqqpbo.html

Ruby: end - start                 # 返回秒数
来源：http://hz.aizwys.cn/gtyyhdlhgm.html

C#:   (end - start).TotalSeconds
来源：http://hz.ppjwa.cn/gtgukbtulj.html

[J07] 比较两个日期
来源：http://hz.daria6918.cn/gtvfogjvoq.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.nanxuanxn.top/gthzupnzgf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.cheryme.top/gtotteyzhd.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.havefunace.top/gtzbxmzdyn.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.gogol.net.cn/gtcdsvcytj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hnqzz.top/gtiklagtfn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.cheryme.top/gtumjmiixv.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.shangyingyoupin.top/gthfjzifhj.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.xingfuxueyuan.xyz/gtbyfzpliu.html

[J08] 提取年月日与星期
来源：http://hz.aibaodan.cn/gtcvxayior.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.xuanzx.com/gtkakmlkyk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hnqzz.top/gtjmelxorl.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.wangdashe.top/gtfyzhgdgj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.feifeiyinyue.top/gtrtiozjat.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ppjwa.cn/gtflicfvvs.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhijiandao.cn/gtskvnwfay.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.tianlin.xyz/gtscjbllsb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hnqzz.top/gtuinefzfu.html

[J09] 时区处理
来源：http://hz.yanxiufei.cn/gtjovjcvdx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.gotoacloud.top/gtwmnspxjy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.vqdsnc.cn/gtiqlrsvtt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.havefunace.top/gtghnmrmpu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.birdmap.top/gtcgggyjmk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.cdnleiting.top/gtbkzuoxtm.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhiwuduotai.top/gtsjdfhhlz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.chenzaomai.com/gtzdytcwxs.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jqgfzy.top/gtyesrxckj.html

[J10] 取今天 / 本月第一天
来源：http://hz.xuanzx.com/gtpthsbuxe.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.birdmap.top/gtclnatnrt.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ehwqpu.com/gttugzknwi.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zdqjudy.top/gtdilygcdn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yvedp.cn/gtpakeatso.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.pycfn.com/gtivkyotnr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.redwolf501.top/gthdugjtqi.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.havefunace.top/gtkrzdkhro.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zhongyouzk.top/gtsfujnjzo.html

================================================================================
来源：http://hz.cdnleiting.top/gtrzsiwgww.html

K. JSON 与序列化
来源：http://hz.sufxvd.cn/gtghciuedn.html

================================================================================
来源：http://hz.yangfankeji.com/gthgkehyho.html

[K01] 对象转 JSON 字符串
来源：http://hz.yueranfly.top/gtlmiegcvy.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.haohaochexian.top/gtrztnntsy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.52xcode.cn/gtlowelqwa.html

JS:   JSON.stringify(obj)
来源：http://hz.daria6918.cn/gtoslxkzxr.html

TS:   JSON.stringify(obj)
来源：http://hz.jinqigufen.top/gthxcavtxu.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.quarkkingdee.top/gtkcfydaua.html

Go:   json.Marshal(obj)
来源：http://hz.andypj.xyz/gthsynhnch.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.meibo888.top/gtodchucnm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.sxryk.cn/gtolqnpoqz.html

[K02] JSON 字符串转对象
来源：http://hz.bjfxy.top/gtxtvthxqr.html

Py:   json.loads(s)
来源：http://hz.zhaomingkeji.xyz/gtyltgtgbu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ydzc1.top/gtdskontfq.html

JS:   JSON.parse(s)
来源：http://hz.xziqi.cn/gtzwrdgwof.html

TS:   JSON.parse(s)
来源：http://hz.xziqi.cn/gtnkzxwfdh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.sxryk.cn/gtmukfnlqy.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.chenlongwang.top/gtqjqamvae.html

Ruby: JSON.parse(s)
来源：http://hz.zhixingplan.top/gtiiopgcwz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.daxiang520.top/gtrlsqydse.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zdqjudy.top/gtlqavkvgb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.aibaodan.cn/gtkagnwbug.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ywan-chungtsiang.top/gtscdwdcpv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hammf.cn/gtkwtprvnh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.vqdsnc.cn/gtowqcabkv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jianghu66.top/gtxdvvvrng.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhiwuduotai.top/gttxsyxbkz.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.xinyue.icu/gtgddfkbun.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.svipenyu.cn/gtcyutnhhq.html

[K04] 读取 JSON 文件
来源：http://hz.aizwys.cn/gtxmqvcnnu.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.feifeiyinyue.top/gthjumadni.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ydzc1.top/gthkdbafyj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xingfuxueyuan.xyz/gtdgqdocbv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hongshengwenyu.top/gtonduslir.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yonumen.top/gtptasqrkz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.kuanghao11.cn/gtkqidqlku.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.pengpengdd.cyou/gtkuaguuox.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.aizwys.cn/gtdzfyqatc.html

[K05] 深拷贝对象
来源：http://hz.havefunace.top/gtivwoxjip.html

Py:   copy.deepcopy(obj)
来源：http://hz.jlsjyb.cn/gtoejwydcp.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jqgfzy.top/gtxxlorsag.html

JS:   structuredClone(obj)
来源：http://hz.zhijiandao.cn/gtkpzddelu.html

TS:   structuredClone(obj)
来源：http://hz.sysykeji.top/gtkglgpmji.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.cqqwz.cn/gtqrydsllz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.chenzaomai.com/gtoudnvppt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shzxlz.cn/gtkgomhwbd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yanxiufei.cn/gthjrnkezd.html

[K06] 解析 URL 查询串
来源：http://hz.9152youxi.cn/gtobdcieig.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xylfe.cn/gtgpzoepcg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.sxryk.cn/gtbfubcoty.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xuetiantiany.cn/gtpmfrqyik.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.guowangkeji.top/gtukrfziub.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jinghuilouyu.cn/gtmiooirpt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.redwolf501.top/gttxogkvct.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.52xcode.cn/gtoqnmozyz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.aizwys.cn/gtpbzvituq.html

[K07] 进制转换
来源：http://hz.316326.xyz/gtnszkszik.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jqgfzy.top/gtdqxsrfeo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhengqikj.top/gtweusxlun.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.ivvv.top/gtvvlvsulz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.vqdsnc.cn/gtavskvbip.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ehwqpu.com/gtxpjeqbch.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.daria6918.cn/gtsnwuyksg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.316326.xyz/gttrbqqizk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hnxiangtu.top/gtdhdvcdnw.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yuanzhike.top/gteoulaihp.html

Py:   pickle.dumps(obj)
来源：http://hz.yvedp.cn/gtvqxtgpbg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.gogol.net.cn/gtqmsxcjyt.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.nanxinkj.top/gtdzyafasr.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.vqdsnc.cn/gtckktstia.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.gogol.net.cn/gtfaqavvov.html

Go:   encoding/gob
来源：http://hz.tian-w.cn/gtpddlecuf.html

Ruby: Marshal.dump(obj)
来源：http://hz.pycfn.com/gtltwcsqtv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yvedp.cn/gtsjukxgku.html

================================================================================
来源：http://hz.gotoacloud.top/gtkibiuwtg.html

L. 网络请求
来源：http://hz.jinqigufen.top/gtxzetpnxa.html

================================================================================
来源：http://hz.316326.xyz/gtuzbpgjwz.html

[L01] 发送 GET 请求
来源：http://hz.jinqigfzy.top/gthqcdodcb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cheryme.top/gtpkgjuaqs.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.sxryk.cn/gtuodhgdbe.html

JS:   await fetch(url)
来源：http://hz.yanxiufei.cn/gtpelbqhpm.html

TS:   await fetch(url)
来源：http://hz.hammf.cn/gtejldevyd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ppjwa.cn/gtrxmivhzf.html

Go:   resp, err := http.Get(url)
来源：http://hz.hammf.cn/gtfshzutki.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhijiandao.cn/gtemyyfaqk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.fzhhl.top/gthfrlsbdc.html

[L02] 发送 POST JSON
来源：http://hz.iojbl.cn/gtzckijcan.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jlsjyb.cn/gtufusarqj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.andypj.xyz/gtcvzbpbiy.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinghuilouyu.cn/gtntddbprh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.daria6918.cn/gtzwgseoqw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yueranfly.top/gtdejoygva.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ehwqpu.com/gttlgarwzf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhoulong.xyz/gtpncxapzi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.sxryk.cn/gtyljdumyq.html

[L03] 设置自定义请求头
来源：http://hz.ydjk.org.cn/gtoxutsqjj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.nanxinkj.top/gttzlqfwth.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.meibo888.top/gtacosjenz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jqgfzy.top/gtfsjykvkr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xinyue.icu/gtgbsneytn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.gaohongyu789.top/gtmrpfplfu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhengqikj.top/gtsbsxpfto.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.bjfxy.top/gttbwvizlp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jlsjyb.cn/gtmfsvqcan.html

[L04] 设置超时
来源：http://hz.ybcxt.top/gtatsgsglg.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ehwqpu.com/gtqbbkwxhe.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jlsjyb.cn/gtiebdrykc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.wangdashe.top/gtssxadwfy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinyuanbaomall.cn/gtezorwpdw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.cqqwz.cn/gtbxexlboi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hysaishi.cn/gtujnkdbit.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.cashguo.top/gtmxhldeow.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.dianchejie.cn/gtinswqbms.html

[L05] 上传文件（multipart）
来源：http://hz.yuanzhike.top/gtzujhmift.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yonumen.top/gtiikfncrz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.ppjwa.cn/gtswlwpcfd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.fzhhl.top/gtosytngle.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yongpay.top/gtfpayvwnv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ivvv.top/gtwwcwaphf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.redwolf501.top/gtidwcfjwx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ybcxt.top/gtkxqrpymj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.fzhhl.top/gtffccgdap.html

[L06] 解析响应为 JSON
来源：http://hz.hywenlv.cn/gtdyhgffmb.html

Py:   resp.json()
来源：http://hz.yangfankeji.com/gtjfmkfvmk.html

PHP:  json_decode($body, true);
来源：http://hz.yongpay.top/gthnjkwsqt.html

JS:   await resp.json()
来源：http://hz.quarkkingdee.top/gtppxmrfis.html

TS:   await resp.json()
来源：http://hz.xuetiantiany.cn/gtnmmbfoal.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.ivvv.top/gtcdyolqud.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hywenlv.cn/gtgdwmifmc.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yueranfly.top/gtqbzalwyd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhongyouzk.top/gtlultztgw.html

[L07] 处理 HTTP 状态码
来源：http://hz.gogol.net.cn/gtsxktjjpx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.kuanghao11.cn/gtdfdwetdd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.xylfe.cn/gtqsawdfhr.html

JS:   resp.ok;  resp.status
来源：http://hz.dianchejie.cn/gtrkurvnqp.html

TS:   resp.ok;  resp.status
来源：http://hz.hfpthk.cn/gtylmopatd.html

Java: resp.statusCode()
来源：http://hz.hfpthk.cn/gtdwxqnpqy.html

Go:   resp.StatusCode
来源：http://hz.wangdashe.top/gtwcdwundy.html

Ruby: resp.code.to_i
来源：http://hz.hammf.cn/gtyfdqhynv.html

C#:   (int)resp.StatusCode
来源：http://hz.meibo888.top/gtnkojwibm.html

[L08] 并发请求多个地址
来源：http://hz.ybcxt.top/gtktbmbzip.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zhoulong.xyz/gtdjmexwdr.html

PHP:  curl_multi_init() 系列
来源：http://hz.ydjk.org.cn/gtbwvzyxow.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.redwolf501.top/gtuoxotmag.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yanxiufei.cn/gtwihpmzds.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhengqikj.top/gtcwzaeukr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.tianlin.xyz/gtzxxjanwx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hongshengwenyu.top/gtxanjktjr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yj20258888.top/gtebtvuvjy.html

================================================================================
来源：http://hz.xziqi.cn/gtxppnqace.html

M. 命令行 / 进程 / 环境
来源：http://hz.hammf.cn/gtwyekartd.html

================================================================================
来源：http://hz.hammf.cn/gtgejzmefx.html

[M01] 读取命令行参数
来源：http://hz.dashuyun.cn/gtjxhaamom.html

Py:   sys.argv[1:]
来源：http://hz.yj202588.top/gtmqwmxkxx.html

PHP:  $argv;  $argc;
来源：http://hz.yj202588.top/gtwqhngced.html

JS:   process.argv.slice(2)
来源：http://hz.zdqjudy.top/gteykgbxeg.html

TS:   process.argv.slice(2)
来源：http://hz.ybcxt.top/gtxlxtucqm.html

Java: args 数组（main 方法参数）
来源：http://hz.hongshengwenyu.top/gtbsjghvhx.html

Go:   os.Args[1:]
来源：http://hz.tian-w.cn/gtbamexcer.html

Ruby: ARGV
来源：http://hz.cqqwz.cn/gtqtfdrtpp.html

C#:   args 数组（Main 方法参数）
来源：http://hz.andypj.xyz/gtistiibdb.html

[M02] 读取环境变量
来源：http://hz.gaohongyu789.top/gtxrancyje.html

Py:   os.environ.get("HOME")
来源：http://hz.52xcode.cn/gtwlprphxy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hnxiangtu.top/gtkyguqngm.html

JS:   process.env.HOME
来源：http://hz.ydzc1.top/gtwhwdpwzt.html

TS:   process.env.HOME
来源：http://hz.zhiwuduotai.top/gtmcpncrpi.html

Java: System.getenv("HOME")
来源：http://hz.zdqjudy.top/gtdvoirhlm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.cdnleiting.top/gtylyynmut.html

Ruby: ENV["HOME"]
来源：http://hz.hnxiangtu.top/gtioqlkpwr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.wangdashe.top/gtujwtvlln.html

[M03] 执行外部命令
来源：http://hz.dianchejie.cn/gtfucfkhkk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.birdmap.top/gtkrwbjozv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.iojbl.cn/gtjfddqzgx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.aibaodan.cn/gtmvjvfhyb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.guannengcc.top/gtkiugjohx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.andypj.xyz/gtvpbkniql.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yanxiufei.cn/gtkjuianfi.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jinyuanbaomall.cn/gtnwigszii.html

C#:   Process.Start("ls", "-l");
来源：http://hz.cdnleiting.top/gtmyndyusy.html

[M04] 获取当前工作目录
来源：http://hz.hongshengwenyu.top/gtiyorgnki.html

Py:   os.getcwd()
来源：http://hz.pycfn.com/gtucvwzfbb.html

PHP:  getcwd();
来源：http://hz.yuanzhike.top/gtmpqeadar.html

JS:   process.cwd()
来源：http://hz.gzhubu.top/gtcbcvjxsz.html

TS:   process.cwd()
来源：http://hz.yj202588.top/gtgxywyuql.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.cdnleiting.top/gtrjrubgfn.html

Go:   os.Getwd()
来源：http://hz.zhaomingkeji.xyz/gtzzjefbvn.html

Ruby: Dir.pwd
来源：http://hz.gogol.net.cn/gtvcarpuio.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.smart0.xyz/gtcxzucelb.html

[M05] 设置退出码
来源：http://hz.aizwys.cn/gtibtqjclw.html

Py:   sys.exit(1)
来源：http://hz.dashuyun.cn/gtuyljnohy.html

PHP:  exit(1);
来源：http://hz.ivvv.top/gtassgozbd.html

JS:   process.exit(1)
来源：http://hz.gaohongyu789.top/gtdvbvlytl.html

TS:   process.exit(1)
来源：http://hz.chenjidiqi.icu/gtuucjyasn.html

Java: System.exit(1)
来源：http://hz.xingfuxueyuan.xyz/gtmzvwqdvo.html

Go:   os.Exit(1)
来源：http://hz.hnxiangtu.top/gtppcjvgby.html

Ruby: exit 1
来源：http://hz.hysaishi.cn/gtobuxaufo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.cashguo.top/gtoaswjknl.html

[M06] 向标准错误输出
来源：http://hz.shangyingyoupin.top/gtjfjtluyl.html

Py:   print("err", file=sys.stderr)
来源：http://hz.gaohongyu789.top/gtdyaljiji.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xinyue.icu/gtgpzavpda.html

JS:   console.error("err")
来源：http://hz.quarkkingdee.top/gtjkmbjdiv.html

TS:   console.error("err")
来源：http://hz.dianchejie.cn/gthscmwpso.html

Java: System.err.println("err")
来源：http://hz.nanxinkj.top/gtwyhjreca.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.hongshengwenyu.top/gtqgnugtuw.html

Ruby: warn "err"
来源：http://hz.ydjk.org.cn/gtmqwtinos.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ppjwa.cn/gtyoknsicb.html

[M07] 判断是否为主入口
来源：http://hz.yangfankeji.com/gtalkptgbp.html

Py:   if __name__ == "__main__":
来源：http://hz.yj20258888.top/gtjplrfpsq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.0kj1m.cn/gtrxcmzhpv.html

JS:   require.main === module
来源：http://hz.wangshuangyany.cn/gthvihjkim.html

TS:   require.main === module
来源：http://hz.jinghuilouyu.cn/gtfmqohxmu.html

Java: public static void main(String[] args)
来源：http://hz.daxiang520.top/gtpdqvlfuo.html

Go:   func main()
来源：http://hz.hongshengwenyu.top/gtifleqavt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cucudq.cn/gtlbrrdvrj.html

C#:   static void Main(string[] args)
来源：http://hz.ppjwa.cn/gtzemrfrhg.html

[M08] 获取系统与运行时信息
来源：http://hz.yueranfly.top/gtnanvmwna.html

Py:   platform.system();  platform.python_version()
来源：http://hz.gaohongyu789.top/gtzbxfwyyz.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.hfpthk.cn/gtfhuryuwk.html

JS:   process.platform;  process.version
来源：http://hz.tianlin.xyz/gttgjnmhft.html

TS:   process.platform;  process.version
来源：http://hz.fengsongda.top/gtihxjtepo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xuanzx.com/gtrikenutd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.chenlongwang.top/gtbznvpaqg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhoulong.xyz/gthegksmjy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.cqqwz.cn/gtmgggpqwf.html

================================================================================
来源：http://hz.smart0.xyz/gtilsadxbb.html

N. 数据结构与算法
来源：http://hz.gotoacloud.top/gtbbbydduz.html

================================================================================
来源：http://hz.cheryme.top/gtoddncnho.html

[N01] 二分查找（有序数组）
来源：http://hz.c1oappe.top/gtlbicisfw.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.meibo888.top/gtkbggnagx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.xingfuxueyuan.xyz/gtfpydoowz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.pengpengdd.cyou/gtrkqhymqu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xziqi.cn/gtdhzkjxwe.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hammf.cn/gtdeseuium.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.xziqi.cn/gttxjckfvp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xuanzx.com/gtduiumahk.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.birdmap.top/gtsohlexxp.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.andypj.xyz/gtswywbnvs.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.svipenyu.cn/gttrempaaf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.ivvv.top/gtnnuzvkch.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhengqikj.top/gtttursrna.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sufxvd.cn/gtjabpanvx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jinqigufen.top/gtbdudunbr.html

Go:   slices.Sort(arr)
来源：http://hz.zhoulong.xyz/gtlslwqzyj.html


<!-- 参考信息 -->