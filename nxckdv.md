代发 wailian999

Py:   (end - start).total_seconds()
来源：http://hz.nanxinkj.top/gtjclxhpun.html

PHP:  $end->diff($start)->days;
来源：http://hz.yueranfly.top/gtsmhdhoew.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.52xcode.cn/gtzebojvps.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jinqigfzy.top/gtevxgvewd.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.0kj1m.cn/gtevctggfg.html

Go:   end.Sub(start).Hours()
来源：http://hz.shzxlz.cn/gtyolnupmz.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zdqjudy.top/gtlcnijxyn.html

C#:   (end - start).TotalSeconds
来源：http://hz.cashguo.top/gttdrdfysn.html

[J07] 比较两个日期
来源：http://hz.zhijiandao.cn/gtixfepgzu.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.gaohongyu789.top/gtajvtbcij.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jqgufenzy.top/gtzuitayet.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.guowangkeji.top/gtffkrqeka.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shuidangran.top/gtzxtvosbg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jiagoushi.top/gtaszawixj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jianghu66.top/gtggfqcqtp.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jianghu66.top/gtxsnzvnqi.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.kuanghao11.cn/gtzrnlnbfn.html

[J08] 提取年月日与星期
来源：http://hz.sxryk.cn/gtyjkhngpn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.xuetiantiany.cn/gtnkfzzdpv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.pycfn.com/gtdpjktoye.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.guannengcc.top/gtzmawgbjg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.cashguo.top/gtwszptlrb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.smart0.xyz/gtfqstlbqp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.316326.xyz/gtyepfroen.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.tian-w.cn/gtwromykwb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.havefunace.top/gtpuhrukij.html

[J09] 时区处理
来源：http://hz.ehwqpu.com/gtjfwcnphm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shanyushiyangkeji.top/gtbcvsryqg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.kuanghao11.cn/gtxhpuewam.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nanxuanxn.top/gtwgrzrlmc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhaomingkeji.xyz/gtewqkosua.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.feifeiyinyue.top/gtruekyplb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ybcxt.top/gtilwjbjbx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.nanxinkj.top/gtoeejxzjj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ivvv.top/gtuuyzvbvi.html

[J10] 取今天 / 本月第一天
来源：http://hz.ppjwa.cn/gtwwqppasl.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yj202588.top/gtpfxetnpw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yonumen.top/gtgzytjxmt.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.bjfxy.top/gtmtidnqos.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ppjwa.cn/gtyvfnqfpi.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jinqigufen.top/gtnvldvqpc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.chenlongwang.top/gtgfzbgmjf.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jinyuanbaomall.cn/gtsbgvvwop.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.daxiang520.top/gtppegtsih.html

================================================================================
来源：http://hz.yangfankeji.com/gtyoztnldw.html

K. JSON 与序列化
来源：http://hz.meibo888.top/gtgshlrdpb.html

================================================================================
来源：http://hz.hfpthk.cn/gtgsvkamqw.html

[K01] 对象转 JSON 字符串
来源：http://hz.chenlongwang.top/gtezawymnv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.xingfuxueyuan.xyz/gtdoabcuxx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jinghuilouyu.cn/gtmxoovjyn.html

JS:   JSON.stringify(obj)
来源：http://hz.quarkkingdee.top/gtlugswruj.html

TS:   JSON.stringify(obj)
来源：http://hz.tanke756.top/gtmwmetszp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.daxiang520.top/gthqbpcrln.html

Go:   json.Marshal(obj)
来源：http://hz.ivvv.top/gtsdgnjmvk.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.pycfn.com/gtbvbzvefd.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.tanke756.top/gtggnsmtpf.html

[K02] JSON 字符串转对象
来源：http://hz.hywenlv.cn/gtrkdnvbqa.html

Py:   json.loads(s)
来源：http://hz.zhaomingkeji.xyz/gtwszthrlv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.dashuyun.cn/gtxfwionik.html

JS:   JSON.parse(s)
来源：http://hz.jinqigufen.top/gtipxycxkw.html

TS:   JSON.parse(s)
来源：http://hz.jlsjyb.cn/gtuxvgdymh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.dashuyun.cn/gtcwqslijv.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.cashguo.top/gtuvbbifgr.html

Ruby: JSON.parse(s)
来源：http://hz.pycfn.com/gtiudmnljw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.cdnleiting.top/gtjbxpxvgz.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.dashuyun.cn/gtdjhxfxxp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hysaishi.cn/gtowcfiglj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.chenjidiqi.icu/gtzcsoxcgb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.guowangkeji.top/gtkbjaktow.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yangfankeji.com/gtfisanimc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.smart0.xyz/gtxlxmixni.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.haohaochexian.top/gtrebjdlke.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hysaishi.cn/gtjzxzmssj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.9152youxi.cn/gtrgjzwmqq.html

[K04] 读取 JSON 文件
来源：http://hz.jqgufenzy.top/gtiwrnnzhm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.aizwys.cn/gtpkcrrurk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cashguo.top/gtujhxpbai.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.chenzaomai.com/gtlugnjhdh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.quarkkingdee.top/gtqeukzgki.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.dianchejie.cn/gtihgsmogj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.nanxinkj.top/gtgsrqopuh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.daria6918.cn/gtsnxdlnfl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.shuidangran.top/gtcolzmmbm.html

[K05] 深拷贝对象
来源：http://hz.yonumen.top/gttvbdaqgg.html

Py:   copy.deepcopy(obj)
来源：http://hz.ydzc1.top/gtcxpwuttw.html

PHP:  unserialize(serialize($obj));
来源：http://hz.snrcjt.cn/gtrvffrcid.html

JS:   structuredClone(obj)
来源：http://hz.yueranfly.top/gthfmudnhh.html

TS:   structuredClone(obj)
来源：http://hz.zhoulong.xyz/gtghskqtip.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.316326.xyz/gtmuxwycmh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.shzxlz.cn/gtzyhxcdqm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.mhx1999.top/gtzprbynav.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.smart0.xyz/gtxggkdxjo.html

[K06] 解析 URL 查询串
来源：http://hz.hammf.cn/gtcbfqileu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.nanxinkj.top/gtlklowrnv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zdqjudy.top/gtyemezcsr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.pycfn.com/gtkjzozche.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hnqzz.top/gtovnuoryw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yvedp.cn/gtmqevqdnc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jianghu66.top/gtjxyybtem.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.sufxvd.cn/gtqyzcerbf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.wangshuangyany.cn/gtvwmyybqo.html

[K07] 进制转换
来源：http://hz.chenlongwang.top/gtqwoqbvfu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zycfv.cn/gtxxjddujz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ppjwa.cn/gthtcwphel.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.nanxuanxn.top/gtruobfjai.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.gaohongyu789.top/gtiwfsgxnc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.52xcode.cn/gthexhbmia.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.guowangkeji.top/gtuthlfmjt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xingfuxueyuan.xyz/gtdzjlopqr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.fzhhl.top/gtuiaaanlz.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.316326.xyz/gtgjjsojiw.html

Py:   pickle.dumps(obj)
来源：http://hz.zhongyouzk.top/gtdkwrpoau.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yanxiufei.cn/gtzevogmnn.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.xingfuxueyuan.xyz/gtixhcsywl.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.316326.xyz/gttfnzfdjt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhaomingkeji.xyz/gtqkgjxtfz.html

Go:   encoding/gob
来源：http://hz.wangdashe.top/gtjrjoolzp.html

Ruby: Marshal.dump(obj)
来源：http://hz.yuanzhike.top/gtbycimibu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xuanzx.com/gtuhewaihd.html

================================================================================
来源：http://hz.hywenlv.cn/gtmpcjwoqy.html

L. 网络请求
来源：http://hz.jinyuanbaomall.cn/gtxabthczd.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtxeqgpzho.html

[L01] 发送 GET 请求
来源：http://hz.gaohongyu789.top/gtxbexpfqo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hfpthk.cn/gtbinevbel.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.c1oappe.top/gtckipnxjm.html

JS:   await fetch(url)
来源：http://hz.shangyingyoupin.top/gtkboxbyhm.html

TS:   await fetch(url)
来源：http://hz.zhaomingkeji.xyz/gtmilpvjte.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.9152youxi.cn/gtsdywjkwe.html

Go:   resp, err := http.Get(url)
来源：http://hz.zdqjudy.top/gtmuaervpm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.svipenyu.cn/gtbqfblhlj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jyoumei.cn/gtqnicoysc.html

[L02] 发送 POST JSON
来源：http://hz.xuetiantiany.cn/gtahshelzo.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.chenlongwang.top/gtmzcpeyop.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yj202588.top/gtyzckzylf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xinyue.icu/gtlykoohty.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.snrcjt.cn/gtgdrfffij.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.sxryk.cn/gttiswkxuo.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xuetiantiany.cn/gtlmdpwkht.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.daxiang520.top/gtpelnrqdi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.andypj.xyz/gtlmltskon.html

[L03] 设置自定义请求头
来源：http://hz.hnqzz.top/gtbvxkpouk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.mhx1999.top/gtbexauoft.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.xziqi.cn/gtkltjklkn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinqigfzy.top/gtvzfpfhtl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xinyue.icu/gtszfldumg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ydzc1.top/gtzghyykaw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yongpay.top/gthpohwdro.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.sweek.top/gtmhvydxcq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.pengpengdd.cyou/gtxhekukko.html

[L04] 设置超时
来源：http://hz.yanxiufei.cn/gtiuatrdae.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zhaomingkeji.xyz/gtjgdxncqy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.sysykeji.top/gtgaeauthf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhoulong.xyz/gtbfgnggtz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nanxuanxn.top/gtjqchfvgk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hysaishi.cn/gtdjbfjcdg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.bjfxy.top/gtgrtlpxbr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jqgfzy.top/gtnkltpmzc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.gaohongyu789.top/gtdhsombgm.html

[L05] 上传文件（multipart）
来源：http://hz.tianlin.xyz/gtuweuzvaa.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.nanxinkj.top/gtderchfxe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.haohaochexian.top/gtpizvjxtm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.guowangkeji.top/gtfxlonebv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yueranfly.top/gtkkzfkqdh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ywan-chungtsiang.top/gtliospqeh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.cqqwz.cn/gthgkcotmv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ehwqpu.com/gtwkijrour.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.fzhhl.top/gtnrbouwwg.html

[L06] 解析响应为 JSON
来源：http://hz.jqgufenzy.top/gtoabpsikr.html

Py:   resp.json()
来源：http://hz.cheryme.top/gtqrkgajft.html

PHP:  json_decode($body, true);
来源：http://hz.jiagoushi.top/gtadtskahe.html

JS:   await resp.json()
来源：http://hz.nanxinkj.top/gtwpwkjzjp.html

TS:   await resp.json()
来源：http://hz.nanxuanxn.top/gtgbmksscl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jianghu66.top/gtsehdjnlj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.pycfn.com/gtwkzflejl.html

Ruby: JSON.parse(resp.body)
来源：http://hz.daria6918.cn/gtycytfvng.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.guannengcc.top/gtnqidpsfz.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhiwuduotai.top/gttvumonut.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xylfe.cn/gtflqkubtk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.sxryk.cn/gtsifrsznm.html

JS:   resp.ok;  resp.status
来源：http://hz.316326.xyz/gtsvxcbamr.html

TS:   resp.ok;  resp.status
来源：http://hz.chenzaomai.com/gtdvwzhrbm.html

Java: resp.statusCode()
来源：http://hz.ybcxt.top/gthkoryplk.html

Go:   resp.StatusCode
来源：http://hz.jqgufenzy.top/gtpdynkldr.html

Ruby: resp.code.to_i
来源：http://hz.zdqjudy.top/gtazotqciu.html

C#:   (int)resp.StatusCode
来源：http://hz.ppjwa.cn/gtovwgbwho.html

[L08] 并发请求多个地址
来源：http://hz.yj20258.top/gtcydjndho.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.0kj1m.cn/gtjatrkpqo.html

PHP:  curl_multi_init() 系列
来源：http://hz.c1oappe.top/gtdejczvgt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xingfuxueyuan.xyz/gtyjlscipn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenjidiqi.icu/gterzoqjth.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhijiandao.cn/gtkvsjcyjn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.pengpengdd.cyou/gtcpubvrpw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.birdmap.top/gtqygkgbxq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ydzc1.top/gtmnbzxaoy.html

================================================================================
来源：http://hz.316326.xyz/gtdyinymcr.html

M. 命令行 / 进程 / 环境
来源：http://hz.smart0.xyz/gtxzdgfgcw.html

================================================================================
来源：http://hz.ivvv.top/gtqqvvpzli.html

[M01] 读取命令行参数
来源：http://hz.zhijiandao.cn/gtaprxzqft.html

Py:   sys.argv[1:]
来源：http://hz.nanxinkj.top/gtbcejbpky.html

PHP:  $argv;  $argc;
来源：http://hz.birdmap.top/gtncqzflln.html

JS:   process.argv.slice(2)
来源：http://hz.iojbl.cn/gtshuprchy.html

TS:   process.argv.slice(2)
来源：http://hz.zdqjudy.top/gtupaxrbcw.html

Java: args 数组（main 方法参数）
来源：http://hz.xuanzx.com/gtufdqsdez.html

Go:   os.Args[1:]
来源：http://hz.bjfxy.top/gtsckrzhqj.html

Ruby: ARGV
来源：http://hz.jqgufenzy.top/gtoxivyvkz.html

C#:   args 数组（Main 方法参数）
来源：http://hz.gogol.net.cn/gtowaxfevi.html

[M02] 读取环境变量
来源：http://hz.hnqzz.top/gtvfzxkjix.html

Py:   os.environ.get("HOME")
来源：http://hz.feifeiyinyue.top/gttifoxakr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.sxryk.cn/gthhwugszk.html

JS:   process.env.HOME
来源：http://hz.jqgufenzy.top/gtegwrnmox.html

TS:   process.env.HOME
来源：http://hz.jqgfzy.top/gtmymefook.html

Java: System.getenv("HOME")
来源：http://hz.redwolf501.top/gtfkhxpcfs.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.tanke756.top/gtisnzfhxk.html

Ruby: ENV["HOME"]
来源：http://hz.jinqigufen.top/gtsntwdbqy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhengqikj.top/gtixlsuwod.html

[M03] 执行外部命令
来源：http://hz.chenlongwang.top/gthdelgkbw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ydzc1.top/gtsspuheia.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.9152youxi.cn/gtkfuxlzsb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.sxryk.cn/gtxxtbcidv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.aibaodan.cn/gtfhbmwlfn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.smart0.xyz/gtzcxltmqa.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hfpthk.cn/gtvuugaiwg.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.xinyue.icu/gtltxptxmh.html

C#:   Process.Start("ls", "-l");
来源：http://hz.bjfxy.top/gtprgtbgsb.html

[M04] 获取当前工作目录
来源：http://hz.jinqigfzy.top/gtphtwrrri.html

Py:   os.getcwd()
来源：http://hz.gotoacloud.top/gtywdshzno.html

PHP:  getcwd();
来源：http://hz.316326.xyz/gtsgvimhtz.html

JS:   process.cwd()
来源：http://hz.gaohongyu789.top/gtrxctherf.html

TS:   process.cwd()
来源：http://hz.ydzc1.top/gtbhszkutg.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xylfe.cn/gtslbgphku.html

Go:   os.Getwd()
来源：http://hz.316326.xyz/gtyyqidjck.html

Ruby: Dir.pwd
来源：http://hz.bjfxy.top/gthmrywplo.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.chenlongwang.top/gtajpbwevw.html

[M05] 设置退出码
来源：http://hz.tian-w.cn/gtqkyhnqpa.html

Py:   sys.exit(1)
来源：http://hz.xylfe.cn/gttklcdibw.html

PHP:  exit(1);
来源：http://hz.pycfn.com/gteitkijrp.html

JS:   process.exit(1)
来源：http://hz.yj202588.top/gtgluowzre.html

TS:   process.exit(1)
来源：http://hz.zhoulong.xyz/gtystgbrng.html

Java: System.exit(1)
来源：http://hz.gogol.net.cn/gtqhhluudu.html

Go:   os.Exit(1)
来源：http://hz.chenjidiqi.icu/gtkvnulzva.html

Ruby: exit 1
来源：http://hz.fengsongda.top/gtmpmunzzx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.iojbl.cn/gtlkzgnail.html

[M06] 向标准错误输出
来源：http://hz.havefunace.top/gtibuhcxsc.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ivvv.top/gtnfjioklh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.dashuyun.cn/gtarilmlnd.html

JS:   console.error("err")
来源：http://hz.316326.xyz/gtylzdygff.html

TS:   console.error("err")
来源：http://hz.yj20258.top/gtzdmzukvu.html

Java: System.err.println("err")
来源：http://hz.zdqjudy.top/gtkdepdfky.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.wangdashe.top/gtzukgcymo.html

Ruby: warn "err"
来源：http://hz.tian-w.cn/gtnqprziin.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhiwuduotai.top/gthgopailn.html

[M07] 判断是否为主入口
来源：http://hz.sweek.top/gtqyjviaaa.html

Py:   if __name__ == "__main__":
来源：http://hz.jinqigufen.top/gtqimjprxv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yangfankeji.com/gtbgxedeqk.html

JS:   require.main === module
来源：http://hz.shzxlz.cn/gttcmimhhj.html

TS:   require.main === module
来源：http://hz.hnxiangtu.top/gtvifnwjih.html

Java: public static void main(String[] args)
来源：http://hz.jlsjyb.cn/gtbcyhvaij.html

Go:   func main()
来源：http://hz.hammf.cn/gtfoiqxheq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.guannengcc.top/gtkczyvwpu.html

C#:   static void Main(string[] args)
来源：http://hz.fzhhl.top/gtrdjmfgnl.html

[M08] 获取系统与运行时信息
来源：http://hz.shanyushiyangkeji.top/gtvvxsdhjy.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zdqjudy.top/gtchnunhjt.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.tanke756.top/gtvrrmtujs.html

JS:   process.platform;  process.version
来源：http://hz.jinghuilouyu.cn/gtnylcjhge.html

TS:   process.platform;  process.version
来源：http://hz.jqgfzy.top/gtnddubaiy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.guannengcc.top/gtnqlnfdrk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.9152youxi.cn/gtlbqhqbny.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.shangyingyoupin.top/gthwkrgafq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jyoumei.cn/gtamhkzopv.html

================================================================================
来源：http://hz.jinqigufen.top/gtljzvsnyg.html

N. 数据结构与算法
来源：http://hz.yj202588.top/gtajmdyqhu.html

================================================================================
来源：http://hz.wangdashe.top/gtclrhgubg.html

[N01] 二分查找（有序数组）
来源：http://hz.shangyingyoupin.top/gtfaczwatv.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.cheryme.top/gtvejuzbiy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ehwqpu.com/gtezxfrnxq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.316326.xyz/gtqcwmsjeh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jqgfzy.top/gtzindzylb.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.cqqwz.cn/gtdidrdksn.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.shangyingyoupin.top/gtpavrbdxs.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhijiandao.cn/gthwnptreu.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.wangdashe.top/gtwssuuiox.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jqgufenzy.top/gthvjzokri.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gaohongyu789.top/gtxiwkypuh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.cdnleiting.top/gtgivdjckj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nanxuanxn.top/gtchlgdqhr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.daria6918.cn/gtepbdsftp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhaomingkeji.xyz/gtuplxmxgz.html

Go:   slices.Sort(arr)
来源：http://hz.aizwys.cn/gtwiotjfxp.html

Ruby: arr.sort
来源：http://hz.hysaishi.cn/gtgrhtddvw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.cheryme.top/gttzhbgput.html

[N03] 快速排序（分治示例）
来源：http://hz.jlsjyb.cn/gtqnhjxidd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.andypj.xyz/gtjboutcwq.html

PHP:  // 递归实现，或用 usort
来源：http://hz.bjfxy.top/gtpnljyshk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xylfe.cn/gtkbrxbyhv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shanyushiyangkeji.top/gtgfvxeuhy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.cdnleiting.top/gtjpsdqcjq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.bjfxy.top/gtsduzjlla.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.52xcode.cn/gtrowyilmz.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jianghu66.top/gtqfqfpgkj.html

[N04] 斐波那契数列
来源：http://hz.hnqzz.top/gtxmmxfmco.html


<!-- 参考信息 -->