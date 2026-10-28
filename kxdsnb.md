代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhoulong.xyz/gtioqwzbhq.html

[J08] 提取年月日与星期
来源：http://hz.tanke756.top/gtssicolzj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.xuanzx.com/gtjssklqzs.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.ywan-chungtsiang.top/gtylpettap.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.wangshuangyany.cn/gtlyjkgfsf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yangfankeji.com/gtmibgvqlg.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhoulong.xyz/gtndofqnoy.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.c1oappe.top/gtkqhvhujc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xziqi.cn/gtrsaodzmc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.c1oappe.top/gtpesyjpcj.html

[J09] 时区处理
来源：http://hz.316326.xyz/gtzzkdgpkx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shzxlz.cn/gtyjscxfeb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.gzhubu.top/gtlpjepseh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zdqjudy.top/gtfdogwknp.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yanxiufei.cn/gtcbxbrqfc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.nanxuanxn.top/gtqrsjivis.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhengqikj.top/gtymlbgsbr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yvedp.cn/gtultugdps.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.havefunace.top/gtseikhsbr.html

[J10] 取今天 / 本月第一天
来源：http://hz.quarkkingdee.top/gtierlzdin.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.aizwys.cn/gtqhozowwf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xuanzx.com/gtjikevdrb.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yanxiufei.cn/gtcijlkpkv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.nwbrower.top/gthkckyuuj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.tian-w.cn/gtaiixhjri.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.sweek.top/gtmcxcxfal.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jlsjyb.cn/gtuoqmeqyz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.nwbrower.top/gtmmxycilc.html

================================================================================
来源：http://hz.chenzaomai.com/gtzdqmtuax.html

K. JSON 与序列化
来源：http://hz.xingfuxueyuan.xyz/gtegvcctxy.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtnqdbjcqb.html

[K01] 对象转 JSON 字符串
来源：http://hz.cdnleiting.top/gtljybvsgw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zhijiandao.cn/gtlgrapfym.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xuetiantiany.cn/gtbqhuavow.html

JS:   JSON.stringify(obj)
来源：http://hz.hammf.cn/gtzchiqdfz.html

TS:   JSON.stringify(obj)
来源：http://hz.cucudq.cn/gttzvkqrsv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yongpay.top/gtuyepursf.html

Go:   json.Marshal(obj)
来源：http://hz.nanxuanxn.top/gtwgprhkqn.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.fzhhl.top/gtbivhreeo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jlsjyb.cn/gtffiqnzbi.html

[K02] JSON 字符串转对象
来源：http://hz.iojbl.cn/gtmmdgkfhq.html

Py:   json.loads(s)
来源：http://hz.yongpay.top/gtrjcajydf.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.fengsongda.top/gtvhtykvap.html

JS:   JSON.parse(s)
来源：http://hz.cdnleiting.top/gthyurblun.html

TS:   JSON.parse(s)
来源：http://hz.shanyushiyangkeji.top/gtqkxpitjj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xinyue.icu/gtqqnxeosp.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhijiandao.cn/gthugwlxfp.html

Ruby: JSON.parse(s)
来源：http://hz.ppjwa.cn/gttgtwjzqt.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hysaishi.cn/gtowxfztqt.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.nanxuanxn.top/gtsrdbqgcb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.chenjidiqi.icu/gtxlqbqkue.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.andypj.xyz/gtwppdyrsy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.guowangkeji.top/gtotjazkob.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.nwbrower.top/gtwgjrfjne.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jqgufenzy.top/gtwwbovnzv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.52xcode.cn/gtbdtuqvcp.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hammf.cn/gtpjleqcae.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.havefunace.top/gthuhosksc.html

[K04] 读取 JSON 文件
来源：http://hz.yvedp.cn/gtzgmfzgac.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ydjk.org.cn/gtmjcyrbcf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.chenlongwang.top/gtzgkrfguk.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.aizwys.cn/gtnjprppeu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ppjwa.cn/gtygfafecr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.redwolf501.top/gtbbycnlob.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yangfankeji.com/gtrovcautv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.cqqwz.cn/gtjqasjaed.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jiagoushi.top/gtwqohptoa.html

[K05] 深拷贝对象
来源：http://hz.zhijiandao.cn/gtwpjzvwun.html

Py:   copy.deepcopy(obj)
来源：http://hz.gaohongyu789.top/gtnjyqwisz.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhijiandao.cn/gtcmkbmdzv.html

JS:   structuredClone(obj)
来源：http://hz.hfpthk.cn/gtsexvrwdm.html

TS:   structuredClone(obj)
来源：http://hz.jiagoushi.top/gtnalyomzj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ivvv.top/gtwvbxqanf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yueranfly.top/gtsrnjpslu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hammf.cn/gtdpvqplwh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.sxryk.cn/gtrxeywvmg.html

[K06] 解析 URL 查询串
来源：http://hz.yvedp.cn/gtanniakze.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.shzxlz.cn/gtdganauto.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zdqjudy.top/gtsexdedgo.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhoulong.xyz/gtmwfsnjbe.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yongpay.top/gtxmbwhiml.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.9152youxi.cn/gthnwzqbjd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.feifeiyinyue.top/gtpcwpaoyg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jqgufenzy.top/gtmrrjdpmz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.shuidangran.top/gtvtkbqwdz.html

[K07] 进制转换
来源：http://hz.sufxvd.cn/gtjrgzimbk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yvedp.cn/gtpqabwetx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhaomingkeji.xyz/gtawggvutz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.guannengcc.top/gtaicyfoue.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.snrcjt.cn/gtpmrhusra.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.snrcjt.cn/gtorqjhbop.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.snrcjt.cn/gtwazcodtg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.hnxiangtu.top/gtmdwmhtzk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.9152youxi.cn/gtyfzrwrzv.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.chenlongwang.top/gtmrgzdjwd.html

Py:   pickle.dumps(obj)
来源：http://hz.feifeiyinyue.top/gtmjhxlxiu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.haohaochexian.top/gtwyxnjikm.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.chenjidiqi.icu/gtlqjipqhj.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.gotoacloud.top/gtpuatroli.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hfpthk.cn/gtfqesszgb.html

Go:   encoding/gob
来源：http://hz.aibaodan.cn/gtufeblydh.html

Ruby: Marshal.dump(obj)
来源：http://hz.meibo888.top/gtsrpvqusl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xuetiantiany.cn/gtxudbflas.html

================================================================================
来源：http://hz.wangdashe.top/gtexxjzcch.html

L. 网络请求
来源：http://hz.bjfxy.top/gtuhrvvkja.html

================================================================================
来源：http://hz.ydjk.org.cn/gtbwdojfjv.html

[L01] 发送 GET 请求
来源：http://hz.svipenyu.cn/gtnerstdhs.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jinqigufen.top/gtgqevcrux.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.cucudq.cn/gtvnuijaka.html

JS:   await fetch(url)
来源：http://hz.ywan-chungtsiang.top/gtovzkezij.html

TS:   await fetch(url)
来源：http://hz.jqgufenzy.top/gttjqymuvg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jinghuilouyu.cn/gtfetqkvld.html

Go:   resp, err := http.Get(url)
来源：http://hz.yuanzhike.top/gtczethkss.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.ivvv.top/gtycufcnvb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.feifeiyinyue.top/gtvmxbwpiw.html

[L02] 发送 POST JSON
来源：http://hz.yuanzhike.top/gtfzqnkvag.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.dianchejie.cn/gtmhzuyktw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jiagoushi.top/gtikrnvclj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shangyingyoupin.top/gtxbsrwxqh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.c1oappe.top/gtnomhbrct.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.daxiang520.top/gtkkfbobwq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xziqi.cn/gtocrzczsg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.shzxlz.cn/gtoocbihfc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hysaishi.cn/gtvgegbxgx.html

[L03] 设置自定义请求头
来源：http://hz.quarkkingdee.top/gtymldbwtu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hongshengwenyu.top/gthmalnkop.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zhiwuduotai.top/gtlzudjcym.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gotoacloud.top/gtlksakhgh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhijiandao.cn/gtjrzxptqg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yvedp.cn/gtgmpqkwbe.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.c1oappe.top/gtfbkuyzdp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.xziqi.cn/gtpnhmqnpc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhongyouzk.top/gtnkdooafv.html

[L04] 设置超时
来源：http://hz.zhijiandao.cn/gtzblqldjq.html

Py:   requests.get(url, timeout=5)
来源：http://hz.iojbl.cn/gtfhowzwto.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.sweek.top/gtxsghnxnc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hfpthk.cn/gtlpaypeqe.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ehwqpu.com/gtuctnlcko.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yj20258.top/gtutyzojgj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.gzhubu.top/gtxjjvnqah.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.kuanghao11.cn/gthuxyenph.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.redwolf501.top/gtyrelqslt.html

[L05] 上传文件（multipart）
来源：http://hz.nwbrower.top/gtmpfggsod.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.shanyushiyangtech.top/gtsqcqtrdu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.cucudq.cn/gtlfylzhuo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hnqzz.top/gthsvivyge.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zdqjudy.top/gtdlggzlvt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.aibaodan.cn/gtiroymuhf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.haohaochexian.top/gtronustmy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.pengpengdd.cyou/gtwkkzdemv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.mhx1999.top/gtxougebvg.html

[L06] 解析响应为 JSON
来源：http://hz.chenlongwang.top/gtquitacnr.html

Py:   resp.json()
来源：http://hz.pengpengdd.cyou/gtbfqaanxx.html

PHP:  json_decode($body, true);
来源：http://hz.sxryk.cn/gtvwmgehdt.html

JS:   await resp.json()
来源：http://hz.jqgfzy.top/gtjlluuwgd.html

TS:   await resp.json()
来源：http://hz.havefunace.top/gtzkrobxeg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jqgufenzy.top/gtxkydldju.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.tian-w.cn/gtcxgshmci.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ydzc1.top/gthbzbewnh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jinyuanbaomall.cn/gtrkiwlpgh.html

[L07] 处理 HTTP 状态码
来源：http://hz.gzhubu.top/gtaijukxni.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.ehwqpu.com/gtttqrnkbn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.chenlongwang.top/gtzsqxucxh.html

JS:   resp.ok;  resp.status
来源：http://hz.zdqjudy.top/gtqlsjyzzi.html

TS:   resp.ok;  resp.status
来源：http://hz.daria6918.cn/gtmhumywwq.html

Java: resp.statusCode()
来源：http://hz.jinqigfzy.top/gtyasaqkyq.html

Go:   resp.StatusCode
来源：http://hz.shangyingyoupin.top/gtkrshikqg.html

Ruby: resp.code.to_i
来源：http://hz.iojbl.cn/gtmzhulixc.html

C#:   (int)resp.StatusCode
来源：http://hz.vqdsnc.cn/gtzkdddfgu.html

[L08] 并发请求多个地址
来源：http://hz.snrcjt.cn/gtdycrbrhn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ydzc1.top/gtjodkpjti.html

PHP:  curl_multi_init() 系列
来源：http://hz.guowangkeji.top/gtipcijnkn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.9152youxi.cn/gttjwhpkbc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yuxming.cn/gtlniqugqu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.tian-w.cn/gtlxnykeji.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yuxming.cn/gtdfelkcnj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jiagoushi.top/gtotipriza.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ydjk.org.cn/gtftahhizz.html

================================================================================
来源：http://hz.dianchejie.cn/gtblyqjbno.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhiwuduotai.top/gtlbzdadzj.html

================================================================================
来源：http://hz.daxiang520.top/gtmcsuwwfj.html

[M01] 读取命令行参数
来源：http://hz.hysaishi.cn/gtpygwmvcm.html

Py:   sys.argv[1:]
来源：http://hz.yj20258888.top/gtrcumhmmh.html

PHP:  $argv;  $argc;
来源：http://hz.iojbl.cn/gtetnwgiit.html

JS:   process.argv.slice(2)
来源：http://hz.xuanzx.com/gtledqdehf.html

TS:   process.argv.slice(2)
来源：http://hz.zhoulong.xyz/gtzilamlgi.html

Java: args 数组（main 方法参数）
来源：http://hz.jyoumei.cn/gtpkcnhsjd.html

Go:   os.Args[1:]
来源：http://hz.chenlongwang.top/gtjbqlvhcd.html

Ruby: ARGV
来源：http://hz.chenzaomai.com/gtlezesexn.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhaomingkeji.xyz/gthfowdapm.html

[M02] 读取环境变量
来源：http://hz.cheryme.top/gtmeofmufm.html

Py:   os.environ.get("HOME")
来源：http://hz.316326.xyz/gtqfaiuenp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.haohaochexian.top/gtbsffutjy.html

JS:   process.env.HOME
来源：http://hz.hongshengwenyu.top/gtfxqhoibz.html

TS:   process.env.HOME
来源：http://hz.sweek.top/gtgxlxfpoc.html

Java: System.getenv("HOME")
来源：http://hz.yuanzhike.top/gtelpnaboa.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.vqdsnc.cn/gtmrtggqhe.html

Ruby: ENV["HOME"]
来源：http://hz.jinqigufen.top/gtlksankfv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shzxlz.cn/gtxfihfibn.html

[M03] 执行外部命令
来源：http://hz.c1oappe.top/gtbhbrnzvt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xylfe.cn/gtfdsvwikz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jianghu66.top/gtierlqyvg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xuetiantiany.cn/gtdmqjdffo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinqigfzy.top/gtyatmpxda.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.9152youxi.cn/gtzzjolrfv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.wangshuangyany.cn/gtkychifss.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.dashuyun.cn/gtgdlwvktp.html

C#:   Process.Start("ls", "-l");
来源：http://hz.pengpengdd.cyou/gttlsizihy.html

[M04] 获取当前工作目录
来源：http://hz.tian-w.cn/gtrqlwjlzt.html

Py:   os.getcwd()
来源：http://hz.xylfe.cn/gtxbfiqtiv.html

PHP:  getcwd();
来源：http://hz.cheryme.top/gtowxbbqko.html

JS:   process.cwd()
来源：http://hz.gaohongyu789.top/gtvayzzvvz.html

TS:   process.cwd()
来源：http://hz.daxiang520.top/gtxbtftdke.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.quarkkingdee.top/gtfpqnhdwi.html

Go:   os.Getwd()
来源：http://hz.jinqigfzy.top/gtnmeaemgq.html

Ruby: Dir.pwd
来源：http://hz.guannengcc.top/gtdduswurr.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hnqzz.top/gtstvyzioi.html

[M05] 设置退出码
来源：http://hz.zhiwuduotai.top/gtsblbcqmg.html

Py:   sys.exit(1)
来源：http://hz.kuanghao11.cn/gtnlaroghw.html

PHP:  exit(1);
来源：http://hz.shzxlz.cn/gtztdrjtdc.html

JS:   process.exit(1)
来源：http://hz.yuxming.cn/gtwmokdfqt.html

TS:   process.exit(1)
来源：http://hz.smart0.xyz/gtktssojmc.html

Java: System.exit(1)
来源：http://hz.mhx1999.top/gthhhrpact.html

Go:   os.Exit(1)
来源：http://hz.cashguo.top/gtchczpihm.html

Ruby: exit 1
来源：http://hz.cucudq.cn/gtwrotoqds.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zhengqikj.top/gtkovozxwy.html

[M06] 向标准错误输出
来源：http://hz.ppjwa.cn/gtsvniwwjn.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yangfankeji.com/gtgcugijyj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.wangshuangyany.cn/gtpzaeyhir.html

JS:   console.error("err")
来源：http://hz.jinqigufen.top/gtisdutrdm.html

TS:   console.error("err")
来源：http://hz.yongpay.top/gtfqpbhhlv.html

Java: System.err.println("err")
来源：http://hz.gotoacloud.top/gtaxkgaagu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yvedp.cn/gtwpeaokjt.html

Ruby: warn "err"
来源：http://hz.zhixingplan.top/gtzrzimlfl.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.aibaodan.cn/gtnuzwsoiv.html

[M07] 判断是否为主入口
来源：http://hz.svipenyu.cn/gthdgzksjl.html

Py:   if __name__ == "__main__":
来源：http://hz.jqgfzy.top/gtdwjboycv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.wangdashe.top/gtbhjafouh.html

JS:   require.main === module
来源：http://hz.dianchejie.cn/gtruozbply.html

TS:   require.main === module
来源：http://hz.xziqi.cn/gtphxcnfcb.html

Java: public static void main(String[] args)
来源：http://hz.zhijiandao.cn/gtmtspkozy.html

Go:   func main()
来源：http://hz.ehwqpu.com/gtnyirnziq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jinghuilouyu.cn/gtbgpovrib.html

C#:   static void Main(string[] args)
来源：http://hz.andypj.xyz/gtrdknveny.html

[M08] 获取系统与运行时信息
来源：http://hz.dianchejie.cn/gtjinvtsma.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ybcxt.top/gtghwrddit.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhaomingkeji.xyz/gtmzeqkqts.html

JS:   process.platform;  process.version
来源：http://hz.gogol.net.cn/gtqrshjemn.html

TS:   process.platform;  process.version
来源：http://hz.birdmap.top/gtyiytzahn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xuanzx.com/gthwlgcqej.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.ydzc1.top/gtscqhvrxl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jianghu66.top/gtnzqrleir.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.tianlin.xyz/gtoxynsbnm.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtysbbiafg.html

N. 数据结构与算法
来源：http://hz.yongpay.top/gtqrzixdmz.html

================================================================================
来源：http://hz.zdqjudy.top/gtdffwtiqv.html

[N01] 二分查找（有序数组）
来源：http://hz.zhixingplan.top/gtyhlsyzgi.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.cucudq.cn/gtjyzbpkvo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.wangshuangyany.cn/gtoackvjci.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yangfankeji.com/gtmzcudvgc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhongyouzk.top/gttixyubme.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jqgufenzy.top/gtunnmxhgc.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.aibaodan.cn/gtzbnkzewq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ehwqpu.com/gtcczpduvi.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.redwolf501.top/gtnfcoqxoh.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.sweek.top/gtyhugmjbr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ywan-chungtsiang.top/gthuifxhrk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.ydjk.org.cn/gtqcejyoeh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.dianchejie.cn/gtwjfgazsz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.9152youxi.cn/gtpapvwhtc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.316326.xyz/gtbkbwtahi.html

Go:   slices.Sort(arr)
来源：http://hz.xinyue.icu/gtfwfezeqw.html

Ruby: arr.sort
来源：http://hz.yvedp.cn/gttpcnabjy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ywan-chungtsiang.top/gtssimtbsg.html

[N03] 快速排序（分治示例）
来源：http://hz.zhengqikj.top/gtlnrggjfn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.fengsongda.top/gtdaippgzy.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zhongyouzk.top/gtqqcasapt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.vqdsnc.cn/gtgmvycvca.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.snrcjt.cn/gtbfsuxtkz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.xuanzx.com/gtbfvtwsva.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.chenzaomai.com/gtumhdscxk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.havefunace.top/gtrutlpvmv.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.0kj1m.cn/gtucxeqhqt.html

[N04] 斐波那契数列
来源：http://hz.guowangkeji.top/gtnazojtxv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.shzxlz.cn/gtqezulcoe.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hammf.cn/gtporwhcbd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cdnleiting.top/gtxqnwxyhy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.havefunace.top/gtlafnwohr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jqgufenzy.top/gtcqrvfaim.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.chenzaomai.com/gtoolsaiho.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.0kj1m.cn/gtlxidkylv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jianghu66.top/gthtushfml.html

[N05] 最大公约数
来源：http://hz.birdmap.top/gtdjsoqbnk.html

Py:   math.gcd(a, b)
来源：http://hz.aizwys.cn/gtgipfcmvh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.cdnleiting.top/gtgvvevxiz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gzhubu.top/gtgxsnldmo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shangyingyoupin.top/gtzyzsvsxs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.kuanghao11.cn/gtfzpsxcpv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yj202588.top/gtajmexsnq.html

Ruby: a.gcd(b)
来源：http://hz.jinqigufen.top/gtdjyazuji.html


<!-- 参考信息 -->