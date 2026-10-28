代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258.top/gtptogszui.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.daria6918.cn/gtnmvwhfrh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.haohaochexian.top/gtqwiurkzy.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zhiwuduotai.top/gtfqongvyx.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yj202588.top/gtmzkfihog.html

[J08] 提取年月日与星期
来源：http://hz.xylfe.cn/gturyjxmik.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yuanzhike.top/gtmshixuau.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yj20258.top/gttwcbtsbz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.fengsongda.top/gtpwznbgrj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ywan-chungtsiang.top/gtiwtjdoip.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.fzhhl.top/gtqjsvyjpo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.gzhubu.top/gtxixbknok.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.meibo888.top/gtzkoirmcv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ywan-chungtsiang.top/gtovcoxsge.html

[J09] 时区处理
来源：http://hz.mhx1999.top/gtqvukpmsa.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jqgfzy.top/gtdmthatww.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.snrcjt.cn/gtitalmcoe.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.birdmap.top/gtltjwbjpi.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ehwqpu.com/gtapauribw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yvedp.cn/gtfuckjtqq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.316326.xyz/gtcuovpljv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.aizwys.cn/gtcifvzytc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shanyushiyangtech.top/gtztgesyvb.html

[J10] 取今天 / 本月第一天
来源：http://hz.sxryk.cn/gtsgoyvzax.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yj20258.top/gtdanucyfu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jianghu66.top/gtjraqyuel.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.tianlin.xyz/gtwyykqdxn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.chenjidiqi.icu/gtzplladhq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yueranfly.top/gthgesekpj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.wangshuangyany.cn/gtevinyrsy.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.gzhubu.top/gtlzychmte.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jqgufenzy.top/gtjtvjpyap.html

================================================================================
来源：http://hz.daria6918.cn/gtcsmbfkxl.html

K. JSON 与序列化
来源：http://hz.jianghu66.top/gtkqgnuyjf.html

================================================================================
来源：http://hz.jianghu66.top/gthfniaejh.html

[K01] 对象转 JSON 字符串
来源：http://hz.xuanzx.com/gttiumgycm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hammf.cn/gtehhyrrpc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.0kj1m.cn/gtzzbshfmp.html

JS:   JSON.stringify(obj)
来源：http://hz.xziqi.cn/gtrwvfwiva.html

TS:   JSON.stringify(obj)
来源：http://hz.quarkkingdee.top/gtgixrvhxv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xuanzx.com/gtvpilvizu.html

Go:   json.Marshal(obj)
来源：http://hz.shanyushiyangkeji.top/gtdzfahnhf.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhoulong.xyz/gtyiembznk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.guannengcc.top/gtfbngsfgn.html

[K02] JSON 字符串转对象
来源：http://hz.shanyushiyangtech.top/gtrbitgvci.html

Py:   json.loads(s)
来源：http://hz.gzhubu.top/gtijokzkww.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.c1oappe.top/gthnsgonnb.html

JS:   JSON.parse(s)
来源：http://hz.sxryk.cn/gtuprdrsvk.html

TS:   JSON.parse(s)
来源：http://hz.nanxinkj.top/gtjltvttls.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.tanke756.top/gtzerzmrry.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.shanyushiyangtech.top/gtrjucsedd.html

Ruby: JSON.parse(s)
来源：http://hz.yuxming.cn/gtyazlyfbu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yj20258.top/gtslmzqqic.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.haohaochexian.top/gtqdasggvt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yangfankeji.com/gtmmtictbv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.cdnleiting.top/gtdkoytkcs.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.cqqwz.cn/gtgombpxti.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.quarkkingdee.top/gtadqxkifm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hysaishi.cn/gtxxlqcxow.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jinqigfzy.top/gtttldujpc.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ybcxt.top/gtayilvjsd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.shangyingyoupin.top/gtazztjktc.html

[K04] 读取 JSON 文件
来源：http://hz.sweek.top/gtvsonhvqw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.nwbrower.top/gtbvfomibn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.gzhubu.top/gtybdcgbeh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yongpay.top/gtrtwjvmoe.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.chenlongwang.top/gtagvmltxi.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhaomingkeji.xyz/gttdooocpo.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.chenzaomai.com/gtwwvdtbpl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.kuanghao11.cn/gtovjdweeb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hnxiangtu.top/gtjbpudcdn.html

[K05] 深拷贝对象
来源：http://hz.aibaodan.cn/gtzngirzlj.html

Py:   copy.deepcopy(obj)
来源：http://hz.sufxvd.cn/gtwtbheamn.html

PHP:  unserialize(serialize($obj));
来源：http://hz.mhx1999.top/gtwsgjsmak.html

JS:   structuredClone(obj)
来源：http://hz.sweek.top/gtbguzsrhp.html

TS:   structuredClone(obj)
来源：http://hz.xuanzx.com/gtaxcsfujw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.bjfxy.top/gtbtwmbbta.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hnqzz.top/gtuvmcezan.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.tian-w.cn/gtpsowqhow.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhengqikj.top/gtkihtfklw.html

[K06] 解析 URL 查询串
来源：http://hz.jqgufenzy.top/gtgjdmtqxj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.fzhhl.top/gtsvexizxd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.guowangkeji.top/gtdpinqmbz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.iojbl.cn/gtlsyadihe.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shanyushiyangtech.top/gtllzohlfr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.xingfuxueyuan.xyz/gtkutyhrmj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.wangdashe.top/gtnfxkiffl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.meibo888.top/gtqmrymncq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.fengsongda.top/gtmxwqbrvs.html

[K07] 进制转换
来源：http://hz.zhoulong.xyz/gtlunltzma.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.sufxvd.cn/gthbxfgpbi.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.pycfn.com/gtltdryqqv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shanyushiyangtech.top/gtqtnovsxi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.sufxvd.cn/gtwjzviegh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xingfuxueyuan.xyz/gtlgwhhzih.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.daxiang520.top/gtrrkzjjqv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zdqjudy.top/gtjquyonot.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhaomingkeji.xyz/gteuxhtnfn.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yonumen.top/gtrafljbjj.html

Py:   pickle.dumps(obj)
来源：http://hz.shangyingyoupin.top/gtbzbrpsdv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.cqqwz.cn/gtzpphxqgu.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shzxlz.cn/gtuzztbplm.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhixingplan.top/gtdsznbvrp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yj20258888.top/gtgrpyoinf.html

Go:   encoding/gob
来源：http://hz.jyoumei.cn/gtlrmqgeqc.html

Ruby: Marshal.dump(obj)
来源：http://hz.feifeiyinyue.top/gtybppkckb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.pycfn.com/gtrbwpcbme.html

================================================================================
来源：http://hz.sxryk.cn/gtkpuhgpzb.html

L. 网络请求
来源：http://hz.shzxlz.cn/gtfkeeudic.html

================================================================================
来源：http://hz.shuidangran.top/gtwxblnqkz.html

[L01] 发送 GET 请求
来源：http://hz.jyoumei.cn/gtcrxqmzxn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.snrcjt.cn/gtsnveeiqw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hnxiangtu.top/gtltuxehga.html

JS:   await fetch(url)
来源：http://hz.mhx1999.top/gthgzztjyp.html

TS:   await fetch(url)
来源：http://hz.yuanzhike.top/gtjpjatymc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.pycfn.com/gtlkkqqxdf.html

Go:   resp, err := http.Get(url)
来源：http://hz.snrcjt.cn/gtkigleezo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zdqjudy.top/gtrhxqkrwx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.wangshuangyany.cn/gtbffquesc.html

[L02] 发送 POST JSON
来源：http://hz.zhoulong.xyz/gteqtttzbj.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yanxiufei.cn/gtjuxqwkfn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.chenzaomai.com/gtkjrpduxh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yonumen.top/gtfuisjfrp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.pycfn.com/gtroygcqdn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.0kj1m.cn/gteecefcgs.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jinyuanbaomall.cn/gtolvejjab.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.guannengcc.top/gtdwcaozry.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yj20258888.top/gtkjcqebko.html

[L03] 设置自定义请求头
来源：http://hz.ybcxt.top/gtoruuuath.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.cashguo.top/gtihftrzyb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.9152youxi.cn/gtdxumzkzy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yuanzhike.top/gtrxkfnlmo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.dianchejie.cn/gtcwgmfcnj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.xziqi.cn/gtrdrcovnv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.shangyingyoupin.top/gtysbcizkv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhongyouzk.top/gtkkkpixza.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.xinyue.icu/gtbmtubluz.html

[L04] 设置超时
来源：http://hz.dashuyun.cn/gtunoifeqf.html

Py:   requests.get(url, timeout=5)
来源：http://hz.havefunace.top/gtlnuzfuuj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.iojbl.cn/gtktpczyok.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.c1oappe.top/gtofobapme.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.daxiang520.top/gtrahtvhka.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xingfuxueyuan.xyz/gtfkrcaahg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.gogol.net.cn/gtbmogythb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yj202588.top/gtfhbutakj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xinyue.icu/gtnqfskfgb.html

[L05] 上传文件（multipart）
来源：http://hz.cashguo.top/gtuqetuyuk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.shzxlz.cn/gtarylrykm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.andypj.xyz/gtudstwmxg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.aizwys.cn/gtirklgkxt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.wangshuangyany.cn/gtbzslxxtv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.shangyingyoupin.top/gtbisvpbkk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.quarkkingdee.top/gtxjcqgcbu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.guowangkeji.top/gtjhqibmju.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.ivvv.top/gtfwzcdjik.html

[L06] 解析响应为 JSON
来源：http://hz.hfpthk.cn/gtoxifvyfb.html

Py:   resp.json()
来源：http://hz.nanxuanxn.top/gturnrshvd.html

PHP:  json_decode($body, true);
来源：http://hz.ppjwa.cn/gtxdvmvtmk.html

JS:   await resp.json()
来源：http://hz.daxiang520.top/gtsxvwhvzd.html

TS:   await resp.json()
来源：http://hz.tianlin.xyz/gtzulhtknr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.gaohongyu789.top/gtxcijaefz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.mhx1999.top/gtppejgapr.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yvedp.cn/gtecffhakt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.guowangkeji.top/gtpizookvq.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhoulong.xyz/gtbrgseddx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.vqdsnc.cn/gtseouszri.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.fengsongda.top/gtggxbupxr.html

JS:   resp.ok;  resp.status
来源：http://hz.9152youxi.cn/gttdcqzztq.html

TS:   resp.ok;  resp.status
来源：http://hz.svipenyu.cn/gtnkwwmmwt.html

Java: resp.statusCode()
来源：http://hz.daria6918.cn/gtjsmefdyb.html

Go:   resp.StatusCode
来源：http://hz.tian-w.cn/gtazbwbbyc.html

Ruby: resp.code.to_i
来源：http://hz.gzhubu.top/gtlqhblgnn.html

C#:   (int)resp.StatusCode
来源：http://hz.sysykeji.top/gtqvqjlgxu.html

[L08] 并发请求多个地址
来源：http://hz.ywan-chungtsiang.top/gtnosbibkv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hnqzz.top/gtpkiigdup.html

PHP:  curl_multi_init() 系列
来源：http://hz.wangdashe.top/gtcixjtmop.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hongshengwenyu.top/gttfzjrzwj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tianlin.xyz/gtfrxdwnoz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.0kj1m.cn/gtwdrovlhy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zdqjudy.top/gtieilvteq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.nwbrower.top/gtytjgqgba.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yonumen.top/gtxgsuuwhh.html

================================================================================
来源：http://hz.chenlongwang.top/gtkjkvjkje.html

M. 命令行 / 进程 / 环境
来源：http://hz.havefunace.top/gttvjvubct.html

================================================================================
来源：http://hz.yanxiufei.cn/gtcydlyyyz.html

[M01] 读取命令行参数
来源：http://hz.jinqigfzy.top/gtqtaipvgx.html

Py:   sys.argv[1:]
来源：http://hz.guowangkeji.top/gtzyfqgdml.html

PHP:  $argv;  $argc;
来源：http://hz.hnqzz.top/gtetwaxunt.html

JS:   process.argv.slice(2)
来源：http://hz.zhongyouzk.top/gtmaxleeku.html

TS:   process.argv.slice(2)
来源：http://hz.svipenyu.cn/gtkkolfcdb.html

Java: args 数组（main 方法参数）
来源：http://hz.yj20258.top/gtgxmfhdrr.html

Go:   os.Args[1:]
来源：http://hz.tanke756.top/gtpnxbhhij.html

Ruby: ARGV
来源：http://hz.xziqi.cn/gtvdhtyovp.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ppjwa.cn/gtvwifgdss.html

[M02] 读取环境变量
来源：http://hz.gogol.net.cn/gttzaojngl.html

Py:   os.environ.get("HOME")
来源：http://hz.quarkkingdee.top/gtekygdqlp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.gzhubu.top/gtkddxvine.html

JS:   process.env.HOME
来源：http://hz.iojbl.cn/gtepyxfivz.html

TS:   process.env.HOME
来源：http://hz.yongpay.top/gtmwuqtheh.html

Java: System.getenv("HOME")
来源：http://hz.guannengcc.top/gttlmmgcir.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hysaishi.cn/gtvqphboua.html

Ruby: ENV["HOME"]
来源：http://hz.nanxinkj.top/gttvdenbxy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.c1oappe.top/gtpxyfnsqa.html

[M03] 执行外部命令
来源：http://hz.nanxinkj.top/gtcnfysstf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhijiandao.cn/gtlyqxugzl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.tian-w.cn/gtoktmbgmr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.0kj1m.cn/gtpnevxfti.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.gogol.net.cn/gtxzlzqnem.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jinyuanbaomall.cn/gtaxcothvi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.tanke756.top/gtqwzhkubi.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yuxming.cn/gtphphycim.html

C#:   Process.Start("ls", "-l");
来源：http://hz.316326.xyz/gtojdbgcnf.html

[M04] 获取当前工作目录
来源：http://hz.shanyushiyangkeji.top/gtknhqvwqz.html

Py:   os.getcwd()
来源：http://hz.pengpengdd.cyou/gtowfhpufs.html

PHP:  getcwd();
来源：http://hz.jinqigfzy.top/gtrpmzklsw.html

JS:   process.cwd()
来源：http://hz.yanxiufei.cn/gtvudjmifb.html

TS:   process.cwd()
来源：http://hz.jyoumei.cn/gtvxqdcmrn.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hnqzz.top/gtlmiiuhdk.html

Go:   os.Getwd()
来源：http://hz.yj20258888.top/gtbfrsboca.html

Ruby: Dir.pwd
来源：http://hz.zhixingplan.top/gtqbbsquyh.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.xuanzx.com/gtkeyzkujz.html

[M05] 设置退出码
来源：http://hz.yueranfly.top/gtbpqziizr.html

Py:   sys.exit(1)
来源：http://hz.hnxiangtu.top/gtzlvivway.html

PHP:  exit(1);
来源：http://hz.c1oappe.top/gtiiqunawh.html

JS:   process.exit(1)
来源：http://hz.sufxvd.cn/gtdatxjugr.html

TS:   process.exit(1)
来源：http://hz.tanke756.top/gtfuriswiy.html

Java: System.exit(1)
来源：http://hz.snrcjt.cn/gtvlsbpusu.html

Go:   os.Exit(1)
来源：http://hz.guowangkeji.top/gtyhgifjos.html

Ruby: exit 1
来源：http://hz.yangfankeji.com/gttymbgfto.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.hnxiangtu.top/gtktydpivb.html

[M06] 向标准错误输出
来源：http://hz.hammf.cn/gtqgpgcagb.html

Py:   print("err", file=sys.stderr)
来源：http://hz.cucudq.cn/gtjajpstwb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.gzhubu.top/gtbmnvuefv.html

JS:   console.error("err")
来源：http://hz.jinqigufen.top/gtkvargqto.html

TS:   console.error("err")
来源：http://hz.guowangkeji.top/gtjcaisqwh.html

Java: System.err.println("err")
来源：http://hz.cashguo.top/gtrzchhksr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.shanyushiyangkeji.top/gtluametfv.html

Ruby: warn "err"
来源：http://hz.zhijiandao.cn/gtvfwydoqo.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.feifeiyinyue.top/gtdduocmix.html

[M07] 判断是否为主入口
来源：http://hz.xuanzx.com/gtpemdbobl.html

Py:   if __name__ == "__main__":
来源：http://hz.ywan-chungtsiang.top/gtwrgfrevh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.bjfxy.top/gtircpisuj.html

JS:   require.main === module
来源：http://hz.ydzc1.top/gtwpwiufpb.html

TS:   require.main === module
来源：http://hz.aizwys.cn/gtmnltuorh.html

Java: public static void main(String[] args)
来源：http://hz.hnxiangtu.top/gtmymplfnm.html

Go:   func main()
来源：http://hz.shanyushiyangkeji.top/gtdlricixm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yj20258888.top/gthuilicff.html

C#:   static void Main(string[] args)
来源：http://hz.zhengqikj.top/gtifpdyeso.html

[M08] 获取系统与运行时信息
来源：http://hz.shanyushiyangtech.top/gtqhlnuzhh.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhoulong.xyz/gtllyrzyyz.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yanxiufei.cn/gtmklwreyf.html

JS:   process.platform;  process.version
来源：http://hz.pengpengdd.cyou/gtjktzflkb.html

TS:   process.platform;  process.version
来源：http://hz.nanxuanxn.top/gtdqyxnrlh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.ehwqpu.com/gtrykyiuim.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zhiwuduotai.top/gtjjxyvjvy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jinqigufen.top/gtspzgzmsk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jinyuanbaomall.cn/gtblkjbxig.html

================================================================================
来源：http://hz.daria6918.cn/gtyxaerrjz.html

N. 数据结构与算法
来源：http://hz.vqdsnc.cn/gtztcxogva.html

================================================================================
来源：http://hz.zhiwuduotai.top/gteqzyjehv.html

[N01] 二分查找（有序数组）
来源：http://hz.dianchejie.cn/gtehtigolj.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.nanxinkj.top/gtvhzwzqge.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.smart0.xyz/gtvmfwrmxb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.aizwys.cn/gtrdztwbtf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ybcxt.top/gtcmyxmgpb.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.snrcjt.cn/gtstxegxqz.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.pengpengdd.cyou/gteuecrdmg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jqgufenzy.top/gtbohtncue.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.shuidangran.top/gtxyluhxeb.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jlsjyb.cn/gtayagpdsl.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.vqdsnc.cn/gtjecrgnli.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yuanzhike.top/gtsrgllvza.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shzxlz.cn/gtbclevofr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.tanke756.top/gttttfggzj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.0kj1m.cn/gthrllkjvk.html

Go:   slices.Sort(arr)
来源：http://hz.ywan-chungtsiang.top/gtuzbwghjo.html

Ruby: arr.sort
来源：http://hz.wangshuangyany.cn/gttzslrowz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.hnqzz.top/gtizikkamf.html

[N03] 快速排序（分治示例）
来源：http://hz.gogol.net.cn/gtselqqrep.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ydzc1.top/gtuoineblx.html

PHP:  // 递归实现，或用 usort
来源：http://hz.pengpengdd.cyou/gtsfckztyq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hammf.cn/gttzdnpqxr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cqqwz.cn/gtouztzizl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.gzhubu.top/gtgxiujjiu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.meibo888.top/gtjidkhtkj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.meibo888.top/gtuchvziru.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.iojbl.cn/gtgukwqcie.html

[N04] 斐波那契数列
来源：http://hz.hysaishi.cn/gtjeuoimiz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.0kj1m.cn/gtdnqpcuzx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.vqdsnc.cn/gtytjvvgsr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ydjk.org.cn/gtavuxrvsf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zycfv.cn/gtjtembgdu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.sxryk.cn/gtaiugdlyk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.sufxvd.cn/gtxfjzdogy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.pengpengdd.cyou/gtnkrievyw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jqgfzy.top/gtfuuegpbp.html

[N05] 最大公约数
来源：http://hz.sysykeji.top/gtpcdwufpl.html

Py:   math.gcd(a, b)
来源：http://hz.yuxming.cn/gtqfmqkkee.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.xinyue.icu/gtckdstska.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.feifeiyinyue.top/gtcbpwqgeq.html


<!-- 参考信息 -->