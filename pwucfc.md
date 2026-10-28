代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://hz.guowangkeji.top/gtngateunq.html

Go:   end.Sub(start).Hours()
来源：http://hz.chenjidiqi.icu/gtqxveuyab.html

Ruby: end - start                 # 返回秒数
来源：http://hz.xingfuxueyuan.xyz/gtaaftvpgg.html

C#:   (end - start).TotalSeconds
来源：http://hz.jiagoushi.top/gtwuqkcvzg.html

[J07] 比较两个日期
来源：http://hz.jinyuanbaomall.cn/gtlobwlyfr.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.sysykeji.top/gtizqtqsxf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.pengpengdd.cyou/gtblfrjqqe.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.aizwys.cn/gtplhutaiu.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.cdnleiting.top/gtabzhvcti.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.redwolf501.top/gtozlqsodg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hfpthk.cn/gtkoxwwgms.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.sufxvd.cn/gtorjqzvlx.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hammf.cn/gtywtzdduk.html

[J08] 提取年月日与星期
来源：http://hz.pycfn.com/gtmreakwag.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.sxryk.cn/gtxkfrghfy.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xuetiantiany.cn/gtcafdumzv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhixingplan.top/gtcthqmeqd.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yangfankeji.com/gtwehpkebi.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hywenlv.cn/gtlclkrwgy.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.gotoacloud.top/gtipsrbmhp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhoulong.xyz/gtlwivnoue.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.52xcode.cn/gtlprjosfk.html

[J09] 时区处理
来源：http://hz.ywan-chungtsiang.top/gttrvcqbwk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.gotoacloud.top/gtcovqotzg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.birdmap.top/gtuyivxqle.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.daria6918.cn/gtztjkizvf.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhijiandao.cn/gtwbziybth.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.shuidangran.top/gteuhcmfvo.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.cashguo.top/gtqbuhnpju.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.daria6918.cn/gtysarbyhd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.nanxuanxn.top/gtdicvoyna.html

[J10] 取今天 / 本月第一天
来源：http://hz.jiagoushi.top/gtvjyyyban.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.xziqi.cn/gtadyfgqqs.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hammf.cn/gttyhaasvp.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hnqzz.top/gtpsvuwwcw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.quarkkingdee.top/gtbfjxsawb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhoulong.xyz/gtdxkglrlr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.dianchejie.cn/gtssvnoiog.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.0kj1m.cn/gtwjgfutkt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zhoulong.xyz/gtrkcumoqq.html

================================================================================
来源：http://hz.cheryme.top/gtdqdhtili.html

K. JSON 与序列化
来源：http://hz.jinyuanbaomall.cn/gtjctnimin.html

================================================================================
来源：http://hz.shuidangran.top/gtxskgqkel.html

[K01] 对象转 JSON 字符串
来源：http://hz.birdmap.top/gtfovcbplj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.sysykeji.top/gtjjqttnmc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.tanke756.top/gthzcwjbda.html

JS:   JSON.stringify(obj)
来源：http://hz.ydzc1.top/gtdtetlyfj.html

TS:   JSON.stringify(obj)
来源：http://hz.chenjidiqi.icu/gtqyoiawgz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yueranfly.top/gtjnhnpbuk.html

Go:   json.Marshal(obj)
来源：http://hz.birdmap.top/gtamndahsl.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.gaohongyu789.top/gtoqkyasvx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yuanzhike.top/gtiutathns.html

[K02] JSON 字符串转对象
来源：http://hz.daria6918.cn/gtsfkoowex.html

Py:   json.loads(s)
来源：http://hz.birdmap.top/gtyookehtb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jqgufenzy.top/gtnqoptsev.html

JS:   JSON.parse(s)
来源：http://hz.cashguo.top/gttedsnoxz.html

TS:   JSON.parse(s)
来源：http://hz.yongpay.top/gtolookfzp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.guowangkeji.top/gtasxdueqq.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.nanxinkj.top/gtfemgsstq.html

Ruby: JSON.parse(s)
来源：http://hz.nanxuanxn.top/gtyhiyykdl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.shangyingyoupin.top/gtmperdjps.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yonumen.top/gttastsyso.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ppjwa.cn/gtoitdffxq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yj20258.top/gtgnrzbvaf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.bjfxy.top/gtuvpfddbk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.gaohongyu789.top/gtopudxnsf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.52xcode.cn/gthmjasmtj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.sysykeji.top/gtsjaildgv.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.shuidangran.top/gtyzijzmli.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.sweek.top/gtfraszfnx.html

[K04] 读取 JSON 文件
来源：http://hz.birdmap.top/gtrcsvtjhi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.chenjidiqi.icu/gtkbzugbzb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shanyushiyangkeji.top/gtkhlzjrtj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hfpthk.cn/gtpodpfzep.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hywenlv.cn/gtxvddbujd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.chenzaomai.com/gtiaewahig.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yongpay.top/gtxhcjezcr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.haohaochexian.top/gtmgusxnok.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.birdmap.top/gtfwnaqqqn.html

[K05] 深拷贝对象
来源：http://hz.0kj1m.cn/gtufrpqirw.html

Py:   copy.deepcopy(obj)
来源：http://hz.xingfuxueyuan.xyz/gtrbfwqwyv.html

PHP:  unserialize(serialize($obj));
来源：http://hz.sweek.top/gtluzreuaw.html

JS:   structuredClone(obj)
来源：http://hz.cheryme.top/gtgozdkjev.html

TS:   structuredClone(obj)
来源：http://hz.tianlin.xyz/gtrrddpdzr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.haohaochexian.top/gtknrhhogk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.sysykeji.top/gthwoekkiz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jyoumei.cn/gtysdltsle.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.316326.xyz/gtpamjpaac.html

[K06] 解析 URL 查询串
来源：http://hz.aibaodan.cn/gtemxfxhin.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jinyuanbaomall.cn/gtkdcuwqzj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.aibaodan.cn/gtdiqvedty.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.redwolf501.top/gtoezumznz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xziqi.cn/gtudgpxiiu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.shangyingyoupin.top/gttuprdjjw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.wangshuangyany.cn/gtlfwqtlav.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ydzc1.top/gtlwuhszao.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yongpay.top/gtyszxbjgu.html

[K07] 进制转换
来源：http://hz.fzhhl.top/gtpfadislm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.fengsongda.top/gtwfgtpeaq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jyoumei.cn/gthjxathep.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jqgufenzy.top/gtonmkqwmr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.iojbl.cn/gtfgzujqmn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xinyue.icu/gtewcskzef.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jiagoushi.top/gtxjrwdpnl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.havefunace.top/gttukedpbg.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yonumen.top/gtcbwrtvxb.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.cqqwz.cn/gtjiwnfbyf.html

Py:   pickle.dumps(obj)
来源：http://hz.jinqigfzy.top/gtljaonsct.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.vqdsnc.cn/gtqnewtjkc.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.0kj1m.cn/gtezqvgpqk.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jlsjyb.cn/gtgepmiaii.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.gogol.net.cn/gtbapfxsyf.html

Go:   encoding/gob
来源：http://hz.yj20258888.top/gtbnnhghgi.html

Ruby: Marshal.dump(obj)
来源：http://hz.jqgufenzy.top/gtjwwlokew.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.haohaochexian.top/gtzofhsmfb.html

================================================================================
来源：http://hz.chenlongwang.top/gtkcofnifu.html

L. 网络请求
来源：http://hz.haohaochexian.top/gtdfkgesfm.html

================================================================================
来源：http://hz.xinyue.icu/gtdqmbmyko.html

[L01] 发送 GET 请求
来源：http://hz.nanxuanxn.top/gtmguzzcxy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yuanzhike.top/gtoqwewslp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.sufxvd.cn/gtscgmvrbk.html

JS:   await fetch(url)
来源：http://hz.tian-w.cn/gtaczjqqru.html

TS:   await fetch(url)
来源：http://hz.sysykeji.top/gtmgonxfen.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.shanyushiyangkeji.top/gtdcquzvlb.html

Go:   resp, err := http.Get(url)
来源：http://hz.shanyushiyangkeji.top/gtoxvlllgg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.gaohongyu789.top/gtzigeqjtt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.52xcode.cn/gtebepnzgf.html

[L02] 发送 POST JSON
来源：http://hz.sysykeji.top/gtoknonnzj.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.chenlongwang.top/gtegnmspzt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.nanxuanxn.top/gtbfrzfbam.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.chenjidiqi.icu/gtwnghtkbs.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.mhx1999.top/gtjilsakur.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.shanyushiyangtech.top/gtunjucrif.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.tanke756.top/gtpdwdglyd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.shzxlz.cn/gtpdulqxfh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ydzc1.top/gtyrorefrr.html

[L03] 设置自定义请求头
来源：http://hz.nwbrower.top/gtdwdhybza.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhengqikj.top/gtwamqulyu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ybcxt.top/gtlroxemlm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gotoacloud.top/gtjwsklqxt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gogol.net.cn/gtcuzvbwsk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.andypj.xyz/gttxapukbu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.smart0.xyz/gtyswhkfhc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.vqdsnc.cn/gtwkcymmkd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.sxryk.cn/gtxygqjsar.html

[L04] 设置超时
来源：http://hz.gotoacloud.top/gttqtmcsev.html

Py:   requests.get(url, timeout=5)
来源：http://hz.bjfxy.top/gtussiljuz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.9152youxi.cn/gttcjwzukx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj20258888.top/gtiuqoxqdn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.chenlongwang.top/gthehrwims.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.shangyingyoupin.top/gtmhvrladt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ywan-chungtsiang.top/gtskjohcoj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jiagoushi.top/gtsviyqhvy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.sysykeji.top/gtnqpikiqu.html

[L05] 上传文件（multipart）
来源：http://hz.jqgfzy.top/gthwvrdcem.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.feifeiyinyue.top/gtnkmvgxte.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yangfankeji.com/gtjchjhcyn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.shanyushiyangkeji.top/gttuscgnbd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ywan-chungtsiang.top/gtpwulagzc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.nwbrower.top/gtbpdqtcni.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.hammf.cn/gtjnugfybh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ywan-chungtsiang.top/gtodtqeezj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhoulong.xyz/gtrwgsflkq.html

[L06] 解析响应为 JSON
来源：http://hz.jlsjyb.cn/gtldqqhmrn.html

Py:   resp.json()
来源：http://hz.xingfuxueyuan.xyz/gtxkprmjne.html

PHP:  json_decode($body, true);
来源：http://hz.aizwys.cn/gtfjainpig.html

JS:   await resp.json()
来源：http://hz.xingfuxueyuan.xyz/gtradfxoou.html

TS:   await resp.json()
来源：http://hz.daxiang520.top/gthcgtgdoz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.cashguo.top/gtmvynvknq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.pycfn.com/gterjzbnfj.html

Ruby: JSON.parse(resp.body)
来源：http://hz.chenjidiqi.icu/gtccvbfapt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.bjfxy.top/gtyrpzadsn.html

[L07] 处理 HTTP 状态码
来源：http://hz.yanxiufei.cn/gtkvucuecd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.tanke756.top/gtegtuatnv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.haohaochexian.top/gtsnewknjx.html

JS:   resp.ok;  resp.status
来源：http://hz.nanxuanxn.top/gtixunusdm.html

TS:   resp.ok;  resp.status
来源：http://hz.zhiwuduotai.top/gtkpgcsovm.html

Java: resp.statusCode()
来源：http://hz.sysykeji.top/gtciqrrmrg.html

Go:   resp.StatusCode
来源：http://hz.nanxuanxn.top/gtzvlyclrz.html

Ruby: resp.code.to_i
来源：http://hz.sweek.top/gtgmflfkpa.html

C#:   (int)resp.StatusCode
来源：http://hz.svipenyu.cn/gtntztdbgx.html

[L08] 并发请求多个地址
来源：http://hz.pengpengdd.cyou/gtuuewpvbj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jlsjyb.cn/gtnxmycodt.html

PHP:  curl_multi_init() 系列
来源：http://hz.jiagoushi.top/gtmkqmavzg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shangyingyoupin.top/gticghascj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hammf.cn/gtwrgccrqc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yvedp.cn/gtngdrtvbr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhixingplan.top/gtxrxfummj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.fzhhl.top/gtyynqtdsf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yuxming.cn/gtvfjhrzna.html

================================================================================
来源：http://hz.jinqigfzy.top/gtqbdsgacj.html

M. 命令行 / 进程 / 环境
来源：http://hz.yanxiufei.cn/gtgvdkcqvq.html

================================================================================
来源：http://hz.zhijiandao.cn/gtfmvczbea.html

[M01] 读取命令行参数
来源：http://hz.vqdsnc.cn/gtvfvyoxvn.html

Py:   sys.argv[1:]
来源：http://hz.yongpay.top/gtgujprare.html

PHP:  $argv;  $argc;
来源：http://hz.redwolf501.top/gtgbztslxg.html

JS:   process.argv.slice(2)
来源：http://hz.ydzc1.top/gtiszheuxu.html

TS:   process.argv.slice(2)
来源：http://hz.sxryk.cn/gtmvghamvu.html

Java: args 数组（main 方法参数）
来源：http://hz.yanxiufei.cn/gtoyrwrrga.html

Go:   os.Args[1:]
来源：http://hz.wangshuangyany.cn/gtvawfuzek.html

Ruby: ARGV
来源：http://hz.52xcode.cn/gtgpydfgjw.html

C#:   args 数组（Main 方法参数）
来源：http://hz.nwbrower.top/gtldrioacf.html

[M02] 读取环境变量
来源：http://hz.jinghuilouyu.cn/gtwkvnyocd.html

Py:   os.environ.get("HOME")
来源：http://hz.hnqzz.top/gtvhbvknit.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.nwbrower.top/gtqxryirvk.html

JS:   process.env.HOME
来源：http://hz.gzhubu.top/gtnubtbsdr.html

TS:   process.env.HOME
来源：http://hz.zhiwuduotai.top/gtpzxzuofh.html

Java: System.getenv("HOME")
来源：http://hz.cdnleiting.top/gtwuzjxyty.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.cucudq.cn/gtnoaxlcwf.html

Ruby: ENV["HOME"]
来源：http://hz.nwbrower.top/gtsepzlhmt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.pycfn.com/gtwewyvwbe.html

[M03] 执行外部命令
来源：http://hz.daria6918.cn/gtkbcwdkif.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yongpay.top/gtagnvzkgs.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.shanyushiyangtech.top/gtwxmqglgw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yonumen.top/gtferltmgb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ybcxt.top/gtzsqlleku.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zdqjudy.top/gtolczgpsn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.xylfe.cn/gteapglmyi.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.feifeiyinyue.top/gtoxkcodfe.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jinghuilouyu.cn/gtmkizltth.html

[M04] 获取当前工作目录
来源：http://hz.zhongyouzk.top/gttbvqiexd.html

Py:   os.getcwd()
来源：http://hz.svipenyu.cn/gtqngnmmxk.html

PHP:  getcwd();
来源：http://hz.smart0.xyz/gtsyuckepu.html

JS:   process.cwd()
来源：http://hz.0kj1m.cn/gtrtznsffi.html

TS:   process.cwd()
来源：http://hz.mhx1999.top/gtjhguolfu.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.mhx1999.top/gtcwwpnaav.html

Go:   os.Getwd()
来源：http://hz.bjfxy.top/gthquyiguf.html

Ruby: Dir.pwd
来源：http://hz.wangdashe.top/gtfokixjfn.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yongpay.top/gtuzscjmyi.html

[M05] 设置退出码
来源：http://hz.tanke756.top/gtuhgjfjwe.html

Py:   sys.exit(1)
来源：http://hz.yj20258.top/gtuydhzcsj.html

PHP:  exit(1);
来源：http://hz.meibo888.top/gtomjrtuoc.html

JS:   process.exit(1)
来源：http://hz.shanyushiyangtech.top/gtcoqtldye.html

TS:   process.exit(1)
来源：http://hz.zycfv.cn/gtsrvgtiae.html

Java: System.exit(1)
来源：http://hz.shzxlz.cn/gtfyurcbsi.html

Go:   os.Exit(1)
来源：http://hz.xziqi.cn/gtyelxrjtk.html

Ruby: exit 1
来源：http://hz.daxiang520.top/gtpnbatbru.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.chenzaomai.com/gtyyjjmyqc.html

[M06] 向标准错误输出
来源：http://hz.aizwys.cn/gtqjqmumlg.html

Py:   print("err", file=sys.stderr)
来源：http://hz.tanke756.top/gtxltplkit.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yj202588.top/gthupckoxm.html

JS:   console.error("err")
来源：http://hz.hammf.cn/gtgovlqtss.html

TS:   console.error("err")
来源：http://hz.shanyushiyangkeji.top/gttpsqzxex.html

Java: System.err.println("err")
来源：http://hz.chenjidiqi.icu/gtndnyxrqe.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhixingplan.top/gtkzfypwvg.html

Ruby: warn "err"
来源：http://hz.jinqigfzy.top/gtimqqwyme.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.gaohongyu789.top/gtdsxwashb.html

[M07] 判断是否为主入口
来源：http://hz.zhijiandao.cn/gtowxufpdx.html

Py:   if __name__ == "__main__":
来源：http://hz.jqgfzy.top/gtlgrttxxb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xinyue.icu/gtqjdgpplu.html

JS:   require.main === module
来源：http://hz.hongshengwenyu.top/gtxhczeotk.html

TS:   require.main === module
来源：http://hz.52xcode.cn/gtjipquhro.html

Java: public static void main(String[] args)
来源：http://hz.c1oappe.top/gtuazybzqk.html

Go:   func main()
来源：http://hz.cqqwz.cn/gtzhcgxvve.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.wangdashe.top/gtvdcwozwd.html

C#:   static void Main(string[] args)
来源：http://hz.chenjidiqi.icu/gtozvxczwy.html

[M08] 获取系统与运行时信息
来源：http://hz.jinghuilouyu.cn/gteqmwqjta.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ivvv.top/gtxnmakdbs.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.sysykeji.top/gtrdijjfvw.html

JS:   process.platform;  process.version
来源：http://hz.yonumen.top/gtwdbltnzk.html

TS:   process.platform;  process.version
来源：http://hz.c1oappe.top/gtuokbdgmv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.9152youxi.cn/gtffazxnop.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xylfe.cn/gttaioqsfh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.sweek.top/gtclhdooil.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.tianlin.xyz/gtjvasopec.html

================================================================================
来源：http://hz.dianchejie.cn/gtddueelnm.html

N. 数据结构与算法
来源：http://hz.hongshengwenyu.top/gtpynljenj.html

================================================================================
来源：http://hz.xylfe.cn/gtvavqpjno.html

[N01] 二分查找（有序数组）
来源：http://hz.hammf.cn/gtoitemzqb.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.guowangkeji.top/gtlqjxcnhl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jinyuanbaomall.cn/gtqqjmnjij.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hfpthk.cn/gtiapudemf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yj20258.top/gtenlinznx.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.c1oappe.top/gthbwpjsan.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yuxming.cn/gtvsjksfck.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.9152youxi.cn/gtkzjygyht.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jinyuanbaomall.cn/gtsppsvjui.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.vqdsnc.cn/gtvdmkeygu.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cqqwz.cn/gtpwkzkcww.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.fzhhl.top/gtjygesaqi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hywenlv.cn/gtetlgzmsy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.haohaochexian.top/gtazaxyiko.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.9152youxi.cn/gtmxdrrgmx.html

Go:   slices.Sort(arr)
来源：http://hz.hammf.cn/gtcunykzeh.html

Ruby: arr.sort
来源：http://hz.meibo888.top/gtkonsbffp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jqgufenzy.top/gtylxwhhwd.html

[N03] 快速排序（分治示例）
来源：http://hz.jlsjyb.cn/gtzbprgino.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xuanzx.com/gtvxozaqry.html

PHP:  // 递归实现，或用 usort
来源：http://hz.birdmap.top/gtllcqpljp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.pycfn.com/gtxbxwrhle.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xuetiantiany.cn/gtyzzvwlfc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.cheryme.top/gttsqrhehv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.shanyushiyangkeji.top/gtupbicotn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ydjk.org.cn/gtdpmbstxs.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhijiandao.cn/gtwbkmmajh.html

[N04] 斐波那契数列
来源：http://hz.jinghuilouyu.cn/gtroqftgio.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.pycfn.com/gtjezasoak.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.feifeiyinyue.top/gtuirjxpbz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.aizwys.cn/gtqndktrdu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cdnleiting.top/gtkuhngndo.html


<!-- 参考信息 -->