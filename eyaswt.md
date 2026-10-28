代发 wailian999

[J07] 比较两个日期
来源：http://hz.tian-w.cn/gtvzeofhlz.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ydzc1.top/gtvdjjguqq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.wangshuangyany.cn/gtveomctvb.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.daxiang520.top/gtfkixslvc.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hfpthk.cn/gtpnjyvtct.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ydjk.org.cn/gtmmscvfmg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ydzc1.top/gtzcsiksdb.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.fengsongda.top/gtuwwxmqii.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.xingfuxueyuan.xyz/gtcepnerdg.html

[J08] 提取年月日与星期
来源：http://hz.havefunace.top/gtabrapjfe.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.aibaodan.cn/gtkqbfcmlx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jiagoushi.top/gtmhcimfrd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.sxryk.cn/gtyutvnddk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.andypj.xyz/gtbphwvggx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.gzhubu.top/gtcpaldxoy.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yj20258.top/gtleqtjnqb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zycfv.cn/gtfxtyrnbc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jqgufenzy.top/gtixfgiqsu.html

[J09] 时区处理
来源：http://hz.xuetiantiany.cn/gtywkatjqf.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.sysykeji.top/gtawdhisqf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hnxiangtu.top/gtxzawrbyv.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj20258.top/gtpkrphhot.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.bjfxy.top/gtxagaoodc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yueranfly.top/gtslusnnmb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hfpthk.cn/gtgkpuxsmf.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.andypj.xyz/gtfyagqdig.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shangyingyoupin.top/gtjccurarc.html

[J10] 取今天 / 本月第一天
来源：http://hz.aizwys.cn/gtkpmozpki.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.chenjidiqi.icu/gtnpnbmfse.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.wangdashe.top/gtbwhonkrp.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jqgfzy.top/gtuknjvocw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.iojbl.cn/gtgehbytrz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jqgfzy.top/gttwirwbxf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xinyue.icu/gtmkkgvswi.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.guowangkeji.top/gtdlqemgyn.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yj20258888.top/gtpoicilum.html

================================================================================
来源：http://hz.yj202588.top/gtymgqdpzs.html

K. JSON 与序列化
来源：http://hz.52xcode.cn/gtpycooyjc.html

================================================================================
来源：http://hz.jqgfzy.top/gtdhrrtiej.html

[K01] 对象转 JSON 字符串
来源：http://hz.gaohongyu789.top/gtvxmblafd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.c1oappe.top/gtzkbudbcq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.chenlongwang.top/gtsoqtjbvf.html

JS:   JSON.stringify(obj)
来源：http://hz.ybcxt.top/gtejmcvdgm.html

TS:   JSON.stringify(obj)
来源：http://hz.feifeiyinyue.top/gtxwrjmclm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.fengsongda.top/gtiiipbdyt.html

Go:   json.Marshal(obj)
来源：http://hz.gogol.net.cn/gtpgjyycjk.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.ppjwa.cn/gtuxtbtjhf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.guowangkeji.top/gtrgsghqlx.html

[K02] JSON 字符串转对象
来源：http://hz.0kj1m.cn/gtunwvgcwk.html

Py:   json.loads(s)
来源：http://hz.jyoumei.cn/gtbxujpoov.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.quarkkingdee.top/gtspeacxyy.html

JS:   JSON.parse(s)
来源：http://hz.hammf.cn/gtdfagnsyr.html

TS:   JSON.parse(s)
来源：http://hz.hnxiangtu.top/gtsnattovy.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.cashguo.top/gtfeymbalr.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhixingplan.top/gtndessast.html

Ruby: JSON.parse(s)
来源：http://hz.ivvv.top/gtsycgvijk.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xingfuxueyuan.xyz/gtualyhvva.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhaomingkeji.xyz/gtwmpetyhv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhoulong.xyz/gtlclzbwoy.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.daria6918.cn/gtdpugybjh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.cashguo.top/gtbupeyvqe.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj20258888.top/gtijnwautn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jinyuanbaomall.cn/gtrppgicfw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hongshengwenyu.top/gthcmlaryx.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hfpthk.cn/gtfgvkitwi.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.aizwys.cn/gtjbqgifga.html

[K04] 读取 JSON 文件
来源：http://hz.sweek.top/gtxwjumszw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.0kj1m.cn/gtqbmlvzxk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cqqwz.cn/gtyobmhglx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hnqzz.top/gtfmtnfhwe.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhaomingkeji.xyz/gtkvgzzotg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.xuetiantiany.cn/gttsmxvhdo.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xuanzx.com/gtwouqdlyc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yongpay.top/gtvqoxiupr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.birdmap.top/gtcoixdzwp.html

[K05] 深拷贝对象
来源：http://hz.yj20258.top/gtxcdoqcfz.html

Py:   copy.deepcopy(obj)
来源：http://hz.hfpthk.cn/gtjzzeuspa.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ehwqpu.com/gtjnmhyzoj.html

JS:   structuredClone(obj)
来源：http://hz.gaohongyu789.top/gttrxpeynd.html

TS:   structuredClone(obj)
来源：http://hz.chenzaomai.com/gtvifhfwfz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ydjk.org.cn/gtnsqzqiqi.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.shzxlz.cn/gtplozvfnw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.chenlongwang.top/gtzcrqtgbm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhiwuduotai.top/gtxahweglf.html

[K06] 解析 URL 查询串
来源：http://hz.tianlin.xyz/gtknoivuze.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.guannengcc.top/gtqcmsooso.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hywenlv.cn/gtqbtlmfkt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sufxvd.cn/gtjpsrjhgo.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.wangdashe.top/gtmevjsowe.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.tian-w.cn/gtaaemtsly.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yuxming.cn/gtkbiytqfu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.nanxuanxn.top/gtztfgasnf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhoulong.xyz/gthlqeswaf.html

[K07] 进制转换
来源：http://hz.jqgfzy.top/gtqukcpfwm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhiwuduotai.top/gtgixsvwwb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yuanzhike.top/gtspzxlwnq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.meibo888.top/gtbgkslkst.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.gaohongyu789.top/gthsmafoxj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.meibo888.top/gtaewongvn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.nwbrower.top/gtdiwfkgrh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zhongyouzk.top/gtllaokysa.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.birdmap.top/gticnqsapj.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.mhx1999.top/gtrofwrhwm.html

Py:   pickle.dumps(obj)
来源：http://hz.shzxlz.cn/gthdryjoai.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.vqdsnc.cn/gtxnzidmkz.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.fengsongda.top/gtzuowzpcf.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jinqigfzy.top/gtssspplzz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.aibaodan.cn/gtlkfgzrgl.html

Go:   encoding/gob
来源：http://hz.jinqigfzy.top/gtelxgjqmw.html

Ruby: Marshal.dump(obj)
来源：http://hz.svipenyu.cn/gtzbrwsryx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhongyouzk.top/gtyxqtcseh.html

================================================================================
来源：http://hz.ybcxt.top/gtlbkmtmzo.html

L. 网络请求
来源：http://hz.shzxlz.cn/gtzhpveymn.html

================================================================================
来源：http://hz.jinqigufen.top/gtdubexsgp.html

[L01] 发送 GET 请求
来源：http://hz.shanyushiyangtech.top/gtmvpevqcf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.tianlin.xyz/gtimfwucvn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yangfankeji.com/gtcwzwwmcj.html

JS:   await fetch(url)
来源：http://hz.ybcxt.top/gtoyoxlrtf.html

TS:   await fetch(url)
来源：http://hz.ywan-chungtsiang.top/gtoqbmdxix.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yueranfly.top/gtnqhsbpot.html

Go:   resp, err := http.Get(url)
来源：http://hz.nanxuanxn.top/gtuxdqgggv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.wangshuangyany.cn/gtsbwgjtio.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.xziqi.cn/gtsboeyjmp.html

[L02] 发送 POST JSON
来源：http://hz.birdmap.top/gtzaxabxyn.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhixingplan.top/gtrsebacna.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.sxryk.cn/gtcftjtkku.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tian-w.cn/gtfrrljytp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yuanzhike.top/gtlnvxyxps.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.xuanzx.com/gtcsogwavc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.quarkkingdee.top/gtznllgbdm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.cheryme.top/gtgyhejtzp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ywan-chungtsiang.top/gtgyxpcpyo.html

[L03] 设置自定义请求头
来源：http://hz.hnqzz.top/gttobizlgm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xingfuxueyuan.xyz/gtnypdfxkc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yongpay.top/gtqanjazhn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhaomingkeji.xyz/gtecqausrp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.0kj1m.cn/gtpeswxuxj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jiagoushi.top/gtndwyojce.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yj202588.top/gtrigmkbhw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.aibaodan.cn/gtttipweig.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.xuetiantiany.cn/gtkqopuxby.html

[L04] 设置超时
来源：http://hz.gogol.net.cn/gtbcsmidui.html

Py:   requests.get(url, timeout=5)
来源：http://hz.andypj.xyz/gtredwjglp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.vqdsnc.cn/gtqjnacvnm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.aizwys.cn/gtjyjbsier.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.daria6918.cn/gtvvopmhhc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.0kj1m.cn/gtgwkqzavn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.xingfuxueyuan.xyz/gtqwpkudqa.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.sxryk.cn/gthfhagdhx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xuanzx.com/gtrsqllnel.html

[L05] 上传文件（multipart）
来源：http://hz.zhongyouzk.top/gtrrvlbnnw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.nwbrower.top/gtokuozjsf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhaomingkeji.xyz/gtehgjbyjz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinqigfzy.top/gtnfgcplyf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenzaomai.com/gtwrdpecig.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.c1oappe.top/gtxangbexv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.nanxuanxn.top/gtzuoqwjpb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.hfpthk.cn/gtatlshzzc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jinqigufen.top/gtpfcnmpyb.html

[L06] 解析响应为 JSON
来源：http://hz.jinyuanbaomall.cn/gtasvqibub.html

Py:   resp.json()
来源：http://hz.zhoulong.xyz/gtvvcbutci.html

PHP:  json_decode($body, true);
来源：http://hz.guowangkeji.top/gtdjsgvydg.html

JS:   await resp.json()
来源：http://hz.yuanzhike.top/gtscxttrxa.html

TS:   await resp.json()
来源：http://hz.gotoacloud.top/gtijxpqjdf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.xziqi.cn/gtscalbkpj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.ydzc1.top/gtwpbmshfq.html

Ruby: JSON.parse(resp.body)
来源：http://hz.quarkkingdee.top/gtutwimbzj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jlsjyb.cn/gtrfdbubhz.html

[L07] 处理 HTTP 状态码
来源：http://hz.yueranfly.top/gtznsejfve.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xingfuxueyuan.xyz/gtjlwqabap.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yvedp.cn/gteaqgixfn.html

JS:   resp.ok;  resp.status
来源：http://hz.xylfe.cn/gtytyrgxxy.html

TS:   resp.ok;  resp.status
来源：http://hz.zhaomingkeji.xyz/gttfgdnkws.html

Java: resp.statusCode()
来源：http://hz.9152youxi.cn/gtracidltf.html

Go:   resp.StatusCode
来源：http://hz.havefunace.top/gttabaxqdz.html

Ruby: resp.code.to_i
来源：http://hz.gotoacloud.top/gtqnfriixv.html

C#:   (int)resp.StatusCode
来源：http://hz.shanyushiyangkeji.top/gtzumbrbsr.html

[L08] 并发请求多个地址
来源：http://hz.zhijiandao.cn/gtjbwaswvn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.snrcjt.cn/gtlsyusqux.html

PHP:  curl_multi_init() 系列
来源：http://hz.redwolf501.top/gtyxiuirhk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.pycfn.com/gtzbbuttck.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhiwuduotai.top/gtinthlxzw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.sweek.top/gtknyqfxse.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.dashuyun.cn/gtmclubzwa.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.dashuyun.cn/gtzqnpybno.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jinghuilouyu.cn/gtqkkkrmgm.html

================================================================================
来源：http://hz.ybcxt.top/gthzhquflb.html

M. 命令行 / 进程 / 环境
来源：http://hz.yanxiufei.cn/gtucygodpd.html

================================================================================
来源：http://hz.sufxvd.cn/gttlzxiwuh.html

[M01] 读取命令行参数
来源：http://hz.jqgfzy.top/gtvidnluxl.html

Py:   sys.argv[1:]
来源：http://hz.dashuyun.cn/gtuzquwrrs.html

PHP:  $argv;  $argc;
来源：http://hz.meibo888.top/gtbnhrpcoh.html

JS:   process.argv.slice(2)
来源：http://hz.yj20258888.top/gtmbvgeuor.html

TS:   process.argv.slice(2)
来源：http://hz.tanke756.top/gtrgumsqah.html

Java: args 数组（main 方法参数）
来源：http://hz.yj202588.top/gtnbalchgy.html

Go:   os.Args[1:]
来源：http://hz.tanke756.top/gtygrropeu.html

Ruby: ARGV
来源：http://hz.yanxiufei.cn/gtorscakbl.html

C#:   args 数组（Main 方法参数）
来源：http://hz.gotoacloud.top/gtgzciqjpz.html

[M02] 读取环境变量
来源：http://hz.yj20258.top/gtkvynzres.html

Py:   os.environ.get("HOME")
来源：http://hz.hammf.cn/gtglknalhv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.feifeiyinyue.top/gtqmnhgqqb.html

JS:   process.env.HOME
来源：http://hz.hongshengwenyu.top/gtrxlzhpbb.html

TS:   process.env.HOME
来源：http://hz.zycfv.cn/gtgjfbneie.html

Java: System.getenv("HOME")
来源：http://hz.xingfuxueyuan.xyz/gtfjrunrmc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.9152youxi.cn/gtsogznarr.html

Ruby: ENV["HOME"]
来源：http://hz.zhaomingkeji.xyz/gtfdorpjog.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.chenjidiqi.icu/gtmzlsydje.html

[M03] 执行外部命令
来源：http://hz.c1oappe.top/gthmxcegfq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.smart0.xyz/gtkbsrtfhm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zdqjudy.top/gtqktunpsl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.iojbl.cn/gtpqhgkgob.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.kuanghao11.cn/gtxtairapk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhiwuduotai.top/gtzouexnjw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yongpay.top/gtmywucekh.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.gotoacloud.top/gtndkrabat.html

C#:   Process.Start("ls", "-l");
来源：http://hz.dashuyun.cn/gtadaovmdh.html

[M04] 获取当前工作目录
来源：http://hz.hammf.cn/gtzckesjmo.html

Py:   os.getcwd()
来源：http://hz.gogol.net.cn/gtlnyawttz.html

PHP:  getcwd();
来源：http://hz.shuidangran.top/gtavyqubjk.html

JS:   process.cwd()
来源：http://hz.yvedp.cn/gtcdtxtrkv.html

TS:   process.cwd()
来源：http://hz.zhixingplan.top/gtqoyajcap.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.wangdashe.top/gtnkvjjxpb.html

Go:   os.Getwd()
来源：http://hz.cdnleiting.top/gtkeaffwri.html

Ruby: Dir.pwd
来源：http://hz.jianghu66.top/gtlkioxhnf.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.havefunace.top/gtewnfpima.html

[M05] 设置退出码
来源：http://hz.xinyue.icu/gteaymmyvb.html

Py:   sys.exit(1)
来源：http://hz.yj202588.top/gtlwufrebg.html

PHP:  exit(1);
来源：http://hz.zhijiandao.cn/gtqlfaqbxv.html

JS:   process.exit(1)
来源：http://hz.hfpthk.cn/gtpbpcsgdj.html

TS:   process.exit(1)
来源：http://hz.andypj.xyz/gtzpmunmaf.html

Java: System.exit(1)
来源：http://hz.xuetiantiany.cn/gtaayswocv.html

Go:   os.Exit(1)
来源：http://hz.jinyuanbaomall.cn/gtkofredvh.html

Ruby: exit 1
来源：http://hz.snrcjt.cn/gtkyehwnxm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yanxiufei.cn/gtnuknqxlh.html

[M06] 向标准错误输出
来源：http://hz.xingfuxueyuan.xyz/gthtensowa.html

Py:   print("err", file=sys.stderr)
来源：http://hz.gogol.net.cn/gttsjpewlk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ybcxt.top/gtxfqrslce.html

JS:   console.error("err")
来源：http://hz.andypj.xyz/gtluckjzpr.html

TS:   console.error("err")
来源：http://hz.shanyushiyangtech.top/gtqnfsjfbn.html

Java: System.err.println("err")
来源：http://hz.yj20258888.top/gtxnpzqstv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.redwolf501.top/gtilpgesdz.html

Ruby: warn "err"
来源：http://hz.iojbl.cn/gtkbvjeryo.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ivvv.top/gtzxjfhbhd.html

[M07] 判断是否为主入口
来源：http://hz.9152youxi.cn/gtslkdeotn.html

Py:   if __name__ == "__main__":
来源：http://hz.jinqigufen.top/gtnpxzjtfc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.hywenlv.cn/gtdqpyvrbe.html

JS:   require.main === module
来源：http://hz.jlsjyb.cn/gtrgujjinj.html

TS:   require.main === module
来源：http://hz.tian-w.cn/gtwafibqjf.html

Java: public static void main(String[] args)
来源：http://hz.yj20258888.top/gtzowgvued.html

Go:   func main()
来源：http://hz.smart0.xyz/gtzzctiouh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.hnqzz.top/gtywrleleg.html

C#:   static void Main(string[] args)
来源：http://hz.zhongyouzk.top/gtifpwjudv.html

[M08] 获取系统与运行时信息
来源：http://hz.zhongyouzk.top/gtnxudmatt.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhengqikj.top/gtdnivobus.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.redwolf501.top/gtquypdlgw.html

JS:   process.platform;  process.version
来源：http://hz.ybcxt.top/gtjubaygsl.html

TS:   process.platform;  process.version
来源：http://hz.tian-w.cn/gtpjsagyjc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.ivvv.top/gtgupzjogw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.cqqwz.cn/gthnkpbdkm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.chenlongwang.top/gtxkoxeeae.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhoulong.xyz/gtqcejfhws.html

================================================================================
来源：http://hz.hfpthk.cn/gtvblcgvoa.html

N. 数据结构与算法
来源：http://hz.jiagoushi.top/gtxwzbwbrh.html

================================================================================
来源：http://hz.52xcode.cn/gtmbewraae.html

[N01] 二分查找（有序数组）
来源：http://hz.yj202588.top/gtxkgongjx.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.pycfn.com/gtvthjfgfy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.andypj.xyz/gtyceldpxz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hammf.cn/gthkpbxges.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hnxiangtu.top/gtbdupaumd.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.ppjwa.cn/gtyfaslass.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.sweek.top/gtpzmkafkj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jinqigfzy.top/gtwevjtgii.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.smart0.xyz/gtfzsvtcem.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.wangshuangyany.cn/gturjyitph.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhixingplan.top/gtiauhecwc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jianghu66.top/gtdkdcmtjr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hywenlv.cn/gtivzucnjb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jlsjyb.cn/gtlrprjaie.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.52xcode.cn/gtndddgnom.html

Go:   slices.Sort(arr)
来源：http://hz.chenlongwang.top/gtngxgrack.html

Ruby: arr.sort
来源：http://hz.svipenyu.cn/gtljdswzhh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.hfpthk.cn/gtnlxwdain.html

[N03] 快速排序（分治示例）
来源：http://hz.aizwys.cn/gtokrumezv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yonumen.top/gtrlcnfjgf.html

PHP:  // 递归实现，或用 usort
来源：http://hz.cqqwz.cn/gtacbsmyhe.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cucudq.cn/gtnvxkbprk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.pengpengdd.cyou/gthkliuhgq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.snrcjt.cn/gtbkozjrxg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yj202588.top/gttedewjqt.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.xziqi.cn/gtxdibrdqp.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.pycfn.com/gthxekzczh.html

[N04] 斐波那契数列
来源：http://hz.hnqzz.top/gtrgoxmbkv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.havefunace.top/gtgbqyfbyh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yongpay.top/gtvcysxbnp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhaomingkeji.xyz/gtwgannsxq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nwbrower.top/gtshnitxlu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.chenzaomai.com/gtukqahule.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.sweek.top/gtztbereug.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhixingplan.top/gtzyjitfhb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.gogol.net.cn/gtgzszobvg.html


<!-- 参考信息 -->