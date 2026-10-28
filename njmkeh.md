代发 wailian999

[J07] 比较两个日期
来源：http://hz.hfpthk.cn/gtqsxyqefj.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.guowangkeji.top/gtxhhtbiwn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hongshengwenyu.top/gtmogoclex.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zycfv.cn/gtubtwanbp.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.kuanghao11.cn/gthajmefip.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhixingplan.top/gtqdtdhtmz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yj20258888.top/gthgjrmvzp.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yanxiufei.cn/gtvpbcbecs.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hfpthk.cn/gtvgtoshbr.html

[J08] 提取年月日与星期
来源：http://hz.shanyushiyangkeji.top/gtkhjlxsmg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.c1oappe.top/gtnvizpkbe.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.daxiang520.top/gtywcysxgd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.wangshuangyany.cn/gthobfwnvz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.gaohongyu789.top/gtnznggnxd.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hammf.cn/gttdprybqv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zycfv.cn/gtduzquzhf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jiagoushi.top/gtlwovfdbz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.wangdashe.top/gtexwrbyrx.html

[J09] 时区处理
来源：http://hz.daria6918.cn/gtgdqzilwf.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.chenlongwang.top/gtxnblyblp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.0kj1m.cn/gtcuijbtmj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yangfankeji.com/gthqomouhf.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cashguo.top/gtigtzyvtx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yuxming.cn/gtvywxhleo.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.birdmap.top/gtxgjqiixs.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hnqzz.top/gtiralbfer.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.guannengcc.top/gtzhedaojj.html

[J10] 取今天 / 本月第一天
来源：http://hz.yongpay.top/gtouxnngmg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jinghuilouyu.cn/gtzjsmvhxv.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.c1oappe.top/gtfiscpjbt.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ehwqpu.com/gtxmlimqcq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yongpay.top/gttkmqdlby.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.daxiang520.top/gtumxafvyy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xuanzx.com/gtgaymorau.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.redwolf501.top/gtwadlpxfx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.gzhubu.top/gtliflvbvq.html

================================================================================
来源：http://hz.zhoulong.xyz/gtorhnginu.html

K. JSON 与序列化
来源：http://hz.xuetiantiany.cn/gtnmaopdne.html

================================================================================
来源：http://hz.wangdashe.top/gtqwwntfxq.html

[K01] 对象转 JSON 字符串
来源：http://hz.sufxvd.cn/gtwlfalnks.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.wangdashe.top/gtuwtqiqsm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.daxiang520.top/gteztsvmwv.html

JS:   JSON.stringify(obj)
来源：http://hz.redwolf501.top/gtjdksmdyp.html

TS:   JSON.stringify(obj)
来源：http://hz.haohaochexian.top/gtgqtrvsit.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yj20258888.top/gtgcqixrih.html

Go:   json.Marshal(obj)
来源：http://hz.daria6918.cn/gtwuqtssvu.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.birdmap.top/gtbhcsgoys.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.andypj.xyz/gtvjnhajip.html

[K02] JSON 字符串转对象
来源：http://hz.jiagoushi.top/gtcwbmafzc.html

Py:   json.loads(s)
来源：http://hz.jlsjyb.cn/gtjzwgpquf.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hongshengwenyu.top/gtotqxesrj.html

JS:   JSON.parse(s)
来源：http://hz.fengsongda.top/gtfgggjrmr.html

TS:   JSON.parse(s)
来源：http://hz.shuidangran.top/gtrjilsgdp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yueranfly.top/gtakadmwvd.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yj20258.top/gtbwilqfxm.html

Ruby: JSON.parse(s)
来源：http://hz.yvedp.cn/gtidegeuho.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.kuanghao11.cn/gtgffndggf.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hongshengwenyu.top/gtobdwwclf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.smart0.xyz/gtlfthyhtf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhoulong.xyz/gtemjrpqju.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xingfuxueyuan.xyz/gtdfnqatiz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.shangyingyoupin.top/gtpntghjyp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hammf.cn/gtxcjxphgd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xuetiantiany.cn/gtpkqoxarg.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ydzc1.top/gtknzppdks.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.nanxuanxn.top/gtroukcdhc.html

[K04] 读取 JSON 文件
来源：http://hz.meibo888.top/gtxkcbnctd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.sysykeji.top/gtyeomdjut.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.birdmap.top/gtdclkgpzc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinqigfzy.top/gtlrkaaqkx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.aizwys.cn/gthhjcadvx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.shanyushiyangkeji.top/gtpbjewrry.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.aizwys.cn/gtqabacpke.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.feifeiyinyue.top/gtqnavzlpi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.chenlongwang.top/gtoytecuwk.html

[K05] 深拷贝对象
来源：http://hz.pycfn.com/gtkbdmycii.html

Py:   copy.deepcopy(obj)
来源：http://hz.316326.xyz/gtjzpsjxzl.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hongshengwenyu.top/gtzgcbmpkk.html

JS:   structuredClone(obj)
来源：http://hz.guowangkeji.top/gtufeaqskv.html

TS:   structuredClone(obj)
来源：http://hz.haohaochexian.top/gtfuyhmhfs.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.aizwys.cn/gtnykizgoy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zdqjudy.top/gtycckpnyq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yueranfly.top/gtiqrrefba.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.sxryk.cn/gtcymuiskd.html

[K06] 解析 URL 查询串
来源：http://hz.nwbrower.top/gtnhdcpcvy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.aibaodan.cn/gtsbcxnsjd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.tanke756.top/gteetwdtvm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yanxiufei.cn/gtlkjyqzov.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhaomingkeji.xyz/gtwngeijab.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.tianlin.xyz/gtozgxnhyc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhijiandao.cn/gtsglxibii.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.nwbrower.top/gtffuaigvc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhiwuduotai.top/gtrmlpfvuu.html

[K07] 进制转换
来源：http://hz.yueranfly.top/gtxpqoggyw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhongyouzk.top/gtopqklchj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.nanxinkj.top/gtxbgblcop.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.quarkkingdee.top/gtdkqblako.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.sxryk.cn/gtnyihrilm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.gzhubu.top/gtwjzqiblj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.guowangkeji.top/gtthvaaeef.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.redwolf501.top/gtcrtzmdyj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ppjwa.cn/gtqewzvoyt.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.xinyue.icu/gtbgyptfhi.html

Py:   pickle.dumps(obj)
来源：http://hz.shangyingyoupin.top/gtjtizslee.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.dashuyun.cn/gtwbtdtzqx.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.wangdashe.top/gtotlztifc.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.snrcjt.cn/gtytqfzygx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ywan-chungtsiang.top/gtwtfewpmp.html

Go:   encoding/gob
来源：http://hz.nwbrower.top/gtveaqyrur.html

Ruby: Marshal.dump(obj)
来源：http://hz.52xcode.cn/gtqxdafavm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.hammf.cn/gtjjpqfyio.html

================================================================================
来源：http://hz.yvedp.cn/gtmjyheoou.html

L. 网络请求
来源：http://hz.xuanzx.com/gtuejjhdvn.html

================================================================================
来源：http://hz.cdnleiting.top/gtrgpubqqb.html

[L01] 发送 GET 请求
来源：http://hz.nanxuanxn.top/gtbfnykexm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.sxryk.cn/gtecmitizw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.tanke756.top/gteadeglad.html

JS:   await fetch(url)
来源：http://hz.guannengcc.top/gtaxjkngef.html

TS:   await fetch(url)
来源：http://hz.sysykeji.top/gtzrkasghc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hywenlv.cn/gtgjnfquri.html

Go:   resp, err := http.Get(url)
来源：http://hz.dashuyun.cn/gtwfssilnp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.fengsongda.top/gtndpkfxxy.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.pycfn.com/gtrnlndate.html

[L02] 发送 POST JSON
来源：http://hz.fzhhl.top/gtwqcdaahf.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.redwolf501.top/gtgyvbpbra.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yvedp.cn/gtbcuefmen.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.iojbl.cn/gtkxbbgida.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhixingplan.top/gtpqpqfgtg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.shanyushiyangtech.top/gtjkafweaj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.shuidangran.top/gtreutusys.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhoulong.xyz/gttkizepqo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.c1oappe.top/gteceeisji.html

[L03] 设置自定义请求头
来源：http://hz.aizwys.cn/gtnmbyeyoe.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xuanzx.com/gtriciumam.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.daxiang520.top/gtqyljjhaz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.havefunace.top/gtuigidejq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.snrcjt.cn/gthsmbyuzz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.svipenyu.cn/gtrxiowbhj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yj202588.top/gtypyuassu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.cashguo.top/gthryglkwd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.shuidangran.top/gtsjchddos.html

[L04] 设置超时
来源：http://hz.daria6918.cn/gtwjxhznsf.html

Py:   requests.get(url, timeout=5)
来源：http://hz.daria6918.cn/gtdyguzqnc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.quarkkingdee.top/gtpjilouuf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hnxiangtu.top/gtfxepttoy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hammf.cn/gtfxopexjb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhijiandao.cn/gthzbuujpz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.cheryme.top/gtvmvvgtep.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.0kj1m.cn/gtdxlsmrsg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhijiandao.cn/gtrmilndau.html

[L05] 上传文件（multipart）
来源：http://hz.fzhhl.top/gtqdjmuwjy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.fengsongda.top/gtxqxivcjh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xingfuxueyuan.xyz/gtgvbrbegu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.dianchejie.cn/gtetosjoam.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ivvv.top/gtmoldrihg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.c1oappe.top/gtiazrqjtn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yonumen.top/gtvugtgizn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.chenzaomai.com/gtcrobyrri.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtnfqhwtbx.html

[L06] 解析响应为 JSON
来源：http://hz.yonumen.top/gtpyghgzrr.html

Py:   resp.json()
来源：http://hz.52xcode.cn/gtgykxnhcp.html

PHP:  json_decode($body, true);
来源：http://hz.aizwys.cn/gtzlqoszph.html

JS:   await resp.json()
来源：http://hz.xuetiantiany.cn/gtxhmvaach.html

TS:   await resp.json()
来源：http://hz.dianchejie.cn/gtmeocttuh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.guowangkeji.top/gtnibddduf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zycfv.cn/gtbavfyngf.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jiagoushi.top/gtslohjnan.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhengqikj.top/gtyrhyfbke.html

[L07] 处理 HTTP 状态码
来源：http://hz.hnxiangtu.top/gthexlbcon.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhengqikj.top/gtzfjrxdtv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhiwuduotai.top/gtpuuxfnvk.html

JS:   resp.ok;  resp.status
来源：http://hz.chenjidiqi.icu/gtvugshuqn.html

TS:   resp.ok;  resp.status
来源：http://hz.zdqjudy.top/gtihuxmkmz.html

Java: resp.statusCode()
来源：http://hz.shanyushiyangtech.top/gtnnftjkky.html

Go:   resp.StatusCode
来源：http://hz.9152youxi.cn/gtonaqhklh.html

Ruby: resp.code.to_i
来源：http://hz.shanyushiyangkeji.top/gtofusdykc.html

C#:   (int)resp.StatusCode
来源：http://hz.yongpay.top/gtgzybvysr.html

[L08] 并发请求多个地址
来源：http://hz.iojbl.cn/gtklagynzv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.chenlongwang.top/gtzxdexatb.html

PHP:  curl_multi_init() 系列
来源：http://hz.ehwqpu.com/gtgmgjckwm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yongpay.top/gtvsjtbuup.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yvedp.cn/gtiwtnnxfq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xuetiantiany.cn/gtskbmeksx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.wangshuangyany.cn/gtsdzytvti.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.gaohongyu789.top/gtcepetgzz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jinghuilouyu.cn/gtslsegnrk.html

================================================================================
来源：http://hz.tanke756.top/gtnfbtfdpw.html

M. 命令行 / 进程 / 环境
来源：http://hz.xuetiantiany.cn/gtbtdyrloz.html

================================================================================
来源：http://hz.shzxlz.cn/gtwafmtydo.html

[M01] 读取命令行参数
来源：http://hz.shanyushiyangkeji.top/gtetslwgsb.html

Py:   sys.argv[1:]
来源：http://hz.jqgfzy.top/gtgxgzcusm.html

PHP:  $argv;  $argc;
来源：http://hz.zhengqikj.top/gtownssbdo.html

JS:   process.argv.slice(2)
来源：http://hz.havefunace.top/gtuotdngfo.html

TS:   process.argv.slice(2)
来源：http://hz.iojbl.cn/gtteidxsiq.html

Java: args 数组（main 方法参数）
来源：http://hz.tanke756.top/gtpubkistz.html

Go:   os.Args[1:]
来源：http://hz.redwolf501.top/gtjjbxwerw.html

Ruby: ARGV
来源：http://hz.nwbrower.top/gtopbbienf.html

C#:   args 数组（Main 方法参数）
来源：http://hz.316326.xyz/gtjdgiqlqv.html

[M02] 读取环境变量
来源：http://hz.dianchejie.cn/gttsfyzhyf.html

Py:   os.environ.get("HOME")
来源：http://hz.zhengqikj.top/gtbfqxjsos.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.xinyue.icu/gtvvdhzpmo.html

JS:   process.env.HOME
来源：http://hz.jinghuilouyu.cn/gtyfkobizr.html

TS:   process.env.HOME
来源：http://hz.xuanzx.com/gtdhoffrlj.html

Java: System.getenv("HOME")
来源：http://hz.meibo888.top/gtkpwztlsl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.xuanzx.com/gtwsrkqypz.html

Ruby: ENV["HOME"]
来源：http://hz.9152youxi.cn/gtyfhubqdl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.fzhhl.top/gtsyeenjym.html

[M03] 执行外部命令
来源：http://hz.yuanzhike.top/gthdjuyfhq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.cashguo.top/gtbhqsrjhp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.0kj1m.cn/gtoxhkzngz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.sxryk.cn/gthypdlpto.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinqigfzy.top/gtgltmqfyy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jqgufenzy.top/gtxcampzzi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.svipenyu.cn/gtynmzowvo.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.meibo888.top/gtixrwntof.html

C#:   Process.Start("ls", "-l");
来源：http://hz.gotoacloud.top/gtjejxbjlo.html

[M04] 获取当前工作目录
来源：http://hz.aizwys.cn/gtqyamhify.html

Py:   os.getcwd()
来源：http://hz.cheryme.top/gtwylirvgt.html

PHP:  getcwd();
来源：http://hz.ydzc1.top/gtdxwnekgf.html

JS:   process.cwd()
来源：http://hz.hongshengwenyu.top/gtunwbciqa.html

TS:   process.cwd()
来源：http://hz.vqdsnc.cn/gteugzszvi.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yonumen.top/gtlsolymst.html

Go:   os.Getwd()
来源：http://hz.yuxming.cn/gtctwjgout.html

Ruby: Dir.pwd
来源：http://hz.nanxinkj.top/gtmerappmh.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.shanyushiyangkeji.top/gtvkgyfxzi.html

[M05] 设置退出码
来源：http://hz.cdnleiting.top/gtebpxxlcu.html

Py:   sys.exit(1)
来源：http://hz.sysykeji.top/gtxjpajpgf.html

PHP:  exit(1);
来源：http://hz.zhongyouzk.top/gthgkmdzor.html

JS:   process.exit(1)
来源：http://hz.kuanghao11.cn/gtddofkkgt.html

TS:   process.exit(1)
来源：http://hz.daria6918.cn/gtavazbsrq.html

Java: System.exit(1)
来源：http://hz.52xcode.cn/gtgpqntjkt.html

Go:   os.Exit(1)
来源：http://hz.sufxvd.cn/gtlychbbvg.html

Ruby: exit 1
来源：http://hz.chenlongwang.top/gteaonbyeb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.tanke756.top/gtcusivtnf.html

[M06] 向标准错误输出
来源：http://hz.jinghuilouyu.cn/gtbcoxeztx.html

Py:   print("err", file=sys.stderr)
来源：http://hz.shanyushiyangkeji.top/gtbnvjjemv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xinyue.icu/gtsoafgeoz.html

JS:   console.error("err")
来源：http://hz.pengpengdd.cyou/gtvqeiyylj.html

TS:   console.error("err")
来源：http://hz.dianchejie.cn/gtywopujht.html

Java: System.err.println("err")
来源：http://hz.52xcode.cn/gtriitonzq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhiwuduotai.top/gtvrmrxaxn.html

Ruby: warn "err"
来源：http://hz.nanxuanxn.top/gtdtljnvas.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.havefunace.top/gtuvdckugq.html

[M07] 判断是否为主入口
来源：http://hz.redwolf501.top/gtzfieimva.html

Py:   if __name__ == "__main__":
来源：http://hz.yvedp.cn/gtrupilvsc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yuxming.cn/gthriftgqj.html

JS:   require.main === module
来源：http://hz.guannengcc.top/gtaywcolap.html

TS:   require.main === module
来源：http://hz.jiagoushi.top/gtagfzxhiv.html

Java: public static void main(String[] args)
来源：http://hz.wangdashe.top/gtltvwcnos.html

Go:   func main()
来源：http://hz.sweek.top/gtsoblnfrb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhengqikj.top/gtxiefwlmi.html

C#:   static void Main(string[] args)
来源：http://hz.shanyushiyangtech.top/gtdatpwvdf.html

[M08] 获取系统与运行时信息
来源：http://hz.zhengqikj.top/gtentqrvnr.html

Py:   platform.system();  platform.python_version()
来源：http://hz.guannengcc.top/gtsbhlkscp.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jiagoushi.top/gtyiezwjky.html

JS:   process.platform;  process.version
来源：http://hz.smart0.xyz/gtoupbermv.html

TS:   process.platform;  process.version
来源：http://hz.smart0.xyz/gtlkmnflbr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hywenlv.cn/gtwargiddw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.ehwqpu.com/gtrvkdwrss.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.sweek.top/gthdpbuxwp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhengqikj.top/gtdrhrqvub.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtfgpfnrix.html

N. 数据结构与算法
来源：http://hz.guannengcc.top/gtyjdkaquk.html

================================================================================
来源：http://hz.yueranfly.top/gtjzigzxsf.html

[N01] 二分查找（有序数组）
来源：http://hz.shanyushiyangkeji.top/gtxsjhqlda.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.shangyingyoupin.top/gtgwscrhnk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.xylfe.cn/gtvyxyiclc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ppjwa.cn/gtxdrwpamp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.wangshuangyany.cn/gtncfijmoc.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.chenzaomai.com/gtmwwgxvwk.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cheryme.top/gtvvqvdapf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jqgfzy.top/gtmkokmffh.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zhongyouzk.top/gtdrolbdtw.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.shanyushiyangkeji.top/gtyxewpjzw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hnxiangtu.top/gtjvczwjph.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yj20258888.top/gteacpsthk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yj202588.top/gtcuqpqiwl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sweek.top/gttolkatzo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.gogol.net.cn/gtmnjxbruy.html

Go:   slices.Sort(arr)
来源：http://hz.tanke756.top/gtszjuocxm.html

Ruby: arr.sort
来源：http://hz.feifeiyinyue.top/gticbkkvgm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.hammf.cn/gtpwepxlmx.html

[N03] 快速排序（分治示例）
来源：http://hz.gzhubu.top/gtadvzllyz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yueranfly.top/gtflihpdzb.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jianghu66.top/gteavudzlj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yvedp.cn/gtmafnbapl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.svipenyu.cn/gtcvmbzwmp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.cashguo.top/gtwxqxezzo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.gzhubu.top/gtbegepssn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.kuanghao11.cn/gtlgrzytkw.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhixingplan.top/gtwoimhrox.html

[N04] 斐波那契数列
来源：http://hz.yuxming.cn/gtaboayuok.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ivvv.top/gtssztizjs.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jinyuanbaomall.cn/gtitrstqmy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yuxming.cn/gtkeytfttc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.52xcode.cn/gtoehjcwgw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.andypj.xyz/gtyiwynlrq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.gotoacloud.top/gtbtijyaaz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.dashuyun.cn/gtxjgmdkjb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.c1oappe.top/gtwmhqmzwt.html


<!-- 参考信息 -->