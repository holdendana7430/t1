代发 wailian999

[J07] 比较两个日期
来源：http://hz.ydzc1.top/gtuabvihud.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhengqikj.top/gtlhpamxsm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.pycfn.com/gtdogqexta.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.9152youxi.cn/gtxtwrluvd.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hongshengwenyu.top/gtzrkbnsen.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.gotoacloud.top/gtstftsmju.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhoulong.xyz/gtjalklaxv.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.wangdashe.top/gtzlcyqkgq.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jinqigufen.top/gtknifhzxq.html

[J08] 提取年月日与星期
来源：http://hz.shanyushiyangtech.top/gtlvqsjrwb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.xuetiantiany.cn/gtyhbnpiik.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jinqigufen.top/gtjfnromxz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hammf.cn/gtvuwbaskd.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yueranfly.top/gtgzhntcek.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.chenzaomai.com/gtooddcfju.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hnxiangtu.top/gtdmnfaazd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.gaohongyu789.top/gtmjetmxqr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.dianchejie.cn/gtggkpojrm.html

[J09] 时区处理
来源：http://hz.hysaishi.cn/gtbdavdeqw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.mhx1999.top/gtlonrfkmg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.andypj.xyz/gtumqknutl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.svipenyu.cn/gtmxoykmtt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj20258888.top/gtfczxkjii.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.cucudq.cn/gtgxcmmwhf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.guannengcc.top/gtdxsxnbve.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhongyouzk.top/gtysarhwxo.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shuidangran.top/gtmplnbbkl.html

[J10] 取今天 / 本月第一天
来源：http://hz.hysaishi.cn/gtmvaiolul.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ybcxt.top/gtxcwyfhja.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.dianchejie.cn/gtihwvqhrq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xingfuxueyuan.xyz/gtaycgtsju.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jlsjyb.cn/gtqdmjedaq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.pengpengdd.cyou/gtcjzffgne.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ehwqpu.com/gtamuvilrq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.316326.xyz/gtahqtjond.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.hfpthk.cn/gttpgyabia.html

================================================================================
来源：http://hz.pycfn.com/gtzsrushdz.html

K. JSON 与序列化
来源：http://hz.wangdashe.top/gtdxvebwrd.html

================================================================================
来源：http://hz.hnqzz.top/gtuawjkccl.html

[K01] 对象转 JSON 字符串
来源：http://hz.yonumen.top/gtkfzuvvjl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shanyushiyangkeji.top/gtiranxixs.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hysaishi.cn/gtbkegfwfg.html

JS:   JSON.stringify(obj)
来源：http://hz.aizwys.cn/gtmzpmmcpu.html

TS:   JSON.stringify(obj)
来源：http://hz.andypj.xyz/gtirxmmcsd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.quarkkingdee.top/gtsbbubhvv.html

Go:   json.Marshal(obj)
来源：http://hz.yongpay.top/gtoqdhenfz.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yongpay.top/gtkegyvkfj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jianghu66.top/gtjwkbgkeu.html

[K02] JSON 字符串转对象
来源：http://hz.9152youxi.cn/gtdvdiyifq.html

Py:   json.loads(s)
来源：http://hz.quarkkingdee.top/gthkotplnt.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jinqigfzy.top/gtzbagrfrz.html

JS:   JSON.parse(s)
来源：http://hz.shuidangran.top/gtennqbtxe.html

TS:   JSON.parse(s)
来源：http://hz.hywenlv.cn/gtwdizxyez.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jinghuilouyu.cn/gtbrfyjxhi.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.gotoacloud.top/gtxxbhmkjm.html

Ruby: JSON.parse(s)
来源：http://hz.dashuyun.cn/gthktctvai.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ppjwa.cn/gtymvrmumm.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jiagoushi.top/gtawizafwr.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhoulong.xyz/gtvluycqmy.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.dianchejie.cn/gthftnahkf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xinyue.icu/gtwetyvfed.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.quarkkingdee.top/gtycljlcwu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ybcxt.top/gtozwsvexv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ydzc1.top/gtzdsisxds.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.smart0.xyz/gtxcrbjrtb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yuanzhike.top/gtojbkdnmi.html

[K04] 读取 JSON 文件
来源：http://hz.jinqigfzy.top/gtgkshwjke.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xuetiantiany.cn/gthbnotysh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.snrcjt.cn/gtnhpehalr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hywenlv.cn/gtndhbluyl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xziqi.cn/gtxrcstrek.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.shuidangran.top/gtfgvcxjgg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.shangyingyoupin.top/gtirbwcehf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.vqdsnc.cn/gtazfvgtug.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hfpthk.cn/gtqfftfmrz.html

[K05] 深拷贝对象
来源：http://hz.shzxlz.cn/gtychptabz.html

Py:   copy.deepcopy(obj)
来源：http://hz.gaohongyu789.top/gtlwzrugbo.html

PHP:  unserialize(serialize($obj));
来源：http://hz.tian-w.cn/gtxnnhflxl.html

JS:   structuredClone(obj)
来源：http://hz.sufxvd.cn/gttnqxiwzf.html

TS:   structuredClone(obj)
来源：http://hz.jinqigfzy.top/gthwdfeagj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jlsjyb.cn/gtmnhtxiac.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jinghuilouyu.cn/gtkdalnbmo.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shangyingyoupin.top/gtzuptmxww.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jinghuilouyu.cn/gtbkavcizj.html

[K06] 解析 URL 查询串
来源：http://hz.cheryme.top/gtyovqttkx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ppjwa.cn/gtjltduyka.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.shangyingyoupin.top/gtxsoapahc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.bjfxy.top/gtowqtxqnv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sxryk.cn/gtjrkxbnec.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yonumen.top/gtscskdhaq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.nwbrower.top/gttuzuytvs.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ydzc1.top/gtshzbjaho.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.tian-w.cn/gtlzsvtegc.html

[K07] 进制转换
来源：http://hz.yueranfly.top/gtgifdstke.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yonumen.top/gtzhucuhmh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jinqigfzy.top/gteejhxgwt.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hfpthk.cn/gtyhkykaqa.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.mhx1999.top/gtzkhufowq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cheryme.top/gteybfujzt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.mhx1999.top/gteasszpch.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ppjwa.cn/gtempxrqkh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.cqqwz.cn/gtetrczgfx.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhaomingkeji.xyz/gtsgrerkjz.html

Py:   pickle.dumps(obj)
来源：http://hz.yuanzhike.top/gtiyxneyoo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.smart0.xyz/gtodsqqfah.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ydjk.org.cn/gtgbzpuxvm.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.shanyushiyangkeji.top/gtokkepcug.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yj20258.top/gtkiavgmpo.html

Go:   encoding/gob
来源：http://hz.aizwys.cn/gtdsjznoil.html

Ruby: Marshal.dump(obj)
来源：http://hz.cashguo.top/gtwydabjhk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shanyushiyangtech.top/gtvivqeduh.html

================================================================================
来源：http://hz.zhijiandao.cn/gtchyjlaeu.html

L. 网络请求
来源：http://hz.hnqzz.top/gtxzvcenfy.html

================================================================================
来源：http://hz.jyoumei.cn/gtegmecmla.html

[L01] 发送 GET 请求
来源：http://hz.yangfankeji.com/gtbmmeskji.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.daria6918.cn/gtwzojsfpa.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.xuanzx.com/gtyijltvyo.html

JS:   await fetch(url)
来源：http://hz.xylfe.cn/gtxqwlseun.html

TS:   await fetch(url)
来源：http://hz.jqgufenzy.top/gtsphreprn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zdqjudy.top/gtovtsygfl.html

Go:   resp, err := http.Get(url)
来源：http://hz.yj202588.top/gtxehkignw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jqgfzy.top/gtfobftide.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.gogol.net.cn/gtwcmlklsv.html

[L02] 发送 POST JSON
来源：http://hz.9152youxi.cn/gtirmnwfxx.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.chenzaomai.com/gtskfavpxj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.bjfxy.top/gtvswcpsab.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shuidangran.top/gthwrczhxf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cashguo.top/gtvubbichr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jqgfzy.top/gtiacphpsm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.gogol.net.cn/gtkjhxbncd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.dashuyun.cn/gttqcghopk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jqgufenzy.top/gtwxhonivy.html

[L03] 设置自定义请求头
来源：http://hz.jlsjyb.cn/gteysjnmny.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.cheryme.top/gtephiewwk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hammf.cn/gttqzzwqvd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.snrcjt.cn/gtiecwsoxp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yuxming.cn/gttyajetws.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.snrcjt.cn/gtuncvmjct.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yongpay.top/gtjehjcwvn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.sxryk.cn/gttlyuwgab.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhijiandao.cn/gtyzirrqst.html

[L04] 设置超时
来源：http://hz.zycfv.cn/gtkrgkozyo.html

Py:   requests.get(url, timeout=5)
来源：http://hz.316326.xyz/gthidigraw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.chenzaomai.com/gtkwvwuhpe.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ybcxt.top/gtycgzcfxi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.redwolf501.top/gtijnldagn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.chenzaomai.com/gtakicuxgk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ydjk.org.cn/gtdxgsseec.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.feifeiyinyue.top/gtdjtinluq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.cucudq.cn/gtdlbhqnyb.html

[L05] 上传文件（multipart）
来源：http://hz.sysykeji.top/gtqcozihjl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhijiandao.cn/gtjwsghano.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.pengpengdd.cyou/gtmlrljaah.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.pycfn.com/gtaajajwhh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.smart0.xyz/gthxaoxmpz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jqgufenzy.top/gtqmttgwwl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.havefunace.top/gtkrlcnlmh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.pengpengdd.cyou/gtotkgotal.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jqgufenzy.top/gtcwnzingh.html

[L06] 解析响应为 JSON
来源：http://hz.vqdsnc.cn/gtxaxxdmyb.html

Py:   resp.json()
来源：http://hz.jqgufenzy.top/gteuojgmcl.html

PHP:  json_decode($body, true);
来源：http://hz.jiagoushi.top/gtryodzutv.html

JS:   await resp.json()
来源：http://hz.zhongyouzk.top/gtgzbwuxal.html

TS:   await resp.json()
来源：http://hz.iojbl.cn/gtaqankfcj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhixingplan.top/gthzgujlmt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jlsjyb.cn/gthjjojelj.html

Ruby: JSON.parse(resp.body)
来源：http://hz.quarkkingdee.top/gtbnoavufd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ydzc1.top/gtsqlhevdp.html

[L07] 处理 HTTP 状态码
来源：http://hz.yueranfly.top/gtcnpxviuy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jqgfzy.top/gtsieoyduu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.meibo888.top/gtbqhilwla.html

JS:   resp.ok;  resp.status
来源：http://hz.gzhubu.top/gteuaowaql.html

TS:   resp.ok;  resp.status
来源：http://hz.nwbrower.top/gtdmtapest.html

Java: resp.statusCode()
来源：http://hz.ppjwa.cn/gtglmcawdc.html

Go:   resp.StatusCode
来源：http://hz.jqgfzy.top/gtjcgtndrq.html

Ruby: resp.code.to_i
来源：http://hz.jinghuilouyu.cn/gtkdioorjk.html

C#:   (int)resp.StatusCode
来源：http://hz.yuanzhike.top/gtxkoilsim.html

[L08] 并发请求多个地址
来源：http://hz.tianlin.xyz/gtutnqgkpd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ybcxt.top/gtuyfxdeze.html

PHP:  curl_multi_init() 系列
来源：http://hz.hfpthk.cn/gttpqcubtp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yj20258.top/gtohqstsel.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hfpthk.cn/gtcvmxemqv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yj202588.top/gtozzixomi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.daria6918.cn/gtgrfrnhnb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jiagoushi.top/gtlzquupsi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.svipenyu.cn/gtszmditqo.html

================================================================================
来源：http://hz.tian-w.cn/gtzajteqol.html

M. 命令行 / 进程 / 环境
来源：http://hz.ybcxt.top/gtdqpembev.html

================================================================================
来源：http://hz.yonumen.top/gtkbbvooae.html

[M01] 读取命令行参数
来源：http://hz.yanxiufei.cn/gtyhszbdaz.html

Py:   sys.argv[1:]
来源：http://hz.xuetiantiany.cn/gtigsguouf.html

PHP:  $argv;  $argc;
来源：http://hz.yuxming.cn/gtwszhsigg.html

JS:   process.argv.slice(2)
来源：http://hz.shanyushiyangkeji.top/gtfrdulfbj.html

TS:   process.argv.slice(2)
来源：http://hz.yuxming.cn/gtcxsugcgz.html

Java: args 数组（main 方法参数）
来源：http://hz.fengsongda.top/gtgqdjfanp.html

Go:   os.Args[1:]
来源：http://hz.ehwqpu.com/gtalehlrel.html

Ruby: ARGV
来源：http://hz.birdmap.top/gtxscmlnex.html

C#:   args 数组（Main 方法参数）
来源：http://hz.iojbl.cn/gtbgdftbnz.html

[M02] 读取环境变量
来源：http://hz.zhixingplan.top/gtjwcnksnp.html

Py:   os.environ.get("HOME")
来源：http://hz.xylfe.cn/gtowyjjgqi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yj20258888.top/gtmtirxgso.html

JS:   process.env.HOME
来源：http://hz.zhaomingkeji.xyz/gtjyrmtnpd.html

TS:   process.env.HOME
来源：http://hz.zhoulong.xyz/gtocpbxdwc.html

Java: System.getenv("HOME")
来源：http://hz.cqqwz.cn/gtaafxxglo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.c1oappe.top/gtoubwjloy.html

Ruby: ENV["HOME"]
来源：http://hz.vqdsnc.cn/gthcyktehv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.dianchejie.cn/gtowrbiqil.html

[M03] 执行外部命令
来源：http://hz.c1oappe.top/gtakhpqewj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.andypj.xyz/gtxfbgbrdk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hfpthk.cn/gtxbfmesyr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.mhx1999.top/gtlgpifjsc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hysaishi.cn/gtjqghlwrw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.tanke756.top/gtlepvsgmt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.svipenyu.cn/gtvzlxqaqc.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shuidangran.top/gtspgfxnyb.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yj202588.top/gtngzpbyvp.html

[M04] 获取当前工作目录
来源：http://hz.jinqigfzy.top/gtaquffubq.html

Py:   os.getcwd()
来源：http://hz.jlsjyb.cn/gtqsmulrvx.html

PHP:  getcwd();
来源：http://hz.shanyushiyangkeji.top/gtbilgyscm.html

JS:   process.cwd()
来源：http://hz.jinqigfzy.top/gtilwekjnj.html

TS:   process.cwd()
来源：http://hz.ydjk.org.cn/gtyxdgwpzo.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.fzhhl.top/gtwyakgnbt.html

Go:   os.Getwd()
来源：http://hz.yj20258.top/gtehnzesdt.html

Ruby: Dir.pwd
来源：http://hz.shangyingyoupin.top/gtqsltyoke.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.wangshuangyany.cn/gttvcjljfm.html

[M05] 设置退出码
来源：http://hz.smart0.xyz/gttteshcoq.html

Py:   sys.exit(1)
来源：http://hz.xylfe.cn/gtwldcvrru.html

PHP:  exit(1);
来源：http://hz.hongshengwenyu.top/gtyhfmxkxg.html

JS:   process.exit(1)
来源：http://hz.gogol.net.cn/gtfrtsuprw.html

TS:   process.exit(1)
来源：http://hz.mhx1999.top/gttpltngce.html

Java: System.exit(1)
来源：http://hz.yongpay.top/gtaluppcru.html

Go:   os.Exit(1)
来源：http://hz.0kj1m.cn/gtncnqoqmw.html

Ruby: exit 1
来源：http://hz.yj202588.top/gtiyylbrvw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.chenjidiqi.icu/gtdenncwxv.html

[M06] 向标准错误输出
来源：http://hz.xylfe.cn/gtyrbuldcx.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yuxming.cn/gteanqjuqx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ywan-chungtsiang.top/gtktjzxlkl.html

JS:   console.error("err")
来源：http://hz.guowangkeji.top/gtwcvgunjv.html

TS:   console.error("err")
来源：http://hz.yuxming.cn/gtsmfqupyr.html

Java: System.err.println("err")
来源：http://hz.xylfe.cn/gtwslaqpnh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ybcxt.top/gtmvtpbrcf.html

Ruby: warn "err"
来源：http://hz.jinyuanbaomall.cn/gtsslutcaq.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.xuetiantiany.cn/gtibdmtovu.html

[M07] 判断是否为主入口
来源：http://hz.ybcxt.top/gtgqfadttu.html

Py:   if __name__ == "__main__":
来源：http://hz.cheryme.top/gtnwntkmur.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.dashuyun.cn/gtstblekvd.html

JS:   require.main === module
来源：http://hz.nanxinkj.top/gtauomrcsu.html

TS:   require.main === module
来源：http://hz.xinyue.icu/gtjcnpfvfe.html

Java: public static void main(String[] args)
来源：http://hz.wangdashe.top/gtfvmzaczs.html

Go:   func main()
来源：http://hz.jqgufenzy.top/gtsbipphkt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.quarkkingdee.top/gtnfeuybxq.html

C#:   static void Main(string[] args)
来源：http://hz.dianchejie.cn/gtgbpeuxdv.html

[M08] 获取系统与运行时信息
来源：http://hz.cheryme.top/gtefvixjsq.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hywenlv.cn/gtosxsjayj.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.wangshuangyany.cn/gtknohcjxa.html

JS:   process.platform;  process.version
来源：http://hz.jqgfzy.top/gtwkuudbes.html

TS:   process.platform;  process.version
来源：http://hz.tianlin.xyz/gtqutmakgt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yj202588.top/gtgdubrerp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.sufxvd.cn/gtidyzmujg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.sufxvd.cn/gtadwydcnq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ywan-chungtsiang.top/gttgsdzhxp.html

================================================================================
来源：http://hz.guannengcc.top/gtxmqyzful.html

N. 数据结构与算法
来源：http://hz.9152youxi.cn/gtzbtzjcfu.html

================================================================================
来源：http://hz.ppjwa.cn/gtxvcgefay.html

[N01] 二分查找（有序数组）
来源：http://hz.jinyuanbaomall.cn/gtwrrxcrxj.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.shanyushiyangtech.top/gtuqnqhjyk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.sysykeji.top/gtbqrgfnpq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ywan-chungtsiang.top/gtdsttywki.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.dianchejie.cn/gtdnfxxrmr.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hnqzz.top/gtcmbchzdr.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jinqigfzy.top/gtianwjyys.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.sysykeji.top/gtmlujzmsz.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.cashguo.top/gttgknhowi.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ydjk.org.cn/gtkdskaucw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shanyushiyangtech.top/gtjjwibtkw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.316326.xyz/gttxrxhsbq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhongyouzk.top/gtkvsgzveb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhongyouzk.top/gtomewzgxl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jiagoushi.top/gtletiqobk.html

Go:   slices.Sort(arr)
来源：http://hz.ivvv.top/gtftcaxctm.html

Ruby: arr.sort
来源：http://hz.zhoulong.xyz/gtbttvhjpw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yj202588.top/gtxgdtdchk.html

[N03] 快速排序（分治示例）
来源：http://hz.daria6918.cn/gtgdvqhkkr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.vqdsnc.cn/gtsqmwaupw.html

PHP:  // 递归实现，或用 usort
来源：http://hz.shanyushiyangkeji.top/gtahnahnhm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jiagoushi.top/gtciwbjzaj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tanke756.top/gtmmbbkogi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.fzhhl.top/gtupdpztdd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.9152youxi.cn/gthpcgtwwb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.feifeiyinyue.top/gtkqgadqmk.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.vqdsnc.cn/gtaadrzmzd.html

[N04] 斐波那契数列
来源：http://hz.smart0.xyz/gtiqtrxdge.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.nanxuanxn.top/gtmbutefjp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.fengsongda.top/gtdudvhuqk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhaomingkeji.xyz/gthbdajhsm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.chenlongwang.top/gtyikvlctj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jinqigufen.top/gtcsscbdse.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.xziqi.cn/gtvpbehmqu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.shanyushiyangkeji.top/gtaxpckfea.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jlsjyb.cn/gteegmuxrz.html


<!-- 参考信息 -->