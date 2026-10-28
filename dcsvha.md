代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://hz.bjfxy.top/gthlwbbegp.html

[J08] 提取年月日与星期
来源：http://hz.cqqwz.cn/gtympunjdm.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.mhx1999.top/gtozrtoevk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.shanyushiyangkeji.top/gtkvqokhzu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.xziqi.cn/gtqjixxpxd.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.pycfn.com/gtlbplosye.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.xuanzx.com/gtwlwtkgde.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hongshengwenyu.top/gtzxmrftpi.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yj20258.top/gtwyswumsb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.aibaodan.cn/gttqgkmrpa.html

[J09] 时区处理
来源：http://hz.shuidangran.top/gtgsdtyarq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.tian-w.cn/gtxnlrcciz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.shzxlz.cn/gtaioegtmq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gogol.net.cn/gtsffgcwpo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yanxiufei.cn/gtkgqzpkhg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.chenjidiqi.icu/gtycxdypxm.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xuetiantiany.cn/gtayysgzyw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hammf.cn/gtqsmcgsyt.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.c1oappe.top/gtonxxpymf.html

[J10] 取今天 / 本月第一天
来源：http://hz.yuanzhike.top/gtqdntkvkr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hywenlv.cn/gtstxajkwj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ppjwa.cn/gtdqzfcsnz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.chenzaomai.com/gtenucqjhd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ehwqpu.com/gtnobfyall.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shzxlz.cn/gtqglistyd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhengqikj.top/gtubaingif.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhiwuduotai.top/gtiddwrjrx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.shzxlz.cn/gtdcrifkkf.html

================================================================================
来源：http://hz.yvedp.cn/gtfirxotsg.html

K. JSON 与序列化
来源：http://hz.ywan-chungtsiang.top/gtllwmaiqi.html

================================================================================
来源：http://hz.zhongyouzk.top/gtoonxwedn.html

[K01] 对象转 JSON 字符串
来源：http://hz.ydjk.org.cn/gtroyllzlb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.tanke756.top/gtkkrajbnf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yongpay.top/gtdimbuisk.html

JS:   JSON.stringify(obj)
来源：http://hz.jiagoushi.top/gtliytqpuw.html

TS:   JSON.stringify(obj)
来源：http://hz.shzxlz.cn/gtkgwmpzss.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhiwuduotai.top/gtjzwstkee.html

Go:   json.Marshal(obj)
来源：http://hz.yangfankeji.com/gtqvfveqap.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.pengpengdd.cyou/gtmapkgheb.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.cdnleiting.top/gtblcdvdzn.html

[K02] JSON 字符串转对象
来源：http://hz.hywenlv.cn/gthchrtxrq.html

Py:   json.loads(s)
来源：http://hz.ppjwa.cn/gtduhernmn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cqqwz.cn/gtwywojgks.html

JS:   JSON.parse(s)
来源：http://hz.tianlin.xyz/gtfucfqcam.html

TS:   JSON.parse(s)
来源：http://hz.snrcjt.cn/gtaojvhewy.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jiagoushi.top/gtloswlmxx.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.chenzaomai.com/gtktwwrgzt.html

Ruby: JSON.parse(s)
来源：http://hz.yueranfly.top/gtnoeaujil.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yj20258888.top/gtprshyzbj.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.sxryk.cn/gthsmiuoii.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.c1oappe.top/gtlfcqabjy.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yonumen.top/gtumaaizvq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hfpthk.cn/gtstkoiocx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hnqzz.top/gtzlozkdjg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yj202588.top/gtjebxdrlh.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zycfv.cn/gtfnpowknl.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zycfv.cn/gtzchzolxa.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yangfankeji.com/gtcvyjgipc.html

[K04] 读取 JSON 文件
来源：http://hz.ywan-chungtsiang.top/gtcrbrfzjf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.guowangkeji.top/gtpsngigqn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.52xcode.cn/gtzxiandkv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.aizwys.cn/gtmduenjmo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zycfv.cn/gtlajbfbza.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.gaohongyu789.top/gtaoshjgai.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xylfe.cn/gtkphryapl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jinqigufen.top/gtdnfzfudg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.fengsongda.top/gtcqmooiii.html

[K05] 深拷贝对象
来源：http://hz.nanxuanxn.top/gtsquvgfjw.html

Py:   copy.deepcopy(obj)
来源：http://hz.daria6918.cn/gtmqixpkyt.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hysaishi.cn/gtvcftehxq.html

JS:   structuredClone(obj)
来源：http://hz.havefunace.top/gttsaomptd.html

TS:   structuredClone(obj)
来源：http://hz.zhijiandao.cn/gtitykpfqd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xinyue.icu/gtikdjqqwu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.9152youxi.cn/gtlcqbwize.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhongyouzk.top/gtctfpelrs.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhijiandao.cn/gtdzqgrxmd.html

[K06] 解析 URL 查询串
来源：http://hz.tian-w.cn/gtwabcfqju.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yj20258.top/gtxcarygar.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.smart0.xyz/gtoixnfybc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zdqjudy.top/gtsewlzupa.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj20258.top/gtzrksruqw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jinyuanbaomall.cn/gtlccrhhif.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jqgufenzy.top/gtxjwzehdm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yj20258.top/gtnevwohdj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yuanzhike.top/gtebjpczlr.html

[K07] 进制转换
来源：http://hz.fengsongda.top/gtkhkkhpld.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zycfv.cn/gtxrghelpx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.9152youxi.cn/gtxvmicmxu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xziqi.cn/gthvwjugql.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hfpthk.cn/gtdojxlebk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.snrcjt.cn/gtegjqdlmh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hywenlv.cn/gtqczswqgs.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xinyue.icu/gtacyqbfmv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.dashuyun.cn/gtwzqjzzlu.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.dashuyun.cn/gttnudqtle.html

Py:   pickle.dumps(obj)
来源：http://hz.hammf.cn/gtngacholz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.fengsongda.top/gtjevmhelr.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.pycfn.com/gtklnbtmpo.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.guowangkeji.top/gtbkrzgqjb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hongshengwenyu.top/gtselhinuc.html

Go:   encoding/gob
来源：http://hz.xylfe.cn/gteyaqlqng.html

Ruby: Marshal.dump(obj)
来源：http://hz.jlsjyb.cn/gtcrshknnj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.9152youxi.cn/gtkpkujlro.html

================================================================================
来源：http://hz.yuxming.cn/gtmyvbmtth.html

L. 网络请求
来源：http://hz.yvedp.cn/gtuxjtzpwd.html

================================================================================
来源：http://hz.jqgufenzy.top/gtswsnzeyd.html

[L01] 发送 GET 请求
来源：http://hz.yj202588.top/gtlsvpnavv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.316326.xyz/gtgpvmmlcp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.tian-w.cn/gtxujunpnt.html

JS:   await fetch(url)
来源：http://hz.tian-w.cn/gtgldhctts.html

TS:   await fetch(url)
来源：http://hz.xuetiantiany.cn/gtwslnvlki.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yvedp.cn/gtjurdzguq.html

Go:   resp, err := http.Get(url)
来源：http://hz.yj20258888.top/gtylabrnbt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jinqigfzy.top/gtdobvsgfm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hnqzz.top/gtjyqxxtxf.html

[L02] 发送 POST JSON
来源：http://hz.chenzaomai.com/gtyfdgjiac.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yj20258.top/gtwrjqrkoy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.0kj1m.cn/gtwgwlfiav.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cheryme.top/gttvwnvzlw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.daria6918.cn/gtnifgtscz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.chenjidiqi.icu/gtvmbkrafx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhongyouzk.top/gtnikpayfp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yj20258888.top/gtaqszcdrc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yonumen.top/gtdqbjqybf.html

[L03] 设置自定义请求头
来源：http://hz.hnxiangtu.top/gtprktbcim.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.sufxvd.cn/gtlfwpdwzo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.iojbl.cn/gtgflvmshi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.daxiang520.top/gtdehfkkgj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xylfe.cn/gtcpvlnvbj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jinghuilouyu.cn/gtdqtskngt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ybcxt.top/gtibuwaycm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.sweek.top/gtajnmljjz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.fzhhl.top/gtjlyqoils.html

[L04] 设置超时
来源：http://hz.cqqwz.cn/gtmmkbatvu.html

Py:   requests.get(url, timeout=5)
来源：http://hz.kuanghao11.cn/gtaqwfeczd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jqgufenzy.top/gtlcfteozb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.daxiang520.top/gtlxxagyqq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shzxlz.cn/gtlhcfrmpj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zycfv.cn/gtljukgagi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.gzhubu.top/gtswmdfgqn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jyoumei.cn/gtkfwrkptb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.0kj1m.cn/gtrkynjhij.html

[L05] 上传文件（multipart）
来源：http://hz.kuanghao11.cn/gtfgplhrmn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.haohaochexian.top/gtbojqqaol.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.kuanghao11.cn/gtkzrbokqt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yj20258888.top/gtzquemhjr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.cdnleiting.top/gtumtfoupz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.iojbl.cn/gttqwzvpkw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.aizwys.cn/gtwxydqfzq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.smart0.xyz/gtxhrxihyo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.cashguo.top/gtzrrjbyxi.html

[L06] 解析响应为 JSON
来源：http://hz.hammf.cn/gtckwnhrbw.html

Py:   resp.json()
来源：http://hz.zhaomingkeji.xyz/gtktxwxlkt.html

PHP:  json_decode($body, true);
来源：http://hz.cqqwz.cn/gtawhovdbx.html

JS:   await resp.json()
来源：http://hz.shanyushiyangtech.top/gtmxpoxnoi.html

TS:   await resp.json()
来源：http://hz.ydzc1.top/gtzfbhqxgw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhengqikj.top/gthqlodviy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.havefunace.top/gttoqgvuhe.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xinyue.icu/gtwcyysiyf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.daria6918.cn/gtktysyowz.html

[L07] 处理 HTTP 状态码
来源：http://hz.kuanghao11.cn/gtdyfebjay.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.wangshuangyany.cn/gtfqezexel.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hysaishi.cn/gtoekxebwa.html

JS:   resp.ok;  resp.status
来源：http://hz.hfpthk.cn/gtigtkbbxw.html

TS:   resp.ok;  resp.status
来源：http://hz.vqdsnc.cn/gtodbylvaw.html

Java: resp.statusCode()
来源：http://hz.yongpay.top/gtwbohkxog.html

Go:   resp.StatusCode
来源：http://hz.ehwqpu.com/gtzshdrgbk.html

Ruby: resp.code.to_i
来源：http://hz.svipenyu.cn/gtiecmkaft.html

C#:   (int)resp.StatusCode
来源：http://hz.xuetiantiany.cn/gtbzyhiiwc.html

[L08] 并发请求多个地址
来源：http://hz.hammf.cn/gtfxfttebb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yanxiufei.cn/gtwiwubiot.html

PHP:  curl_multi_init() 系列
来源：http://hz.hysaishi.cn/gtrjqqhydr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinqigfzy.top/gttsaftiye.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xuanzx.com/gtnvapyhux.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.aibaodan.cn/gtwogdwqai.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.shanyushiyangtech.top/gtbjscqect.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.gogol.net.cn/gtvmtnlkkh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhoulong.xyz/gtsonwargn.html

================================================================================
来源：http://hz.dashuyun.cn/gtbxyhlyvk.html

M. 命令行 / 进程 / 环境
来源：http://hz.yvedp.cn/gtrxcmlzbk.html

================================================================================
来源：http://hz.andypj.xyz/gtsxntzvhx.html

[M01] 读取命令行参数
来源：http://hz.zhongyouzk.top/gtkmwkbwse.html

Py:   sys.argv[1:]
来源：http://hz.xuetiantiany.cn/gtivhhjwtj.html

PHP:  $argv;  $argc;
来源：http://hz.nanxinkj.top/gteatdxtcp.html

JS:   process.argv.slice(2)
来源：http://hz.kuanghao11.cn/gtuxwzrzcb.html

TS:   process.argv.slice(2)
来源：http://hz.yvedp.cn/gtszdnthgv.html

Java: args 数组（main 方法参数）
来源：http://hz.tianlin.xyz/gtkhqnfjga.html

Go:   os.Args[1:]
来源：http://hz.yuxming.cn/gtnmkqhpyd.html

Ruby: ARGV
来源：http://hz.zhaomingkeji.xyz/gtajvehshd.html

C#:   args 数组（Main 方法参数）
来源：http://hz.gaohongyu789.top/gtkrvxktvb.html

[M02] 读取环境变量
来源：http://hz.meibo888.top/gtkmynmenp.html

Py:   os.environ.get("HOME")
来源：http://hz.dianchejie.cn/gtdrvnijhw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.aizwys.cn/gtfudiozma.html

JS:   process.env.HOME
来源：http://hz.ppjwa.cn/gtkdczxjng.html

TS:   process.env.HOME
来源：http://hz.cdnleiting.top/gteqxmvckt.html

Java: System.getenv("HOME")
来源：http://hz.ehwqpu.com/gtgsdclqwg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.xylfe.cn/gtvwaokxzv.html

Ruby: ENV["HOME"]
来源：http://hz.haohaochexian.top/gtotmoxiuf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yuxming.cn/gthvhhwqjj.html

[M03] 执行外部命令
来源：http://hz.iojbl.cn/gtdrdbgskj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.shangyingyoupin.top/gtqmfdgchx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.gzhubu.top/gtrhtryjnp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zdqjudy.top/gtjworjcsh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.nwbrower.top/gtsoyulrfi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jinqigufen.top/gtxqlndnxm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.iojbl.cn/gtozpgsins.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.wangshuangyany.cn/gtftmrhjue.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hammf.cn/gtboduwlsl.html

[M04] 获取当前工作目录
来源：http://hz.ywan-chungtsiang.top/gtakwpxrrt.html

Py:   os.getcwd()
来源：http://hz.yvedp.cn/gtxopjqyyq.html

PHP:  getcwd();
来源：http://hz.hfpthk.cn/gtafgyutns.html

JS:   process.cwd()
来源：http://hz.c1oappe.top/gtbqgppicg.html

TS:   process.cwd()
来源：http://hz.hysaishi.cn/gtqjerrquz.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.dianchejie.cn/gtbkvyfrkc.html

Go:   os.Getwd()
来源：http://hz.jqgfzy.top/gtmlffxmxc.html

Ruby: Dir.pwd
来源：http://hz.52xcode.cn/gtzpdvupic.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.fzhhl.top/gthzigepdv.html

[M05] 设置退出码
来源：http://hz.haohaochexian.top/gtfzahzqzs.html

Py:   sys.exit(1)
来源：http://hz.nanxuanxn.top/gtzipvvflp.html

PHP:  exit(1);
来源：http://hz.zdqjudy.top/gthowvtrnr.html

JS:   process.exit(1)
来源：http://hz.ehwqpu.com/gtfrjkrtjk.html

TS:   process.exit(1)
来源：http://hz.daria6918.cn/gtmorwqvta.html

Java: System.exit(1)
来源：http://hz.nwbrower.top/gtfiambgim.html

Go:   os.Exit(1)
来源：http://hz.ywan-chungtsiang.top/gtihcmniny.html

Ruby: exit 1
来源：http://hz.daxiang520.top/gtrefwswax.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.andypj.xyz/gtxbrbhvlm.html

[M06] 向标准错误输出
来源：http://hz.daxiang520.top/gtvdpeubqv.html

Py:   print("err", file=sys.stderr)
来源：http://hz.tian-w.cn/gtucwtlppt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yvedp.cn/gtzememlyx.html

JS:   console.error("err")
来源：http://hz.zhoulong.xyz/gtffdaoctx.html

TS:   console.error("err")
来源：http://hz.xuanzx.com/gthprvoeoq.html

Java: System.err.println("err")
来源：http://hz.birdmap.top/gtkiosutem.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xuetiantiany.cn/gtdkitqgjl.html

Ruby: warn "err"
来源：http://hz.zhoulong.xyz/gtjydwxkbh.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hywenlv.cn/gtiraafnzr.html

[M07] 判断是否为主入口
来源：http://hz.yuanzhike.top/gthllsfoer.html

Py:   if __name__ == "__main__":
来源：http://hz.guowangkeji.top/gtelsdxuoh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yangfankeji.com/gtibdnkieh.html

JS:   require.main === module
来源：http://hz.yvedp.cn/gtryhiyfel.html

TS:   require.main === module
来源：http://hz.guannengcc.top/gtpopfowqj.html

Java: public static void main(String[] args)
来源：http://hz.wangshuangyany.cn/gtkgluygis.html

Go:   func main()
来源：http://hz.cdnleiting.top/gtznmonhtl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.nwbrower.top/gtuijpqhjb.html

C#:   static void Main(string[] args)
来源：http://hz.xingfuxueyuan.xyz/gtzrjvuftg.html

[M08] 获取系统与运行时信息
来源：http://hz.cdnleiting.top/gtrofnhers.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yvedp.cn/gtcoutpfsv.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yonumen.top/gtlpofjrcf.html

JS:   process.platform;  process.version
来源：http://hz.svipenyu.cn/gtptbtvqzb.html

TS:   process.platform;  process.version
来源：http://hz.yj20258.top/gtxlzaltiq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xingfuxueyuan.xyz/gtlpbcsdnb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.pengpengdd.cyou/gtqiqeaeii.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.gotoacloud.top/gttgctjgoq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.snrcjt.cn/gtzqtkwxhh.html

================================================================================
来源：http://hz.nanxinkj.top/gtsplvgpyu.html

N. 数据结构与算法
来源：http://hz.xylfe.cn/gtmuffktcl.html

================================================================================
来源：http://hz.hysaishi.cn/gtggsyipxp.html

[N01] 二分查找（有序数组）
来源：http://hz.pengpengdd.cyou/gtjtasnrjz.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.pengpengdd.cyou/gtxusedypu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ehwqpu.com/gtoldnbnen.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhijiandao.cn/gtxpdvkmad.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ivvv.top/gthqmpijor.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.cucudq.cn/gttjdfxcds.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.52xcode.cn/gtpawtdbch.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.daxiang520.top/gtvcyregzq.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yj202588.top/gtzmgwzycr.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhiwuduotai.top/gttxibgcli.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yvedp.cn/gtdgcknpdq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yj20258.top/gtfexrdcmu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhixingplan.top/gttzlbzzev.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ywan-chungtsiang.top/gtziieorpg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yonumen.top/gtcyobqjmz.html

Go:   slices.Sort(arr)
来源：http://hz.mhx1999.top/gtqdsmnybl.html

Ruby: arr.sort
来源：http://hz.sufxvd.cn/gtqfiqvykd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.hysaishi.cn/gtcsikieif.html

[N03] 快速排序（分治示例）
来源：http://hz.zhixingplan.top/gthhqpqqmb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhaomingkeji.xyz/gtqiyxorxn.html

PHP:  // 递归实现，或用 usort
来源：http://hz.gogol.net.cn/gtxrreklci.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xziqi.cn/gtvpezaxqp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.redwolf501.top/gtdrixkeqv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.sufxvd.cn/gtkapfbczo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.ehwqpu.com/gtrbqioxrc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.shanyushiyangtech.top/gtdwfydpbu.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.meibo888.top/gttzbfplrx.html

[N04] 斐波那契数列
来源：http://hz.havefunace.top/gtmfwlyymg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.guannengcc.top/gtalygoalr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.ydjk.org.cn/gtpstnujqc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cqqwz.cn/gtlgviyivc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yvedp.cn/gtxiqyfuyc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.52xcode.cn/gtxfxvbbwz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ybcxt.top/gtouqvzwfi.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.52xcode.cn/gtkazdwyaj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hammf.cn/gtypywgygz.html

[N05] 最大公约数
来源：http://hz.tian-w.cn/gtachoovhw.html

Py:   math.gcd(a, b)
来源：http://hz.guannengcc.top/gtxtfqqkup.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.meibo888.top/gtauhlrghm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cheryme.top/gthcymkozd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.tian-w.cn/gtujgdsfmh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.nanxinkj.top/gtjdsxpahw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.nwbrower.top/gtkuoimrxv.html

Ruby: a.gcd(b)
来源：http://hz.ehwqpu.com/gtllvtpbma.html


<!-- 参考信息 -->