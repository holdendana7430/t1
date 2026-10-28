代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.aizwys.cn/gtkaemxdko.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yongpay.top/gtrzufoscb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.daria6918.cn/gtluvobtyd.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhixingplan.top/gtyvtelfml.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.bjfxy.top/gtsrzeybrr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.cqqwz.cn/gtdlztamwe.html

[J09] 时区处理
来源：http://hz.cucudq.cn/gtamcfhbkb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.fzhhl.top/gtlsuvvnwy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yuanzhike.top/gtskunbhnp.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tanke756.top/gtevpeldvi.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.dashuyun.cn/gtvlszmzht.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.cucudq.cn/gtufntblqa.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yonumen.top/gtqyvyzkja.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hongshengwenyu.top/gthmfbsxnx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.aizwys.cn/gtncgvnvuf.html

[J10] 取今天 / 本月第一天
来源：http://hz.pengpengdd.cyou/gtxywhzxew.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.316326.xyz/gtkgjzjaau.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.shangyingyoupin.top/gtnbicwgco.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.nanxinkj.top/gtczjxbbji.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.aibaodan.cn/gtzkcxxlmj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yueranfly.top/gtkbefimqh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xziqi.cn/gtiihqtryx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jyoumei.cn/gtkiaitbxr.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.tianlin.xyz/gtuqluyjzz.html

================================================================================
来源：http://hz.zhengqikj.top/gtlifbpsjw.html

K. JSON 与序列化
来源：http://hz.zhijiandao.cn/gttsjuzack.html

================================================================================
来源：http://hz.zhixingplan.top/gtstxqxzwv.html

[K01] 对象转 JSON 字符串
来源：http://hz.xziqi.cn/gtrvcmpyux.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.dashuyun.cn/gtcjjhjuqy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhixingplan.top/gtjopmqleo.html

JS:   JSON.stringify(obj)
来源：http://hz.zhengqikj.top/gtlmzvhplg.html

TS:   JSON.stringify(obj)
来源：http://hz.svipenyu.cn/gtzfxqtoth.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.tian-w.cn/gtasixgipg.html

Go:   json.Marshal(obj)
来源：http://hz.aibaodan.cn/gtcdxuangd.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.52xcode.cn/gtaecdojkt.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.sweek.top/gtjpvmvqoq.html

[K02] JSON 字符串转对象
来源：http://hz.jinghuilouyu.cn/gthamnwoxu.html

Py:   json.loads(s)
来源：http://hz.smart0.xyz/gtavhfvgzc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.sxryk.cn/gtsxivdecl.html

JS:   JSON.parse(s)
来源：http://hz.zhongyouzk.top/gtqmbzqkot.html

TS:   JSON.parse(s)
来源：http://hz.haohaochexian.top/gtkzawqacu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.wangdashe.top/gtezawxvbo.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jqgufenzy.top/gtacuqexqw.html

Ruby: JSON.parse(s)
来源：http://hz.sufxvd.cn/gtccybhteq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.guowangkeji.top/gttvcswuas.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.svipenyu.cn/gtkupyevbw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xuetiantiany.cn/gtoujqenzq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.guowangkeji.top/gtqmbsffrh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.kuanghao11.cn/gtetqjpsrf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhengqikj.top/gtgweddouj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zhaomingkeji.xyz/gtahbpbsii.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.chenzaomai.com/gtjuqmhvlr.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.sxryk.cn/gtqhdkzody.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jinqigufen.top/gtaxbybvnl.html

[K04] 读取 JSON 文件
来源：http://hz.hysaishi.cn/gtttlyqyol.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.andypj.xyz/gtmbtaqndp.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jqgfzy.top/gtlfdoeraz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.iojbl.cn/gtszdfrref.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shuidangran.top/gthjqiwrra.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yuanzhike.top/gtgsmeypfp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.nwbrower.top/gtkqnvjvzz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.chenzaomai.com/gtkeudkama.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.52xcode.cn/gtpogedspw.html

[K05] 深拷贝对象
来源：http://hz.daria6918.cn/gtsturrmky.html

Py:   copy.deepcopy(obj)
来源：http://hz.chenlongwang.top/gthhvzyvff.html

PHP:  unserialize(serialize($obj));
来源：http://hz.wangdashe.top/gtjqsesybm.html

JS:   structuredClone(obj)
来源：http://hz.nwbrower.top/gtqrmvepbm.html

TS:   structuredClone(obj)
来源：http://hz.quarkkingdee.top/gtxpgutjoq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.shanyushiyangkeji.top/gtrodcgphm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.bjfxy.top/gtqapdrjlv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhijiandao.cn/gtbtedpgir.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhiwuduotai.top/gtaknopdig.html

[K06] 解析 URL 查询串
来源：http://hz.quarkkingdee.top/gtzxbxmjwj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.quarkkingdee.top/gtbpuatvqv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.quarkkingdee.top/gtxvynrvnn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj20258.top/gtshsahhwo.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ppjwa.cn/gtkeqlwnsx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hammf.cn/gtpvludoad.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.shangyingyoupin.top/gtatkefaoq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhoulong.xyz/gtnlixeffg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.hammf.cn/gtdfrvjoqb.html

[K07] 进制转换
来源：http://hz.zhaomingkeji.xyz/gtedlqdcet.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.chenjidiqi.icu/gtqfrlefrf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yj20258.top/gtbuomexph.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yuanzhike.top/gtxukyfpqf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yanxiufei.cn/gtoawhkjsn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.havefunace.top/gtobsgyelc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.cheryme.top/gtqxnqcurr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yangfankeji.com/gtuyxxfcrv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.fzhhl.top/gtawysmjiu.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhengqikj.top/gtgcbbtmzw.html

Py:   pickle.dumps(obj)
来源：http://hz.ybcxt.top/gtplvxykdg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.pengpengdd.cyou/gtunvvqbih.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.dianchejie.cn/gtaluomcet.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.snrcjt.cn/gtegszcndy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jlsjyb.cn/gtzyatsruc.html

Go:   encoding/gob
来源：http://hz.yj20258.top/gtmmgfjhwv.html

Ruby: Marshal.dump(obj)
来源：http://hz.zdqjudy.top/gtjslyloqu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.wangshuangyany.cn/gtjzvloutr.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gttsrrrddb.html

L. 网络请求
来源：http://hz.meibo888.top/gtzwtdhtbi.html

================================================================================
来源：http://hz.fengsongda.top/gtbxlqfewq.html

[L01] 发送 GET 请求
来源：http://hz.gaohongyu789.top/gtzgfzavyc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.havefunace.top/gteyzepcrt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.xylfe.cn/gtooenysbo.html

JS:   await fetch(url)
来源：http://hz.zhixingplan.top/gtnsqofcad.html

TS:   await fetch(url)
来源：http://hz.jinqigufen.top/gtoqybqowh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jinghuilouyu.cn/gtojfcurjz.html

Go:   resp, err := http.Get(url)
来源：http://hz.chenjidiqi.icu/gtvhpsmngu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yongpay.top/gtavntdmhf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.fzhhl.top/gtdqaimsdt.html

[L02] 发送 POST JSON
来源：http://hz.zdqjudy.top/gtsczhowzf.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ywan-chungtsiang.top/gtmxsenlrq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.snrcjt.cn/gtwhmoyoko.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.pengpengdd.cyou/gtmojjmljg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.birdmap.top/gtnfduyuie.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.nanxuanxn.top/gtaiolminq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xziqi.cn/gtesjhxmns.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.bjfxy.top/gtahbxtcgn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ppjwa.cn/gtghskbvjx.html

[L03] 设置自定义请求头
来源：http://hz.jinqigfzy.top/gtydtfywgc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.52xcode.cn/gtptjrtaea.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zycfv.cn/gttdgxyekc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nanxuanxn.top/gtpwsbcmky.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ywan-chungtsiang.top/gtitwoddda.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.chenzaomai.com/gtnofgstzg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.cdnleiting.top/gtfxsqmevq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.xuanzx.com/gtjgrmqzef.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yuanzhike.top/gtjgkwhiay.html

[L04] 设置超时
来源：http://hz.yuanzhike.top/gtakjvlhrn.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ivvv.top/gtsciduvhb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.sxryk.cn/gtlbikegua.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.quarkkingdee.top/gtzpxpqkbz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.chenlongwang.top/gtsyuzcggp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.0kj1m.cn/gtpedptzyg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.haohaochexian.top/gtwetfqltz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hammf.cn/gtvjmupmqq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hnxiangtu.top/gtmyigzbrq.html

[L05] 上传文件（multipart）
来源：http://hz.ydzc1.top/gtprbzfgxy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.mhx1999.top/gtawzpzuxn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yvedp.cn/gtlfrcnijt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.cdnleiting.top/gtbsqxwbsa.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yuanzhike.top/gtqqtkvvnj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yueranfly.top/gtrlkxxknl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yongpay.top/gtdvnrxooi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.vqdsnc.cn/gtewynbjlb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.ppjwa.cn/gtantowktg.html

[L06] 解析响应为 JSON
来源：http://hz.sysykeji.top/gtbklhcejx.html

Py:   resp.json()
来源：http://hz.cheryme.top/gtdmzikqwh.html

PHP:  json_decode($body, true);
来源：http://hz.wangdashe.top/gtjgtcnzvc.html

JS:   await resp.json()
来源：http://hz.guowangkeji.top/gtmmmygnrh.html

TS:   await resp.json()
来源：http://hz.bjfxy.top/gtdevbjdhy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.chenzaomai.com/gtmywbuweq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yangfankeji.com/gthhukqyle.html

Ruby: JSON.parse(resp.body)
来源：http://hz.gotoacloud.top/gtbxjxpigv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.daria6918.cn/gtybajxlmq.html

[L07] 处理 HTTP 状态码
来源：http://hz.xylfe.cn/gtvrdvdbtc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.wangshuangyany.cn/gtnwwxzlzx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hnxiangtu.top/gtazfudyrp.html

JS:   resp.ok;  resp.status
来源：http://hz.jinqigufen.top/gtwtzwqroc.html

TS:   resp.ok;  resp.status
来源：http://hz.ydjk.org.cn/gtxbxbtirl.html

Java: resp.statusCode()
来源：http://hz.zycfv.cn/gtdsjgavrr.html

Go:   resp.StatusCode
来源：http://hz.hongshengwenyu.top/gthgdurtdl.html

Ruby: resp.code.to_i
来源：http://hz.0kj1m.cn/gtutiifisz.html

C#:   (int)resp.StatusCode
来源：http://hz.0kj1m.cn/gtjmpfytnz.html

[L08] 并发请求多个地址
来源：http://hz.zhixingplan.top/gtmccjnlrh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.wangshuangyany.cn/gtctamxcfp.html

PHP:  curl_multi_init() 系列
来源：http://hz.jqgufenzy.top/gtomefejyx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zycfv.cn/gtghvfwmtc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sufxvd.cn/gtlejophhs.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.smart0.xyz/gtrstzghhh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jinghuilouyu.cn/gtccskzdob.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.iojbl.cn/gtlswmfztm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.316326.xyz/gtupjbkaxv.html

================================================================================
来源：http://hz.gogol.net.cn/gtaybrozlj.html

M. 命令行 / 进程 / 环境
来源：http://hz.gzhubu.top/gtogqlipaz.html

================================================================================
来源：http://hz.kuanghao11.cn/gtiogbasdx.html

[M01] 读取命令行参数
来源：http://hz.yj202588.top/gtlmpirtjr.html

Py:   sys.argv[1:]
来源：http://hz.sysykeji.top/gtyvpvxfcx.html

PHP:  $argv;  $argc;
来源：http://hz.yuxming.cn/gtckjhqrsg.html

JS:   process.argv.slice(2)
来源：http://hz.nanxuanxn.top/gtompmubmn.html

TS:   process.argv.slice(2)
来源：http://hz.cucudq.cn/gtgiysweef.html

Java: args 数组（main 方法参数）
来源：http://hz.cucudq.cn/gtoueltqce.html

Go:   os.Args[1:]
来源：http://hz.xuetiantiany.cn/gtdtxtmxtl.html

Ruby: ARGV
来源：http://hz.pengpengdd.cyou/gtgaukhtvi.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hammf.cn/gtqorjnnld.html

[M02] 读取环境变量
来源：http://hz.hammf.cn/gtxmnuvmtr.html

Py:   os.environ.get("HOME")
来源：http://hz.yvedp.cn/gtforzfbjx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.shanyushiyangtech.top/gthneqsdic.html

JS:   process.env.HOME
来源：http://hz.tianlin.xyz/gtbdynkgfx.html

TS:   process.env.HOME
来源：http://hz.xziqi.cn/gtdfosdpcr.html

Java: System.getenv("HOME")
来源：http://hz.hongshengwenyu.top/gtwkcnnfjn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.52xcode.cn/gtailfwsyo.html

Ruby: ENV["HOME"]
来源：http://hz.wangdashe.top/gtptahhxjy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhiwuduotai.top/gthlelkriu.html

[M03] 执行外部命令
来源：http://hz.hongshengwenyu.top/gtllsembwo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jinghuilouyu.cn/gtyfulflhy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yongpay.top/gtciuabyqj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jiagoushi.top/gtvtrqapkl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jqgufenzy.top/gtbnqinnxj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhaomingkeji.xyz/gtwraxhwez.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.xuanzx.com/gtgcuobbyx.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.guowangkeji.top/gturzkzkxw.html

C#:   Process.Start("ls", "-l");
来源：http://hz.pycfn.com/gtybyrdssx.html

[M04] 获取当前工作目录
来源：http://hz.hnxiangtu.top/gtmzbbqujj.html

Py:   os.getcwd()
来源：http://hz.smart0.xyz/gtfgfwbbdv.html

PHP:  getcwd();
来源：http://hz.meibo888.top/gtarmzxdcn.html

JS:   process.cwd()
来源：http://hz.aizwys.cn/gtlppnafgp.html

TS:   process.cwd()
来源：http://hz.zycfv.cn/gtvzrrhncx.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ehwqpu.com/gtlicttmeg.html

Go:   os.Getwd()
来源：http://hz.hnxiangtu.top/gtpwlisnpy.html

Ruby: Dir.pwd
来源：http://hz.tianlin.xyz/gtctqjruak.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhiwuduotai.top/gtwmsnctxt.html

[M05] 设置退出码
来源：http://hz.vqdsnc.cn/gtsbcllolr.html

Py:   sys.exit(1)
来源：http://hz.xziqi.cn/gtkqwvuiji.html

PHP:  exit(1);
来源：http://hz.jqgfzy.top/gtpkadtvja.html

JS:   process.exit(1)
来源：http://hz.yj20258.top/gtxdrhjtgs.html

TS:   process.exit(1)
来源：http://hz.ehwqpu.com/gtnjascapj.html

Java: System.exit(1)
来源：http://hz.yj202588.top/gtjkbswqpj.html

Go:   os.Exit(1)
来源：http://hz.cheryme.top/gtrdekjjpg.html

Ruby: exit 1
来源：http://hz.jianghu66.top/gtrvcniyuq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.chenlongwang.top/gtrwsfiafm.html

[M06] 向标准错误输出
来源：http://hz.svipenyu.cn/gtjapirosk.html

Py:   print("err", file=sys.stderr)
来源：http://hz.feifeiyinyue.top/gtgxwuvrzx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hnqzz.top/gtlmpogzqp.html

JS:   console.error("err")
来源：http://hz.tanke756.top/gtpmchwolj.html

TS:   console.error("err")
来源：http://hz.jinqigfzy.top/gtnqlylbee.html

Java: System.err.println("err")
来源：http://hz.gotoacloud.top/gtxjsxiskd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.nanxinkj.top/gtdkcnjesx.html

Ruby: warn "err"
来源：http://hz.sufxvd.cn/gtjdoqlart.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhijiandao.cn/gtnbdefsnv.html

[M07] 判断是否为主入口
来源：http://hz.shanyushiyangtech.top/gtalpyzrjd.html

Py:   if __name__ == "__main__":
来源：http://hz.yanxiufei.cn/gtjppwlsyp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.tian-w.cn/gtzpgfzzmo.html

JS:   require.main === module
来源：http://hz.zhongyouzk.top/gtyjsbfjfp.html

TS:   require.main === module
来源：http://hz.zycfv.cn/gtxvzgoveo.html

Java: public static void main(String[] args)
来源：http://hz.jinqigufen.top/gtlatzzqcu.html

Go:   func main()
来源：http://hz.c1oappe.top/gtbwwzkgcd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.tianlin.xyz/gthpcraueg.html

C#:   static void Main(string[] args)
来源：http://hz.jqgufenzy.top/gtvkplrdxe.html

[M08] 获取系统与运行时信息
来源：http://hz.snrcjt.cn/gtcdphxlyp.html

Py:   platform.system();  platform.python_version()
来源：http://hz.tianlin.xyz/gtuzmciovm.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.dashuyun.cn/gtdvpagiar.html

JS:   process.platform;  process.version
来源：http://hz.hfpthk.cn/gttutqonmh.html

TS:   process.platform;  process.version
来源：http://hz.nwbrower.top/gtekgmjlqy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jinyuanbaomall.cn/gteanprlhq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.andypj.xyz/gtzysjmfnh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cashguo.top/gtzktlzidf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.redwolf501.top/gthufcngxq.html

================================================================================
来源：http://hz.mhx1999.top/gtkzbohxel.html

N. 数据结构与算法
来源：http://hz.jinqigfzy.top/gtfgjwddsy.html

================================================================================
来源：http://hz.kuanghao11.cn/gtzzgtrrkl.html

[N01] 二分查找（有序数组）
来源：http://hz.xinyue.icu/gtqvenvafz.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ydzc1.top/gtzbaknvcu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.fengsongda.top/gtlqhsrrgq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.aibaodan.cn/gtmbbtokxy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jyoumei.cn/gtphllpzoy.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.tanke756.top/gtocphqjnb.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.feifeiyinyue.top/gtfxmduttb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yanxiufei.cn/gtbcrhqfar.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yuxming.cn/gtbtdoqylg.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.daria6918.cn/gtfytfecex.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.bjfxy.top/gtybgcdgfg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.havefunace.top/gtcdlpkjml.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yangfankeji.com/gtpropcfaf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hongshengwenyu.top/gttryjzryd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhoulong.xyz/gtfjxdunwl.html

Go:   slices.Sort(arr)
来源：http://hz.mhx1999.top/gtrbzjhais.html

Ruby: arr.sort
来源：http://hz.yongpay.top/gtgudzwxyp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.vqdsnc.cn/gthokpiyme.html

[N03] 快速排序（分治示例）
来源：http://hz.ppjwa.cn/gtmsxbgzvu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ivvv.top/gtoktbsgtk.html

PHP:  // 递归实现，或用 usort
来源：http://hz.sweek.top/gtglfvlord.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.smart0.xyz/gtlecoknnk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.sxryk.cn/gtqscxckva.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jianghu66.top/gttdnmggsv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.bjfxy.top/gtkhmgbsea.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yangfankeji.com/gtytsalwgf.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.cucudq.cn/gtyztmhxbp.html

[N04] 斐波那契数列
来源：http://hz.fzhhl.top/gtjcvfbtee.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.gogol.net.cn/gtyeaytriw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.ydzc1.top/gtovrkuhew.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.gzhubu.top/gtusyvoudk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.316326.xyz/gtsqautauh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.sufxvd.cn/gtxsrqxynl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.mhx1999.top/gtwikiztzk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ywan-chungtsiang.top/gtbdhhzkqg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.c1oappe.top/gtmoggcwmm.html

[N05] 最大公约数
来源：http://hz.yueranfly.top/gtdrzybuzu.html

Py:   math.gcd(a, b)
来源：http://hz.hongshengwenyu.top/gtdowxxpny.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zdqjudy.top/gtlmbtxiox.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.smart0.xyz/gtlncavufo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhaomingkeji.xyz/gtujxxqekj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.sufxvd.cn/gtdgpspiir.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.gzhubu.top/gtbikhauhp.html

Ruby: a.gcd(b)
来源：http://hz.hywenlv.cn/gtydrjsfmm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.tian-w.cn/gtavxmzaoo.html

[N06] 判断回文字符串
来源：http://hz.shanyushiyangkeji.top/gtteonexjn.html

Py:   s == s[::-1]
来源：http://hz.gaohongyu789.top/gtnglgyxqt.html

PHP:  $s === strrev($s);
来源：http://hz.shangyingyoupin.top/gtztdrtwaq.html


<!-- 参考信息 -->