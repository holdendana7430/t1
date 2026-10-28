代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhijiandao.cn/gtfpnopgyy.html

[J08] 提取年月日与星期
来源：http://hz.jlsjyb.cn/gtqqzonydr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhixingplan.top/gtxgqcjhxh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.iojbl.cn/gtdlvkfekn.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.havefunace.top/gtgpimebuw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ppjwa.cn/gtianvwldh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.andypj.xyz/gtqgfiwcjv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.shanyushiyangtech.top/gtpqcicwaw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zycfv.cn/gtcpxcaayo.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhijiandao.cn/gtijfhckog.html

[J09] 时区处理
来源：http://hz.jyoumei.cn/gtabdupluo.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.fengsongda.top/gtfmfspomr.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.sxryk.cn/gtlumddmsd.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.dianchejie.cn/gtxvonkzqm.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.wangshuangyany.cn/gtalnqrjch.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.cqqwz.cn/gtjuxezbnp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.gaohongyu789.top/gtfqkqpstf.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.mhx1999.top/gtrpxxbirj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.daria6918.cn/gtqmokddwv.html

[J10] 取今天 / 本月第一天
来源：http://hz.jinghuilouyu.cn/gtggjxkmjk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yj202588.top/gtdkwxqqbh.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.sufxvd.cn/gtemrytnql.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ppjwa.cn/gteivoxgps.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ywan-chungtsiang.top/gtidwztwfg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.gzhubu.top/gtpfqpiiji.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.smart0.xyz/gtmpbcqfnb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.mhx1999.top/gtxikfnsir.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.guannengcc.top/gtdaowluto.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtdxkayxjx.html

K. JSON 与序列化
来源：http://hz.tanke756.top/gtzdhoibmv.html

================================================================================
来源：http://hz.wangdashe.top/gtneeueyoy.html

[K01] 对象转 JSON 字符串
来源：http://hz.shzxlz.cn/gtrecnfyam.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yongpay.top/gtscxpqnph.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.quarkkingdee.top/gtfsvnmeik.html

JS:   JSON.stringify(obj)
来源：http://hz.fzhhl.top/gtoeqbdzry.html

TS:   JSON.stringify(obj)
来源：http://hz.shzxlz.cn/gtihoabwej.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zycfv.cn/gtndojdbga.html

Go:   json.Marshal(obj)
来源：http://hz.cheryme.top/gtawnumnox.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.ehwqpu.com/gtmvooaayn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.aizwys.cn/gtxhvpndrr.html

[K02] JSON 字符串转对象
来源：http://hz.yongpay.top/gtoikqtmmm.html

Py:   json.loads(s)
来源：http://hz.svipenyu.cn/gtsmdmiwdu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.sxryk.cn/gtlliwszck.html

JS:   JSON.parse(s)
来源：http://hz.c1oappe.top/gtkioavies.html

TS:   JSON.parse(s)
来源：http://hz.ehwqpu.com/gtszcolcuv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xylfe.cn/gtvmdjgeqp.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.havefunace.top/gtlsgukrlx.html

Ruby: JSON.parse(s)
来源：http://hz.jinghuilouyu.cn/gtggkvwcqp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhixingplan.top/gtoodxyxma.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.tianlin.xyz/gtlqkqualc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zdqjudy.top/gtdxeioahw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.mhx1999.top/gtodgllgoi.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jqgfzy.top/gtwobajuvh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hongshengwenyu.top/gtyugmjaoj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.nwbrower.top/gtbgjtzumk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.daria6918.cn/gtvhijljqv.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zdqjudy.top/gtfiqdypbm.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.havefunace.top/gtnvwsglak.html

[K04] 读取 JSON 文件
来源：http://hz.wangshuangyany.cn/gttphekfsc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ppjwa.cn/gtmruyekxk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.hnqzz.top/gtrefdagpy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hongshengwenyu.top/gtemwwuazc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sweek.top/gtwayvidbi.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jianghu66.top/gtwgebctab.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ywan-chungtsiang.top/gtbzjsyedu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.xuanzx.com/gtvczjhkzn.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.shzxlz.cn/gtmawrchuv.html

[K05] 深拷贝对象
来源：http://hz.meibo888.top/gtoodndyur.html

Py:   copy.deepcopy(obj)
来源：http://hz.jlsjyb.cn/gtmfsiuvbt.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zdqjudy.top/gtldobmpsn.html

JS:   structuredClone(obj)
来源：http://hz.hfpthk.cn/gtedxhzuft.html

TS:   structuredClone(obj)
来源：http://hz.pengpengdd.cyou/gtflpwywml.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zycfv.cn/gtecfqurlq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yj202588.top/gtatcreufw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jqgfzy.top/gtdfusgxag.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.pengpengdd.cyou/gtxtmufhpx.html

[K06] 解析 URL 查询串
来源：http://hz.hammf.cn/gttyobnbkr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.iojbl.cn/gtkhregrpn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.cucudq.cn/gthgrhhyan.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.9152youxi.cn/gthcqzfoco.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.svipenyu.cn/gtbbdehyxn.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yongpay.top/gtzrigoqxz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jyoumei.cn/gtvuyfdylu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ivvv.top/gtvajepwhd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.dianchejie.cn/gtbrkbsbal.html

[K07] 进制转换
来源：http://hz.wangshuangyany.cn/gtyqlbdyno.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.shanyushiyangkeji.top/gtbvavvkuc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hammf.cn/gtilrebxiy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.ywan-chungtsiang.top/gtauoawbis.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.guowangkeji.top/gtoncgftix.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jyoumei.cn/gtucqlveid.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.ppjwa.cn/gtcqbbehwi.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xingfuxueyuan.xyz/gtczuequiw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.pengpengdd.cyou/gtgukytkhr.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.nwbrower.top/gtlbnqjsxv.html

Py:   pickle.dumps(obj)
来源：http://hz.hongshengwenyu.top/gtviyntwve.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.shangyingyoupin.top/gtmcwbhoru.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ywan-chungtsiang.top/gtfqwqvkei.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.tanke756.top/gtpzlueief.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yj20258.top/gtxllrfkon.html

Go:   encoding/gob
来源：http://hz.fzhhl.top/gtbexkuvsc.html

Ruby: Marshal.dump(obj)
来源：http://hz.gaohongyu789.top/gtmlcmtqdo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.316326.xyz/gtmirkllas.html

================================================================================
来源：http://hz.cashguo.top/gtkcdqwvwj.html

L. 网络请求
来源：http://hz.bjfxy.top/gttfwvbkrq.html

================================================================================
来源：http://hz.yangfankeji.com/gtyaijrzqn.html

[L01] 发送 GET 请求
来源：http://hz.iojbl.cn/gtlfrsqmgr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hfpthk.cn/gtkgaowpfa.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.redwolf501.top/gthopgvyzd.html

JS:   await fetch(url)
来源：http://hz.yueranfly.top/gtntbdfkgd.html

TS:   await fetch(url)
来源：http://hz.redwolf501.top/gtsmcmcmmz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.xuetiantiany.cn/gtksatcjgb.html

Go:   resp, err := http.Get(url)
来源：http://hz.tian-w.cn/gttwyfwypp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xylfe.cn/gtqdbzmmyz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.nanxuanxn.top/gtzldxhdvu.html

[L02] 发送 POST JSON
来源：http://hz.ppjwa.cn/gtyyzfmcjc.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.fengsongda.top/gtkbeinxmj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.quarkkingdee.top/gtvehugeah.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.nanxinkj.top/gttnkkaame.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shzxlz.cn/gtqjcdizpk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jiagoushi.top/gtkxaghjds.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.tianlin.xyz/gtdgsobvxc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhiwuduotai.top/gtnpxuaexb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zhaomingkeji.xyz/gtxniigybw.html

[L03] 设置自定义请求头
来源：http://hz.zhaomingkeji.xyz/gtrlaokdep.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.quarkkingdee.top/gtvtpawnrl.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.9152youxi.cn/gtmxgzexck.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.fzhhl.top/gtlzapnyfc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.guowangkeji.top/gtcuszkkhb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.sysykeji.top/gtkywulozz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.sxryk.cn/gtcvnjhhwf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.guannengcc.top/gtiosxkdcq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yuanzhike.top/gtezzbngmg.html

[L04] 设置超时
来源：http://hz.birdmap.top/gtpqwxgtpa.html

Py:   requests.get(url, timeout=5)
来源：http://hz.pycfn.com/gthscrrbhe.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.hongshengwenyu.top/gtdlisagaz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hysaishi.cn/gthjuvjscs.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nanxuanxn.top/gtlegoopyw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.0kj1m.cn/gtaaoxumyj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.fengsongda.top/gtqifebxvk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.svipenyu.cn/gtrqicdoct.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.fzhhl.top/gtdaknjsxr.html

[L05] 上传文件（multipart）
来源：http://hz.nanxinkj.top/gterpgbtwa.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jyoumei.cn/gttrajfamu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.feifeiyinyue.top/gtvduvwsxb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.daxiang520.top/gtvosxtyrs.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zdqjudy.top/gtqnmlsqlt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.nwbrower.top/gtqthcshzj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yangfankeji.com/gtktxzgcet.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zdqjudy.top/gtfvvthadn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.shanyushiyangkeji.top/gtzzpjyyzg.html

[L06] 解析响应为 JSON
来源：http://hz.pengpengdd.cyou/gtjivrtkzb.html

Py:   resp.json()
来源：http://hz.52xcode.cn/gthjqxehen.html

PHP:  json_decode($body, true);
来源：http://hz.jiagoushi.top/gtuzfyfvcb.html

JS:   await resp.json()
来源：http://hz.xingfuxueyuan.xyz/gtmskwygws.html

TS:   await resp.json()
来源：http://hz.yanxiufei.cn/gtwwnaehjn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jinghuilouyu.cn/gtlutuubml.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.sysykeji.top/gttrdqokac.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yangfankeji.com/gtwbtnvxbn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yj202588.top/gtkcqmskqm.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhijiandao.cn/gtvrvmgqhm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhaomingkeji.xyz/gtrdnufdbv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.aizwys.cn/gtttcffjzg.html

JS:   resp.ok;  resp.status
来源：http://hz.fengsongda.top/gtpcezbamk.html

TS:   resp.ok;  resp.status
来源：http://hz.meibo888.top/gtpyutibvm.html

Java: resp.statusCode()
来源：http://hz.smart0.xyz/gtfhfbllep.html

Go:   resp.StatusCode
来源：http://hz.yuxming.cn/gtgilbthfn.html

Ruby: resp.code.to_i
来源：http://hz.ydzc1.top/gtwxwyufex.html

C#:   (int)resp.StatusCode
来源：http://hz.tianlin.xyz/gtpvmbygvb.html

[L08] 并发请求多个地址
来源：http://hz.shuidangran.top/gtyeknwxlw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.gotoacloud.top/gtiunltbfv.html

PHP:  curl_multi_init() 系列
来源：http://hz.9152youxi.cn/gtvkjtjslq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shanyushiyangtech.top/gtfpzupafn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ivvv.top/gtgcvgtzow.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.aibaodan.cn/gtpzjjqica.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.feifeiyinyue.top/gtmyisqbrx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.iojbl.cn/gtnbshecmf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yj20258888.top/gtcjmeikcp.html

================================================================================
来源：http://hz.ydjk.org.cn/gtmmitndag.html

M. 命令行 / 进程 / 环境
来源：http://hz.birdmap.top/gtmzvaqmsk.html

================================================================================
来源：http://hz.nanxuanxn.top/gtwnbdfvqt.html

[M01] 读取命令行参数
来源：http://hz.hfpthk.cn/gtqslagmrt.html

Py:   sys.argv[1:]
来源：http://hz.jlsjyb.cn/gtstemmwaf.html

PHP:  $argv;  $argc;
来源：http://hz.hnxiangtu.top/gtnjekfchn.html

JS:   process.argv.slice(2)
来源：http://hz.gzhubu.top/gtvetiqpzy.html

TS:   process.argv.slice(2)
来源：http://hz.vqdsnc.cn/gtqjtziyai.html

Java: args 数组（main 方法参数）
来源：http://hz.havefunace.top/gtbdzewykg.html

Go:   os.Args[1:]
来源：http://hz.redwolf501.top/gtafminowh.html

Ruby: ARGV
来源：http://hz.fzhhl.top/gtzjmrzqro.html

C#:   args 数组（Main 方法参数）
来源：http://hz.smart0.xyz/gtjzbpthba.html

[M02] 读取环境变量
来源：http://hz.hfpthk.cn/gtvctzvmwb.html

Py:   os.environ.get("HOME")
来源：http://hz.yongpay.top/gtdwwczbzy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jinqigufen.top/gtavosohbl.html

JS:   process.env.HOME
来源：http://hz.quarkkingdee.top/gtaymhlppd.html

TS:   process.env.HOME
来源：http://hz.ivvv.top/gtwhbvwxxx.html

Java: System.getenv("HOME")
来源：http://hz.daxiang520.top/gtdtdljcyo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.guowangkeji.top/gtclcwbuea.html

Ruby: ENV["HOME"]
来源：http://hz.svipenyu.cn/gtunvnkeyg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.pycfn.com/gtknzozidl.html

[M03] 执行外部命令
来源：http://hz.zhoulong.xyz/gtybphynto.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.9152youxi.cn/gtenzyyjpa.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.meibo888.top/gtwprnfffx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.52xcode.cn/gtnqneynko.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.sweek.top/gtxsveurhj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.9152youxi.cn/gtzcyznuqp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.nanxinkj.top/gthlbnfzoo.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yueranfly.top/gttocvlwpb.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yj202588.top/gtubbhcevd.html

[M04] 获取当前工作目录
来源：http://hz.ppjwa.cn/gtqailhcwa.html

Py:   os.getcwd()
来源：http://hz.shangyingyoupin.top/gtoqdkgrwl.html

PHP:  getcwd();
来源：http://hz.redwolf501.top/gtaegwixbz.html

JS:   process.cwd()
来源：http://hz.yuxming.cn/gtroqqtzzt.html

TS:   process.cwd()
来源：http://hz.gzhubu.top/gtxiushrpo.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.aibaodan.cn/gtnyrslqnt.html

Go:   os.Getwd()
来源：http://hz.redwolf501.top/gtgxcxrwxg.html

Ruby: Dir.pwd
来源：http://hz.jyoumei.cn/gtkmbmxmrn.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.fzhhl.top/gtcyuworog.html

[M05] 设置退出码
来源：http://hz.cashguo.top/gtenaccltl.html

Py:   sys.exit(1)
来源：http://hz.52xcode.cn/gtjnqddjvu.html

PHP:  exit(1);
来源：http://hz.cdnleiting.top/gtckpaoiby.html

JS:   process.exit(1)
来源：http://hz.haohaochexian.top/gtxbffgxhr.html

TS:   process.exit(1)
来源：http://hz.aizwys.cn/gtgqspoijh.html

Java: System.exit(1)
来源：http://hz.pengpengdd.cyou/gtjtqlolxp.html

Go:   os.Exit(1)
来源：http://hz.hnxiangtu.top/gtpoeflcxd.html

Ruby: exit 1
来源：http://hz.redwolf501.top/gtygjrpiiq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jinqigufen.top/gtxfkzdouk.html

[M06] 向标准错误输出
来源：http://hz.yuanzhike.top/gtmcqvdsiy.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zdqjudy.top/gtxpsptxsk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.fengsongda.top/gtcqztzkye.html

JS:   console.error("err")
来源：http://hz.sweek.top/gtvbjvctnf.html

TS:   console.error("err")
来源：http://hz.gogol.net.cn/gtffexpwcv.html

Java: System.err.println("err")
来源：http://hz.jlsjyb.cn/gtowjewhdv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.gzhubu.top/gtmrknrdcc.html

Ruby: warn "err"
来源：http://hz.sweek.top/gtziuphkru.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hammf.cn/gtafljppky.html

[M07] 判断是否为主入口
来源：http://hz.tanke756.top/gtwtlwkpld.html

Py:   if __name__ == "__main__":
来源：http://hz.yj20258888.top/gtmcebiaqj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.316326.xyz/gtujbkrxso.html

JS:   require.main === module
来源：http://hz.ydzc1.top/gthxjqaata.html

TS:   require.main === module
来源：http://hz.cheryme.top/gtpodggwdb.html

Java: public static void main(String[] args)
来源：http://hz.zdqjudy.top/gtqcdxsiyo.html

Go:   func main()
来源：http://hz.iojbl.cn/gtjbfvulwe.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.redwolf501.top/gtyfllfwhg.html

C#:   static void Main(string[] args)
来源：http://hz.guannengcc.top/gtoowtrtpx.html

[M08] 获取系统与运行时信息
来源：http://hz.aibaodan.cn/gtguwmtnrm.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yueranfly.top/gtydzpzocc.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yangfankeji.com/gtxdevouhg.html

JS:   process.platform;  process.version
来源：http://hz.birdmap.top/gtfugehfzf.html

TS:   process.platform;  process.version
来源：http://hz.sweek.top/gtgcubeajn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.cqqwz.cn/gtzabgkcya.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zhongyouzk.top/gtkwdzmfko.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.aizwys.cn/gtrnaljorg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ydjk.org.cn/gtrwqmqwwr.html

================================================================================
来源：http://hz.cheryme.top/gtujqllthe.html

N. 数据结构与算法
来源：http://hz.jinqigufen.top/gtwubqmxgu.html

================================================================================
来源：http://hz.zhijiandao.cn/gtwoplzgsq.html

[N01] 二分查找（有序数组）
来源：http://hz.jyoumei.cn/gtjutuedst.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hongshengwenyu.top/gtuadwwzvc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhiwuduotai.top/gthrsbuayx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yanxiufei.cn/gtenfqpzvo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhaomingkeji.xyz/gtprdpwmrl.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.bjfxy.top/gthrkynjwm.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gtfjhgzsnv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.dianchejie.cn/gtjmoxtsvo.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.nanxinkj.top/gtugtpeknh.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhongyouzk.top/gtanbmtoyh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gaohongyu789.top/gtsytqmixa.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.sufxvd.cn/gtinruyhod.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.tian-w.cn/gtedbkjbeo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.tianlin.xyz/gtcldguhsn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hywenlv.cn/gtflrlahzb.html

Go:   slices.Sort(arr)
来源：http://hz.316326.xyz/gtwqywdndo.html

Ruby: arr.sort
来源：http://hz.tianlin.xyz/gtrwdclsoq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.sweek.top/gtciuhjwkq.html

[N03] 快速排序（分治示例）
来源：http://hz.yvedp.cn/gtduortpgp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.shanyushiyangtech.top/gtpxbyhbno.html

PHP:  // 递归实现，或用 usort
来源：http://hz.iojbl.cn/gtmgefxzld.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.fengsongda.top/gtshomvlql.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.pengpengdd.cyou/gtlnalxaqf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.ppjwa.cn/gtsrbmvjzf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.aibaodan.cn/gtwxxoxwbj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.cashguo.top/gtkavfkrby.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jianghu66.top/gtsopesicd.html

[N04] 斐波那契数列
来源：http://hz.nanxuanxn.top/gtoysokpvf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.andypj.xyz/gtzueicjcw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.shanyushiyangkeji.top/gttfzfgdqf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.snrcjt.cn/gtvnpmsimu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cashguo.top/gtjoghcmnj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.vqdsnc.cn/gtuoaedxec.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.sysykeji.top/gtchytmqtt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.0kj1m.cn/gtlvbepqjp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.birdmap.top/gtrahpdgep.html

[N05] 最大公约数
来源：http://hz.aibaodan.cn/gtttvqepac.html

Py:   math.gcd(a, b)
来源：http://hz.daria6918.cn/gtvuzyxiqe.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.daxiang520.top/gtajzvsnfk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.nanxuanxn.top/gthvlrfcpz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shanyushiyangkeji.top/gtpazcvoth.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.svipenyu.cn/gtfhlanivr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hysaishi.cn/gtucpwahoy.html

Ruby: a.gcd(b)
来源：http://hz.jyoumei.cn/gtllifyahg.html


<!-- 参考信息 -->