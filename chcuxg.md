代发 wailian999

[J07] 比较两个日期
来源：http://hz.guannengcc.top/gtqijqrngt.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hywenlv.cn/gtakfofptb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.fzhhl.top/gtgikkiuzf.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.meibo888.top/gtjhdnrkat.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.c1oappe.top/gttzlempqf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.shanyushiyangtech.top/gtkrzyjszj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ppjwa.cn/gtxnoxuspl.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.gotoacloud.top/gtcjoqzkcg.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.xuanzx.com/gtmygwttfn.html

[J08] 提取年月日与星期
来源：http://hz.ivvv.top/gtqfxjnaom.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.smart0.xyz/gtvveuhhzk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.gzhubu.top/gtamqvgjxe.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hfpthk.cn/gtodgujnlx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.0kj1m.cn/gtroyqedbq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ivvv.top/gteyocpnlc.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.bjfxy.top/gtfprxngem.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xingfuxueyuan.xyz/gtsusiuxba.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jinqigfzy.top/gtpmgesvum.html

[J09] 时区处理
来源：http://hz.xziqi.cn/gtkkwmjxif.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zycfv.cn/gtpvysuxwx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ivvv.top/gtgijzgjeo.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.52xcode.cn/gtzisfzwfs.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.daxiang520.top/gtemmcclsr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ybcxt.top/gtucmvifph.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.pengpengdd.cyou/gtcdbbyrpp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.havefunace.top/gtpdrdmtwy.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hywenlv.cn/gtfqofctgz.html

[J10] 取今天 / 本月第一天
来源：http://hz.52xcode.cn/gtzqkzmljk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zdqjudy.top/gtqhppkpcj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.pengpengdd.cyou/gtnzmqxups.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.andypj.xyz/gtovyqueti.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yonumen.top/gtpfjmswmn.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yuxming.cn/gtqqbxwtez.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhoulong.xyz/gtzswcdscg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.shuidangran.top/gtidgfyagz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ywan-chungtsiang.top/gtxvqdkfop.html

================================================================================
来源：http://hz.yongpay.top/gtigkmrxvs.html

K. JSON 与序列化
来源：http://hz.ydjk.org.cn/gtqzttjnpy.html

================================================================================
来源：http://hz.iojbl.cn/gtmzbfftyx.html

[K01] 对象转 JSON 字符串
来源：http://hz.dianchejie.cn/gtzxzgnoeg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ivvv.top/gtnledtjij.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.andypj.xyz/gtmadsrueu.html

JS:   JSON.stringify(obj)
来源：http://hz.daria6918.cn/gtullsxfmc.html

TS:   JSON.stringify(obj)
来源：http://hz.jinqigfzy.top/gtuubqnpym.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.pengpengdd.cyou/gtpyofwpwr.html

Go:   json.Marshal(obj)
来源：http://hz.zdqjudy.top/gtetsajdpf.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shzxlz.cn/gtrkylnppk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.cheryme.top/gtxmsfkwnm.html

[K02] JSON 字符串转对象
来源：http://hz.mhx1999.top/gtdufqkpnb.html

Py:   json.loads(s)
来源：http://hz.52xcode.cn/gtpkdjxxwu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hnqzz.top/gtqvhywczm.html

JS:   JSON.parse(s)
来源：http://hz.snrcjt.cn/gtpfvxnmde.html

TS:   JSON.parse(s)
来源：http://hz.sxryk.cn/gtqfchntju.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.cashguo.top/gtxpfkllyd.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.havefunace.top/gtbsaxwgbm.html

Ruby: JSON.parse(s)
来源：http://hz.wangshuangyany.cn/gtxojddmyz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.fzhhl.top/gtzlbfdbor.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hnqzz.top/gtjisbmsea.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.cdnleiting.top/gtjlihhwfa.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhaomingkeji.xyz/gttdqykrhp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.nanxinkj.top/gtdyyheslw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.pengpengdd.cyou/gtvlvlmmep.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.xylfe.cn/gtbcwtptmd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yanxiufei.cn/gtutvexbzf.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yonumen.top/gtgyakpzff.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhoulong.xyz/gtbuoiqfka.html

[K04] 读取 JSON 文件
来源：http://hz.xziqi.cn/gtgfbpsacf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.feifeiyinyue.top/gtaebedyji.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cucudq.cn/gtxochbrwn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yongpay.top/gtoasuytns.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.nwbrower.top/gtvtvxgeuy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.52xcode.cn/gtlghaukky.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.gogol.net.cn/gtccuhqefi.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.meibo888.top/gtkmkqbcae.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.shuidangran.top/gtlqlfstoo.html

[K05] 深拷贝对象
来源：http://hz.zdqjudy.top/gtvxfjvmiu.html

Py:   copy.deepcopy(obj)
来源：http://hz.chenjidiqi.icu/gtuvewvhdc.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jiagoushi.top/gtecnovwwv.html

JS:   structuredClone(obj)
来源：http://hz.dashuyun.cn/gthssqtpvr.html

TS:   structuredClone(obj)
来源：http://hz.zdqjudy.top/gtmduraegi.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zycfv.cn/gtirtahvoa.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.bjfxy.top/gtgsouxzjh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.sweek.top/gtynuvrfhk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zycfv.cn/gthmlwskhi.html

[K06] 解析 URL 查询串
来源：http://hz.cashguo.top/gtzcmeactg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yangfankeji.com/gtphnbxrtk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.shanyushiyangkeji.top/gtgsqqbbid.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.guowangkeji.top/gtboudowxs.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cucudq.cn/gthxxjwxhf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhengqikj.top/gtoduccztz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zycfv.cn/gtptfxohwi.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hnqzz.top/gtnjjdbchp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhengqikj.top/gtezebnqta.html

[K07] 进制转换
来源：http://hz.316326.xyz/gtpveodvxb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhengqikj.top/gtpdoqjlpk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhoulong.xyz/gtoqutlkvz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shangyingyoupin.top/gtpdkaquag.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jinyuanbaomall.cn/gtktphhlmn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hammf.cn/gtdfpgkscc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.kuanghao11.cn/gtpfzggjcy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.nwbrower.top/gtvdqvygje.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yj20258.top/gthooxfwyb.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.gaohongyu789.top/gtseyzjsop.html

Py:   pickle.dumps(obj)
来源：http://hz.hysaishi.cn/gtpfjzdpfj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.tianlin.xyz/gtmigwslsi.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhoulong.xyz/gtklrjqciy.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yuanzhike.top/gtrnhypotz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhiwuduotai.top/gtxtslicgj.html

Go:   encoding/gob
来源：http://hz.yangfankeji.com/gtlggxlwke.html

Ruby: Marshal.dump(obj)
来源：http://hz.chenzaomai.com/gtggbvyhpr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shanyushiyangtech.top/gtftrpkbhl.html

================================================================================
来源：http://hz.jlsjyb.cn/gtsuncrogq.html

L. 网络请求
来源：http://hz.shangyingyoupin.top/gtcwyoysfu.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtopybywkm.html

[L01] 发送 GET 请求
来源：http://hz.ydjk.org.cn/gtjpumbdmk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jinqigfzy.top/gtpvkhhytc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.gotoacloud.top/gtcjwfdotj.html

JS:   await fetch(url)
来源：http://hz.wangshuangyany.cn/gthatgkper.html

TS:   await fetch(url)
来源：http://hz.hammf.cn/gtwqgckfda.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.nwbrower.top/gttlywepvw.html

Go:   resp, err := http.Get(url)
来源：http://hz.jlsjyb.cn/gtddajtnzo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jinghuilouyu.cn/gtvieiviic.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.dashuyun.cn/gtgmkjkosj.html

[L02] 发送 POST JSON
来源：http://hz.zhengqikj.top/gtpvckuqiz.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ppjwa.cn/gtajncdjxb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.wangshuangyany.cn/gtnnljfzqm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.dianchejie.cn/gtfwzxenhk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.0kj1m.cn/gtfpyepgfo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jianghu66.top/gtuivkmqkd.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.shanyushiyangkeji.top/gtufyeacfb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.cqqwz.cn/gtfvjhcowb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.gaohongyu789.top/gtfmmqwlmu.html

[L03] 设置自定义请求头
来源：http://hz.tian-w.cn/gtlqhhzwqr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.mhx1999.top/gtkfjitamg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.aizwys.cn/gtvdvswufn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.wangdashe.top/gtzpldiftd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.pengpengdd.cyou/gtspmihuua.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.xylfe.cn/gtdjfsbpnt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.sysykeji.top/gtfcihsvjl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhengqikj.top/gtliatxuqf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.316326.xyz/gtnlbegmxl.html

[L04] 设置超时
来源：http://hz.zhaomingkeji.xyz/gtxevfpoqj.html

Py:   requests.get(url, timeout=5)
来源：http://hz.meibo888.top/gtywamepgk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yanxiufei.cn/gtdcxiakrg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.dianchejie.cn/gtomwdbpnj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xuanzx.com/gtkvswinbf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhengqikj.top/gtkclsffyj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.fzhhl.top/gtvmpmehzx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.mhx1999.top/gtdeviwhrr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhongyouzk.top/gtswbnhbtj.html

[L05] 上传文件（multipart）
来源：http://hz.0kj1m.cn/gtothfotks.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jianghu66.top/gtlmkigpkr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jinqigufen.top/gtsptfcomq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.cashguo.top/gtwxltujqb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ydjk.org.cn/gtvghlukxl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yangfankeji.com/gtfuvjbdbb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.sxryk.cn/gtpczrohjx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.fzhhl.top/gtcvemadoa.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.sweek.top/gttppnjegs.html

[L06] 解析响应为 JSON
来源：http://hz.gotoacloud.top/gtbcdzjzow.html

Py:   resp.json()
来源：http://hz.nanxuanxn.top/gtdrerqvbw.html

PHP:  json_decode($body, true);
来源：http://hz.yonumen.top/gtalmyfuzi.html

JS:   await resp.json()
来源：http://hz.redwolf501.top/gtntjwwsgy.html

TS:   await resp.json()
来源：http://hz.vqdsnc.cn/gtljaczwnu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yvedp.cn/gthxsatgan.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jianghu66.top/gtkgjqtkyl.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yangfankeji.com/gttyvzbnpi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.shanyushiyangtech.top/gthcbfuxid.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhixingplan.top/gtiapzicdm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.ydjk.org.cn/gtohtdztbw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.mhx1999.top/gttatoryyp.html

JS:   resp.ok;  resp.status
来源：http://hz.mhx1999.top/gtnlaafetn.html

TS:   resp.ok;  resp.status
来源：http://hz.9152youxi.cn/gtjahvaltk.html

Java: resp.statusCode()
来源：http://hz.gotoacloud.top/gtyehjjrir.html

Go:   resp.StatusCode
来源：http://hz.hammf.cn/gtfhfctvvl.html

Ruby: resp.code.to_i
来源：http://hz.316326.xyz/gtlhtfdonw.html

C#:   (int)resp.StatusCode
来源：http://hz.52xcode.cn/gtinwnftkf.html

[L08] 并发请求多个地址
来源：http://hz.hywenlv.cn/gtlrxbuyqn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.xylfe.cn/gtaewwjmny.html

PHP:  curl_multi_init() 系列
来源：http://hz.pengpengdd.cyou/gtnubcnvqi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jiagoushi.top/gtodogfpcz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.wangshuangyany.cn/gtqmhgtbfg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ybcxt.top/gtfveykosf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.sxryk.cn/gtwxokwngg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yonumen.top/gtcdyffdcu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.quarkkingdee.top/gtjopkorue.html

================================================================================
来源：http://hz.smart0.xyz/gtmdvansib.html

M. 命令行 / 进程 / 环境
来源：http://hz.quarkkingdee.top/gtrffnuqiq.html

================================================================================
来源：http://hz.guowangkeji.top/gtjvhkiapp.html

[M01] 读取命令行参数
来源：http://hz.dianchejie.cn/gtkmcvcznt.html

Py:   sys.argv[1:]
来源：http://hz.fzhhl.top/gtvtcddhoh.html

PHP:  $argv;  $argc;
来源：http://hz.jqgfzy.top/gtbxjngghq.html

JS:   process.argv.slice(2)
来源：http://hz.ydzc1.top/gtcnfsptdl.html

TS:   process.argv.slice(2)
来源：http://hz.jinqigfzy.top/gtfevxnnbs.html

Java: args 数组（main 方法参数）
来源：http://hz.guowangkeji.top/gtgktgkibb.html

Go:   os.Args[1:]
来源：http://hz.ybcxt.top/gtromlnyga.html

Ruby: ARGV
来源：http://hz.andypj.xyz/gtuuetsxhg.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yj20258.top/gtilncytdh.html

[M02] 读取环境变量
来源：http://hz.nwbrower.top/gtiiphxotx.html

Py:   os.environ.get("HOME")
来源：http://hz.pycfn.com/gtegtzlmxi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.cheryme.top/gtbibtwmda.html

JS:   process.env.HOME
来源：http://hz.hnqzz.top/gtfmfddzbz.html

TS:   process.env.HOME
来源：http://hz.wangdashe.top/gtqdekfxuy.html

Java: System.getenv("HOME")
来源：http://hz.yvedp.cn/gtvqreevri.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.andypj.xyz/gtioqbqsha.html

Ruby: ENV["HOME"]
来源：http://hz.chenjidiqi.icu/gtbnvtcmuy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.tianlin.xyz/gtenhrmagj.html

[M03] 执行外部命令
来源：http://hz.aizwys.cn/gtbeavtmfh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jiagoushi.top/gtxmjssrce.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.aizwys.cn/gtfyhtghwb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yj20258888.top/gtcitpczcr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.meibo888.top/gtuuhqmvjr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.snrcjt.cn/gtukbwdizo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.daria6918.cn/gtdknpmwqi.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jinghuilouyu.cn/gtnzupdgoj.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xinyue.icu/gttyfmmauc.html

[M04] 获取当前工作目录
来源：http://hz.zycfv.cn/gtluticowi.html

Py:   os.getcwd()
来源：http://hz.fzhhl.top/gtecjzycue.html

PHP:  getcwd();
来源：http://hz.zhiwuduotai.top/gtyzlpqemj.html

JS:   process.cwd()
来源：http://hz.jqgfzy.top/gtanzwnjyj.html

TS:   process.cwd()
来源：http://hz.gzhubu.top/gtntdhbxal.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.9152youxi.cn/gtvhldvbpq.html

Go:   os.Getwd()
来源：http://hz.kuanghao11.cn/gtbqkfgjcs.html

Ruby: Dir.pwd
来源：http://hz.yuxming.cn/gtasgvztdk.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zycfv.cn/gtlleckdjj.html

[M05] 设置退出码
来源：http://hz.cashguo.top/gtoqwyctbt.html

Py:   sys.exit(1)
来源：http://hz.sweek.top/gtkrnzvzbt.html

PHP:  exit(1);
来源：http://hz.zhengqikj.top/gtswsgkluy.html

JS:   process.exit(1)
来源：http://hz.jqgufenzy.top/gtpfcbqqex.html

TS:   process.exit(1)
来源：http://hz.nanxuanxn.top/gtotlacjza.html

Java: System.exit(1)
来源：http://hz.jiagoushi.top/gtgkkujiqg.html

Go:   os.Exit(1)
来源：http://hz.dianchejie.cn/gtuhokzfza.html

Ruby: exit 1
来源：http://hz.haohaochexian.top/gttdpnssrc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jqgfzy.top/gtleggcpzz.html

[M06] 向标准错误输出
来源：http://hz.sweek.top/gtyjgzlhbh.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jinqigfzy.top/gtezjhyxsq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.nanxuanxn.top/gtswmexjqc.html

JS:   console.error("err")
来源：http://hz.gzhubu.top/gtluxueced.html

TS:   console.error("err")
来源：http://hz.yonumen.top/gthyptiuie.html

Java: System.err.println("err")
来源：http://hz.chenlongwang.top/gtxtkmwdai.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ydzc1.top/gtwjpcqnri.html

Ruby: warn "err"
来源：http://hz.ivvv.top/gtxwlohtqb.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ydjk.org.cn/gtociirqlq.html

[M07] 判断是否为主入口
来源：http://hz.ydjk.org.cn/gthqmhxuxa.html

Py:   if __name__ == "__main__":
来源：http://hz.zhixingplan.top/gthgeuqyir.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cucudq.cn/gtzxtvsmsl.html

JS:   require.main === module
来源：http://hz.zycfv.cn/gtairbrwpj.html

TS:   require.main === module
来源：http://hz.nwbrower.top/gtqqpcluin.html

Java: public static void main(String[] args)
来源：http://hz.jqgufenzy.top/gtbqpzleol.html

Go:   func main()
来源：http://hz.ivvv.top/gtgazefnmm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.gogol.net.cn/gtmfkfgqvi.html

C#:   static void Main(string[] args)
来源：http://hz.hysaishi.cn/gtnckrbmib.html

[M08] 获取系统与运行时信息
来源：http://hz.ppjwa.cn/gtjbpzalbq.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hnqzz.top/gtzulxvzhz.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.dashuyun.cn/gtlzvlkymk.html

JS:   process.platform;  process.version
来源：http://hz.shuidangran.top/gtbzknlump.html

TS:   process.platform;  process.version
来源：http://hz.haohaochexian.top/gtrytchtzp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.cdnleiting.top/gtwvgqtatj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.sysykeji.top/gtzlypcksv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.sysykeji.top/gtvitdlkwh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hnqzz.top/gtdlhgdmtc.html

================================================================================
来源：http://hz.yongpay.top/gtvgkpkfld.html

N. 数据结构与算法
来源：http://hz.52xcode.cn/gtlhqfvicl.html

================================================================================
来源：http://hz.yj20258.top/gtoicrhyyu.html

[N01] 二分查找（有序数组）
来源：http://hz.yangfankeji.com/gtstujuftu.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.dashuyun.cn/gtvkqobvsi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.52xcode.cn/gttunisoza.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hfpthk.cn/gtccycvsiy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.feifeiyinyue.top/gtzmwrczpw.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.shanyushiyangtech.top/gtiiwqhfrf.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.nanxinkj.top/gtptaqeoaq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.shangyingyoupin.top/gtvupeueae.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zhoulong.xyz/gtjuqltzev.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.gaohongyu789.top/gtnsvmulrx.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yj20258888.top/gtuxdnaylm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.chenjidiqi.icu/gtqxwhfeeb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jqgfzy.top/gtwjztqoza.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hfpthk.cn/gthjlolmpo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.iojbl.cn/gtzyejhlsd.html

Go:   slices.Sort(arr)
来源：http://hz.yj202588.top/gtmhaedqjp.html

Ruby: arr.sort
来源：http://hz.chenzaomai.com/gttfivqget.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhengqikj.top/gtgncmudub.html

[N03] 快速排序（分治示例）
来源：http://hz.tian-w.cn/gtbdvczgek.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.gzhubu.top/gtlbkjnfjw.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jqgufenzy.top/gtbrcuzksk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.0kj1m.cn/gtlnuyveca.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.bjfxy.top/gtxicyjeiv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhoulong.xyz/gtnbevznim.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yj20258888.top/gtznxvyrbl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.shanyushiyangtech.top/gtxrxhfyhk.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhengqikj.top/gtfljthija.html

[N04] 斐波那契数列
来源：http://hz.316326.xyz/gtwlmuvzum.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.dianchejie.cn/gtxbxvezlm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yj202588.top/gtefzvmnyh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ehwqpu.com/gtykfodepe.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shangyingyoupin.top/gtiohridkw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.kuanghao11.cn/gtatjwffsr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jinyuanbaomall.cn/gtmmfzgktd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hnqzz.top/gtwnwxlbsh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhaomingkeji.xyz/gtimlkuzcd.html


<!-- 参考信息 -->