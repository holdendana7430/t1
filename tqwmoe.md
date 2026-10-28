代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hnqzz.top/gtgjaxpmzk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yuanzhike.top/gtlsmyjeww.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.quarkkingdee.top/gtegwzfkhq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.xinyue.icu/gtnqwsctxb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.sxryk.cn/gttxvgcvcc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jqgufenzy.top/gthxqhrwno.html

[J09] 时区处理
来源：http://hz.tanke756.top/gtdfetncsk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jyoumei.cn/gtfaxihbrk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.svipenyu.cn/gtomuiruqw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nanxuanxn.top/gtrqsnkgtf.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.fengsongda.top/gtraacmfzs.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jinqigfzy.top/gtnnsozero.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jqgufenzy.top/gtbbhwbsem.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jinqigfzy.top/gtxkzzefeg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.sweek.top/gtpenilxtx.html

[J10] 取今天 / 本月第一天
来源：http://hz.cheryme.top/gtzppmypey.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.meibo888.top/gtnkdqxpix.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.shanyushiyangtech.top/gtnixiohrc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.gaohongyu789.top/gtvzwjcouv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ybcxt.top/gtvsuarfyk.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shzxlz.cn/gthcnkpunn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhengqikj.top/gtlurbaezp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jqgfzy.top/gtabplcpew.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.meibo888.top/gtqpmoqjbi.html

================================================================================
来源：http://hz.jinqigufen.top/gttxziotge.html

K. JSON 与序列化
来源：http://hz.c1oappe.top/gtadrexmvn.html

================================================================================
来源：http://hz.jiagoushi.top/gtwqpuebqa.html

[K01] 对象转 JSON 字符串
来源：http://hz.tian-w.cn/gtlcsrswux.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zhaomingkeji.xyz/gtbaluxyah.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.haohaochexian.top/gtucxfgwvl.html

JS:   JSON.stringify(obj)
来源：http://hz.wangshuangyany.cn/gtigkjtmxq.html

TS:   JSON.stringify(obj)
来源：http://hz.52xcode.cn/gtrktztzuo.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.shzxlz.cn/gtjxymowks.html

Go:   json.Marshal(obj)
来源：http://hz.quarkkingdee.top/gtlanzlois.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hywenlv.cn/gtgcbtqtgl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.vqdsnc.cn/gtzejrjtqq.html

[K02] JSON 字符串转对象
来源：http://hz.tian-w.cn/gtnnlewtut.html

Py:   json.loads(s)
来源：http://hz.feifeiyinyue.top/gtbypmpfrb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.shanyushiyangkeji.top/gtedqngemi.html

JS:   JSON.parse(s)
来源：http://hz.dashuyun.cn/gtnvpgtbez.html

TS:   JSON.parse(s)
来源：http://hz.svipenyu.cn/gtzxnvetxp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhengqikj.top/gtrkcusmoz.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.smart0.xyz/gtyhmopcrx.html

Ruby: JSON.parse(s)
来源：http://hz.gaohongyu789.top/gtrwvrgdhq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hnxiangtu.top/gtolzmlupg.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.nanxuanxn.top/gtvdbaxkrr.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.c1oappe.top/gtvrqdvrde.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.snrcjt.cn/gtepkeqnmo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.daria6918.cn/gtnextgzlm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cqqwz.cn/gtinfbjgqu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.bjfxy.top/gtbshwbrsk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yonumen.top/gtrwjbuomw.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jinyuanbaomall.cn/gticeawpol.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hnxiangtu.top/gtaqgrhagz.html

[K04] 读取 JSON 文件
来源：http://hz.yanxiufei.cn/gtpxnuuhcf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.cashguo.top/gtliuoijen.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yangfankeji.com/gtvfityycc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.quarkkingdee.top/gtismvhxkn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yangfankeji.com/gtdglwnfng.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.xylfe.cn/gtobcazozc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.meibo888.top/gthtgjdnfc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.guannengcc.top/gtxldniwdh.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yongpay.top/gtyihlsocx.html

[K05] 深拷贝对象
来源：http://hz.haohaochexian.top/gtbgkdoqna.html

Py:   copy.deepcopy(obj)
来源：http://hz.sufxvd.cn/gtrlirobms.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hfpthk.cn/gtqevdspgt.html

JS:   structuredClone(obj)
来源：http://hz.hywenlv.cn/gtztfuykmu.html

TS:   structuredClone(obj)
来源：http://hz.ydjk.org.cn/gtqufgiqwm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yueranfly.top/gtdpqbxcsf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.sweek.top/gththhthiy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ivvv.top/gtpbgwkabk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.0kj1m.cn/gtecwokrcv.html

[K06] 解析 URL 查询串
来源：http://hz.chenzaomai.com/gtjnupgpdt.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.wangdashe.top/gtspckdnrv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.nwbrower.top/gtzezstweg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhongyouzk.top/gtxpgtpyfb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.dianchejie.cn/gtthqijxib.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jqgufenzy.top/gtrfmvhixf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.daxiang520.top/gtxdqaeqdc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.sufxvd.cn/gtvzqvidxo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.nanxinkj.top/gtokocesui.html

[K07] 进制转换
来源：http://hz.guannengcc.top/gtscnvsvxp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yuanzhike.top/gtzfhazmtc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hongshengwenyu.top/gtvgdnphds.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.pycfn.com/gtbvbgwkgz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.nanxinkj.top/gtgeggonhs.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hongshengwenyu.top/gtrpdhlrpq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.ydzc1.top/gteldmlxey.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.hammf.cn/gtwjtkhcjm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xuetiantiany.cn/gtazmehypm.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.meibo888.top/gtfvcdhdvf.html

Py:   pickle.dumps(obj)
来源：http://hz.snrcjt.cn/gtyjxzdbqv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jqgufenzy.top/gtyhmyiopr.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shangyingyoupin.top/gtxsuuewht.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hongshengwenyu.top/gtczlrtjxu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhoulong.xyz/gtyohtytsz.html

Go:   encoding/gob
来源：http://hz.havefunace.top/gtaoqtctjy.html

Ruby: Marshal.dump(obj)
来源：http://hz.yangfankeji.com/gtxxluqhio.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.dashuyun.cn/gtirvozdkj.html

================================================================================
来源：http://hz.zhongyouzk.top/gtokjtimtm.html

L. 网络请求
来源：http://hz.gogol.net.cn/gtltvvausc.html

================================================================================
来源：http://hz.316326.xyz/gtjmkiaovo.html

[L01] 发送 GET 请求
来源：http://hz.cdnleiting.top/gtnsanhnvl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yongpay.top/gtwnbuiyeh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.pycfn.com/gtcrfriqxd.html

JS:   await fetch(url)
来源：http://hz.sysykeji.top/gttcxcssbt.html

TS:   await fetch(url)
来源：http://hz.316326.xyz/gtidcudyah.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.svipenyu.cn/gtbiiehypp.html

Go:   resp, err := http.Get(url)
来源：http://hz.guannengcc.top/gtkemkkeif.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.ppjwa.cn/gtixbwxlgl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.tianlin.xyz/gtscxvalbp.html

[L02] 发送 POST JSON
来源：http://hz.cucudq.cn/gtotlwvaee.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhiwuduotai.top/gttaozcjcr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yuxming.cn/gtipvsjmem.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sweek.top/gtpjibewoy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.birdmap.top/gtqqdlpoor.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.52xcode.cn/gtwhxlerla.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.316326.xyz/gthvpjaxsw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jianghu66.top/gtenvdqftz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.aizwys.cn/gtrgtbyuqz.html

[L03] 设置自定义请求头
来源：http://hz.chenjidiqi.icu/gtwfitkszh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.iojbl.cn/gtbnbwxtep.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yongpay.top/gtrydpfrsz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhongyouzk.top/gtqhlaefez.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jyoumei.cn/gtyedcchki.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.feifeiyinyue.top/gtvpnxiuvg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.sysykeji.top/gtbdulrjwg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhijiandao.cn/gtakwrnxhd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhoulong.xyz/gtodiedrjv.html

[L04] 设置超时
来源：http://hz.bjfxy.top/gttqrdytbd.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zhixingplan.top/gtvglvloio.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yj20258888.top/gtgkrxcdvk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.tian-w.cn/gtqgtmioul.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.haohaochexian.top/gtcknobgoe.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.shangyingyoupin.top/gthsygouwt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jyoumei.cn/gtcwuplxpi.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.haohaochexian.top/gtyigwamvx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yj20258888.top/gtluajutei.html

[L05] 上传文件（multipart）
来源：http://hz.fengsongda.top/gtaylekqce.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhaomingkeji.xyz/gtacstyuob.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jinyuanbaomall.cn/gtsfcapxmz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.feifeiyinyue.top/gtebqebsfg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yuxming.cn/gtaglsejja.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.bjfxy.top/gtlcxuoubo.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.aizwys.cn/gttfvevmql.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.cucudq.cn/gtcxkzrvah.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yongpay.top/gtfmdkjgtd.html

[L06] 解析响应为 JSON
来源：http://hz.yanxiufei.cn/gtztrkvcfe.html

Py:   resp.json()
来源：http://hz.redwolf501.top/gttrdkhuer.html

PHP:  json_decode($body, true);
来源：http://hz.pycfn.com/gtsjunqwrb.html

JS:   await resp.json()
来源：http://hz.sysykeji.top/gtgdihmepg.html

TS:   await resp.json()
来源：http://hz.haohaochexian.top/gtahmccnkb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.ehwqpu.com/gtpmqjhlhc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.ivvv.top/gtnsznnaog.html

Ruby: JSON.parse(resp.body)
来源：http://hz.9152youxi.cn/gtpzpnoojj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.xuetiantiany.cn/gtgfozlidf.html

[L07] 处理 HTTP 状态码
来源：http://hz.tanke756.top/gtiezcyuvc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.vqdsnc.cn/gtujcrtxvt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jinyuanbaomall.cn/gtvlbfmwlr.html

JS:   resp.ok;  resp.status
来源：http://hz.gogol.net.cn/gtubcjhsql.html

TS:   resp.ok;  resp.status
来源：http://hz.cqqwz.cn/gtmdpegnde.html

Java: resp.statusCode()
来源：http://hz.wangdashe.top/gtndkpfwpa.html

Go:   resp.StatusCode
来源：http://hz.hnxiangtu.top/gtjdrhuufb.html

Ruby: resp.code.to_i
来源：http://hz.hammf.cn/gtjmdkksrv.html

C#:   (int)resp.StatusCode
来源：http://hz.yvedp.cn/gtaumsgznt.html

[L08] 并发请求多个地址
来源：http://hz.ywan-chungtsiang.top/gtdpsbbtbj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.xylfe.cn/gtmmrhjmzi.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhongyouzk.top/gtcfqsverd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.svipenyu.cn/gtafuwldik.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shuidangran.top/gtennrzttu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.wangdashe.top/gtltjqgtjm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hammf.cn/gtipcrlnoc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jlsjyb.cn/gtvofthfoy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jqgfzy.top/gtzubuejqp.html

================================================================================
来源：http://hz.tianlin.xyz/gtiqqqcfpt.html

M. 命令行 / 进程 / 环境
来源：http://hz.c1oappe.top/gttzzjkzqs.html

================================================================================
来源：http://hz.sxryk.cn/gtllvjmbwn.html

[M01] 读取命令行参数
来源：http://hz.bjfxy.top/gtjaxwcooq.html

Py:   sys.argv[1:]
来源：http://hz.xylfe.cn/gtvuwibuea.html

PHP:  $argv;  $argc;
来源：http://hz.quarkkingdee.top/gtgvlnkhnt.html

JS:   process.argv.slice(2)
来源：http://hz.meibo888.top/gtsxinrzrj.html

TS:   process.argv.slice(2)
来源：http://hz.chenlongwang.top/gtlsdaswqx.html

Java: args 数组（main 方法参数）
来源：http://hz.chenzaomai.com/gtaovnvyar.html

Go:   os.Args[1:]
来源：http://hz.zhongyouzk.top/gtndugzetf.html

Ruby: ARGV
来源：http://hz.yueranfly.top/gthbyylhww.html

C#:   args 数组（Main 方法参数）
来源：http://hz.aibaodan.cn/gtfowrgglo.html

[M02] 读取环境变量
来源：http://hz.yangfankeji.com/gtdhleniyo.html

Py:   os.environ.get("HOME")
来源：http://hz.gaohongyu789.top/gtnkcfzxfl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.svipenyu.cn/gtqfisdrzh.html

JS:   process.env.HOME
来源：http://hz.jinyuanbaomall.cn/gtezfngkdh.html

TS:   process.env.HOME
来源：http://hz.yvedp.cn/gtrgfjlbhz.html

Java: System.getenv("HOME")
来源：http://hz.gotoacloud.top/gtkmjxcjyc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yj20258888.top/gtmrneduhy.html

Ruby: ENV["HOME"]
来源：http://hz.yvedp.cn/gtcwcberkj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.0kj1m.cn/gtqgpnysgi.html

[M03] 执行外部命令
来源：http://hz.tanke756.top/gtwubhhfsn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.cheryme.top/gtyoubkbuy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.c1oappe.top/gtfcdoxtli.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.dashuyun.cn/gtiqgrvhvp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yuxming.cn/gtkbtthsti.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.dianchejie.cn/gteyteynkw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.daxiang520.top/gtxtjnbcwy.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.haohaochexian.top/gtuontfgwv.html

C#:   Process.Start("ls", "-l");
来源：http://hz.mhx1999.top/gtkabgbfbs.html

[M04] 获取当前工作目录
来源：http://hz.zhoulong.xyz/gtqwuvqudh.html

Py:   os.getcwd()
来源：http://hz.jlsjyb.cn/gtibroysst.html

PHP:  getcwd();
来源：http://hz.nwbrower.top/gtzwsezjfd.html

JS:   process.cwd()
来源：http://hz.ydzc1.top/gtforvhinl.html

TS:   process.cwd()
来源：http://hz.jiagoushi.top/gtcqjfzhdt.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.fzhhl.top/gtbqrjghsg.html

Go:   os.Getwd()
来源：http://hz.snrcjt.cn/gttakaonfo.html

Ruby: Dir.pwd
来源：http://hz.redwolf501.top/gtvobiojyi.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jinyuanbaomall.cn/gtmwilfgxd.html

[M05] 设置退出码
来源：http://hz.hysaishi.cn/gtgzlrgibk.html

Py:   sys.exit(1)
来源：http://hz.ehwqpu.com/gteagurmiy.html

PHP:  exit(1);
来源：http://hz.yuanzhike.top/gtqenxvqov.html

JS:   process.exit(1)
来源：http://hz.mhx1999.top/gtaeffrinr.html

TS:   process.exit(1)
来源：http://hz.yangfankeji.com/gttqchltgr.html

Java: System.exit(1)
来源：http://hz.yj20258888.top/gtrpikpygb.html

Go:   os.Exit(1)
来源：http://hz.xinyue.icu/gtjhhmrvec.html

Ruby: exit 1
来源：http://hz.jyoumei.cn/gtnccurqow.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yj20258.top/gtszjcmwok.html

[M06] 向标准错误输出
来源：http://hz.aibaodan.cn/gtoquodqzg.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jqgufenzy.top/gtycjbxpky.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.redwolf501.top/gtdvcbvmnm.html

JS:   console.error("err")
来源：http://hz.jinqigufen.top/gtqgsicxzm.html

TS:   console.error("err")
来源：http://hz.chenlongwang.top/gtxozohfzx.html

Java: System.err.println("err")
来源：http://hz.ivvv.top/gtwvhmdxly.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yvedp.cn/gtsughorbj.html

Ruby: warn "err"
来源：http://hz.kuanghao11.cn/gtlfnptszl.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ydzc1.top/gtdpkiirjb.html

[M07] 判断是否为主入口
来源：http://hz.dashuyun.cn/gtcszezvdt.html

Py:   if __name__ == "__main__":
来源：http://hz.yongpay.top/gttfshhznu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cucudq.cn/gthzzusdqw.html

JS:   require.main === module
来源：http://hz.yvedp.cn/gtwdicjisa.html

TS:   require.main === module
来源：http://hz.tanke756.top/gtjxekgfda.html

Java: public static void main(String[] args)
来源：http://hz.jqgfzy.top/gtoqowmdvs.html

Go:   func main()
来源：http://hz.aizwys.cn/gtnzerroup.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.nanxuanxn.top/gtucvoulzc.html

C#:   static void Main(string[] args)
来源：http://hz.ehwqpu.com/gtrtufelna.html

[M08] 获取系统与运行时信息
来源：http://hz.nwbrower.top/gthbffghsx.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hnqzz.top/gtkkmtacfv.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.shanyushiyangkeji.top/gtvjgwhqxj.html

JS:   process.platform;  process.version
来源：http://hz.hnxiangtu.top/gtlyqvthpx.html

TS:   process.platform;  process.version
来源：http://hz.ivvv.top/gthziqvupb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.cucudq.cn/gttlthkbal.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zhijiandao.cn/gtsgidmhps.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.tianlin.xyz/gtqwpmqbld.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhengqikj.top/gtbgbklrpn.html

================================================================================
来源：http://hz.quarkkingdee.top/gtxhuhtkce.html

N. 数据结构与算法
来源：http://hz.yj20258888.top/gtospapvgo.html

================================================================================
来源：http://hz.zdqjudy.top/gtwtvkzvet.html

[N01] 二分查找（有序数组）
来源：http://hz.fengsongda.top/gtxuriwpmf.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.shuidangran.top/gtbqxubjyg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.nanxuanxn.top/gttubpffgn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.chenzaomai.com/gtrwdihfwh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.pengpengdd.cyou/gtqtqhnfdw.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.snrcjt.cn/gtbtfvhizq.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.316326.xyz/gtmbtlthyg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.0kj1m.cn/gtcosvmqeg.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.guowangkeji.top/gtmqlgkrlt.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.xylfe.cn/gtyfvsfqfc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gaohongyu789.top/gtufcgcfru.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.aibaodan.cn/gtaximtpxb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.316326.xyz/gtqbwtpzgf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.guannengcc.top/gtzlelxewv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.quarkkingdee.top/gtxtmfoyws.html

Go:   slices.Sort(arr)
来源：http://hz.nwbrower.top/gttxspbnza.html

Ruby: arr.sort
来源：http://hz.xziqi.cn/gtfagzyzaj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zdqjudy.top/gtvycrvavm.html

[N03] 快速排序（分治示例）
来源：http://hz.xuanzx.com/gtsllewxcl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xuetiantiany.cn/gtjlqqwake.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yj202588.top/gtsoyramng.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.haohaochexian.top/gtedvpmpwh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tanke756.top/gtluvstkep.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yueranfly.top/gtmcluagwz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yvedp.cn/gtrfzcdgbm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hnxiangtu.top/gtnfcxjfsu.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ppjwa.cn/gtgotjaxab.html

[N04] 斐波那契数列
来源：http://hz.zhongyouzk.top/gthunaanhh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yuxming.cn/gtvrccfnpj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.sxryk.cn/gtabacvmmu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhixingplan.top/gtrbxalvly.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.havefunace.top/gtohgulcke.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.hfpthk.cn/gtlypvgisn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.gogol.net.cn/gtliecxmal.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.shuidangran.top/gtxbzyxhmy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.havefunace.top/gtpfqorvmk.html

[N05] 最大公约数
来源：http://hz.ybcxt.top/gtnmdkcnav.html

Py:   math.gcd(a, b)
来源：http://hz.cheryme.top/gtsbygubqc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.dashuyun.cn/gtazdaswww.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.bjfxy.top/gtxqjkmsnl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zycfv.cn/gtcvqxymwe.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.fzhhl.top/gtwgzibhap.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.chenlongwang.top/gtdcmpavwd.html

Ruby: a.gcd(b)
来源：http://hz.gaohongyu789.top/gtiwzhblyp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jinqigufen.top/gtxxmpdbxg.html

[N06] 判断回文字符串
来源：http://hz.ydzc1.top/gtwpmbdzht.html

Py:   s == s[::-1]
来源：http://hz.feifeiyinyue.top/gtpudkeubw.html

PHP:  $s === strrev($s);
来源：http://hz.daxiang520.top/gtpydsvcex.html


<!-- 参考信息 -->