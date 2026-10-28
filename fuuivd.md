代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://hz.dianchejie.cn/gtcgjzlvuy.html

Go:   end.Sub(start).Hours()
来源：http://hz.ywan-chungtsiang.top/gtjufsretz.html

Ruby: end - start                 # 返回秒数
来源：http://hz.gzhubu.top/gtufhvyjme.html

C#:   (end - start).TotalSeconds
来源：http://hz.wangdashe.top/gtblbzqxte.html

[J07] 比较两个日期
来源：http://hz.meibo888.top/gtacqydmyr.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hammf.cn/gtfjwkuqoa.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hammf.cn/gthkdsbkls.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.fzhhl.top/gtnkdcdxcg.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.mhx1999.top/gtdjrjodwl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhiwuduotai.top/gtddteposz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.daxiang520.top/gtienggzmq.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hongshengwenyu.top/gtpvnpxyph.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.9152youxi.cn/gtlihkuceq.html

[J08] 提取年月日与星期
来源：http://hz.0kj1m.cn/gtfbljrgyh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zycfv.cn/gtxlteuouc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jlsjyb.cn/gtcqboeubx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jiagoushi.top/gtqlojbpfs.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.xylfe.cn/gtrvfmsldg.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.fzhhl.top/gteejwxroh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.nwbrower.top/gtlupqoywr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ywan-chungtsiang.top/gtrzojerpx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhongyouzk.top/gtquliocek.html

[J09] 时区处理
来源：http://hz.shangyingyoupin.top/gtvpvfagam.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cdnleiting.top/gtlcgbvguk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.chenzaomai.com/gtbjbictdn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yonumen.top/gtddxuzkdq.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hfpthk.cn/gtywuuammk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yongpay.top/gtacakfido.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.fzhhl.top/gthqnhpjrf.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.kuanghao11.cn/gtyrcmrrpe.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.havefunace.top/gtzplovytq.html

[J10] 取今天 / 本月第一天
来源：http://hz.yj20258888.top/gtlocpqpgu.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.wangdashe.top/gtkoauuejc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.vqdsnc.cn/gtfxxzkbmi.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hammf.cn/gtijqzkicw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hfpthk.cn/gtrziftpia.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shzxlz.cn/gtvuhoqqtk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.316326.xyz/gtbqmhmuwj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jinyuanbaomall.cn/gtsjytykib.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jqgufenzy.top/gtineornjs.html

================================================================================
来源：http://hz.xziqi.cn/gtdomscffr.html

K. JSON 与序列化
来源：http://hz.jinqigufen.top/gtgyizwfpt.html

================================================================================
来源：http://hz.yonumen.top/gtwzkaiadr.html

[K01] 对象转 JSON 字符串
来源：http://hz.chenlongwang.top/gtlqdrdbhn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ppjwa.cn/gtfzcesvwn.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jyoumei.cn/gtsmbffxpo.html

JS:   JSON.stringify(obj)
来源：http://hz.zycfv.cn/gtteetumlt.html

TS:   JSON.stringify(obj)
来源：http://hz.iojbl.cn/gtzhdpubgu.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yanxiufei.cn/gtjmtivvbz.html

Go:   json.Marshal(obj)
来源：http://hz.hnqzz.top/gthnnqajuz.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cashguo.top/gtmmgwoumv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.svipenyu.cn/gtnixswzjj.html

[K02] JSON 字符串转对象
来源：http://hz.yuanzhike.top/gtqhkxmrqn.html

Py:   json.loads(s)
来源：http://hz.316326.xyz/gtucxpdqat.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.c1oappe.top/gtlvyceiur.html

JS:   JSON.parse(s)
来源：http://hz.dianchejie.cn/gtorjzqcjb.html

TS:   JSON.parse(s)
来源：http://hz.0kj1m.cn/gtpknqfzcb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jinyuanbaomall.cn/gtrfpgsjjv.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jqgfzy.top/gtonallnba.html

Ruby: JSON.parse(s)
来源：http://hz.yvedp.cn/gtbjwqxstl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhoulong.xyz/gtdepxnnap.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.redwolf501.top/gtxmainuvu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yonumen.top/gtgayyfjpd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.quarkkingdee.top/gtpgiquqjz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.cashguo.top/gtxdmpeyhs.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cheryme.top/gtqcwstdyr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.sxryk.cn/gtakwmjajk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hysaishi.cn/gthpeyvbso.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jianghu66.top/gtcqgwqebh.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.sxryk.cn/gtauuyjeuq.html

[K04] 读取 JSON 文件
来源：http://hz.tanke756.top/gtuhsmieke.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hnxiangtu.top/gtrjhypyvq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jqgufenzy.top/gtdgleyvrw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shanyushiyangtech.top/gtnnnkghnn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.chenlongwang.top/gtjsexqfkg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.sysykeji.top/gtqqpwhqyy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.nanxuanxn.top/gtfusjybju.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.quarkkingdee.top/gtxbdhhzal.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.haohaochexian.top/gtxaejlzax.html

[K05] 深拷贝对象
来源：http://hz.9152youxi.cn/gtsehzhgha.html

Py:   copy.deepcopy(obj)
来源：http://hz.guannengcc.top/gttbwcskns.html

PHP:  unserialize(serialize($obj));
来源：http://hz.xylfe.cn/gtjdztiksf.html

JS:   structuredClone(obj)
来源：http://hz.sysykeji.top/gtghydjilm.html

TS:   structuredClone(obj)
来源：http://hz.cheryme.top/gttayigdkk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhaomingkeji.xyz/gtxgdmzzmq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.tianlin.xyz/gtyryrtyby.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.316326.xyz/gtumplhqwv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.gogol.net.cn/gtlzeeksyu.html

[K06] 解析 URL 查询串
来源：http://hz.chenjidiqi.icu/gtmlxrblnb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.0kj1m.cn/gtktjvytjo.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hongshengwenyu.top/gtwopopauh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.snrcjt.cn/gtpakilcor.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yuanzhike.top/gtlwpfuepv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.chenzaomai.com/gtdmpzlcst.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.aizwys.cn/gtunrayyuy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.guowangkeji.top/gtsxkghyqb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.hfpthk.cn/gtmebaviph.html

[K07] 进制转换
来源：http://hz.tanke756.top/gtklfalbjq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.c1oappe.top/gtywwzfgtd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhaomingkeji.xyz/gtfjzzkose.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xziqi.cn/gthbsrasfo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.chenlongwang.top/gtfhdjzhcn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yangfankeji.com/gtuepmquae.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.cheryme.top/gtszeakxjl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.mhx1999.top/gteyjoslrl.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.cqqwz.cn/gttwjppfvg.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.fengsongda.top/gtrujqrknq.html

Py:   pickle.dumps(obj)
来源：http://hz.cdnleiting.top/gtjxkhywqu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.chenzaomai.com/gtfkfapqzp.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.tian-w.cn/gthlybuvup.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.gogol.net.cn/gtvejcjshd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhijiandao.cn/gtqmaxhbhz.html

Go:   encoding/gob
来源：http://hz.dashuyun.cn/gtkqypyaff.html

Ruby: Marshal.dump(obj)
来源：http://hz.zdqjudy.top/gtyewqpavi.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.gaohongyu789.top/gtzpkmziex.html

================================================================================
来源：http://hz.sxryk.cn/gtfknbttpv.html

L. 网络请求
来源：http://hz.hnxiangtu.top/gtcxhsbynz.html

================================================================================
来源：http://hz.redwolf501.top/gtxrhtahsr.html

[L01] 发送 GET 请求
来源：http://hz.mhx1999.top/gtscvcgfjx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.bjfxy.top/gtwgpucfnn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.haohaochexian.top/gttqnffxmp.html

JS:   await fetch(url)
来源：http://hz.shzxlz.cn/gtpsacwhmt.html

TS:   await fetch(url)
来源：http://hz.ydjk.org.cn/gtrfvqfyas.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jinghuilouyu.cn/gtlrkiakto.html

Go:   resp, err := http.Get(url)
来源：http://hz.xylfe.cn/gthcxcydci.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.shanyushiyangtech.top/gtmnodshyp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yongpay.top/gtfxxdyvsk.html

[L02] 发送 POST JSON
来源：http://hz.nanxinkj.top/gtmzivsqyj.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.snrcjt.cn/gtgcqkbyrv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.iojbl.cn/gtvfnkiinu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhoulong.xyz/gtqientgkx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinghuilouyu.cn/gttkxlstig.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.quarkkingdee.top/gthyccwbha.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.52xcode.cn/gteusxxdqb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.ydjk.org.cn/gtsphvooby.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hnxiangtu.top/gtovqaguvi.html

[L03] 设置自定义请求头
来源：http://hz.guowangkeji.top/gtpkcrhzpw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhengqikj.top/gtdpazkubv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.kuanghao11.cn/gthlyazrhu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yanxiufei.cn/gtnbrqftam.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yonumen.top/gtjafagkkn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.haohaochexian.top/gteapclkcp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hnxiangtu.top/gtivldrkwf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yuxming.cn/gtfjpqaxsd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jlsjyb.cn/gtuntawllm.html

[L04] 设置超时
来源：http://hz.cdnleiting.top/gtrknxzjod.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yj20258.top/gtgxofcryf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.tanke756.top/gtwfdmbyzd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.snrcjt.cn/gtdbuxpziu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jyoumei.cn/gtatmtsqip.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.sweek.top/gtkkhunnbz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.gogol.net.cn/gtlkdlhggs.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hfpthk.cn/gtwtdqwzip.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.cdnleiting.top/gtlozszjac.html

[L05] 上传文件（multipart）
来源：http://hz.shzxlz.cn/gtmrwmtpda.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jqgfzy.top/gtslkrhrdt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.sufxvd.cn/gtdsphwdja.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.havefunace.top/gtkhbsgpuh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.bjfxy.top/gtcybshxzl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jlsjyb.cn/gtgkxvbhto.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jqgfzy.top/gtixrkxgob.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.c1oappe.top/gtualypqrh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhengqikj.top/gtvxabaote.html

[L06] 解析响应为 JSON
来源：http://hz.gotoacloud.top/gtyzzsxfts.html

Py:   resp.json()
来源：http://hz.jqgfzy.top/gtvawtgdfj.html

PHP:  json_decode($body, true);
来源：http://hz.ywan-chungtsiang.top/gtmzuodnic.html

JS:   await resp.json()
来源：http://hz.haohaochexian.top/gtqqyjmfzf.html

TS:   await resp.json()
来源：http://hz.snrcjt.cn/gtxxsteosy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhoulong.xyz/gtzphdfklk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yuxming.cn/gtrptaodzs.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jinqigufen.top/gtdvwsoeen.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.cashguo.top/gtxzwapzbk.html

[L07] 处理 HTTP 状态码
来源：http://hz.cashguo.top/gtnqdfruow.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.andypj.xyz/gtlworrujz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhijiandao.cn/gtsndidhxs.html

JS:   resp.ok;  resp.status
来源：http://hz.zycfv.cn/gtchkmlvrv.html

TS:   resp.ok;  resp.status
来源：http://hz.yj202588.top/gtonvywnrx.html

Java: resp.statusCode()
来源：http://hz.cashguo.top/gtofuiadlc.html

Go:   resp.StatusCode
来源：http://hz.ydzc1.top/gtjaozpwll.html

Ruby: resp.code.to_i
来源：http://hz.jinqigfzy.top/gtvoswnzch.html

C#:   (int)resp.StatusCode
来源：http://hz.gzhubu.top/gthscwovse.html

[L08] 并发请求多个地址
来源：http://hz.ywan-chungtsiang.top/gtegwhwyag.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.gaohongyu789.top/gtzrclmhik.html

PHP:  curl_multi_init() 系列
来源：http://hz.0kj1m.cn/gtpmmmhyse.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hywenlv.cn/gtiynrfict.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.bjfxy.top/gtvrsracmq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.meibo888.top/gtwbgebcje.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yj202588.top/gtnskteugc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.redwolf501.top/gtyzderxbk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.havefunace.top/gtyrxefkcx.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtwytdzdrv.html

M. 命令行 / 进程 / 环境
来源：http://hz.jlsjyb.cn/gtryadfpze.html

================================================================================
来源：http://hz.ehwqpu.com/gtudrbzidd.html

[M01] 读取命令行参数
来源：http://hz.nanxuanxn.top/gtmwfpgxsy.html

Py:   sys.argv[1:]
来源：http://hz.aizwys.cn/gthsfqicrb.html

PHP:  $argv;  $argc;
来源：http://hz.zhoulong.xyz/gtevikufwh.html

JS:   process.argv.slice(2)
来源：http://hz.hfpthk.cn/gtesjantig.html

TS:   process.argv.slice(2)
来源：http://hz.xingfuxueyuan.xyz/gtjkoajdyw.html

Java: args 数组（main 方法参数）
来源：http://hz.zdqjudy.top/gtydjrqila.html

Go:   os.Args[1:]
来源：http://hz.wangshuangyany.cn/gtfnsmnfpi.html

Ruby: ARGV
来源：http://hz.yj20258.top/gtitlawlte.html

C#:   args 数组（Main 方法参数）
来源：http://hz.52xcode.cn/gtssjpvilc.html

[M02] 读取环境变量
来源：http://hz.yueranfly.top/gtpvfoqhyg.html

Py:   os.environ.get("HOME")
来源：http://hz.fengsongda.top/gtsmxbglrr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.aizwys.cn/gtlhznljmw.html

JS:   process.env.HOME
来源：http://hz.jinqigufen.top/gtlamvjpfc.html

TS:   process.env.HOME
来源：http://hz.zhengqikj.top/gtkjktuedj.html

Java: System.getenv("HOME")
来源：http://hz.bjfxy.top/gtnyzhjmkx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.gotoacloud.top/gtfvqfybfo.html

Ruby: ENV["HOME"]
来源：http://hz.xuanzx.com/gtwmacopxm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shuidangran.top/gtsuxjxoyh.html

[M03] 执行外部命令
来源：http://hz.pengpengdd.cyou/gtykmxscwv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhongyouzk.top/gtgakpyarr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.aibaodan.cn/gtoefveedf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xingfuxueyuan.xyz/gtuhbuxwjr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.quarkkingdee.top/gtqwdlddae.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yangfankeji.com/gtfksxispe.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.cashguo.top/gtzpgnqusv.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.havefunace.top/gtqqlvwvqg.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhongyouzk.top/gtpbqukxxr.html

[M04] 获取当前工作目录
来源：http://hz.jinghuilouyu.cn/gtxmlkqwre.html

Py:   os.getcwd()
来源：http://hz.yuanzhike.top/gtmluuqwgb.html

PHP:  getcwd();
来源：http://hz.yj202588.top/gtuswcbdlf.html

JS:   process.cwd()
来源：http://hz.xuanzx.com/gtlygttbdl.html

TS:   process.cwd()
来源：http://hz.zdqjudy.top/gtpzqcyuar.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.shanyushiyangkeji.top/gtsxeovflq.html

Go:   os.Getwd()
来源：http://hz.chenzaomai.com/gtgnhuyipq.html

Ruby: Dir.pwd
来源：http://hz.yvedp.cn/gtdtjfptwq.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.wangshuangyany.cn/gtiqovyrbj.html

[M05] 设置退出码
来源：http://hz.xziqi.cn/gtfkaonubp.html

Py:   sys.exit(1)
来源：http://hz.jqgfzy.top/gtluwbvywi.html

PHP:  exit(1);
来源：http://hz.yanxiufei.cn/gtlqnozknc.html

JS:   process.exit(1)
来源：http://hz.52xcode.cn/gtrgxjzuak.html

TS:   process.exit(1)
来源：http://hz.pycfn.com/gtwmmgvdfz.html

Java: System.exit(1)
来源：http://hz.dianchejie.cn/gtwhumxloz.html

Go:   os.Exit(1)
来源：http://hz.tianlin.xyz/gturoqmxkt.html

Ruby: exit 1
来源：http://hz.pengpengdd.cyou/gtknnikfva.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.xuetiantiany.cn/gtkernjdew.html

[M06] 向标准错误输出
来源：http://hz.bjfxy.top/gttwmpsrvh.html

Py:   print("err", file=sys.stderr)
来源：http://hz.aizwys.cn/gtuypyobbv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.snrcjt.cn/gtpsdfcetx.html

JS:   console.error("err")
来源：http://hz.gotoacloud.top/gtjpakvsgc.html

TS:   console.error("err")
来源：http://hz.yj202588.top/gtlawikqsu.html

Java: System.err.println("err")
来源：http://hz.vqdsnc.cn/gtuqxdhmbn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jiagoushi.top/gtwwypubqn.html

Ruby: warn "err"
来源：http://hz.jyoumei.cn/gtbfyvaprb.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.shuidangran.top/gthudcyngv.html

[M07] 判断是否为主入口
来源：http://hz.yuxming.cn/gtvmulixqy.html

Py:   if __name__ == "__main__":
来源：http://hz.jqgufenzy.top/gttctjpvlt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zdqjudy.top/gtntdrdryo.html

JS:   require.main === module
来源：http://hz.pycfn.com/gttgewvsmp.html

TS:   require.main === module
来源：http://hz.quarkkingdee.top/gtgjasddsd.html

Java: public static void main(String[] args)
来源：http://hz.cqqwz.cn/gtdhwlvnjw.html

Go:   func main()
来源：http://hz.yueranfly.top/gtmvnzjcwv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.daria6918.cn/gttmfagzhy.html

C#:   static void Main(string[] args)
来源：http://hz.sweek.top/gtcjkatfyl.html

[M08] 获取系统与运行时信息
来源：http://hz.kuanghao11.cn/gtosshrqcw.html

Py:   platform.system();  platform.python_version()
来源：http://hz.havefunace.top/gtrriiqhxx.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.tianlin.xyz/gtyzpmabub.html

JS:   process.platform;  process.version
来源：http://hz.chenzaomai.com/gthkvbrgmk.html

TS:   process.platform;  process.version
来源：http://hz.gogol.net.cn/gtqeymhkvv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yuxming.cn/gtceunmcqv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.fengsongda.top/gthtmpmcay.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.kuanghao11.cn/gtyhkbvuca.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.c1oappe.top/gtgtwjpajk.html

================================================================================
来源：http://hz.sufxvd.cn/gtcqzfdwqb.html

N. 数据结构与算法
来源：http://hz.shzxlz.cn/gtfsnscrde.html

================================================================================
来源：http://hz.guannengcc.top/gtnzyrdovi.html

[N01] 二分查找（有序数组）
来源：http://hz.aizwys.cn/gtzyncegst.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.meibo888.top/gtjqxhyqab.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.sufxvd.cn/gtizewfmzw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.bjfxy.top/gtonntfsbe.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.svipenyu.cn/gtetctsepy.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.fengsongda.top/gtbttksgqq.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.havefunace.top/gtfstxkhrz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yj20258.top/gtbdmjvioi.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yanxiufei.cn/gtfymayfng.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yj20258888.top/gthflougma.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sxryk.cn/gtyemksmlg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.ehwqpu.com/gtajamkmvf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nwbrower.top/gtccmbfjfg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hysaishi.cn/gtianugpag.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.fengsongda.top/gtczfkkebk.html

Go:   slices.Sort(arr)
来源：http://hz.pengpengdd.cyou/gtjszncvgg.html

Ruby: arr.sort
来源：http://hz.svipenyu.cn/gtjofdzpyk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.meibo888.top/gtriarceky.html

[N03] 快速排序（分治示例）
来源：http://hz.daxiang520.top/gtjiwcyedz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.daxiang520.top/gtygvsuttn.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yonumen.top/gtwxttsfyw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhiwuduotai.top/gtvrokoaza.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.sysykeji.top/gtclacxeql.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.ywan-chungtsiang.top/gtwqkmvirq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.316326.xyz/gtbtmiliar.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.gaohongyu789.top/gtptfqhilr.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jinqigfzy.top/gtvuhstihh.html

[N04] 斐波那契数列
来源：http://hz.aizwys.cn/gtvajyxtyz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.guannengcc.top/gtpududine.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.meibo888.top/gtstqgvidz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xziqi.cn/gtnmdrtldg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhixingplan.top/gtghfjwuxq.html


<!-- 参考信息 -->