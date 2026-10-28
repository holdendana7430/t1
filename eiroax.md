代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hammf.cn/gtmgchxerp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.chenzaomai.com/gtmzakfbdp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hnqzz.top/gtgjffehok.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.chenzaomai.com/gtgszaxxuj.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.shanyushiyangtech.top/gtpodkzuwu.html

[J08] 提取年月日与星期
来源：http://hz.shanyushiyangtech.top/gtpnwevbnz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.kuanghao11.cn/gtacwwytnb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.feifeiyinyue.top/gtpgcjlrjh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shangyingyoupin.top/gttwtcyvto.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ywan-chungtsiang.top/gtwkrtzize.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.cashguo.top/gtrrjwiugi.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhoulong.xyz/gthmcjneli.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jqgufenzy.top/gtokifunyg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yueranfly.top/gtkofhxldb.html

[J09] 时区处理
来源：http://hz.chenzaomai.com/gtqjvisqsx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xziqi.cn/gtiygtrqtp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.sweek.top/gtnccgxplu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nanxuanxn.top/gtxqvlbyym.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.316326.xyz/gtgutmqqzx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jyoumei.cn/gtvkpydvzb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.havefunace.top/gtvmoacbir.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yj20258.top/gtqniqjcdx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.quarkkingdee.top/gthqkxliph.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhongyouzk.top/gtwoufarhc.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jyoumei.cn/gtpomftyak.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zycfv.cn/gtsngcpvin.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.0kj1m.cn/gtzpxwclco.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zdqjudy.top/gttlxvndwm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yueranfly.top/gtejoxaqih.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xuetiantiany.cn/gtfjljpuip.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.nanxuanxn.top/gtrnclyprf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.guannengcc.top/gtrnaosvlr.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtifigudmo.html

K. JSON 与序列化
来源：http://hz.bjfxy.top/gttcnellik.html

================================================================================
来源：http://hz.cheryme.top/gtfiioxwcs.html

[K01] 对象转 JSON 字符串
来源：http://hz.shangyingyoupin.top/gtjutrrboj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yueranfly.top/gtayyfmtgs.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhijiandao.cn/gtfpcbnyva.html

JS:   JSON.stringify(obj)
来源：http://hz.tian-w.cn/gtgjspkjjv.html

TS:   JSON.stringify(obj)
来源：http://hz.zycfv.cn/gtmrrepxsh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.tianlin.xyz/gtlbnpcvyz.html

Go:   json.Marshal(obj)
来源：http://hz.316326.xyz/gtyjcldosx.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cqqwz.cn/gtnoiywwkq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ydjk.org.cn/gttxnqilho.html

[K02] JSON 字符串转对象
来源：http://hz.guannengcc.top/gtfwiepxvu.html

Py:   json.loads(s)
来源：http://hz.pengpengdd.cyou/gtcetmmcsa.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.shuidangran.top/gttbzoklac.html

JS:   JSON.parse(s)
来源：http://hz.shzxlz.cn/gtrysnwjdg.html

TS:   JSON.parse(s)
来源：http://hz.haohaochexian.top/gtltteafdm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.wangshuangyany.cn/gttlxrzfgw.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.316326.xyz/gtedhttpso.html

Ruby: JSON.parse(s)
来源：http://hz.iojbl.cn/gtdetmnbye.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.wangdashe.top/gtqegfbiqq.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.gaohongyu789.top/gtxqkwiwak.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhiwuduotai.top/gtabpyfroh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.pengpengdd.cyou/gtwaimjgop.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.cheryme.top/gtybzjssfh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhijiandao.cn/gtroqwokmu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zhiwuduotai.top/gtqmagkttq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.sufxvd.cn/gtmlanpycf.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yueranfly.top/gtyliciooo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ppjwa.cn/gtlhuxcdtm.html

[K04] 读取 JSON 文件
来源：http://hz.wangshuangyany.cn/gtoaanvxct.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.dianchejie.cn/gtrzgfsogw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cheryme.top/gtgubzybls.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ehwqpu.com/gtvpvcqpze.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.aibaodan.cn/gtknzixaai.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.sysykeji.top/gtiecggdln.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.nanxuanxn.top/gtnkrxlxka.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.pengpengdd.cyou/gttylavywi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.mhx1999.top/gtmltjainn.html

[K05] 深拷贝对象
来源：http://hz.sufxvd.cn/gthsoyyini.html

Py:   copy.deepcopy(obj)
来源：http://hz.nwbrower.top/gtlqymhykz.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yj20258.top/gtrcuszbkt.html

JS:   structuredClone(obj)
来源：http://hz.cucudq.cn/gtcnwucmmr.html

TS:   structuredClone(obj)
来源：http://hz.nanxinkj.top/gtmmxlkwbq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.shanyushiyangkeji.top/gtnizbgdet.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.cqqwz.cn/gtpmpzyuda.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xziqi.cn/gtsxspnhip.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.redwolf501.top/gtfymaqsxv.html

[K06] 解析 URL 查询串
来源：http://hz.sufxvd.cn/gtkyybphkg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.bjfxy.top/gtoplioarf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.vqdsnc.cn/gtuqycmnik.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.redwolf501.top/gtfoddnlvo.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.daxiang520.top/gtpfoyaqtr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.xingfuxueyuan.xyz/gtxfsijpbo.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hysaishi.cn/gtsgsfmsmp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.nanxinkj.top/gtypzerbrd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cdnleiting.top/gtcxrrthfd.html

[K07] 进制转换
来源：http://hz.hysaishi.cn/gtwadmlvtb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yj202588.top/gtfakqsfgb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.tanke756.top/gtjssjwlyz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.gzhubu.top/gtwhdjkpqb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zdqjudy.top/gtqcedlczv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ehwqpu.com/gtqslmxjqp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.birdmap.top/gtuzmhnvex.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jianghu66.top/gtwoqozelz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.fzhhl.top/gtwczqlvae.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.cashguo.top/gtirirgoqf.html

Py:   pickle.dumps(obj)
来源：http://hz.yonumen.top/gtakvqnpwd.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yongpay.top/gtgqyhhofu.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.snrcjt.cn/gtjomzkzli.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.gaohongyu789.top/gtvwjpalqp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.sweek.top/gttwraiuxk.html

Go:   encoding/gob
来源：http://hz.xziqi.cn/gtbitqtxem.html

Ruby: Marshal.dump(obj)
来源：http://hz.hywenlv.cn/gtacwysrbg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yj20258.top/gtmgkctorl.html

================================================================================
来源：http://hz.zhixingplan.top/gtcbvbkezr.html

L. 网络请求
来源：http://hz.sufxvd.cn/gtkyslwlzy.html

================================================================================
来源：http://hz.sysykeji.top/gtlxjbxwki.html

[L01] 发送 GET 请求
来源：http://hz.yueranfly.top/gtizryijfs.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.redwolf501.top/gtldjafiye.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zycfv.cn/gtxwzqfuse.html

JS:   await fetch(url)
来源：http://hz.yj20258.top/gtjmfxhtjm.html

TS:   await fetch(url)
来源：http://hz.cashguo.top/gtkemwzmxc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhijiandao.cn/gttjmfayny.html

Go:   resp, err := http.Get(url)
来源：http://hz.xylfe.cn/gtevmbstoh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.birdmap.top/gtmpilwxhr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hammf.cn/gtycantakp.html

[L02] 发送 POST JSON
来源：http://hz.9152youxi.cn/gtyftbgesc.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.shangyingyoupin.top/gtvewtiwse.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jinqigufen.top/gtbsyjgkev.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sxryk.cn/gtsygfzwrr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ybcxt.top/gtohapswlj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ybcxt.top/gtcqqmuwpv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.sysykeji.top/gtwxsngrcj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.wangshuangyany.cn/gtpqcbpfek.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.chenlongwang.top/gtapiigvnz.html

[L03] 设置自定义请求头
来源：http://hz.jyoumei.cn/gteytggquf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.cashguo.top/gtwedvapln.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jqgfzy.top/gtfohzyyrm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gotoacloud.top/gtndibjbyk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shuidangran.top/gtlwoypanp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.tian-w.cn/gtvtjbjhrs.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.havefunace.top/gtnqhbaqib.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhoulong.xyz/gtguwwnbin.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.xuanzx.com/gtgwraycvy.html

[L04] 设置超时
来源：http://hz.dashuyun.cn/gttukhpiea.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ppjwa.cn/gtmqkobjmq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yuanzhike.top/gtrmucddbc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hnqzz.top/gtsswirlcf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.kuanghao11.cn/gtunjmoxpa.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xinyue.icu/gttogsgvkg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.pycfn.com/gtjhqcyvsa.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.havefunace.top/gttnkzlugc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hnqzz.top/gtibcousdd.html

[L05] 上传文件（multipart）
来源：http://hz.zhongyouzk.top/gtfwjwehio.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.fzhhl.top/gtmopopjvh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.ydjk.org.cn/gtifppedjd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenjidiqi.icu/gtlewhwwxp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.aibaodan.cn/gtslfddmtj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.smart0.xyz/gtzuzcmvss.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.guowangkeji.top/gtcwntcjda.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zdqjudy.top/gtoyadjhlc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.aibaodan.cn/gtxchqquuy.html

[L06] 解析响应为 JSON
来源：http://hz.jinyuanbaomall.cn/gtmdsxsoxk.html

Py:   resp.json()
来源：http://hz.316326.xyz/gtnqlksyqw.html

PHP:  json_decode($body, true);
来源：http://hz.9152youxi.cn/gtbhxmhati.html

JS:   await resp.json()
来源：http://hz.svipenyu.cn/gtbyjmzfke.html

TS:   await resp.json()
来源：http://hz.xziqi.cn/gtldtqbczw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.aizwys.cn/gtvpfncicq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zhoulong.xyz/gtqzajjrul.html

Ruby: JSON.parse(resp.body)
来源：http://hz.fengsongda.top/gtjgpkxsqz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hfpthk.cn/gtyobwdpix.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhengqikj.top/gtosxbyfxc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yvedp.cn/gtrrtyjsuk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.tianlin.xyz/gtppeybijc.html

JS:   resp.ok;  resp.status
来源：http://hz.sufxvd.cn/gtluykcpst.html

TS:   resp.ok;  resp.status
来源：http://hz.gotoacloud.top/gtnxsxsvyh.html

Java: resp.statusCode()
来源：http://hz.yangfankeji.com/gtcqmqpdop.html

Go:   resp.StatusCode
来源：http://hz.nanxinkj.top/gtkgtkvohf.html

Ruby: resp.code.to_i
来源：http://hz.quarkkingdee.top/gtmkysclyh.html

C#:   (int)resp.StatusCode
来源：http://hz.mhx1999.top/gtghvkurvj.html

[L08] 并发请求多个地址
来源：http://hz.hammf.cn/gtgddqyglh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.guannengcc.top/gtwbwglgkt.html

PHP:  curl_multi_init() 系列
来源：http://hz.ydjk.org.cn/gttjaxzbul.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xuanzx.com/gtwbsnzois.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.dashuyun.cn/gtongmqxmo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.fengsongda.top/gtynonzvhu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.snrcjt.cn/gtqghzejzs.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ydjk.org.cn/gtkmaowczn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.chenzaomai.com/gtscpzforf.html

================================================================================
来源：http://hz.nanxinkj.top/gtcdjqsitz.html

M. 命令行 / 进程 / 环境
来源：http://hz.nwbrower.top/gtigfwloju.html

================================================================================
来源：http://hz.jiagoushi.top/gtffevuuhn.html

[M01] 读取命令行参数
来源：http://hz.feifeiyinyue.top/gtarejnamm.html

Py:   sys.argv[1:]
来源：http://hz.hammf.cn/gtokqexbux.html

PHP:  $argv;  $argc;
来源：http://hz.ehwqpu.com/gtphbexssk.html

JS:   process.argv.slice(2)
来源：http://hz.shzxlz.cn/gtpepeptig.html

TS:   process.argv.slice(2)
来源：http://hz.tanke756.top/gtnqkogflf.html

Java: args 数组（main 方法参数）
来源：http://hz.tanke756.top/gtnkfnbmde.html

Go:   os.Args[1:]
来源：http://hz.zdqjudy.top/gtmpvszbqe.html

Ruby: ARGV
来源：http://hz.ivvv.top/gtcprkpzwg.html

C#:   args 数组（Main 方法参数）
来源：http://hz.cucudq.cn/gtayjzgnpt.html

[M02] 读取环境变量
来源：http://hz.cdnleiting.top/gtabcurysu.html

Py:   os.environ.get("HOME")
来源：http://hz.ywan-chungtsiang.top/gtgrjtonnm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.cucudq.cn/gtwxpnzhpg.html

JS:   process.env.HOME
来源：http://hz.zhoulong.xyz/gtkjmrcvwp.html

TS:   process.env.HOME
来源：http://hz.yanxiufei.cn/gteyjjseda.html

Java: System.getenv("HOME")
来源：http://hz.zhongyouzk.top/gtciannivt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hongshengwenyu.top/gtqftitccw.html

Ruby: ENV["HOME"]
来源：http://hz.daxiang520.top/gtwyzhgipw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xziqi.cn/gtflmpgtgp.html

[M03] 执行外部命令
来源：http://hz.jyoumei.cn/gtgzwmlmlp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.shzxlz.cn/gthaihdgwf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jqgfzy.top/gtzrknyvlq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yj20258.top/gtmoxqyjyk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yj202588.top/gtcighyiac.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.fengsongda.top/gtwouyzyts.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yvedp.cn/gtykasdiys.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.nwbrower.top/gtrhxrqpnw.html

C#:   Process.Start("ls", "-l");
来源：http://hz.daxiang520.top/gtatmzhnxq.html

[M04] 获取当前工作目录
来源：http://hz.guannengcc.top/gtnzbzfoeu.html

Py:   os.getcwd()
来源：http://hz.52xcode.cn/gtdxnfwikz.html

PHP:  getcwd();
来源：http://hz.cdnleiting.top/gtgfjsanxg.html

JS:   process.cwd()
来源：http://hz.jinqigfzy.top/gtxgotnzrf.html

TS:   process.cwd()
来源：http://hz.tian-w.cn/gtvjglgwso.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhixingplan.top/gtyorobmal.html

Go:   os.Getwd()
来源：http://hz.zhijiandao.cn/gtopbbdcfi.html

Ruby: Dir.pwd
来源：http://hz.yangfankeji.com/gtfowjiizg.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.daxiang520.top/gtywujbsob.html

[M05] 设置退出码
来源：http://hz.316326.xyz/gtdmuvwnai.html

Py:   sys.exit(1)
来源：http://hz.hammf.cn/gtalpizliu.html

PHP:  exit(1);
来源：http://hz.hnqzz.top/gtksupxirg.html

JS:   process.exit(1)
来源：http://hz.yvedp.cn/gtqbpbupls.html

TS:   process.exit(1)
来源：http://hz.dianchejie.cn/gtynlsafeb.html

Java: System.exit(1)
来源：http://hz.hnqzz.top/gttrycusid.html

Go:   os.Exit(1)
来源：http://hz.birdmap.top/gtowraguaw.html

Ruby: exit 1
来源：http://hz.hfpthk.cn/gtacrfrraf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.smart0.xyz/gtlxhbgtve.html

[M06] 向标准错误输出
来源：http://hz.wangdashe.top/gtmcxapiuw.html

Py:   print("err", file=sys.stderr)
来源：http://hz.cdnleiting.top/gtnuulxsib.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hongshengwenyu.top/gtspxiltvb.html

JS:   console.error("err")
来源：http://hz.yuxming.cn/gtmhaifhwf.html

TS:   console.error("err")
来源：http://hz.snrcjt.cn/gtqnrcruuc.html

Java: System.err.println("err")
来源：http://hz.gzhubu.top/gtwcsftkbr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.chenjidiqi.icu/gtcoowhrnf.html

Ruby: warn "err"
来源：http://hz.cdnleiting.top/gtkhtacvig.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.9152youxi.cn/gtwiextduy.html

[M07] 判断是否为主入口
来源：http://hz.zycfv.cn/gtztyrtfbn.html

Py:   if __name__ == "__main__":
来源：http://hz.xziqi.cn/gtkyzcidfz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.pengpengdd.cyou/gtjaskqpes.html

JS:   require.main === module
来源：http://hz.dashuyun.cn/gtbjftybcq.html

TS:   require.main === module
来源：http://hz.yueranfly.top/gtzvxyzbwc.html

Java: public static void main(String[] args)
来源：http://hz.andypj.xyz/gtawlmjspa.html

Go:   func main()
来源：http://hz.zhijiandao.cn/gtqmimvanb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.aizwys.cn/gtfdfuhyur.html

C#:   static void Main(string[] args)
来源：http://hz.wangshuangyany.cn/gtekakyveu.html

[M08] 获取系统与运行时信息
来源：http://hz.andypj.xyz/gtxboejgoj.html

Py:   platform.system();  platform.python_version()
来源：http://hz.shanyushiyangkeji.top/gtckhypuau.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.guannengcc.top/gtppvtrwvn.html

JS:   process.platform;  process.version
来源：http://hz.jyoumei.cn/gtcffqvmfj.html

TS:   process.platform;  process.version
来源：http://hz.zhiwuduotai.top/gtrbmnrdaz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yanxiufei.cn/gtlosewjya.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yueranfly.top/gtyqrkiacj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.redwolf501.top/gtuapajjvf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hnqzz.top/gthncojefq.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtpxjfkfdk.html

N. 数据结构与算法
来源：http://hz.xuanzx.com/gtuwxckuue.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtfqfbvlki.html

[N01] 二分查找（有序数组）
来源：http://hz.tianlin.xyz/gtqukoisty.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.snrcjt.cn/gtfhzbjuzl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.wangshuangyany.cn/gtiqxmblye.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.tian-w.cn/gtylpztywe.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.fengsongda.top/gtigqrshtz.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.fengsongda.top/gtghdhrtbd.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.andypj.xyz/gtuqqzyxwy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.wangdashe.top/gttxeacrdn.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.0kj1m.cn/gtqrtbdxrv.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.xingfuxueyuan.xyz/gtkyoyirhn.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sweek.top/gtpsxutyew.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.wangshuangyany.cn/gtlmqdkmdv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gotoacloud.top/gtyzisovfy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sweek.top/gtwajdxyui.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.guannengcc.top/gtuhsrmmlb.html

Go:   slices.Sort(arr)
来源：http://hz.jiagoushi.top/gttfizphwy.html

Ruby: arr.sort
来源：http://hz.shanyushiyangkeji.top/gtifgqlszo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.haohaochexian.top/gtaoaiyxlu.html

[N03] 快速排序（分治示例）
来源：http://hz.hysaishi.cn/gtznwpzfwz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xuanzx.com/gtmelxfjxm.html

PHP:  // 递归实现，或用 usort
来源：http://hz.nwbrower.top/gtjtmpxruw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.pycfn.com/gtynqckemb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.c1oappe.top/gtshddtast.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinghuilouyu.cn/gtbrfcnjea.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jinyuanbaomall.cn/gtaxmuksoq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.xingfuxueyuan.xyz/gtjivhnwug.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.wangshuangyany.cn/gtqufdxwgq.html

[N04] 斐波那契数列
来源：http://hz.jinyuanbaomall.cn/gtapltting.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hnqzz.top/gtdgpjukvl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.nanxuanxn.top/gtkwfihxzx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xinyue.icu/gtnmubkdfj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.52xcode.cn/gtxtujckdm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.xylfe.cn/gtkljcqtvq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yj20258888.top/gthxnzihso.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.gzhubu.top/gtryzcrpvb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.havefunace.top/gtdqtkjyze.html

[N05] 最大公约数
来源：http://hz.yj20258888.top/gttyihmflb.html

Py:   math.gcd(a, b)
来源：http://hz.nanxinkj.top/gtzjnhjztq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.ivvv.top/gtstddbiao.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.aibaodan.cn/gtpirkljmz.html


<!-- 参考信息 -->