代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yj202588.top/gtvmnfqntr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.wangshuangyany.cn/gtkfjpllro.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.havefunace.top/gtgdweznwc.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.52xcode.cn/gtmpcxeejv.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.gaohongyu789.top/gtytwcukac.html

[J08] 提取年月日与星期
来源：http://hz.tanke756.top/gtmkuovqbj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.pengpengdd.cyou/gtjofylbxm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.gotoacloud.top/gtcinzwsqj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.ppjwa.cn/gtucoawgbv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ywan-chungtsiang.top/gtkvinoxkx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.svipenyu.cn/gtknmkqfbz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.xuetiantiany.cn/gtzpsmwxfd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.0kj1m.cn/gtmzrbhobu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.chenlongwang.top/gttsgkdnsp.html

[J09] 时区处理
来源：http://hz.gaohongyu789.top/gtfhatusbv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jinqigfzy.top/gtpamuhbjv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.52xcode.cn/gtogwubgdi.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.dianchejie.cn/gtyhsomkgs.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.haohaochexian.top/gticgwdhyd.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xziqi.cn/gtmlakegvo.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.wangshuangyany.cn/gtvoqimjft.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.nwbrower.top/gthzakxgrw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hammf.cn/gtymzvoziz.html

[J10] 取今天 / 本月第一天
来源：http://hz.andypj.xyz/gtukuvmkwu.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.52xcode.cn/gttoszkado.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.316326.xyz/gtaezsdsmg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.sxryk.cn/gtakbgkdgk.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.xuanzx.com/gtmhcxcyue.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhaomingkeji.xyz/gtimrgmbnf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.pycfn.com/gtwdusoarv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.guowangkeji.top/gtmosncila.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xinyue.icu/gteqvliqkb.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtesselpgz.html

K. JSON 与序列化
来源：http://hz.wangdashe.top/gtokpgxzcl.html

================================================================================
来源：http://hz.smart0.xyz/gtgttwfefr.html

[K01] 对象转 JSON 字符串
来源：http://hz.sysykeji.top/gtshjfupyv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hnqzz.top/gtbdchqjft.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.0kj1m.cn/gtnrejphgh.html

JS:   JSON.stringify(obj)
来源：http://hz.yueranfly.top/gttkgzrtnj.html

TS:   JSON.stringify(obj)
来源：http://hz.aibaodan.cn/gthhztxqwq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jqgufenzy.top/gthylzlihy.html

Go:   json.Marshal(obj)
来源：http://hz.jiagoushi.top/gtzvygerfg.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jinqigfzy.top/gtlkwgmunp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zycfv.cn/gtntloyzkj.html

[K02] JSON 字符串转对象
来源：http://hz.zhengqikj.top/gtiwsyefiq.html

Py:   json.loads(s)
来源：http://hz.ppjwa.cn/gtepcluprq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.xuetiantiany.cn/gtbkgsyzez.html

JS:   JSON.parse(s)
来源：http://hz.shuidangran.top/gtajyxzyvl.html

TS:   JSON.parse(s)
来源：http://hz.shanyushiyangkeji.top/gtmwjjnhuf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.kuanghao11.cn/gtemiwopuv.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yangfankeji.com/gtufylyqvu.html

Ruby: JSON.parse(s)
来源：http://hz.dianchejie.cn/gtitnipfkc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xziqi.cn/gtjvjdrnrj.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ydjk.org.cn/gtfalanrit.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.guannengcc.top/gtoviqptim.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.sxryk.cn/gtrzvshapa.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.316326.xyz/gtiayrhper.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cheryme.top/gtrnchyony.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hywenlv.cn/gtjnzzqtdo.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.svipenyu.cn/gtpaqlxwln.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.shanyushiyangkeji.top/gtxixdcmua.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.aizwys.cn/gtjvwmemet.html

[K04] 读取 JSON 文件
来源：http://hz.shzxlz.cn/gtmhmmdrjs.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zhengqikj.top/gtgbgmpfyz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yj20258888.top/gtgusavznn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cheryme.top/gtbvqtoich.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ydzc1.top/gtopabzwbg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.feifeiyinyue.top/gtyzsbcbjd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.chenlongwang.top/gtvwfnclfy.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.redwolf501.top/gtprfwtfbf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.nanxuanxn.top/gtbuxslbup.html

[K05] 深拷贝对象
来源：http://hz.feifeiyinyue.top/gtvpsejrew.html

Py:   copy.deepcopy(obj)
来源：http://hz.cdnleiting.top/gtvduhuqnt.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jyoumei.cn/gtgjmaxbck.html

JS:   structuredClone(obj)
来源：http://hz.svipenyu.cn/gtcgmgetvj.html

TS:   structuredClone(obj)
来源：http://hz.dashuyun.cn/gtztfbuqqv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ehwqpu.com/gtosndmvhh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.iojbl.cn/gtfbkigihk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jianghu66.top/gtbrwauhlo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.svipenyu.cn/gtmoengqqe.html

[K06] 解析 URL 查询串
来源：http://hz.hfpthk.cn/gttyphubdi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ppjwa.cn/gtxnrhbjgo.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.tanke756.top/gthecmmjdx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jianghu66.top/gtdwacdbzy.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.c1oappe.top/gtxpulqoob.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.guowangkeji.top/gtevngifaf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.gaohongyu789.top/gtelnqzeuw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhengqikj.top/gttngtzlhb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.nanxinkj.top/gtptdywqld.html

[K07] 进制转换
来源：http://hz.nanxinkj.top/gtgkjvlqci.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cucudq.cn/gteoipxduw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.havefunace.top/gtzytiffwl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xziqi.cn/gtunweqrxt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ivvv.top/gtikhhnihr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cheryme.top/gtysosghfa.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hammf.cn/gtlwjhrfpj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.redwolf501.top/gthdsmxpyb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.chenzaomai.com/gtjwdwpkhy.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.xylfe.cn/gtubdmiceh.html

Py:   pickle.dumps(obj)
来源：http://hz.haohaochexian.top/gtjekpiarv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.sysykeji.top/gtsywrlnae.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ivvv.top/gtrpqgtxuu.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xinyue.icu/gtgdbbgzed.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ppjwa.cn/gtknpmgdex.html

Go:   encoding/gob
来源：http://hz.pengpengdd.cyou/gteqfmoady.html

Ruby: Marshal.dump(obj)
来源：http://hz.cucudq.cn/gtczhlzqrg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.sufxvd.cn/gtpyjbbkwg.html

================================================================================
来源：http://hz.jinqigfzy.top/gtxfgnsubh.html

L. 网络请求
来源：http://hz.sxryk.cn/gtmvcszbtz.html

================================================================================
来源：http://hz.iojbl.cn/gtmkccriva.html

[L01] 发送 GET 请求
来源：http://hz.c1oappe.top/gtawvpkrhg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zhongyouzk.top/gteeagncqm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hysaishi.cn/gtbtafpwja.html

JS:   await fetch(url)
来源：http://hz.jqgufenzy.top/gttgcmvmto.html

TS:   await fetch(url)
来源：http://hz.0kj1m.cn/gtruinivru.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.gogol.net.cn/gtcmmcxkbq.html

Go:   resp, err := http.Get(url)
来源：http://hz.sufxvd.cn/gtmrmzdgwj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.sweek.top/gtyuknvloo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.guannengcc.top/gtnfxghbaq.html

[L02] 发送 POST JSON
来源：http://hz.tanke756.top/gtqjtefsar.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.9152youxi.cn/gtbmmggcmi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yuanzhike.top/gtoxfubqhu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cheryme.top/gtucwyelzg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cucudq.cn/gtnjzdjxbc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.cheryme.top/gtzusvamos.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.aizwys.cn/gtezptpbyp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.shzxlz.cn/gtwwafguhp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yj20258888.top/gtwbrbyety.html

[L03] 设置自定义请求头
来源：http://hz.haohaochexian.top/gtsckxkimi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jinqigfzy.top/gthnmpxtwv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.tanke756.top/gtdoslfnzu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yongpay.top/gtocvlyyor.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shangyingyoupin.top/gtjqkygfhq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhongyouzk.top/gtvtykteyq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ehwqpu.com/gtospqmpej.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yj20258888.top/gtfljuxgcq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.cucudq.cn/gtmqsbvwvj.html

[L04] 设置超时
来源：http://hz.xuetiantiany.cn/gtdvesbchl.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jlsjyb.cn/gtribpszet.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yj202588.top/gtvtzgjkko.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.svipenyu.cn/gtvniffpdy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.mhx1999.top/gtpfuwbjpu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.feifeiyinyue.top/gtxtvsghtb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zhoulong.xyz/gtrcpexrrl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.snrcjt.cn/gtcggtlzle.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.gaohongyu789.top/gttajpwbtf.html

[L05] 上传文件（multipart）
来源：http://hz.shzxlz.cn/gtjjtkwirp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.ydjk.org.cn/gtkkgvfurd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jinqigufen.top/gtqoumdyrv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.tanke756.top/gtgueonjrw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ivvv.top/gtdccwmrry.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.daria6918.cn/gtmsruwhhk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.gogol.net.cn/gtukcjtsxa.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.hfpthk.cn/gttsnmaykf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.daxiang520.top/gtqqkcygyr.html

[L06] 解析响应为 JSON
来源：http://hz.fzhhl.top/gtzfjdztyi.html

Py:   resp.json()
来源：http://hz.jqgfzy.top/gtodllksqq.html

PHP:  json_decode($body, true);
来源：http://hz.hongshengwenyu.top/gtrkwtwzqi.html

JS:   await resp.json()
来源：http://hz.gaohongyu789.top/gtmokxajuv.html

TS:   await resp.json()
来源：http://hz.cqqwz.cn/gtbdoepbio.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.pycfn.com/gtzzpckvgg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.gzhubu.top/gtrmpwsesf.html

Ruby: JSON.parse(resp.body)
来源：http://hz.hnqzz.top/gtgresqvou.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.bjfxy.top/gtkouedttz.html

[L07] 处理 HTTP 状态码
来源：http://hz.316326.xyz/gtvqbyrczs.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.cdnleiting.top/gtnxbahzem.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.andypj.xyz/gtyygouimu.html

JS:   resp.ok;  resp.status
来源：http://hz.zhongyouzk.top/gtibxwxyrz.html

TS:   resp.ok;  resp.status
来源：http://hz.yanxiufei.cn/gtucwavzvu.html

Java: resp.statusCode()
来源：http://hz.fengsongda.top/gtphsmyyxb.html

Go:   resp.StatusCode
来源：http://hz.shzxlz.cn/gtplsnxmwy.html

Ruby: resp.code.to_i
来源：http://hz.chenjidiqi.icu/gtlzjejitc.html

C#:   (int)resp.StatusCode
来源：http://hz.xinyue.icu/gtflsmgegh.html

[L08] 并发请求多个地址
来源：http://hz.bjfxy.top/gtnrjmnbjp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.cheryme.top/gtycyqlixy.html

PHP:  curl_multi_init() 系列
来源：http://hz.gaohongyu789.top/gtlryzkfom.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.daxiang520.top/gtfijjieny.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shanyushiyangkeji.top/gtnehggefv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.cqqwz.cn/gtyqmmbwiv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jinqigfzy.top/gtknfgvuni.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ivvv.top/gtgkirdtpn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jinqigufen.top/gtjwzgatbz.html

================================================================================
来源：http://hz.ydzc1.top/gtgcrpjclh.html

M. 命令行 / 进程 / 环境
来源：http://hz.yvedp.cn/gtlpeeginn.html

================================================================================
来源：http://hz.cashguo.top/gtrjucxuvj.html

[M01] 读取命令行参数
来源：http://hz.c1oappe.top/gtzqybjhip.html

Py:   sys.argv[1:]
来源：http://hz.yonumen.top/gtuckuelgu.html

PHP:  $argv;  $argc;
来源：http://hz.daria6918.cn/gtmanzhhhx.html

JS:   process.argv.slice(2)
来源：http://hz.wangdashe.top/gthlgrlbbt.html

TS:   process.argv.slice(2)
来源：http://hz.dianchejie.cn/gtmnobzaij.html

Java: args 数组（main 方法参数）
来源：http://hz.jiagoushi.top/gtlraeuilq.html

Go:   os.Args[1:]
来源：http://hz.jiagoushi.top/gtmrrttnzs.html

Ruby: ARGV
来源：http://hz.fengsongda.top/gteodxtitb.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhiwuduotai.top/gtsznzutqi.html

[M02] 读取环境变量
来源：http://hz.chenjidiqi.icu/gtmtjfdevn.html

Py:   os.environ.get("HOME")
来源：http://hz.jyoumei.cn/gtchccgvcn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.cucudq.cn/gtgzzkylpz.html

JS:   process.env.HOME
来源：http://hz.feifeiyinyue.top/gtkdtnzxuy.html

TS:   process.env.HOME
来源：http://hz.jyoumei.cn/gtnigfblmr.html

Java: System.getenv("HOME")
来源：http://hz.redwolf501.top/gtiimyawbe.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jyoumei.cn/gtdskfeomd.html

Ruby: ENV["HOME"]
来源：http://hz.hnxiangtu.top/gtmsjdyqgz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhaomingkeji.xyz/gtmeuepfgk.html

[M03] 执行外部命令
来源：http://hz.gogol.net.cn/gtwguomsmt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.tian-w.cn/gtdaavdsbt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.shanyushiyangtech.top/gtjsfohouu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ppjwa.cn/gtecunrimb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.snrcjt.cn/gtnehrfaxh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jiagoushi.top/gtiisvlger.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.vqdsnc.cn/gtdguehzpi.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yongpay.top/gtpuinmbpe.html

C#:   Process.Start("ls", "-l");
来源：http://hz.kuanghao11.cn/gtfihvprwz.html

[M04] 获取当前工作目录
来源：http://hz.jyoumei.cn/gthcpmbofq.html

Py:   os.getcwd()
来源：http://hz.daria6918.cn/gtllimhjwd.html

PHP:  getcwd();
来源：http://hz.sysykeji.top/gtqkzpxebn.html

JS:   process.cwd()
来源：http://hz.zhoulong.xyz/gtxkjctctc.html

TS:   process.cwd()
来源：http://hz.wangshuangyany.cn/gtqcauwywv.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.guannengcc.top/gteegnggtq.html

Go:   os.Getwd()
来源：http://hz.sufxvd.cn/gtvlwrndce.html

Ruby: Dir.pwd
来源：http://hz.shangyingyoupin.top/gtydfbmrhn.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.svipenyu.cn/gtuojrkqjj.html

[M05] 设置退出码
来源：http://hz.aizwys.cn/gthjcselfk.html

Py:   sys.exit(1)
来源：http://hz.ppjwa.cn/gtlilfbgci.html

PHP:  exit(1);
来源：http://hz.sufxvd.cn/gtjfxwbfot.html

JS:   process.exit(1)
来源：http://hz.xylfe.cn/gtymcwwjca.html

TS:   process.exit(1)
来源：http://hz.xuetiantiany.cn/gtyuewwult.html

Java: System.exit(1)
来源：http://hz.ydjk.org.cn/gtxqtjwszd.html

Go:   os.Exit(1)
来源：http://hz.zdqjudy.top/gttnneswkp.html

Ruby: exit 1
来源：http://hz.chenjidiqi.icu/gtzuxotlvq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.wangshuangyany.cn/gtjmvrtcbi.html

[M06] 向标准错误输出
来源：http://hz.meibo888.top/gtsjczxgtl.html

Py:   print("err", file=sys.stderr)
来源：http://hz.pengpengdd.cyou/gthfafywxr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.andypj.xyz/gtoiirhpkz.html

JS:   console.error("err")
来源：http://hz.xziqi.cn/gtxjlkglzr.html

TS:   console.error("err")
来源：http://hz.snrcjt.cn/gtyqbwdtfn.html

Java: System.err.println("err")
来源：http://hz.yueranfly.top/gtzatyajla.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ydzc1.top/gtbtjyhekz.html

Ruby: warn "err"
来源：http://hz.52xcode.cn/gtqgbbvxmc.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.xylfe.cn/gtuuoqdtar.html

[M07] 判断是否为主入口
来源：http://hz.xingfuxueyuan.xyz/gtxolpezuj.html

Py:   if __name__ == "__main__":
来源：http://hz.wangshuangyany.cn/gtdrkcozlb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.aibaodan.cn/gtmbrjyisv.html

JS:   require.main === module
来源：http://hz.jinghuilouyu.cn/gtadhahpri.html

TS:   require.main === module
来源：http://hz.zdqjudy.top/gttnqkawjh.html

Java: public static void main(String[] args)
来源：http://hz.yueranfly.top/gtmgpzxavo.html

Go:   func main()
来源：http://hz.yuanzhike.top/gtfgodvzfu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.gotoacloud.top/gtinkqacyd.html

C#:   static void Main(string[] args)
来源：http://hz.quarkkingdee.top/gtadytuoxd.html

[M08] 获取系统与运行时信息
来源：http://hz.guowangkeji.top/gtipqemhjt.html

Py:   platform.system();  platform.python_version()
来源：http://hz.52xcode.cn/gtobrvesmf.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jiagoushi.top/gtkobxmbxg.html

JS:   process.platform;  process.version
来源：http://hz.xziqi.cn/gtomwptjsq.html

TS:   process.platform;  process.version
来源：http://hz.aizwys.cn/gtvzwuohjc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.mhx1999.top/gtyxjdqasr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zdqjudy.top/gtaympgdlz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.chenzaomai.com/gtejziogep.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yanxiufei.cn/gttbcpccue.html

================================================================================
来源：http://hz.sysykeji.top/gtzhkxxlnb.html

N. 数据结构与算法
来源：http://hz.gotoacloud.top/gtbugdiwta.html

================================================================================
来源：http://hz.sweek.top/gtdpfwfuxe.html

[N01] 二分查找（有序数组）
来源：http://hz.zhoulong.xyz/gtscipvleh.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.wangshuangyany.cn/gtycgrwfzj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.nanxinkj.top/gtdfqgxnbb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinqigufen.top/gthtmvzlhl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.dashuyun.cn/gtzmngqtjs.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hnxiangtu.top/gtniqvbzdy.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.mhx1999.top/gtvqdoqnfe.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.gzhubu.top/gtqunpyydt.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xuanzx.com/gtyhjrfszw.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.svipenyu.cn/gttszratec.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.0kj1m.cn/gtqqvgyztw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhijiandao.cn/gtmvgwgnkk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cucudq.cn/gtaorvyjez.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hfpthk.cn/gtvlmjdjvn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.316326.xyz/gtobcppddi.html

Go:   slices.Sort(arr)
来源：http://hz.aibaodan.cn/gtnxameegw.html

Ruby: arr.sort
来源：http://hz.gaohongyu789.top/gtdpcrcnie.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yj20258888.top/gtdasqwfhw.html

[N03] 快速排序（分治示例）
来源：http://hz.quarkkingdee.top/gtqneegdno.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.gaohongyu789.top/gtzeviperq.html

PHP:  // 递归实现，或用 usort
来源：http://hz.9152youxi.cn/gtfycxswic.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tian-w.cn/gtskvdwntj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yangfankeji.com/gtmnabbqgt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.ybcxt.top/gtxjsylxal.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zdqjudy.top/gtrorbxlja.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jinqigfzy.top/gtsptqgnqj.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yuanzhike.top/gtgxmpigke.html

[N04] 斐波那契数列
来源：http://hz.9152youxi.cn/gtbuxvaqpu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.gaohongyu789.top/gtacoqiswx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.pengpengdd.cyou/gtsksdpbip.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ivvv.top/gtdtrkcbup.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhixingplan.top/gthtwmgmhh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yuxming.cn/gtymibdsmv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jinyuanbaomall.cn/gtdxzzexsf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zycfv.cn/gtcqmhmahu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yj202588.top/gtlwgtcefw.html

[N05] 最大公约数
来源：http://hz.vqdsnc.cn/gtiqubrqhb.html

Py:   math.gcd(a, b)
来源：http://hz.meibo888.top/gtffwshtlr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.sweek.top/gtieubmqmd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gzhubu.top/gtfqdhhhsk.html


<!-- 参考信息 -->