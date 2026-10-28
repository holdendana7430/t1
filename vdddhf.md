代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://hz.xziqi.cn/gtgpvnmkiy.html

[J08] 提取年月日与星期
来源：http://hz.wangshuangyany.cn/gtcqrzmcoe.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yuxming.cn/gtroynguwp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xinyue.icu/gtvwozujtw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yj20258.top/gtbouazvwz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.xuetiantiany.cn/gtlimfgsqa.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.fzhhl.top/gtnqedumdg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.pengpengdd.cyou/gtouogvenu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hnqzz.top/gtojsepqdd.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhijiandao.cn/gtgrojwysh.html

[J09] 时区处理
来源：http://hz.0kj1m.cn/gtuewjsxfw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jyoumei.cn/gtgwbarkdo.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hywenlv.cn/gtvggejcvh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jiagoushi.top/gtupqxtudm.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nanxinkj.top/gtdsblcytv.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hysaishi.cn/gtwseopqdr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.shanyushiyangtech.top/gtfiphhpdw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.nanxinkj.top/gtwmrzqtfv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.bjfxy.top/gtbqonwcoa.html

[J10] 取今天 / 本月第一天
来源：http://hz.chenzaomai.com/gtxxmzoexw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jyoumei.cn/gtdjknhugk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zycfv.cn/gtxvvnepmz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.9152youxi.cn/gtjgiiqndo.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.sweek.top/gtjokdrmpp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.cashguo.top/gtsgnuofda.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zdqjudy.top/gthfjbnffh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jlsjyb.cn/gtduvcpeya.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.meibo888.top/gtlkjmbnsb.html

================================================================================
来源：http://hz.jqgfzy.top/gtfffufwjw.html

K. JSON 与序列化
来源：http://hz.smart0.xyz/gtduofwjof.html

================================================================================
来源：http://hz.zdqjudy.top/gtmjzmogom.html

[K01] 对象转 JSON 字符串
来源：http://hz.gotoacloud.top/gtevsvgfmn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.nwbrower.top/gtsmtakouo.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.tian-w.cn/gtrvtxrlgn.html

JS:   JSON.stringify(obj)
来源：http://hz.pycfn.com/gtbvcspefr.html

TS:   JSON.stringify(obj)
来源：http://hz.daria6918.cn/gtdmbzeyjq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zdqjudy.top/gtpqkzayzu.html

Go:   json.Marshal(obj)
来源：http://hz.iojbl.cn/gtlvxisger.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.feifeiyinyue.top/gtfpixiwqs.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.dianchejie.cn/gtkepjjckx.html

[K02] JSON 字符串转对象
来源：http://hz.birdmap.top/gtmekfdjwa.html

Py:   json.loads(s)
来源：http://hz.smart0.xyz/gtpbcakviw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yonumen.top/gtvrdbooyt.html

JS:   JSON.parse(s)
来源：http://hz.fzhhl.top/gtqmqovews.html

TS:   JSON.parse(s)
来源：http://hz.9152youxi.cn/gtktorhwcy.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jinqigfzy.top/gttzwkuzjy.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.haohaochexian.top/gtdgspljpj.html

Ruby: JSON.parse(s)
来源：http://hz.yonumen.top/gtigaogopa.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.fzhhl.top/gtilfhioeq.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yuxming.cn/gtivhfptvh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hywenlv.cn/gtjolxmaxg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.nanxinkj.top/gtastwfsxq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.quarkkingdee.top/gtgfftshrj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hysaishi.cn/gtxjlihgsd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.sysykeji.top/gtduqotkbr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.52xcode.cn/gtjnygecot.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.shangyingyoupin.top/gtepjezfii.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.dianchejie.cn/gtsrrmjaiq.html

[K04] 读取 JSON 文件
来源：http://hz.jyoumei.cn/gtfvsujcgw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.0kj1m.cn/gtksqlbxha.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ydzc1.top/gtzbfjhpre.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhongyouzk.top/gtetcjxrdi.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.c1oappe.top/gtyykgailp.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.kuanghao11.cn/gtipgarbgu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jyoumei.cn/gtatsigaqq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.tianlin.xyz/gtsfckfrzg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.chenlongwang.top/gtmaosfujf.html

[K05] 深拷贝对象
来源：http://hz.meibo888.top/gtzlhttekz.html

Py:   copy.deepcopy(obj)
来源：http://hz.yj20258888.top/gtklgakkxa.html

PHP:  unserialize(serialize($obj));
来源：http://hz.bjfxy.top/gtfnnfjhqc.html

JS:   structuredClone(obj)
来源：http://hz.vqdsnc.cn/gteunynqbq.html

TS:   structuredClone(obj)
来源：http://hz.316326.xyz/gtpuuyyivb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.bjfxy.top/gtvywjtlhq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.52xcode.cn/gtjsnaesul.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.cqqwz.cn/gtzwtrriqm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jqgfzy.top/gtngmvswgc.html

[K06] 解析 URL 查询串
来源：http://hz.52xcode.cn/gtpefkzqwq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yj202588.top/gtvktiscni.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.wangdashe.top/gtyikwliei.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jyoumei.cn/gtzusftarm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj20258.top/gtmxglfmni.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.vqdsnc.cn/gtuwoudxzi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yangfankeji.com/gtbeyiznnp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hywenlv.cn/gtcjscivtv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.shzxlz.cn/gtjcxsxzxt.html

[K07] 进制转换
来源：http://hz.feifeiyinyue.top/gtgjipodzs.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hysaishi.cn/gtzevbfkda.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yueranfly.top/gtnzvkhvee.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yueranfly.top/gtokbzikuw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.0kj1m.cn/gtalauwvcd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.kuanghao11.cn/gtqflcqipv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.tian-w.cn/gttshfgsvt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.sxryk.cn/gtisreedue.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.c1oappe.top/gthrkpxdfb.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.aibaodan.cn/gtosvqusiy.html

Py:   pickle.dumps(obj)
来源：http://hz.bjfxy.top/gtxenytfff.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jinqigfzy.top/gtwqusugrv.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yj20258888.top/gtlzjyzrmz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.nanxinkj.top/gtjxmxjjvb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.fzhhl.top/gtvvwqmwgo.html

Go:   encoding/gob
来源：http://hz.pengpengdd.cyou/gtwgifbddy.html

Ruby: Marshal.dump(obj)
来源：http://hz.jinqigfzy.top/gtfhkujgwi.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.andypj.xyz/gtzcgasxug.html

================================================================================
来源：http://hz.cucudq.cn/gtimakbxmb.html

L. 网络请求
来源：http://hz.ydzc1.top/gtzynlkfdt.html

================================================================================
来源：http://hz.tanke756.top/gtmbnbhvmk.html

[L01] 发送 GET 请求
来源：http://hz.jiagoushi.top/gtbydymrfu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jinqigfzy.top/gtpabywgqx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yonumen.top/gtdbcemwhg.html

JS:   await fetch(url)
来源：http://hz.wangshuangyany.cn/gtxwuhlttd.html

TS:   await fetch(url)
来源：http://hz.ydzc1.top/gtqydjkomq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhijiandao.cn/gtqzukfrtz.html

Go:   resp, err := http.Get(url)
来源：http://hz.yanxiufei.cn/gtcwnbhjev.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.316326.xyz/gtddxtahcm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ehwqpu.com/gtlgtwibum.html

[L02] 发送 POST JSON
来源：http://hz.zhengqikj.top/gtyhjhznyz.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.sxryk.cn/gtlqkkxiqj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.iojbl.cn/gttrufnhlr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xuetiantiany.cn/gtskcybjvn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hfpthk.cn/gthmulgwzc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.fzhhl.top/gtksmahijn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hywenlv.cn/gtxkurztqz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jqgfzy.top/gtiwfgtxmm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.gaohongyu789.top/gtgtxhrmxd.html

[L03] 设置自定义请求头
来源：http://hz.0kj1m.cn/gtemubtsdj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ehwqpu.com/gtoylagxdy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zhixingplan.top/gtyhflmsuc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.aizwys.cn/gticyofvyk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.daxiang520.top/gtfxjyvgoe.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.xuanzx.com/gtwnbtaaxt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.redwolf501.top/gtvyjtrikt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hywenlv.cn/gthoueyigl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.tian-w.cn/gtjpziivso.html

[L04] 设置超时
来源：http://hz.0kj1m.cn/gtovvaoooe.html

Py:   requests.get(url, timeout=5)
来源：http://hz.shzxlz.cn/gtcuqurnwx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yvedp.cn/gtymvkvhej.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhaomingkeji.xyz/gtrxchtnfa.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yuxming.cn/gtrtndllig.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.9152youxi.cn/gtbqgbvcwg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ydzc1.top/gthtrbbsqy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.wangdashe.top/gtehyhedzj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.gzhubu.top/gtnzlcnqdj.html

[L05] 上传文件（multipart）
来源：http://hz.pengpengdd.cyou/gtdvoxhkbc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.aizwys.cn/gtnnzunbtc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.tanke756.top/gtuylceqlv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jqgufenzy.top/gtrrchwlhx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yueranfly.top/gtqbwgjztx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhongyouzk.top/gtszgayuvg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.bjfxy.top/gtrwuhtilh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yuanzhike.top/gtxnwozoln.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhoulong.xyz/gtejtuzdoo.html

[L06] 解析响应为 JSON
来源：http://hz.yj20258888.top/gtnikaakwz.html

Py:   resp.json()
来源：http://hz.c1oappe.top/gtphwvbkrm.html

PHP:  json_decode($body, true);
来源：http://hz.zhiwuduotai.top/gtubuyjjkc.html

JS:   await resp.json()
来源：http://hz.fzhhl.top/gttuuvfrpl.html

TS:   await resp.json()
来源：http://hz.c1oappe.top/gtjwhuimjt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zycfv.cn/gtnvnpxdmj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xinyue.icu/gtuopmbcjg.html

Ruby: JSON.parse(resp.body)
来源：http://hz.chenzaomai.com/gtnswhumsx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yueranfly.top/gthtxnqcrm.html

[L07] 处理 HTTP 状态码
来源：http://hz.smart0.xyz/gtihfjhjiu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhiwuduotai.top/gtkilstnwe.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.feifeiyinyue.top/gtmdwighpi.html

JS:   resp.ok;  resp.status
来源：http://hz.yj202588.top/gtfhsztioa.html

TS:   resp.ok;  resp.status
来源：http://hz.sysykeji.top/gtatrfjcvz.html

Java: resp.statusCode()
来源：http://hz.zhijiandao.cn/gtgkbzxynh.html

Go:   resp.StatusCode
来源：http://hz.jinqigfzy.top/gtkiqdtcel.html

Ruby: resp.code.to_i
来源：http://hz.hfpthk.cn/gtkqgddhfm.html

C#:   (int)resp.StatusCode
来源：http://hz.jinyuanbaomall.cn/gtpyiazjzg.html

[L08] 并发请求多个地址
来源：http://hz.shanyushiyangkeji.top/gtkcbgqzub.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zhengqikj.top/gtmriygxok.html

PHP:  curl_multi_init() 系列
来源：http://hz.havefunace.top/gtdtykuktr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nanxuanxn.top/gthelqrztg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.daxiang520.top/gtgykyxjfy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zycfv.cn/gtofwuuuew.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jqgfzy.top/gtqaiofaod.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhoulong.xyz/gthvmmjhrz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.sweek.top/gthimcepzp.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtcqitvynl.html

M. 命令行 / 进程 / 环境
来源：http://hz.yangfankeji.com/gtmnebybcq.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtyflsefmh.html

[M01] 读取命令行参数
来源：http://hz.ehwqpu.com/gtokdxaaon.html

Py:   sys.argv[1:]
来源：http://hz.zhiwuduotai.top/gthvpdycme.html

PHP:  $argv;  $argc;
来源：http://hz.zhaomingkeji.xyz/gtwdsmpzul.html

JS:   process.argv.slice(2)
来源：http://hz.xuetiantiany.cn/gtlcagibkq.html

TS:   process.argv.slice(2)
来源：http://hz.cashguo.top/gtnxniynty.html

Java: args 数组（main 方法参数）
来源：http://hz.hammf.cn/gtwsktrxff.html

Go:   os.Args[1:]
来源：http://hz.nanxuanxn.top/gtnjviohfo.html

Ruby: ARGV
来源：http://hz.jinqigfzy.top/gtbjsmsewh.html

C#:   args 数组（Main 方法参数）
来源：http://hz.guowangkeji.top/gtgeyqxahd.html

[M02] 读取环境变量
来源：http://hz.cheryme.top/gtxmnrznmw.html

Py:   os.environ.get("HOME")
来源：http://hz.meibo888.top/gtelzgeyub.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.mhx1999.top/gtxfdnnakl.html

JS:   process.env.HOME
来源：http://hz.shanyushiyangtech.top/gtuvyhvoxt.html

TS:   process.env.HOME
来源：http://hz.tanke756.top/gtdkvjnjqp.html

Java: System.getenv("HOME")
来源：http://hz.hongshengwenyu.top/gtroighygc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.xuetiantiany.cn/gttcevyazq.html

Ruby: ENV["HOME"]
来源：http://hz.jyoumei.cn/gthhvxlmba.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yueranfly.top/gtgheezuen.html

[M03] 执行外部命令
来源：http://hz.feifeiyinyue.top/gtgoypzape.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.shzxlz.cn/gtcljobsot.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.dianchejie.cn/gtihlqzxkw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.daxiang520.top/gtpmoxclxn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.aibaodan.cn/gtxvcnxxrc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.andypj.xyz/gthlzpofem.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.316326.xyz/gtnzifjybh.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.meibo888.top/gttbjirdkv.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jiagoushi.top/gttwmxqxzr.html

[M04] 获取当前工作目录
来源：http://hz.mhx1999.top/gtplkufmmx.html

Py:   os.getcwd()
来源：http://hz.hysaishi.cn/gtugvgtghi.html

PHP:  getcwd();
来源：http://hz.52xcode.cn/gtnhpwudxa.html

JS:   process.cwd()
来源：http://hz.jqgfzy.top/gtbfbgggxq.html

TS:   process.cwd()
来源：http://hz.yonumen.top/gthdkwtzmf.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.tanke756.top/gtuywnsxgq.html

Go:   os.Getwd()
来源：http://hz.jlsjyb.cn/gtxsuxfxye.html

Ruby: Dir.pwd
来源：http://hz.jqgufenzy.top/gtfkbpscpq.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.pycfn.com/gtssooymap.html

[M05] 设置退出码
来源：http://hz.sweek.top/gtrhufdnuz.html

Py:   sys.exit(1)
来源：http://hz.xingfuxueyuan.xyz/gtuouxqewu.html

PHP:  exit(1);
来源：http://hz.cqqwz.cn/gtdxhwmagg.html

JS:   process.exit(1)
来源：http://hz.0kj1m.cn/gtqpmvrkhl.html

TS:   process.exit(1)
来源：http://hz.jinqigufen.top/gtobgyjaha.html

Java: System.exit(1)
来源：http://hz.gotoacloud.top/gthrjysxxl.html

Go:   os.Exit(1)
来源：http://hz.guannengcc.top/gtwjwqakpq.html

Ruby: exit 1
来源：http://hz.yuanzhike.top/gtimtwmgym.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zhengqikj.top/gtmsusxail.html

[M06] 向标准错误输出
来源：http://hz.gaohongyu789.top/gtfbgmnxct.html

Py:   print("err", file=sys.stderr)
来源：http://hz.9152youxi.cn/gtalhlhdsz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.chenzaomai.com/gtbguiqoqc.html

JS:   console.error("err")
来源：http://hz.ydzc1.top/gtibntopys.html

TS:   console.error("err")
来源：http://hz.yvedp.cn/gtpuaiaohr.html

Java: System.err.println("err")
来源：http://hz.jinqigufen.top/gtgieejnwm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.fengsongda.top/gtnzaescdi.html

Ruby: warn "err"
来源：http://hz.chenjidiqi.icu/gtdvyhqvxt.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ybcxt.top/gtxtbrdbgy.html

[M07] 判断是否为主入口
来源：http://hz.chenzaomai.com/gtthgcelui.html

Py:   if __name__ == "__main__":
来源：http://hz.jlsjyb.cn/gtnxcwyhqq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.316326.xyz/gthqcrckyr.html

JS:   require.main === module
来源：http://hz.yueranfly.top/gtuolhxjgk.html

TS:   require.main === module
来源：http://hz.yangfankeji.com/gtcefvpwrt.html

Java: public static void main(String[] args)
来源：http://hz.xylfe.cn/gtiqkfkvze.html

Go:   func main()
来源：http://hz.birdmap.top/gtslzefcmk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cheryme.top/gtfymmfrlz.html

C#:   static void Main(string[] args)
来源：http://hz.chenjidiqi.icu/gtxkyijqik.html

[M08] 获取系统与运行时信息
来源：http://hz.gogol.net.cn/gtxshoiusz.html

Py:   platform.system();  platform.python_version()
来源：http://hz.dianchejie.cn/gtwlyndtok.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.svipenyu.cn/gtyzmkqxmq.html

JS:   process.platform;  process.version
来源：http://hz.zhoulong.xyz/gtbwesuspr.html

TS:   process.platform;  process.version
来源：http://hz.chenzaomai.com/gtgtjnjyxh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.sxryk.cn/gthqragvji.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zycfv.cn/gtegiamgcn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ivvv.top/gtormaqgln.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhoulong.xyz/gtuudzjvrt.html

================================================================================
来源：http://hz.yuxming.cn/gtdedluwzp.html

N. 数据结构与算法
来源：http://hz.aizwys.cn/gtfitltqpf.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtwnpdxtgs.html

[N01] 二分查找（有序数组）
来源：http://hz.316326.xyz/gtpecumeaa.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.tanke756.top/gteyvcmuyb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jinqigufen.top/gtyxugnzjr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.nanxuanxn.top/gtmtryefny.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhoulong.xyz/gtedpuwnfw.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.redwolf501.top/gtmfiimuet.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.sweek.top/gttudereeu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.smart0.xyz/gtircxucrm.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.sxryk.cn/gtmvagqcfa.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.haohaochexian.top/gtjnowxovz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sweek.top/gtigibyzgm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.chenjidiqi.icu/gtmczhiucp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sweek.top/gthckbyjnk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.pengpengdd.cyou/gtkzmakots.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.daria6918.cn/gtxflzntai.html

Go:   slices.Sort(arr)
来源：http://hz.svipenyu.cn/gtrqukynob.html

Ruby: arr.sort
来源：http://hz.shangyingyoupin.top/gtthfokeiv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.pengpengdd.cyou/gtmiuamzxn.html

[N03] 快速排序（分治示例）
来源：http://hz.meibo888.top/gtjckasvff.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ydjk.org.cn/gttdvrvjaw.html

PHP:  // 递归实现，或用 usort
来源：http://hz.shzxlz.cn/gtjlpcdfpa.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zycfv.cn/gtcfdiwrwu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.bjfxy.top/gtrtsbtbfi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.cqqwz.cn/gtlrwdlqbx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.xylfe.cn/gtxjebmfkh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yvedp.cn/gtepiljjzs.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ehwqpu.com/gtrjqxwgrc.html

[N04] 斐波那契数列
来源：http://hz.tianlin.xyz/gthwpmktnb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhengqikj.top/gtcdlymzpw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.chenzaomai.com/gtduohfdln.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.havefunace.top/gtiqseunou.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhiwuduotai.top/gteftxluat.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.haohaochexian.top/gtjhmnwftr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.gzhubu.top/gtqepcexab.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jqgufenzy.top/gtbrllkfqj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jinqigufen.top/gttcjrawxs.html

[N05] 最大公约数
来源：http://hz.tanke756.top/gthgcvkgch.html

Py:   math.gcd(a, b)
来源：http://hz.hnqzz.top/gtqwsxbpwr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.chenjidiqi.icu/gtcbpgbcba.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.meibo888.top/gtszubqcyn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gaohongyu789.top/gtzqoicxnd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jyoumei.cn/gtgggqqnru.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.cucudq.cn/gtdlfyyvpp.html

Ruby: a.gcd(b)
来源：http://hz.nanxinkj.top/gtpcxpjgct.html


<!-- 参考信息 -->