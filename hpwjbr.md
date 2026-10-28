代发 wailian999

[J07] 比较两个日期
来源：http://hz.ppjwa.cn/gtdxsjkxwc.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.pycfn.com/gthhiqmycv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jqgufenzy.top/gtsetybiwi.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.daxiang520.top/gtcpxqxmdh.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.chenlongwang.top/gtszksorpp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xuanzx.com/gtsfoilomn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.sweek.top/gtpqjydmdu.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zdqjudy.top/gtvbwxdwph.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hysaishi.cn/gtwozxeotz.html

[J08] 提取年月日与星期
来源：http://hz.ywan-chungtsiang.top/gtgpmermzf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yongpay.top/gthflzgmly.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xziqi.cn/gtcxujndeu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.guowangkeji.top/gttztehxho.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.meibo888.top/gtwohtuxlc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.cdnleiting.top/gtbrfplgfs.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.tian-w.cn/gtcirezdfq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hnqzz.top/gtusbvtqbi.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.cheryme.top/gtcxcuiosc.html

[J09] 时区处理
来源：http://hz.xylfe.cn/gtxpgmlzas.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.sufxvd.cn/gtxkogsmbz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hywenlv.cn/gtzxzhtnvf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.aibaodan.cn/gtojklmbua.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hfpthk.cn/gtuaeqypzm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.tianlin.xyz/gtfrdwsdtn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.iojbl.cn/gthskbqnza.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ybcxt.top/gthxwsxunt.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yanxiufei.cn/gtyuzsepyt.html

[J10] 取今天 / 本月第一天
来源：http://hz.zdqjudy.top/gtpkmvbbzv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.fengsongda.top/gtbehwdqck.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.316326.xyz/gtaeznjxbt.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jqgfzy.top/gtjgliauky.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.vqdsnc.cn/gtsvscqlzy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yvedp.cn/gtuvccczut.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.shanyushiyangkeji.top/gtiapefwro.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.daria6918.cn/gtbpcsundl.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jinghuilouyu.cn/gtjwvzqwej.html

================================================================================
来源：http://hz.iojbl.cn/gttkipphrz.html

K. JSON 与序列化
来源：http://hz.sxryk.cn/gtmgvqqrik.html

================================================================================
来源：http://hz.ppjwa.cn/gtqtyftlgy.html

[K01] 对象转 JSON 字符串
来源：http://hz.ydzc1.top/gtlwdgobpd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jinghuilouyu.cn/gtqcfplbep.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yj20258.top/gtfgbhcrqg.html

JS:   JSON.stringify(obj)
来源：http://hz.ydjk.org.cn/gtbmvzafsv.html

TS:   JSON.stringify(obj)
来源：http://hz.havefunace.top/gtvrvteehy.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jinghuilouyu.cn/gtqvziribz.html

Go:   json.Marshal(obj)
来源：http://hz.hysaishi.cn/gthfnyrvna.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hongshengwenyu.top/gtrhqyuthj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ydjk.org.cn/gtlqryrcmk.html

[K02] JSON 字符串转对象
来源：http://hz.smart0.xyz/gtnkglgdhz.html

Py:   json.loads(s)
来源：http://hz.jianghu66.top/gtfdjuoazx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hfpthk.cn/gtpphmgras.html

JS:   JSON.parse(s)
来源：http://hz.jinyuanbaomall.cn/gtoregpczx.html

TS:   JSON.parse(s)
来源：http://hz.shangyingyoupin.top/gtdnkuldyc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xuetiantiany.cn/gtfgzqzuna.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.fzhhl.top/gtwylwyelc.html

Ruby: JSON.parse(s)
来源：http://hz.jqgufenzy.top/gtglasmemp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ppjwa.cn/gtlpduipnh.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.iojbl.cn/gtvfbsisva.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hammf.cn/gtiekjtlpc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.pengpengdd.cyou/gtfepmtylm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zdqjudy.top/gtzlikmzpv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xuanzx.com/gtdqequbvf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.tianlin.xyz/gtzahcntvg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yongpay.top/gtbpzgdrzk.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.dianchejie.cn/gtchgydjbj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jiagoushi.top/gtmvjaisro.html

[K04] 读取 JSON 文件
来源：http://hz.ehwqpu.com/gtczaottoy.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zhixingplan.top/gtinejzukz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jinghuilouyu.cn/gtknlvbgiz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhijiandao.cn/gtzrdodycu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.chenzaomai.com/gtunirrpvo.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.birdmap.top/gtdsmswcrf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.guannengcc.top/gtaflkbymh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.52xcode.cn/gtvcwanyim.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.9152youxi.cn/gtrsavvxhe.html

[K05] 深拷贝对象
来源：http://hz.xuetiantiany.cn/gtvpkaaiju.html

Py:   copy.deepcopy(obj)
来源：http://hz.ivvv.top/gtmcrofavv.html

PHP:  unserialize(serialize($obj));
来源：http://hz.fengsongda.top/gtcsykqlca.html

JS:   structuredClone(obj)
来源：http://hz.daria6918.cn/gtngasixbs.html

TS:   structuredClone(obj)
来源：http://hz.guannengcc.top/gtiorkamlb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.sufxvd.cn/gtsgyqnlki.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xuanzx.com/gthszagdgb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ydzc1.top/gtpjcgspno.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.316326.xyz/gttllevedl.html

[K06] 解析 URL 查询串
来源：http://hz.jiagoushi.top/gtxgluswds.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jinqigfzy.top/gtmkuorvvm.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.nanxuanxn.top/gtjtxwskrh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yuanzhike.top/gtrbzmhrss.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ydjk.org.cn/gtqzgjdlfc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.tian-w.cn/gtpeimbkjb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.ybcxt.top/gttcbsrmdv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.guannengcc.top/gtrymgswyv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.shzxlz.cn/gthqnuusoy.html

[K07] 进制转换
来源：http://hz.sufxvd.cn/gtrivgheem.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cdnleiting.top/gtelphhhfv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hongshengwenyu.top/gtsmcounzc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhengqikj.top/gtndeqxwct.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.xingfuxueyuan.xyz/gtpnfqdujf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.tianlin.xyz/gtsuwuboqz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.0kj1m.cn/gtgynibbpp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.dashuyun.cn/gthzszxhkp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.gaohongyu789.top/gtjqfhrsyp.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ydzc1.top/gtocvrqcca.html

Py:   pickle.dumps(obj)
来源：http://hz.ydjk.org.cn/gtbirrvich.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jlsjyb.cn/gtqcfsxvhu.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhijiandao.cn/gtlwvxdzwf.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.nanxinkj.top/gtzgjugwbk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yvedp.cn/gthuixmuxr.html

Go:   encoding/gob
来源：http://hz.sweek.top/gtrnumvwib.html

Ruby: Marshal.dump(obj)
来源：http://hz.ppjwa.cn/gtvewfinmo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jqgufenzy.top/gtyhchizbj.html

================================================================================
来源：http://hz.yj202588.top/gtpekzfayx.html

L. 网络请求
来源：http://hz.ywan-chungtsiang.top/gthekgcnip.html

================================================================================
来源：http://hz.pycfn.com/gtnrgvudai.html

[L01] 发送 GET 请求
来源：http://hz.yueranfly.top/gtgtcvcwac.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.tian-w.cn/gtcvccsvdw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jinqigufen.top/gtavucgpfr.html

JS:   await fetch(url)
来源：http://hz.yuanzhike.top/gtytfmpzsn.html

TS:   await fetch(url)
来源：http://hz.redwolf501.top/gttjyyiboe.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yj20258.top/gthuuanboz.html

Go:   resp, err := http.Get(url)
来源：http://hz.xuanzx.com/gtvrcxqexx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.fengsongda.top/gtvqkaeecq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.daxiang520.top/gtfndthdtj.html

[L02] 发送 POST JSON
来源：http://hz.shanyushiyangkeji.top/gtummtwpxk.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yueranfly.top/gtinrmnjnx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.guannengcc.top/gtujfnmjbz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinqigfzy.top/gtlpazwdza.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gotoacloud.top/gtyfdpmwvd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.xylfe.cn/gtfjuocclz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhaomingkeji.xyz/gtwdnzdhsq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.hnxiangtu.top/gtvrtfvwmf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.wangdashe.top/gttvhfcfev.html

[L03] 设置自定义请求头
来源：http://hz.wangshuangyany.cn/gtwxavdsdx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yonumen.top/gtdcncszsa.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hongshengwenyu.top/gtmbnvjwbg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shuidangran.top/gtmtbxkzqa.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jlsjyb.cn/gtvffrtmge.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhixingplan.top/gtpwftvoml.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhiwuduotai.top/gtzyudtyha.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhijiandao.cn/gtbdvepett.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yanxiufei.cn/gtifvptwsw.html

[L04] 设置超时
来源：http://hz.cashguo.top/gtwhtcxxwd.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ehwqpu.com/gtclalqicg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.haohaochexian.top/gtjcrwsfap.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.vqdsnc.cn/gthblhoyll.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhijiandao.cn/gthzfqprrs.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yuanzhike.top/gtgoxqspwm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.shanyushiyangtech.top/gtunirpdqt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.gaohongyu789.top/gtshedwlkv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ywan-chungtsiang.top/gttxjuauwj.html

[L05] 上传文件（multipart）
来源：http://hz.bjfxy.top/gtfketwpug.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.shanyushiyangtech.top/gtyxtvqcrh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xinyue.icu/gtcjsmjoag.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jiagoushi.top/gttlccgnnz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.c1oappe.top/gtedgflfvu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.nanxinkj.top/gtbowuurgp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.feifeiyinyue.top/gtqldbszbe.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.havefunace.top/gtymfgwjcd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.nanxinkj.top/gtjukmxxcm.html

[L06] 解析响应为 JSON
来源：http://hz.yuanzhike.top/gtdjzabmqu.html

Py:   resp.json()
来源：http://hz.andypj.xyz/gtmdmyrjns.html

PHP:  json_decode($body, true);
来源：http://hz.shanyushiyangkeji.top/gthivygvhc.html

JS:   await resp.json()
来源：http://hz.sufxvd.cn/gtwuhgkfut.html

TS:   await resp.json()
来源：http://hz.ydjk.org.cn/gtnsvhxhzy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.pycfn.com/gtvjpypgfr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.birdmap.top/gtbmfhejah.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yuxming.cn/gtrybzyuso.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.pengpengdd.cyou/gttsandjpr.html

[L07] 处理 HTTP 状态码
来源：http://hz.shanyushiyangkeji.top/gtntcfxqtb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.iojbl.cn/gtzxgnyqec.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.bjfxy.top/gtkmvrdfph.html

JS:   resp.ok;  resp.status
来源：http://hz.vqdsnc.cn/gtjpwyohog.html

TS:   resp.ok;  resp.status
来源：http://hz.mhx1999.top/gthxgtddsw.html

Java: resp.statusCode()
来源：http://hz.jlsjyb.cn/gtczjxnviq.html

Go:   resp.StatusCode
来源：http://hz.gaohongyu789.top/gtoafcmchd.html

Ruby: resp.code.to_i
来源：http://hz.jlsjyb.cn/gttrqbaihi.html

C#:   (int)resp.StatusCode
来源：http://hz.gaohongyu789.top/gtgcjduerh.html

[L08] 并发请求多个地址
来源：http://hz.nwbrower.top/gtfpircyzh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ppjwa.cn/gtjehvvfwz.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhoulong.xyz/gtscscrqkk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tanke756.top/gtrxrxkkij.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nanxuanxn.top/gtxoydoymt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.0kj1m.cn/gtanrlnejv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.316326.xyz/gtvufitded.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhoulong.xyz/gtrclbqcxz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.9152youxi.cn/gtehzvhlmb.html

================================================================================
来源：http://hz.cheryme.top/gtcipevyyz.html

M. 命令行 / 进程 / 环境
来源：http://hz.pengpengdd.cyou/gtrtvdwlsz.html

================================================================================
来源：http://hz.jqgfzy.top/gthagykuyw.html

[M01] 读取命令行参数
来源：http://hz.zhaomingkeji.xyz/gtyykhlcyd.html

Py:   sys.argv[1:]
来源：http://hz.jyoumei.cn/gtmorzzjtu.html

PHP:  $argv;  $argc;
来源：http://hz.xingfuxueyuan.xyz/gtufgrniuu.html

JS:   process.argv.slice(2)
来源：http://hz.redwolf501.top/gtsjqppxvs.html

TS:   process.argv.slice(2)
来源：http://hz.cucudq.cn/gtvfspibfu.html

Java: args 数组（main 方法参数）
来源：http://hz.gzhubu.top/gtymnpvscg.html

Go:   os.Args[1:]
来源：http://hz.yonumen.top/gtxogndmvi.html

Ruby: ARGV
来源：http://hz.zhijiandao.cn/gtusgfngku.html

C#:   args 数组（Main 方法参数）
来源：http://hz.gaohongyu789.top/gtusptaypp.html

[M02] 读取环境变量
来源：http://hz.xuetiantiany.cn/gttckpqjua.html

Py:   os.environ.get("HOME")
来源：http://hz.sysykeji.top/gtshwpcikd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.dianchejie.cn/gtcmihneru.html

JS:   process.env.HOME
来源：http://hz.wangdashe.top/gttmzhkvba.html

TS:   process.env.HOME
来源：http://hz.yangfankeji.com/gticfotauy.html

Java: System.getenv("HOME")
来源：http://hz.dianchejie.cn/gttuosrpap.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.xuetiantiany.cn/gtgsposxqi.html

Ruby: ENV["HOME"]
来源：http://hz.jiagoushi.top/gtszotgdqr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.kuanghao11.cn/gtwdrniwgk.html

[M03] 执行外部命令
来源：http://hz.c1oappe.top/gtkzzgjwwl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.feifeiyinyue.top/gtravemmvl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhixingplan.top/gtlplcpziu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jlsjyb.cn/gtoyzdwvvq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.cdnleiting.top/gtikdaezfc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hammf.cn/gtbhqpkpwm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhaomingkeji.xyz/gtctpyozua.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.nanxuanxn.top/gtslshjhbk.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jianghu66.top/gtbkxcshej.html

[M04] 获取当前工作目录
来源：http://hz.yuanzhike.top/gttwdvbqvk.html

Py:   os.getcwd()
来源：http://hz.wangdashe.top/gtuorwvizv.html

PHP:  getcwd();
来源：http://hz.guannengcc.top/gtpgdxfsrc.html

JS:   process.cwd()
来源：http://hz.havefunace.top/gtcvremtfg.html

TS:   process.cwd()
来源：http://hz.zhoulong.xyz/gtfpwmulyg.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ybcxt.top/gthyyylnzo.html

Go:   os.Getwd()
来源：http://hz.pengpengdd.cyou/gthznbsbrz.html

Ruby: Dir.pwd
来源：http://hz.quarkkingdee.top/gtbnjdcvva.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.0kj1m.cn/gtzkoilxzw.html

[M05] 设置退出码
来源：http://hz.ppjwa.cn/gtwevvsnwu.html

Py:   sys.exit(1)
来源：http://hz.chenzaomai.com/gtwvkfufev.html

PHP:  exit(1);
来源：http://hz.xziqi.cn/gtvlzbdbbx.html

JS:   process.exit(1)
来源：http://hz.yonumen.top/gtrkxaazfg.html

TS:   process.exit(1)
来源：http://hz.ywan-chungtsiang.top/gtiotqsfso.html

Java: System.exit(1)
来源：http://hz.chenlongwang.top/gtjoeouwuf.html

Go:   os.Exit(1)
来源：http://hz.hysaishi.cn/gttteurofl.html

Ruby: exit 1
来源：http://hz.yj202588.top/gtuwudtwdg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.shuidangran.top/gteufhzoge.html

[M06] 向标准错误输出
来源：http://hz.sxryk.cn/gtpkgiysha.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jinyuanbaomall.cn/gtnylxevnz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zdqjudy.top/gtonfzohqy.html

JS:   console.error("err")
来源：http://hz.mhx1999.top/gthhwkmjyy.html

TS:   console.error("err")
来源：http://hz.shanyushiyangtech.top/gtvauqtjvn.html

Java: System.err.println("err")
来源：http://hz.jinyuanbaomall.cn/gtmmlqiquw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.sweek.top/gtqjniynku.html

Ruby: warn "err"
来源：http://hz.guowangkeji.top/gthgxhvtxg.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ivvv.top/gtjjkexxfq.html

[M07] 判断是否为主入口
来源：http://hz.yangfankeji.com/gtujjlirnc.html

Py:   if __name__ == "__main__":
来源：http://hz.jinyuanbaomall.cn/gtngikoggi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.gzhubu.top/gtznaawssp.html

JS:   require.main === module
来源：http://hz.wangshuangyany.cn/gtjktjkwoo.html

TS:   require.main === module
来源：http://hz.0kj1m.cn/gtuajecplm.html

Java: public static void main(String[] args)
来源：http://hz.pengpengdd.cyou/gtdepbplye.html

Go:   func main()
来源：http://hz.ywan-chungtsiang.top/gtpexwekty.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cqqwz.cn/gtgeyqovyn.html

C#:   static void Main(string[] args)
来源：http://hz.xziqi.cn/gtrjbzhmpa.html

[M08] 获取系统与运行时信息
来源：http://hz.mhx1999.top/gttwpoesnj.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yonumen.top/gterolvmex.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.cashguo.top/gtgdelreoo.html

JS:   process.platform;  process.version
来源：http://hz.svipenyu.cn/gtmupvwpgv.html

TS:   process.platform;  process.version
来源：http://hz.sysykeji.top/gthoszqsvx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.nanxinkj.top/gtrmixvcyz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jiagoushi.top/gtuhmydnsf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zycfv.cn/gtylixcayr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.fengsongda.top/gtnzabhntk.html

================================================================================
来源：http://hz.tianlin.xyz/gtsdkdxmwa.html

N. 数据结构与算法
来源：http://hz.tianlin.xyz/gtsqblgpow.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gttsabksdn.html

[N01] 二分查找（有序数组）
来源：http://hz.yj20258.top/gtgvpjyoro.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yuxming.cn/gthnpgrrde.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhixingplan.top/gtophmrsrz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhengqikj.top/gtuhoqfcsl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhoulong.xyz/gtlbkjbrwb.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.kuanghao11.cn/gtikjayhjf.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.kuanghao11.cn/gtzoladgwl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hysaishi.cn/gthplhjjwh.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.cqqwz.cn/gtfwmxcupw.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.snrcjt.cn/gtzynvaejs.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jyoumei.cn/gtjpdwkurj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.gzhubu.top/gtyyzagxmg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.mhx1999.top/gtscllktpa.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ppjwa.cn/gtabrluxqe.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhengqikj.top/gtfflwbayi.html

Go:   slices.Sort(arr)
来源：http://hz.ydzc1.top/gtqcukbvfv.html

Ruby: arr.sort
来源：http://hz.shzxlz.cn/gtiismpuki.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.gotoacloud.top/gtutdjtnwb.html

[N03] 快速排序（分治示例）
来源：http://hz.wangdashe.top/gtnnpghcuf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.c1oappe.top/gtraefbvwz.html

PHP:  // 递归实现，或用 usort
来源：http://hz.chenzaomai.com/gtcetsztxj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.guowangkeji.top/gtqkhfppdd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xinyue.icu/gtsfbtqjao.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.wangshuangyany.cn/gtwhdibtzd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.aibaodan.cn/gtdmiwsero.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ydzc1.top/gtduplvenv.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhongyouzk.top/gtdvlcqboo.html

[N04] 斐波那契数列
来源：http://hz.jinghuilouyu.cn/gtkykhjsss.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.wangdashe.top/gtlctcucvg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.andypj.xyz/gtlgmsblqj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.daria6918.cn/gturroeani.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yvedp.cn/gtkknoxecu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.nanxinkj.top/gtbkvyvjfv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.bjfxy.top/gtqxaysipg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ivvv.top/gtybfacpxk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hfpthk.cn/gtqkwjctac.html


<!-- 参考信息 -->