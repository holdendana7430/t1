代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yuanzhike.top/gthntbfrng.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.c1oappe.top/gtkybymfeu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yanxiufei.cn/gtsatfkwng.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hongshengwenyu.top/gtflhdinxl.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.bjfxy.top/gtwxjtajqh.html

[J08] 提取年月日与星期
来源：http://hz.shzxlz.cn/gtkukyhrqz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.haohaochexian.top/gtzrbznvri.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jqgfzy.top/gtkgqzchqp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jlsjyb.cn/gtdaladrii.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.0kj1m.cn/gtnyvqkqcz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.mhx1999.top/gtdpzaytny.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jianghu66.top/gtayhocamy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.smart0.xyz/gtqmtljsfy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.havefunace.top/gtqgvyekgc.html

[J09] 时区处理
来源：http://hz.jianghu66.top/gtsgyuunps.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cdnleiting.top/gtyrlrwzmm.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.nanxuanxn.top/gtobisfxtj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhaomingkeji.xyz/gtebdwxaxd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nanxinkj.top/gthblpeawo.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.shanyushiyangtech.top/gtgakmsith.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hammf.cn/gttdioneli.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.aizwys.cn/gtlumfekkp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.quarkkingdee.top/gtcydnlykb.html

[J10] 取今天 / 本月第一天
来源：http://hz.hnqzz.top/gtnfpfkvsa.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.gaohongyu789.top/gtibymcofh.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.gotoacloud.top/gtltehgdjn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ydzc1.top/gtjqxamabs.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhoulong.xyz/gtfsjwogom.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.wangdashe.top/gtpnnhkidm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.cheryme.top/gtbhmoqiil.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.snrcjt.cn/gtdsbsbllu.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.sufxvd.cn/gthetnrrkg.html

================================================================================
来源：http://hz.pengpengdd.cyou/gteghpquxp.html

K. JSON 与序列化
来源：http://hz.nanxuanxn.top/gtdumuisfm.html

================================================================================
来源：http://hz.ehwqpu.com/gtzytsixtj.html

[K01] 对象转 JSON 字符串
来源：http://hz.dianchejie.cn/gtxsrivjqa.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.nanxinkj.top/gtvxsppnzi.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.shanyushiyangtech.top/gtvcspmrrm.html

JS:   JSON.stringify(obj)
来源：http://hz.zhaomingkeji.xyz/gtllgrdojj.html

TS:   JSON.stringify(obj)
来源：http://hz.cqqwz.cn/gtluilvgtl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jiagoushi.top/gtnjynmrur.html

Go:   json.Marshal(obj)
来源：http://hz.jlsjyb.cn/gtescohxrc.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.c1oappe.top/gtduyqacuh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ivvv.top/gtzyflotwl.html

[K02] JSON 字符串转对象
来源：http://hz.xuanzx.com/gtfjehohcg.html

Py:   json.loads(s)
来源：http://hz.jyoumei.cn/gtrncijpof.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.shzxlz.cn/gtmisqbfpm.html

JS:   JSON.parse(s)
来源：http://hz.yueranfly.top/gtrdrbndsp.html

TS:   JSON.parse(s)
来源：http://hz.yonumen.top/gtbludhnix.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yonumen.top/gtrfivxcsh.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xylfe.cn/gtzyoxzvbf.html

Ruby: JSON.parse(s)
来源：http://hz.hysaishi.cn/gtmrpjispu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yongpay.top/gtmylqoyqo.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.fzhhl.top/gtswvriysg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.tian-w.cn/gtdpgqsogq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.xuanzx.com/gtypgzigtr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj20258.top/gtufvputsm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.gogol.net.cn/gtebhxuzok.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.pengpengdd.cyou/gtrraxchqj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.nanxinkj.top/gtezsqpbcy.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ppjwa.cn/gtjegkihsl.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.gotoacloud.top/gtorupnyzt.html

[K04] 读取 JSON 文件
来源：http://hz.yanxiufei.cn/gtljwplhvn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yj20258888.top/gtiaovoneq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.aibaodan.cn/gtcodrgnin.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hnqzz.top/gtkvelzziv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ydzc1.top/gtzkdbewff.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jianghu66.top/gtvghugyak.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.sufxvd.cn/gtkguavunl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ydzc1.top/gtothybjps.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhoulong.xyz/gtrjhcbkxs.html

[K05] 深拷贝对象
来源：http://hz.fengsongda.top/gtppykcrjw.html

Py:   copy.deepcopy(obj)
来源：http://hz.hammf.cn/gtrmnufhcw.html

PHP:  unserialize(serialize($obj));
来源：http://hz.guannengcc.top/gtpdtuyivm.html

JS:   structuredClone(obj)
来源：http://hz.jinyuanbaomall.cn/gtmetpdeoy.html

TS:   structuredClone(obj)
来源：http://hz.vqdsnc.cn/gtlhtxkgrp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.c1oappe.top/gteafxzyiz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ybcxt.top/gtoijrrocc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ppjwa.cn/gtyhcgsagu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ehwqpu.com/gtstlsgprc.html

[K06] 解析 URL 查询串
来源：http://hz.guannengcc.top/gtgvgdqzzz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xuanzx.com/gtcbxzkzxj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.nanxinkj.top/gtzhgyystz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shangyingyoupin.top/gtjjzbdkay.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cucudq.cn/gtenfhckis.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.gzhubu.top/gtknnmrlmf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hammf.cn/gtwfbtvjtt.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.chenzaomai.com/gttyostdwa.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.xziqi.cn/gtejnwcffb.html

[K07] 进制转换
来源：http://hz.feifeiyinyue.top/gtelsjmjvg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.dashuyun.cn/gtlobjphcu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.shuidangran.top/gtlzllilny.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.guowangkeji.top/gtkfgxdxcz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jinghuilouyu.cn/gtrhrctalq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hnqzz.top/gttoesxekt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.gogol.net.cn/gttvlexecd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xuanzx.com/gtjfvmfgkz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.sysykeji.top/gtvksdwaod.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ehwqpu.com/gtvdborinh.html

Py:   pickle.dumps(obj)
来源：http://hz.yongpay.top/gtosldchdx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.mhx1999.top/gtitoffmql.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.cdnleiting.top/gtgwpnubos.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.dianchejie.cn/gtahlnbkhd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yuanzhike.top/gtgxsrnzlf.html

Go:   encoding/gob
来源：http://hz.yongpay.top/gtbzzmhfwg.html

Ruby: Marshal.dump(obj)
来源：http://hz.sysykeji.top/gtuisewsyl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.hfpthk.cn/gtlqlqueau.html

================================================================================
来源：http://hz.chenzaomai.com/gtvqkzscfa.html

L. 网络请求
来源：http://hz.zhixingplan.top/gtcpwhfpng.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtivscihau.html

[L01] 发送 GET 请求
来源：http://hz.yonumen.top/gtukpkluvt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.tian-w.cn/gttfsjzehr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.wangdashe.top/gtxdrmndhn.html

JS:   await fetch(url)
来源：http://hz.9152youxi.cn/gteehbryit.html

TS:   await fetch(url)
来源：http://hz.quarkkingdee.top/gtqfsbcvhx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.dashuyun.cn/gtnshtlcex.html

Go:   resp, err := http.Get(url)
来源：http://hz.birdmap.top/gtmvjmxlhj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.ywan-chungtsiang.top/gtywimvlkc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zhixingplan.top/gtzhpmbfip.html

[L02] 发送 POST JSON
来源：http://hz.jlsjyb.cn/gtizqgyync.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ppjwa.cn/gtiukfdxll.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.smart0.xyz/gtprxbtpqd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sufxvd.cn/gtfhqxstlf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yongpay.top/gtnpoijcux.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.kuanghao11.cn/gtjfprelxj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.cqqwz.cn/gthqlixabu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhengqikj.top/gtekehygny.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jinqigfzy.top/gttwtnqgsy.html

[L03] 设置自定义请求头
来源：http://hz.mhx1999.top/gtjdgxzujy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.snrcjt.cn/gthshpcvdd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.sufxvd.cn/gtpykzopem.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.guannengcc.top/gttillolgl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.feifeiyinyue.top/gtqcdpitjk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.sweek.top/gtmekpeytb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.nwbrower.top/gtocsylzkv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jqgufenzy.top/gtysavswed.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ywan-chungtsiang.top/gtqlpneazp.html

[L04] 设置超时
来源：http://hz.jqgufenzy.top/gtjitoibbf.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zhijiandao.cn/gtdemuogii.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.havefunace.top/gtokpxvtgp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.haohaochexian.top/gtyecirpyh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nwbrower.top/gtsbtndveg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.meibo888.top/gtyagoxmyo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.daxiang520.top/gtitrxdilx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.havefunace.top/gtuxqijxrb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.daxiang520.top/gtvcbbnixf.html

[L05] 上传文件（multipart）
来源：http://hz.shanyushiyangtech.top/gtsamvrxvj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.haohaochexian.top/gtsykrrufq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jqgufenzy.top/gthrfemimj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.nwbrower.top/gtxklmrvjm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jianghu66.top/gteeptzcsd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.haohaochexian.top/gtnxdsxyaa.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhengqikj.top/gtlzleuetk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jqgfzy.top/gtalwopjwo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yj20258.top/gtysuhgfjc.html

[L06] 解析响应为 JSON
来源：http://hz.sweek.top/gtsurfdjah.html

Py:   resp.json()
来源：http://hz.pycfn.com/gtakjhmbna.html

PHP:  json_decode($body, true);
来源：http://hz.sysykeji.top/gtmkmlhdkl.html

JS:   await resp.json()
来源：http://hz.xuetiantiany.cn/gtxicweobd.html

TS:   await resp.json()
来源：http://hz.ydzc1.top/gtbbygffay.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.gogol.net.cn/gtxpxezdjc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.shangyingyoupin.top/gtsgqqfvfq.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhijiandao.cn/gtnuvvaxho.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.wangdashe.top/gtlqwkhbwz.html

[L07] 处理 HTTP 状态码
来源：http://hz.9152youxi.cn/gtkxkvykwc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.ydjk.org.cn/gthyffteye.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.meibo888.top/gtgneboebz.html

JS:   resp.ok;  resp.status
来源：http://hz.yuxming.cn/gtwpbjmjzf.html

TS:   resp.ok;  resp.status
来源：http://hz.jinghuilouyu.cn/gtutjceosd.html

Java: resp.statusCode()
来源：http://hz.fzhhl.top/gtvhyjrfig.html

Go:   resp.StatusCode
来源：http://hz.bjfxy.top/gtatbhldlv.html

Ruby: resp.code.to_i
来源：http://hz.yj20258888.top/gttwppdzvx.html

C#:   (int)resp.StatusCode
来源：http://hz.hnxiangtu.top/gtdmnpflxc.html

[L08] 并发请求多个地址
来源：http://hz.ehwqpu.com/gtbqzzrmbx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zdqjudy.top/gtbsaatvvy.html

PHP:  curl_multi_init() 系列
来源：http://hz.316326.xyz/gtpwzntcmf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yanxiufei.cn/gtbgimckbp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhongyouzk.top/gtjbnbozxa.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yanxiufei.cn/gtmqdpaoch.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hnxiangtu.top/gtfefqvncy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.shzxlz.cn/gtxojrootl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hnxiangtu.top/gtryazytfx.html

================================================================================
来源：http://hz.svipenyu.cn/gttklaanxi.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhijiandao.cn/gtwuuztfll.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtsjsvnsyd.html

[M01] 读取命令行参数
来源：http://hz.xingfuxueyuan.xyz/gtaalltdlo.html

Py:   sys.argv[1:]
来源：http://hz.hnqzz.top/gtjfaaivll.html

PHP:  $argv;  $argc;
来源：http://hz.zhixingplan.top/gtacjdxvyz.html

JS:   process.argv.slice(2)
来源：http://hz.quarkkingdee.top/gtoeorfssq.html

TS:   process.argv.slice(2)
来源：http://hz.hongshengwenyu.top/gtcksgtjch.html

Java: args 数组（main 方法参数）
来源：http://hz.shanyushiyangkeji.top/gtqwmfnjwn.html

Go:   os.Args[1:]
来源：http://hz.meibo888.top/gtbvosnjil.html

Ruby: ARGV
来源：http://hz.yuxming.cn/gtgozxtidx.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ydzc1.top/gtrddeyaaa.html

[M02] 读取环境变量
来源：http://hz.wangdashe.top/gtrgxntpjk.html

Py:   os.environ.get("HOME")
来源：http://hz.shanyushiyangtech.top/gtexyppyyu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.gotoacloud.top/gtqlmhahhp.html

JS:   process.env.HOME
来源：http://hz.zhoulong.xyz/gtitvfqpdh.html

TS:   process.env.HOME
来源：http://hz.pycfn.com/gtfjiyzzwb.html

Java: System.getenv("HOME")
来源：http://hz.yueranfly.top/gtmudvesud.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yj202588.top/gteizvcnlt.html

Ruby: ENV["HOME"]
来源：http://hz.xziqi.cn/gthsmisuiv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.gzhubu.top/gthqbufsiz.html

[M03] 执行外部命令
来源：http://hz.sufxvd.cn/gtjxyspvtg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhaomingkeji.xyz/gtfqhinyao.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.c1oappe.top/gtxzkmtkxi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.shzxlz.cn/gtrbplduxj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.pengpengdd.cyou/gtjskntquq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.xuetiantiany.cn/gtxxivxgli.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.meibo888.top/gtsvrthgus.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.smart0.xyz/gtvdfwjajp.html

C#:   Process.Start("ls", "-l");
来源：http://hz.nanxinkj.top/gtojxwzlih.html

[M04] 获取当前工作目录
来源：http://hz.0kj1m.cn/gththxblxm.html

Py:   os.getcwd()
来源：http://hz.shangyingyoupin.top/gtfzjcypld.html

PHP:  getcwd();
来源：http://hz.yvedp.cn/gtlbboabdn.html

JS:   process.cwd()
来源：http://hz.jqgfzy.top/gttycglevg.html

TS:   process.cwd()
来源：http://hz.iojbl.cn/gtmotkixxk.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hywenlv.cn/gtwzubzmft.html

Go:   os.Getwd()
来源：http://hz.gaohongyu789.top/gtimshtwer.html

Ruby: Dir.pwd
来源：http://hz.hywenlv.cn/gtpnomsogz.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jinyuanbaomall.cn/gtajkbhnil.html

[M05] 设置退出码
来源：http://hz.snrcjt.cn/gttsnzvqrx.html

Py:   sys.exit(1)
来源：http://hz.pengpengdd.cyou/gtqbvafpzt.html

PHP:  exit(1);
来源：http://hz.sweek.top/gtreolqqbi.html

JS:   process.exit(1)
来源：http://hz.kuanghao11.cn/gtwwfzsqig.html

TS:   process.exit(1)
来源：http://hz.tianlin.xyz/gtwafdhsek.html

Java: System.exit(1)
来源：http://hz.shzxlz.cn/gttiwwfouq.html

Go:   os.Exit(1)
来源：http://hz.quarkkingdee.top/gtcvujlmza.html

Ruby: exit 1
来源：http://hz.pycfn.com/gtgxmvzfhp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.guowangkeji.top/gtphajjfjm.html

[M06] 向标准错误输出
来源：http://hz.tianlin.xyz/gtqalfglns.html

Py:   print("err", file=sys.stderr)
来源：http://hz.iojbl.cn/gtkmfqoonf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.c1oappe.top/gtlcoirsdy.html

JS:   console.error("err")
来源：http://hz.zdqjudy.top/gtlpbzdqws.html

TS:   console.error("err")
来源：http://hz.hnxiangtu.top/gtvgnzsfek.html

Java: System.err.println("err")
来源：http://hz.shangyingyoupin.top/gttqhkboxs.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.havefunace.top/gtiuoieono.html

Ruby: warn "err"
来源：http://hz.shuidangran.top/gtcwdjlcbd.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jinqigfzy.top/gtziqldnzy.html

[M07] 判断是否为主入口
来源：http://hz.ppjwa.cn/gtsqotskji.html

Py:   if __name__ == "__main__":
来源：http://hz.gogol.net.cn/gtywvrebwp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.guannengcc.top/gtiumjelmp.html

JS:   require.main === module
来源：http://hz.hfpthk.cn/gtkhpfhegt.html

TS:   require.main === module
来源：http://hz.yangfankeji.com/gtjzlddoev.html

Java: public static void main(String[] args)
来源：http://hz.yanxiufei.cn/gteupbvzik.html

Go:   func main()
来源：http://hz.yangfankeji.com/gtokeurrcy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.snrcjt.cn/gtjfxfdywr.html

C#:   static void Main(string[] args)
来源：http://hz.ppjwa.cn/gtfdjcafrb.html

[M08] 获取系统与运行时信息
来源：http://hz.mhx1999.top/gtozvenaha.html

Py:   platform.system();  platform.python_version()
来源：http://hz.cqqwz.cn/gtyfmqsadm.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jinghuilouyu.cn/gtbnjoiypg.html

JS:   process.platform;  process.version
来源：http://hz.hnxiangtu.top/gtyirhnoam.html

TS:   process.platform;  process.version
来源：http://hz.zhoulong.xyz/gtrrjpbiby.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.ybcxt.top/gtqdctqnpa.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.svipenyu.cn/gtnbblokha.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.nwbrower.top/gtjcemlqtv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hnqzz.top/gtkstdfqoq.html

================================================================================
来源：http://hz.jianghu66.top/gtbbwdhnhr.html

N. 数据结构与算法
来源：http://hz.yongpay.top/gtillylaxu.html

================================================================================
来源：http://hz.gaohongyu789.top/gtrfwaikws.html

[N01] 二分查找（有序数组）
来源：http://hz.xinyue.icu/gtckfvhvoh.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yj202588.top/gtotcuhxxu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jyoumei.cn/gtfjrmbyjq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yj20258.top/gtnktdvpvu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shzxlz.cn/gtdzigzmfm.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yuxming.cn/gtndddlqme.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jqgufenzy.top/gtjbtjgaoe.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.aibaodan.cn/gtompehxqi.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.smart0.xyz/gtgjfopffb.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.gzhubu.top/gtlngrghbh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sxryk.cn/gtsuszfovt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jianghu66.top/gtdwhgmtso.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gogol.net.cn/gtxidpkdvn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hnxiangtu.top/gtwedxilir.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.shzxlz.cn/gtsoukpuyl.html

Go:   slices.Sort(arr)
来源：http://hz.shanyushiyangtech.top/gtjoibcpdz.html

Ruby: arr.sort
来源：http://hz.ppjwa.cn/gtbzdfhthu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.xziqi.cn/gtdrzfavfq.html

[N03] 快速排序（分治示例）
来源：http://hz.yj20258888.top/gtxpmjbbaw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.mhx1999.top/gtfudzxloc.html

PHP:  // 递归实现，或用 usort
来源：http://hz.gotoacloud.top/gtervfjopz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cashguo.top/gtvdjrxayq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.sysykeji.top/gtvvqeeifa.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.daxiang520.top/gtcyvbvbdi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jiagoushi.top/gtpbfucjjm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.wangshuangyany.cn/gtjlgkcroj.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.haohaochexian.top/gtzmdpyauf.html

[N04] 斐波那契数列
来源：http://hz.chenlongwang.top/gtugkitain.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.c1oappe.top/gtgbkqpanq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zycfv.cn/gtppjqkmkf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.pycfn.com/gtqirxklfn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.dashuyun.cn/gtukqisgph.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.shzxlz.cn/gtcqrtwiax.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yj202588.top/gttitbxgcz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.xziqi.cn/gturvvjvss.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xingfuxueyuan.xyz/gtzmtmcpwj.html

[N05] 最大公约数
来源：http://hz.redwolf501.top/gtgtnzirjb.html

Py:   math.gcd(a, b)
来源：http://hz.xziqi.cn/gtblnvkjae.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.guowangkeji.top/gttznvaphp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.birdmap.top/gtgucflqvg.html


<!-- 参考信息 -->