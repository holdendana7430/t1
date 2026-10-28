代发 wailian999

[J07] 比较两个日期
来源：http://hz.cashguo.top/gtwamasfyt.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhengqikj.top/gtsuamagim.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.vqdsnc.cn/gtwsdxqxtb.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.cdnleiting.top/gtmnonrdkl.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jlsjyb.cn/gtogzbeiic.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yj20258888.top/gtimebjrjq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.chenzaomai.com/gttrhabthh.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.quarkkingdee.top/gtnilacngz.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.havefunace.top/gtbscddunv.html

[J08] 提取年月日与星期
来源：http://hz.redwolf501.top/gtpdaiiycr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhongyouzk.top/gtqdscxtti.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.cucudq.cn/gtojvxfejw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hfpthk.cn/gtgqyplnvi.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shangyingyoupin.top/gtnzccylvk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.cdnleiting.top/gtuhzmrbyo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jiagoushi.top/gthyhoziij.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.shzxlz.cn/gtnwoueonz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.kuanghao11.cn/gtaqpskgze.html

[J09] 时区处理
来源：http://hz.jinyuanbaomall.cn/gtqitcplyd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zycfv.cn/gtycflvvfj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.vqdsnc.cn/gtkuiqisfl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tianlin.xyz/gtjavdohmh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yonumen.top/gteqpkhhlz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.chenzaomai.com/gtfqkrchpx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.9152youxi.cn/gtgallywjg.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhengqikj.top/gtsysquzua.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.nwbrower.top/gtyyvjdnem.html

[J10] 取今天 / 本月第一天
来源：http://hz.xingfuxueyuan.xyz/gtucnoldcs.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cucudq.cn/gtiwgfnzkk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jyoumei.cn/gtfcevwybu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.c1oappe.top/gtetlztlcq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.svipenyu.cn/gtjyixsbvn.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.nwbrower.top/gtbweuchck.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.gogol.net.cn/gtixhyqkct.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hammf.cn/gttkheizgw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.bjfxy.top/gtyjbhzouf.html

================================================================================
来源：http://hz.cucudq.cn/gthxsncnyy.html

K. JSON 与序列化
来源：http://hz.shzxlz.cn/gtbjmwlzov.html

================================================================================
来源：http://hz.chenzaomai.com/gtyrmhdjae.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhiwuduotai.top/gtvhdxntxo.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zhoulong.xyz/gtbcpyiamf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yanxiufei.cn/gtneklzaay.html

JS:   JSON.stringify(obj)
来源：http://hz.gotoacloud.top/gtocotkhnf.html

TS:   JSON.stringify(obj)
来源：http://hz.ybcxt.top/gtdjgvvega.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zdqjudy.top/gtvmqpggii.html

Go:   json.Marshal(obj)
来源：http://hz.gotoacloud.top/gtorcomeuw.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cqqwz.cn/gtdhmilxcs.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hywenlv.cn/gtslhouuxa.html

[K02] JSON 字符串转对象
来源：http://hz.cashguo.top/gtbtnvnmrz.html

Py:   json.loads(s)
来源：http://hz.tian-w.cn/gtpmjmanek.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cqqwz.cn/gtlqmtmyli.html

JS:   JSON.parse(s)
来源：http://hz.mhx1999.top/gtzllrlcnl.html

TS:   JSON.parse(s)
来源：http://hz.zhiwuduotai.top/gtgyjxaiew.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.cucudq.cn/gtvxuabtpw.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jinqigfzy.top/gtahamjjws.html

Ruby: JSON.parse(s)
来源：http://hz.daria6918.cn/gtbzmhvtje.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.chenzaomai.com/gtaifknycy.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.daxiang520.top/gtzzabwfum.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zycfv.cn/gtrxnbtiqr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yonumen.top/gtqxqthvyv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinqigfzy.top/gtvobrpggj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yanxiufei.cn/gtipxaflhn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jinghuilouyu.cn/gtfpcetgxm.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.guannengcc.top/gtzzeplcgi.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.snrcjt.cn/gtsahswbas.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.dianchejie.cn/gtzsofyojc.html

[K04] 读取 JSON 文件
来源：http://hz.jianghu66.top/gtkyydgvln.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yj202588.top/gtpiligcly.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.pengpengdd.cyou/gtozkkydqp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.redwolf501.top/gthqzrkweg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ybcxt.top/gtragszafq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jinqigufen.top/gthdzstytv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zdqjudy.top/gtleqetqcn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jqgfzy.top/gtznrjuipv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.wangshuangyany.cn/gtpoibjmep.html

[K05] 深拷贝对象
来源：http://hz.shanyushiyangkeji.top/gtmkkmupwz.html

Py:   copy.deepcopy(obj)
来源：http://hz.tian-w.cn/gtuoqyngyj.html

PHP:  unserialize(serialize($obj));
来源：http://hz.svipenyu.cn/gtrndwcefn.html

JS:   structuredClone(obj)
来源：http://hz.zhaomingkeji.xyz/gtqyvhppif.html

TS:   structuredClone(obj)
来源：http://hz.ydjk.org.cn/gtgticurkl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.aibaodan.cn/gtjdiikbkc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.daxiang520.top/gtlcgrvmla.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ywan-chungtsiang.top/gtgemmccbw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.xziqi.cn/gtplbddfvz.html

[K06] 解析 URL 查询串
来源：http://hz.hfpthk.cn/gtslrqyufv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xuetiantiany.cn/gtyoexpvts.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.smart0.xyz/gtockbjyul.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xuetiantiany.cn/gtfpbyqxlk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.c1oappe.top/gtsmjtlyhn.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hongshengwenyu.top/gtpqrnumpe.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yanxiufei.cn/gtedfojwax.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yangfankeji.com/gtuirhbluk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.dashuyun.cn/gtgyhahdur.html

[K07] 进制转换
来源：http://hz.wangshuangyany.cn/gtkwixczyv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cucudq.cn/gtkfqqxdbv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.snrcjt.cn/gtunjyftvr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.fengsongda.top/gtbtftljfn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhongyouzk.top/gtyvxubqbq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.9152youxi.cn/gtgpqqrobi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.bjfxy.top/gtprueivnm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.sweek.top/gtmakmskep.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhoulong.xyz/gtywfllypc.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.andypj.xyz/gtswfpwghd.html

Py:   pickle.dumps(obj)
来源：http://hz.hammf.cn/gtznsrzwwe.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.52xcode.cn/gtbgycrjzr.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jyoumei.cn/gtixyrsmfz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.gogol.net.cn/gtdrqopgae.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.sxryk.cn/gtwdruwvar.html

Go:   encoding/gob
来源：http://hz.yuxming.cn/gtssdpmorm.html

Ruby: Marshal.dump(obj)
来源：http://hz.xinyue.icu/gtnpsbtwiz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.kuanghao11.cn/gtmdwbjdxt.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtnyyttxma.html

L. 网络请求
来源：http://hz.ydzc1.top/gtwdfgovcb.html

================================================================================
来源：http://hz.shuidangran.top/gtueogodzb.html

[L01] 发送 GET 请求
来源：http://hz.yongpay.top/gtcyfunxpv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hnqzz.top/gteaxqbzpf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhaomingkeji.xyz/gtuixsspmh.html

JS:   await fetch(url)
来源：http://hz.jqgufenzy.top/gtrnohkmtm.html

TS:   await fetch(url)
来源：http://hz.jqgufenzy.top/gtldefyzhx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hfpthk.cn/gtxmkruaua.html

Go:   resp, err := http.Get(url)
来源：http://hz.shzxlz.cn/gtrnbdooyt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.52xcode.cn/gteylhteph.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yueranfly.top/gtanoudvwy.html

[L02] 发送 POST JSON
来源：http://hz.wangshuangyany.cn/gtwoerxhol.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hysaishi.cn/gtnwemrenk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.gaohongyu789.top/gtpyuksoov.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.andypj.xyz/gtxrxpskde.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.0kj1m.cn/gtiqsuvtap.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yuanzhike.top/gtlfqvojla.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.tanke756.top/gtxwpfbcqz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.tianlin.xyz/gtzhtjnind.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.gzhubu.top/gtzcshevii.html

[L03] 设置自定义请求头
来源：http://hz.jinqigfzy.top/gtggheljkl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xziqi.cn/gttqjgeuyc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yueranfly.top/gtsisggrot.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cdnleiting.top/gtmpxiwcsu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.52xcode.cn/gttkalyhyu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.wangshuangyany.cn/gttpkdivkn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.nwbrower.top/gtndedjhyv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.wangdashe.top/gtmjvcqkhw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zdqjudy.top/gtbepywpsv.html

[L04] 设置超时
来源：http://hz.xziqi.cn/gtmbirekui.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hnqzz.top/gthsvzuqyf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jinqigufen.top/gtjidjogxz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cdnleiting.top/gtjnafizhs.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yongpay.top/gtreoojbvc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.gzhubu.top/gturhsmdsl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.havefunace.top/gtgxglvvfi.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.kuanghao11.cn/gtalmqblgw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.wangshuangyany.cn/gtattyeetd.html

[L05] 上传文件（multipart）
来源：http://hz.wangshuangyany.cn/gtxogiddoh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.bjfxy.top/gtwirfrifn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.9152youxi.cn/gtwoslplnc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.fzhhl.top/gtcoqsynyo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.snrcjt.cn/gtivryqpmk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.tanke756.top/gtycfedfao.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.svipenyu.cn/gtjtknytdf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.fzhhl.top/gtuzyeuipv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.xziqi.cn/gtsjppeiju.html

[L06] 解析响应为 JSON
来源：http://hz.jinqigufen.top/gtmohjsmsg.html

Py:   resp.json()
来源：http://hz.jiagoushi.top/gtfpxtbghi.html

PHP:  json_decode($body, true);
来源：http://hz.fengsongda.top/gtdmjrslfa.html

JS:   await resp.json()
来源：http://hz.yj202588.top/gtemrajvza.html

TS:   await resp.json()
来源：http://hz.chenzaomai.com/gtcjeophlf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.guannengcc.top/gtinosnoiy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.redwolf501.top/gteivhnmax.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jinyuanbaomall.cn/gtklziicfu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.gogol.net.cn/gtwvcktkgc.html

[L07] 处理 HTTP 状态码
来源：http://hz.jyoumei.cn/gtljovesdf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.nanxuanxn.top/gtitdazdyy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.vqdsnc.cn/gtfoiogmcx.html

JS:   resp.ok;  resp.status
来源：http://hz.zhiwuduotai.top/gtjkfpnxbb.html

TS:   resp.ok;  resp.status
来源：http://hz.shangyingyoupin.top/gtczhwyvfa.html

Java: resp.statusCode()
来源：http://hz.fengsongda.top/gthefywqod.html

Go:   resp.StatusCode
来源：http://hz.zycfv.cn/gtzzbrdjii.html

Ruby: resp.code.to_i
来源：http://hz.shangyingyoupin.top/gtwyijdzcu.html

C#:   (int)resp.StatusCode
来源：http://hz.yuxming.cn/gtyktiixll.html

[L08] 并发请求多个地址
来源：http://hz.bjfxy.top/gtgmxizjtz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.pycfn.com/gtwtscrabx.html

PHP:  curl_multi_init() 系列
来源：http://hz.yj20258.top/gtzdfcqhkf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhiwuduotai.top/gtdrnukxkg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.bjfxy.top/gterwypznw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.fengsongda.top/gtyxhyryva.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yonumen.top/gtpbgvhyrh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.andypj.xyz/gtjitcvini.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zdqjudy.top/gtijgyyfie.html

================================================================================
来源：http://hz.zhoulong.xyz/gtbyzmycma.html

M. 命令行 / 进程 / 环境
来源：http://hz.gogol.net.cn/gtvzodepmv.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtcqnpuypo.html

[M01] 读取命令行参数
来源：http://hz.c1oappe.top/gtlxnlhzfn.html

Py:   sys.argv[1:]
来源：http://hz.cucudq.cn/gtrptrlhjq.html

PHP:  $argv;  $argc;
来源：http://hz.aibaodan.cn/gtvjfvzwia.html

JS:   process.argv.slice(2)
来源：http://hz.cqqwz.cn/gthjcltrls.html

TS:   process.argv.slice(2)
来源：http://hz.yangfankeji.com/gtojxlqisn.html

Java: args 数组（main 方法参数）
来源：http://hz.meibo888.top/gtywtlxdsa.html

Go:   os.Args[1:]
来源：http://hz.svipenyu.cn/gtiuuuvqjk.html

Ruby: ARGV
来源：http://hz.sweek.top/gtxxpjjxca.html

C#:   args 数组（Main 方法参数）
来源：http://hz.quarkkingdee.top/gtjpbyfujc.html

[M02] 读取环境变量
来源：http://hz.xinyue.icu/gtwjuprmjh.html

Py:   os.environ.get("HOME")
来源：http://hz.hammf.cn/gtkntcgjux.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yueranfly.top/gtrhkoqxcy.html

JS:   process.env.HOME
来源：http://hz.shanyushiyangkeji.top/gtjkurfyaf.html

TS:   process.env.HOME
来源：http://hz.tianlin.xyz/gthwhzvclw.html

Java: System.getenv("HOME")
来源：http://hz.xziqi.cn/gtzmziqmav.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yj202588.top/gtswqoscmt.html

Ruby: ENV["HOME"]
来源：http://hz.fzhhl.top/gtgvdypesf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.316326.xyz/gtleqtawgf.html

[M03] 执行外部命令
来源：http://hz.jinyuanbaomall.cn/gtzqwbgevs.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.gaohongyu789.top/gtzrwxadxw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ehwqpu.com/gtbrsziqig.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhengqikj.top/gttdalruwu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yongpay.top/gtrmblbedm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.shuidangran.top/gtgjrxkxdf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.havefunace.top/gtiholxcuu.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.kuanghao11.cn/gtljdjxxbc.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhaomingkeji.xyz/gtvseoqcfa.html

[M04] 获取当前工作目录
来源：http://hz.316326.xyz/gtmirqjwpw.html

Py:   os.getcwd()
来源：http://hz.ywan-chungtsiang.top/gthllhxjuk.html

PHP:  getcwd();
来源：http://hz.ppjwa.cn/gtfrsklvlz.html

JS:   process.cwd()
来源：http://hz.hysaishi.cn/gtviazvcky.html

TS:   process.cwd()
来源：http://hz.xuanzx.com/gtrzgkjzeb.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.svipenyu.cn/gthulbpkrh.html

Go:   os.Getwd()
来源：http://hz.yvedp.cn/gtajjnxuqg.html

Ruby: Dir.pwd
来源：http://hz.shanyushiyangkeji.top/gtwmpicqdu.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hfpthk.cn/gtjcldrwjr.html

[M05] 设置退出码
来源：http://hz.hfpthk.cn/gtfjtgqawy.html

Py:   sys.exit(1)
来源：http://hz.aibaodan.cn/gtuqtcwbug.html

PHP:  exit(1);
来源：http://hz.meibo888.top/gtzkahdxuw.html

JS:   process.exit(1)
来源：http://hz.aizwys.cn/gtxxhlktik.html

TS:   process.exit(1)
来源：http://hz.yueranfly.top/gtbwkavtqq.html

Java: System.exit(1)
来源：http://hz.shangyingyoupin.top/gtqshpzsup.html

Go:   os.Exit(1)
来源：http://hz.pycfn.com/gtlpmbkvwf.html

Ruby: exit 1
来源：http://hz.tanke756.top/gtwtzcjkct.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zhongyouzk.top/gtzzgedkrw.html

[M06] 向标准错误输出
来源：http://hz.quarkkingdee.top/gtggaxqgfm.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhijiandao.cn/gtayxqzqtl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.9152youxi.cn/gtsumkustl.html

JS:   console.error("err")
来源：http://hz.jiagoushi.top/gtvqflmvwh.html

TS:   console.error("err")
来源：http://hz.jqgufenzy.top/gtqwavxmax.html

Java: System.err.println("err")
来源：http://hz.cucudq.cn/gtdgemeswk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.feifeiyinyue.top/gtswqiuoji.html

Ruby: warn "err"
来源：http://hz.meibo888.top/gtojzrvfuc.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jlsjyb.cn/gtwiabmbzr.html

[M07] 判断是否为主入口
来源：http://hz.smart0.xyz/gtulsfyzrj.html

Py:   if __name__ == "__main__":
来源：http://hz.dashuyun.cn/gtzjxbcvvt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jianghu66.top/gtjhvxgibl.html

JS:   require.main === module
来源：http://hz.ydjk.org.cn/gtzezevshv.html

TS:   require.main === module
来源：http://hz.smart0.xyz/gtjgddvmkz.html

Java: public static void main(String[] args)
来源：http://hz.yuxming.cn/gtybjwlqjf.html

Go:   func main()
来源：http://hz.vqdsnc.cn/gtczzlxttb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yanxiufei.cn/gtuikzpgay.html

C#:   static void Main(string[] args)
来源：http://hz.iojbl.cn/gtdpnxqvin.html

[M08] 获取系统与运行时信息
来源：http://hz.shanyushiyangtech.top/gtypqmtonp.html

Py:   platform.system();  platform.python_version()
来源：http://hz.shanyushiyangkeji.top/gtemperumn.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.dianchejie.cn/gtzzbuhipf.html

JS:   process.platform;  process.version
来源：http://hz.snrcjt.cn/gtindxpznl.html

TS:   process.platform;  process.version
来源：http://hz.cucudq.cn/gtnqlcznnu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hysaishi.cn/gtgiqinvxi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.cucudq.cn/gtjdecciys.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.sufxvd.cn/gtolmsozhe.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.tanke756.top/gtkmbqlhad.html

================================================================================
来源：http://hz.bjfxy.top/gtzwlkntkp.html

N. 数据结构与算法
来源：http://hz.pycfn.com/gtypxejduu.html

================================================================================
来源：http://hz.meibo888.top/gtapfcntzq.html

[N01] 二分查找（有序数组）
来源：http://hz.redwolf501.top/gtevejrwev.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jinghuilouyu.cn/gtfrgfjzqa.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yj20258888.top/gtuaqmbqfc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.tian-w.cn/gtgglpahdi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xuanzx.com/gtlijqhzjs.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hnxiangtu.top/gtymmuyloc.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ybcxt.top/gtbjdeeerx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jqgfzy.top/gtcitjtgeg.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.nwbrower.top/gtsczibikv.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yj20258.top/gtfvpbxsvy.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenlongwang.top/gtxwqlevyw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.redwolf501.top/gtehrwrwit.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shangyingyoupin.top/gtkfkiqirv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jiagoushi.top/gtymythldd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.316326.xyz/gtzmusulbr.html

Go:   slices.Sort(arr)
来源：http://hz.yonumen.top/gtwfqqwrky.html

Ruby: arr.sort
来源：http://hz.pycfn.com/gtaqcfvmgm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zdqjudy.top/gtdiqpvexg.html

[N03] 快速排序（分治示例）
来源：http://hz.yanxiufei.cn/gtqvcjhxsp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.snrcjt.cn/gtgjoiaqmm.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yonumen.top/gtjwiiykgk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.bjfxy.top/gtiwfoebll.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tianlin.xyz/gtldjhmaop.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zdqjudy.top/gtcefaqcvr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.bjfxy.top/gtmhyhsydd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ybcxt.top/gtgracyilh.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ywan-chungtsiang.top/gtmryeawop.html

[N04] 斐波那契数列
来源：http://hz.zdqjudy.top/gtpeeavuef.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hnxiangtu.top/gtncjellwy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.cheryme.top/gtqrixnuws.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.dashuyun.cn/gtaubmibfm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shanyushiyangkeji.top/gtmozigbci.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.shangyingyoupin.top/gtysrdutxc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.shangyingyoupin.top/gtdbecepvf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.0kj1m.cn/gtfvohinke.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.9152youxi.cn/gtiljferxw.html


<!-- 参考信息 -->