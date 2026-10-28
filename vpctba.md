代发 wailian999

[J07] 比较两个日期
来源：http://hz.snrcjt.cn/gtottiweuc.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.smart0.xyz/gtfayscnbf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zycfv.cn/gtzxxupluf.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.tanke756.top/gtfptrymot.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.0kj1m.cn/gtlzrxekiw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yangfankeji.com/gtoarmtuyf.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hnxiangtu.top/gtkqpxqidh.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jinghuilouyu.cn/gthutmempe.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhoulong.xyz/gtgsqjleml.html

[J08] 提取年月日与星期
来源：http://hz.shanyushiyangtech.top/gttvthmdrm.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.cashguo.top/gtlnvdhltx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.kuanghao11.cn/gtlbzznebl.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jiagoushi.top/gtxnkvhpvt.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhoulong.xyz/gtmgcgxapw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.gaohongyu789.top/gtbweqlffo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.chenlongwang.top/gtggvuexyx.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.tian-w.cn/gtctgrrrcy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.sweek.top/gthauadatx.html

[J09] 时区处理
来源：http://hz.daria6918.cn/gteoqstmgc.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xylfe.cn/gtofavzjxd.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhixingplan.top/gtryktwubm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.havefunace.top/gtjkcgpfcb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.snrcjt.cn/gtptcljlaz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jinqigufen.top/gtztbvyrzf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.dashuyun.cn/gthcpzmpum.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.dashuyun.cn/gtfqyvvfxk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhengqikj.top/gtvxysclxj.html

[J10] 取今天 / 本月第一天
来源：http://hz.xinyue.icu/gtvuyvxtng.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.andypj.xyz/gtzozscafz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zycfv.cn/gtpxgkbaev.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yangfankeji.com/gtrsuzqouv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.shzxlz.cn/gtsygpwepx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.svipenyu.cn/gthzqealck.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.fzhhl.top/gtwmqcuegz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.tanke756.top/gtkkcdxnmu.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.cqqwz.cn/gtgkiwooph.html

================================================================================
来源：http://hz.birdmap.top/gtpajttjvi.html

K. JSON 与序列化
来源：http://hz.zhiwuduotai.top/gtgrmqwpji.html

================================================================================
来源：http://hz.daxiang520.top/gtyqffkgvq.html

[K01] 对象转 JSON 字符串
来源：http://hz.yuanzhike.top/gtgknpyuxq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.haohaochexian.top/gtzqlrfork.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhengqikj.top/gtpxkfzygj.html

JS:   JSON.stringify(obj)
来源：http://hz.zhaomingkeji.xyz/gtbnibwkhf.html

TS:   JSON.stringify(obj)
来源：http://hz.zhongyouzk.top/gtuyivpesi.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jinqigufen.top/gtaurjtprr.html

Go:   json.Marshal(obj)
来源：http://hz.tian-w.cn/gtmfmnekwv.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shangyingyoupin.top/gtacbuodwv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhengqikj.top/gteeeqvngf.html

[K02] JSON 字符串转对象
来源：http://hz.aizwys.cn/gthwukoehn.html

Py:   json.loads(s)
来源：http://hz.sxryk.cn/gtpkbyeoah.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.0kj1m.cn/gtvucdrwxk.html

JS:   JSON.parse(s)
来源：http://hz.ivvv.top/gtdotkxfbz.html

TS:   JSON.parse(s)
来源：http://hz.jlsjyb.cn/gttpwyofgx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.52xcode.cn/gtwmauaohe.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yvedp.cn/gtwlssuemb.html

Ruby: JSON.parse(s)
来源：http://hz.yonumen.top/gtpqevawcd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zdqjudy.top/gtchilrdte.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yongpay.top/gtfiquxhxq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.guowangkeji.top/gtpvxehszb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.mhx1999.top/gtimjcybki.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinghuilouyu.cn/gtbngckjbo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinghuilouyu.cn/gtwlytfcxf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.daxiang520.top/gtzzjfudsi.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hongshengwenyu.top/gttczcmefi.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.wangdashe.top/gtivajzqyn.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cheryme.top/gtgagmijhg.html

[K04] 读取 JSON 文件
来源：http://hz.hnqzz.top/gtqkilensb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ywan-chungtsiang.top/gtsfeluuwq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.tianlin.xyz/gtslylvemy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.mhx1999.top/gtqucirzvw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.wangshuangyany.cn/gtjwagvyrg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yj202588.top/gtzxcssdxe.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.shanyushiyangtech.top/gtvjfceyzt.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hfpthk.cn/gthtnjnwaf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.kuanghao11.cn/gtptcxultk.html

[K05] 深拷贝对象
来源：http://hz.shanyushiyangkeji.top/gtqymkjxbq.html

Py:   copy.deepcopy(obj)
来源：http://hz.jinyuanbaomall.cn/gtcfygfbuy.html

PHP:  unserialize(serialize($obj));
来源：http://hz.tianlin.xyz/gtonigmyoy.html

JS:   structuredClone(obj)
来源：http://hz.jqgufenzy.top/gtabmgdqxs.html

TS:   structuredClone(obj)
来源：http://hz.chenlongwang.top/gtlfglokha.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yj20258888.top/gtosxgceeo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xuanzx.com/gttkdegcpj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yonumen.top/gtudecgzwi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yj202588.top/gtwxqywyox.html

[K06] 解析 URL 查询串
来源：http://hz.jqgufenzy.top/gtvhcnwdtp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hywenlv.cn/gtiefgovvz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.meibo888.top/gtsujngxwq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yongpay.top/gtxsqrjoim.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tanke756.top/gtoxufxsvs.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhongyouzk.top/gtbzxxpyck.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yuxming.cn/gtmephxocj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.aibaodan.cn/gtujnlqlzz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.xingfuxueyuan.xyz/gtubccngzr.html

[K07] 进制转换
来源：http://hz.jinqigufen.top/gtxndgvjxf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yonumen.top/gtytmnpymo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.birdmap.top/gtripcimzm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.daria6918.cn/gtcpzvifrx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.vqdsnc.cn/gtobbxklou.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.daxiang520.top/gtlloyqcbo.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hywenlv.cn/gtuawlsjrl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ydzc1.top/gtjubkzkbd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.vqdsnc.cn/gtayirqgsy.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.havefunace.top/gticqxzaxh.html

Py:   pickle.dumps(obj)
来源：http://hz.dianchejie.cn/gtgxcsfkoc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.aibaodan.cn/gtgbggedcb.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhengqikj.top/gtypcztkho.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.vqdsnc.cn/gtjrqmbnac.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yuanzhike.top/gtjouvbhdl.html

Go:   encoding/gob
来源：http://hz.sufxvd.cn/gtfrffrvcx.html

Ruby: Marshal.dump(obj)
来源：http://hz.cdnleiting.top/gtxanvtsno.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xuetiantiany.cn/gtwoszxdcj.html

================================================================================
来源：http://hz.hywenlv.cn/gtdsofasrx.html

L. 网络请求
来源：http://hz.jlsjyb.cn/gtpciifjkq.html

================================================================================
来源：http://hz.xinyue.icu/gtzjeubnss.html

[L01] 发送 GET 请求
来源：http://hz.jiagoushi.top/gtygptvlhd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cqqwz.cn/gtydoinfze.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.cdnleiting.top/gttwmzgrxh.html

JS:   await fetch(url)
来源：http://hz.jyoumei.cn/gtynmgsswc.html

TS:   await fetch(url)
来源：http://hz.xinyue.icu/gtqvugauzl.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.pengpengdd.cyou/gtdnbkbeda.html

Go:   resp, err := http.Get(url)
来源：http://hz.yvedp.cn/gtymvyyqsg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.gotoacloud.top/gtsuqqskmx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ivvv.top/gtbgqveokj.html

[L02] 发送 POST JSON
来源：http://hz.hnxiangtu.top/gtfzzbleam.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.52xcode.cn/gtkypgszfn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jlsjyb.cn/gtbocyffoe.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sxryk.cn/gtkggwsqzg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ydzc1.top/gtexwnjefs.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.guowangkeji.top/gtrotusnfz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.guannengcc.top/gtcfawxjbx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.daria6918.cn/gtamyrzfqs.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.cqqwz.cn/gtccbxlpwr.html

[L03] 设置自定义请求头
来源：http://hz.yuxming.cn/gtbobetjxb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hnxiangtu.top/gtxornornv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hnqzz.top/gtrphfbtrr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cheryme.top/gtqyurfqmh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.pycfn.com/gtdfodgttj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.dianchejie.cn/gtlcqdfzck.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ywan-chungtsiang.top/gtusisernz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.aibaodan.cn/gtgamvqztr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jinghuilouyu.cn/gtzrebvshk.html

[L04] 设置超时
来源：http://hz.jinghuilouyu.cn/gtzzzawzat.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zhixingplan.top/gtelkgtkcy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.vqdsnc.cn/gtbrnlgmys.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yvedp.cn/gtseqtarxh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yuxming.cn/gtbckbpduq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.redwolf501.top/gtoooaillg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hnxiangtu.top/gtpgjbljfg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hnxiangtu.top/gtrsrvqgke.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.fengsongda.top/gtobgneqms.html

[L05] 上传文件（multipart）
来源：http://hz.wangshuangyany.cn/gteljgksdj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.nanxinkj.top/gtdgbrhckw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.tanke756.top/gtbblbpowk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.cucudq.cn/gtgpxhsnbr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.redwolf501.top/gttybodemm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yanxiufei.cn/gtkwpduhwp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.vqdsnc.cn/gtojnawipz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.gaohongyu789.top/gtqfffzrss.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.daxiang520.top/gtzdcwjphe.html

[L06] 解析响应为 JSON
来源：http://hz.birdmap.top/gtlehaohvp.html

Py:   resp.json()
来源：http://hz.zhoulong.xyz/gthztmgjhg.html

PHP:  json_decode($body, true);
来源：http://hz.tian-w.cn/gtmeciofrx.html

JS:   await resp.json()
来源：http://hz.feifeiyinyue.top/gtchnpdvvh.html

TS:   await resp.json()
来源：http://hz.yueranfly.top/gtyyluxhck.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.iojbl.cn/gtqqsuomzq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.gogol.net.cn/gtasqelbnj.html

Ruby: JSON.parse(resp.body)
来源：http://hz.chenzaomai.com/gtcjkhcgsd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ydzc1.top/gtwdpbzxpa.html

[L07] 处理 HTTP 状态码
来源：http://hz.nanxinkj.top/gtomkcvpjn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.haohaochexian.top/gtewdaftld.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.snrcjt.cn/gtgsruhqtl.html

JS:   resp.ok;  resp.status
来源：http://hz.mhx1999.top/gtdflnshnr.html

TS:   resp.ok;  resp.status
来源：http://hz.yonumen.top/gtwnigqibs.html

Java: resp.statusCode()
来源：http://hz.redwolf501.top/gtkggvxnzf.html

Go:   resp.StatusCode
来源：http://hz.pengpengdd.cyou/gtgxrrnxnw.html

Ruby: resp.code.to_i
来源：http://hz.cheryme.top/gtshikorhr.html

C#:   (int)resp.StatusCode
来源：http://hz.jianghu66.top/gtuvnlmaxj.html

[L08] 并发请求多个地址
来源：http://hz.316326.xyz/gttbouapsr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hfpthk.cn/gtouavjfcg.html

PHP:  curl_multi_init() 系列
来源：http://hz.pycfn.com/gtyrskacjx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shanyushiyangkeji.top/gtuznbcrib.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yuxming.cn/gtrfwnqpud.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.wangdashe.top/gtqppuykrc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ybcxt.top/gtjgspyuit.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhongyouzk.top/gtwxvuhuxd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.52xcode.cn/gtahwslnui.html

================================================================================
来源：http://hz.zhijiandao.cn/gtqzebmtvt.html

M. 命令行 / 进程 / 环境
来源：http://hz.yuanzhike.top/gtxfouprdv.html

================================================================================
来源：http://hz.yuanzhike.top/gtmucbcbqy.html

[M01] 读取命令行参数
来源：http://hz.zhixingplan.top/gtjhaggkmc.html

Py:   sys.argv[1:]
来源：http://hz.bjfxy.top/gtccbtyklz.html

PHP:  $argv;  $argc;
来源：http://hz.52xcode.cn/gtntewvawb.html

JS:   process.argv.slice(2)
来源：http://hz.gogol.net.cn/gtidsjmrxg.html

TS:   process.argv.slice(2)
来源：http://hz.andypj.xyz/gtxqdmkbeq.html

Java: args 数组（main 方法参数）
来源：http://hz.mhx1999.top/gtdvicvtht.html

Go:   os.Args[1:]
来源：http://hz.feifeiyinyue.top/gtnkkhgmrb.html

Ruby: ARGV
来源：http://hz.ivvv.top/gtthvvdiba.html

C#:   args 数组（Main 方法参数）
来源：http://hz.dashuyun.cn/gttwdovgdn.html

[M02] 读取环境变量
来源：http://hz.yanxiufei.cn/gtvvcrgjpr.html

Py:   os.environ.get("HOME")
来源：http://hz.ydjk.org.cn/gtfcdxvzvo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hfpthk.cn/gtkutesjtb.html

JS:   process.env.HOME
来源：http://hz.zhiwuduotai.top/gttcmxdwbh.html

TS:   process.env.HOME
来源：http://hz.hongshengwenyu.top/gtlbaiimcd.html

Java: System.getenv("HOME")
来源：http://hz.jinqigufen.top/gtbbkyybwr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.cdnleiting.top/gtttixtytt.html

Ruby: ENV["HOME"]
来源：http://hz.nwbrower.top/gtwsifxjgk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yvedp.cn/gttpmaahlh.html

[M03] 执行外部命令
来源：http://hz.vqdsnc.cn/gtcvktadau.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.guowangkeji.top/gtlhchgrak.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.nwbrower.top/gtxirgoodk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.cqqwz.cn/gtwhsoveqf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.daria6918.cn/gtdrsdrwux.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.quarkkingdee.top/gtotgrdxox.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.shanyushiyangkeji.top/gtudyaynbj.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.fengsongda.top/gtabinwkkm.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xinyue.icu/gtfdnbruzw.html

[M04] 获取当前工作目录
来源：http://hz.ydzc1.top/gtntpdlvrp.html

Py:   os.getcwd()
来源：http://hz.ydjk.org.cn/gtcreuzxxb.html

PHP:  getcwd();
来源：http://hz.aibaodan.cn/gtrmbbhvoa.html

JS:   process.cwd()
来源：http://hz.zhixingplan.top/gtjfnvvmdz.html

TS:   process.cwd()
来源：http://hz.sweek.top/gtjotfpiti.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jqgfzy.top/gtdgehspdw.html

Go:   os.Getwd()
来源：http://hz.mhx1999.top/gtubbkdokz.html

Ruby: Dir.pwd
来源：http://hz.aibaodan.cn/gtserpekub.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ydjk.org.cn/gtxtzhgxjx.html

[M05] 设置退出码
来源：http://hz.ppjwa.cn/gtdmeirfcl.html

Py:   sys.exit(1)
来源：http://hz.xingfuxueyuan.xyz/gtamprxobz.html

PHP:  exit(1);
来源：http://hz.ybcxt.top/gtmuxzbhqu.html

JS:   process.exit(1)
来源：http://hz.ywan-chungtsiang.top/gtciyklgty.html

TS:   process.exit(1)
来源：http://hz.haohaochexian.top/gtavpognne.html

Java: System.exit(1)
来源：http://hz.zycfv.cn/gtmulsnzbd.html

Go:   os.Exit(1)
来源：http://hz.nwbrower.top/gtmzmwiqut.html

Ruby: exit 1
来源：http://hz.mhx1999.top/gtczpojydv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zhiwuduotai.top/gthmdtwczz.html

[M06] 向标准错误输出
来源：http://hz.gogol.net.cn/gtbtvkvxqq.html

Py:   print("err", file=sys.stderr)
来源：http://hz.dashuyun.cn/gtjfuaszup.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ydjk.org.cn/gtyyqxlsjo.html

JS:   console.error("err")
来源：http://hz.ydzc1.top/gtejdekkwt.html

TS:   console.error("err")
来源：http://hz.yueranfly.top/gttpzcwmbe.html

Java: System.err.println("err")
来源：http://hz.chenjidiqi.icu/gtnyhawcid.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.hfpthk.cn/gtutorqodx.html

Ruby: warn "err"
来源：http://hz.hfpthk.cn/gtanxamwfy.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yangfankeji.com/gtzuhvymsz.html

[M07] 判断是否为主入口
来源：http://hz.jinqigfzy.top/gtscuuoayq.html

Py:   if __name__ == "__main__":
来源：http://hz.zhoulong.xyz/gtouxyweie.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.daria6918.cn/gtcxmxzzqd.html

JS:   require.main === module
来源：http://hz.nanxinkj.top/gtidpnnqob.html

TS:   require.main === module
来源：http://hz.chenlongwang.top/gtjnlssiqb.html

Java: public static void main(String[] args)
来源：http://hz.yonumen.top/gtwhnbdnea.html

Go:   func main()
来源：http://hz.ivvv.top/gtrkfunqro.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhijiandao.cn/gtciuomfoa.html

C#:   static void Main(string[] args)
来源：http://hz.hysaishi.cn/gtnjkfrmyw.html

[M08] 获取系统与运行时信息
来源：http://hz.mhx1999.top/gtqoyoawrc.html

Py:   platform.system();  platform.python_version()
来源：http://hz.xylfe.cn/gtjronhmlc.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.c1oappe.top/gtjvchseuj.html

JS:   process.platform;  process.version
来源：http://hz.zhongyouzk.top/gtcdvroqln.html

TS:   process.platform;  process.version
来源：http://hz.shanyushiyangkeji.top/gtykjxtccx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jyoumei.cn/gtneheocnu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xziqi.cn/gtomrqghai.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yonumen.top/gtxcokgqeu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yj20258.top/gtbrnaxxzr.html

================================================================================
来源：http://hz.zhengqikj.top/gtumirdoyg.html

N. 数据结构与算法
来源：http://hz.jianghu66.top/gtpekhnejh.html

================================================================================
来源：http://hz.gogol.net.cn/gtwxllfvvo.html

[N01] 二分查找（有序数组）
来源：http://hz.ivvv.top/gttfuzcnmy.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.gogol.net.cn/gtvvgsanhh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.guannengcc.top/gtwnmafeow.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.pengpengdd.cyou/gtfsvvowqx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinyuanbaomall.cn/gtquxofdag.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.tian-w.cn/gtphgcybkb.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.gzhubu.top/gtrkcrsyrv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.cucudq.cn/gtqdleelly.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jyoumei.cn/gtakbfplwy.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jianghu66.top/gtxqdxwjac.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yangfankeji.com/gtmubstidw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jqgufenzy.top/gtptcavgaa.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cheryme.top/gthcildcqu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.snrcjt.cn/gtfbzfprwr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.dashuyun.cn/gtgxvouwgq.html

Go:   slices.Sort(arr)
来源：http://hz.shangyingyoupin.top/gttxyyszdd.html

Ruby: arr.sort
来源：http://hz.52xcode.cn/gtajipsode.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.aibaodan.cn/gtarcxamms.html

[N03] 快速排序（分治示例）
来源：http://hz.zhengqikj.top/gtvljsagrl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ehwqpu.com/gtkfvndzlf.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xziqi.cn/gtqocosrii.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shuidangran.top/gtazhcowdo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.iojbl.cn/gtxfpcmhbk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.meibo888.top/gtbbcjmrfy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jinqigufen.top/gtzxgjqlqu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ydzc1.top/gtpnmefowl.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.guowangkeji.top/gtnhuekvyn.html

[N04] 斐波那契数列
来源：http://hz.jiagoushi.top/gtzhrixujr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.sxryk.cn/gtitxtnqep.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.52xcode.cn/gtpxdwpihi.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinghuilouyu.cn/gtzivnbiec.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.dianchejie.cn/gtfvcqjaja.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jyoumei.cn/gtosdcuhlj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhongyouzk.top/gtrszhbvrj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.gaohongyu789.top/gtldlylokp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jiagoushi.top/gtikqeyqph.html


<!-- 参考信息 -->