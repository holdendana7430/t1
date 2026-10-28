代发 wailian999

[J07] 比较两个日期
来源：http://hz.yvedp.cn/gtiazkgvad.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ppjwa.cn/gtnwqakoyc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.chenlongwang.top/gtdasnakxr.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.xziqi.cn/gtvueocwss.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.52xcode.cn/gtbkkuhlfy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.fzhhl.top/gtctkqfyfc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.snrcjt.cn/gtseokbsxh.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.fengsongda.top/gtgrhpiiog.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.shanyushiyangkeji.top/gtrwboruhf.html

[J08] 提取年月日与星期
来源：http://hz.chenjidiqi.icu/gtkhwpiekf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hfpthk.cn/gtvtcviwpc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.mhx1999.top/gthxxabsqw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zdqjudy.top/gtjgezxmqi.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jinqigfzy.top/gturtdcrjd.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jyoumei.cn/gtngfwkqfr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jinqigfzy.top/gtglxevefi.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.52xcode.cn/gtuvfrrvjq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xingfuxueyuan.xyz/gtttxbojld.html

[J09] 时区处理
来源：http://hz.xuanzx.com/gtlhlbymjl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ydjk.org.cn/gtesbcuesf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.guowangkeji.top/gtzvcnxdru.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.birdmap.top/gtmcfmxyoo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.haohaochexian.top/gtsburgeji.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jyoumei.cn/gtrxdywohh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.chenzaomai.com/gtnxuqqbxv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.guannengcc.top/gtrpqqkltp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.tianlin.xyz/gttnpmdqcy.html

[J10] 取今天 / 本月第一天
来源：http://hz.hnqzz.top/gtihvnicwj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hysaishi.cn/gtkckvtwcl.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhongyouzk.top/gtupptoydi.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xziqi.cn/gtbiqrasot.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.iojbl.cn/gtilnkdupy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.hysaishi.cn/gteljgxink.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhixingplan.top/gtuzsinkuw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.cdnleiting.top/gtbnajsorg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yanxiufei.cn/gtcdgxxzrf.html

================================================================================
来源：http://hz.yj20258.top/gteigxcxrn.html

K. JSON 与序列化
来源：http://hz.sweek.top/gtoombimli.html

================================================================================
来源：http://hz.tian-w.cn/gtobavwpzb.html

[K01] 对象转 JSON 字符串
来源：http://hz.jinghuilouyu.cn/gtjbrlabke.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.aibaodan.cn/gtdcxxtfxc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.sysykeji.top/gtrltdilwi.html

JS:   JSON.stringify(obj)
来源：http://hz.dashuyun.cn/gtkkqcsfqt.html

TS:   JSON.stringify(obj)
来源：http://hz.52xcode.cn/gtukbfwkrz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.chenjidiqi.icu/gtxddzbbfh.html

Go:   json.Marshal(obj)
来源：http://hz.nanxuanxn.top/gtqvdgcbqc.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shanyushiyangtech.top/gtkumjdbzq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hongshengwenyu.top/gtiwyzpjvh.html

[K02] JSON 字符串转对象
来源：http://hz.cheryme.top/gtudjtmauz.html

Py:   json.loads(s)
来源：http://hz.smart0.xyz/gtrmpyaiag.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jianghu66.top/gtvbtqxvsc.html

JS:   JSON.parse(s)
来源：http://hz.gzhubu.top/gtcxiyvxzm.html

TS:   JSON.parse(s)
来源：http://hz.redwolf501.top/gtswuawdlr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.shanyushiyangtech.top/gtvjjwedqv.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.haohaochexian.top/gtklojapxr.html

Ruby: JSON.parse(s)
来源：http://hz.shzxlz.cn/gtwnjzzkei.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.daxiang520.top/gtkcjurzsu.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.daria6918.cn/gtykubufyc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.cashguo.top/gtjmkrmnfk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.guowangkeji.top/gtsljjiomp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.sufxvd.cn/gtfnqitxza.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj20258888.top/gtpizmuzri.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.guowangkeji.top/gtysvgzyqa.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.pengpengdd.cyou/gtampjhsed.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yonumen.top/gtibpcdass.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hammf.cn/gtssqfghah.html

[K04] 读取 JSON 文件
来源：http://hz.haohaochexian.top/gtfsmckeuz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yueranfly.top/gtwdnellyy.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cashguo.top/gthekcdigd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinqigfzy.top/gtqtwitrep.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sxryk.cn/gtthqkyogr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.316326.xyz/gtpdqrcrsq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.chenzaomai.com/gtpmvvtxte.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.guowangkeji.top/gtpijmloje.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.guowangkeji.top/gtqsbiltcf.html

[K05] 深拷贝对象
来源：http://hz.jlsjyb.cn/gtdzfkdrbd.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhaomingkeji.xyz/gthhqlpdso.html

PHP:  unserialize(serialize($obj));
来源：http://hz.chenjidiqi.icu/gtxctpsroh.html

JS:   structuredClone(obj)
来源：http://hz.sxryk.cn/gtvwlgfwjr.html

TS:   structuredClone(obj)
来源：http://hz.shanyushiyangtech.top/gtexxawoiq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yangfankeji.com/gtcrfvjmpj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.fzhhl.top/gtyzmvklac.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.chenlongwang.top/gtzrrtvvhs.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.gogol.net.cn/gtbctbvhuj.html

[K06] 解析 URL 查询串
来源：http://hz.jyoumei.cn/gtjxedscfg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xuanzx.com/gtheqoehda.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhiwuduotai.top/gtplprpgff.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hammf.cn/gtmckckpmf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xinyue.icu/gtnyhxrhty.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.guowangkeji.top/gtvzadoqgf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.shanyushiyangtech.top/gtpuxlfbfh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yj202588.top/gttusqhkmh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cucudq.cn/gtjdfmjqac.html

[K07] 进制转换
来源：http://hz.ydzc1.top/gtiystibse.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zdqjudy.top/gtoxcetrdl.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hfpthk.cn/gtqoqxmqfm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shzxlz.cn/gtpdfnwhwt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.guannengcc.top/gtywgwbbjx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.redwolf501.top/gthwbbvmjr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.pycfn.com/gtqiqzlrwe.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.shanyushiyangkeji.top/gtlpkkgvun.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.bjfxy.top/gtxuhaeenx.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.shuidangran.top/gtoejyjchj.html

Py:   pickle.dumps(obj)
来源：http://hz.ydjk.org.cn/gtojblwkzo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.nanxuanxn.top/gtdvvtwoxi.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.nwbrower.top/gtlnpngkxe.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.guowangkeji.top/gtggnpyeeu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yj20258.top/gthdxcykcb.html

Go:   encoding/gob
来源：http://hz.gaohongyu789.top/gtmsxrgrso.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhongyouzk.top/gtrmyuyewf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.chenjidiqi.icu/gtlttgphax.html

================================================================================
来源：http://hz.316326.xyz/gthvzrdnrk.html

L. 网络请求
来源：http://hz.kuanghao11.cn/gtitlfypae.html

================================================================================
来源：http://hz.xuanzx.com/gtpqdwqoti.html

[L01] 发送 GET 请求
来源：http://hz.cdnleiting.top/gtbjzmvzli.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.316326.xyz/gtumyvmnyd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ydjk.org.cn/gtrjptzprj.html

JS:   await fetch(url)
来源：http://hz.zhiwuduotai.top/gturkrqbwr.html

TS:   await fetch(url)
来源：http://hz.tian-w.cn/gtwqvuxoby.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.aizwys.cn/gtompblusg.html

Go:   resp, err := http.Get(url)
来源：http://hz.dianchejie.cn/gtliqlszwy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.0kj1m.cn/gtfokacbwi.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.birdmap.top/gtlsabadsd.html

[L02] 发送 POST JSON
来源：http://hz.xylfe.cn/gtkiupleii.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhijiandao.cn/gtvsyzpjom.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hongshengwenyu.top/gtiywwaclf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gzhubu.top/gtobuwdent.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.pycfn.com/gtmumtrcsk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yueranfly.top/gtnlxeaaua.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.sweek.top/gtveovbtlm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yonumen.top/gtkqtwkkgh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.shangyingyoupin.top/gtzvudadea.html

[L03] 设置自定义请求头
来源：http://hz.svipenyu.cn/gtpvwrfvcs.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.nanxinkj.top/gteojewqci.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.pengpengdd.cyou/gtgbdurvfk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gaohongyu789.top/gtneegmvyd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.pengpengdd.cyou/gtbocncscv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.cdnleiting.top/gtpyoqmyqo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.meibo888.top/gtvsyhwkzw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhijiandao.cn/gtiauwffwy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jinghuilouyu.cn/gtbgnmfuxi.html

[L04] 设置超时
来源：http://hz.vqdsnc.cn/gtqozyvnbb.html

Py:   requests.get(url, timeout=5)
来源：http://hz.havefunace.top/gtoqwgsuxk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.havefunace.top/gttflvfodx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.52xcode.cn/gtctgujrqn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.wangshuangyany.cn/gtfpjuslvy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.sysykeji.top/gthowkmcfa.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.feifeiyinyue.top/gtjtewmbft.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.cheryme.top/gtyvkyjxiv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ydjk.org.cn/gtwgywupbt.html

[L05] 上传文件（multipart）
来源：http://hz.hnqzz.top/gtwxgrhjwf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.vqdsnc.cn/gtnjebrfjg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.sweek.top/gtflckiydq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.xuetiantiany.cn/gtitfovbkz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.svipenyu.cn/gtedoqsasj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhoulong.xyz/gtisexdufp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.aibaodan.cn/gtnyrcypql.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shangyingyoupin.top/gtotwapwtb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.kuanghao11.cn/gtqudjgopl.html

[L06] 解析响应为 JSON
来源：http://hz.yvedp.cn/gtjngczopm.html

Py:   resp.json()
来源：http://hz.316326.xyz/gtoahbvfyo.html

PHP:  json_decode($body, true);
来源：http://hz.sweek.top/gtffspabcn.html

JS:   await resp.json()
来源：http://hz.sysykeji.top/gtedonymsz.html

TS:   await resp.json()
来源：http://hz.guannengcc.top/gtkjdyvulv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.birdmap.top/gtmwufudfx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.aizwys.cn/gtolticdun.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zycfv.cn/gtkcanvbuc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.nanxuanxn.top/gtblfsmqxf.html

[L07] 处理 HTTP 状态码
来源：http://hz.smart0.xyz/gtsyyoedmg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hnqzz.top/gtelsyaltr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhaomingkeji.xyz/gtadxxriik.html

JS:   resp.ok;  resp.status
来源：http://hz.hammf.cn/gtjmartkbs.html

TS:   resp.ok;  resp.status
来源：http://hz.tian-w.cn/gtchwnofda.html

Java: resp.statusCode()
来源：http://hz.sxryk.cn/gtffubkqbd.html

Go:   resp.StatusCode
来源：http://hz.shangyingyoupin.top/gttzoqzbqe.html

Ruby: resp.code.to_i
来源：http://hz.hongshengwenyu.top/gtvzimocjt.html

C#:   (int)resp.StatusCode
来源：http://hz.andypj.xyz/gtvnycdvcf.html

[L08] 并发请求多个地址
来源：http://hz.ydzc1.top/gtqvwtsalr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.meibo888.top/gtsfghiiyk.html

PHP:  curl_multi_init() 系列
来源：http://hz.sufxvd.cn/gtlmalhrob.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenjidiqi.icu/gtygcbcmlz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gaohongyu789.top/gtwjuxbuhy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ybcxt.top/gtnseozyid.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.cdnleiting.top/gtbiumvftq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yj20258888.top/gthcmyryxz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.gzhubu.top/gtmkjyyxgy.html

================================================================================
来源：http://hz.hnqzz.top/gtghwcoioz.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhoulong.xyz/gtcqgltanf.html

================================================================================
来源：http://hz.yj20258.top/gtvhcbghtf.html

[M01] 读取命令行参数
来源：http://hz.svipenyu.cn/gtdjfslxat.html

Py:   sys.argv[1:]
来源：http://hz.hammf.cn/gtviqqusxm.html

PHP:  $argv;  $argc;
来源：http://hz.jqgufenzy.top/gtaxbmbppf.html

JS:   process.argv.slice(2)
来源：http://hz.cashguo.top/gtbqrqymex.html

TS:   process.argv.slice(2)
来源：http://hz.c1oappe.top/gtmybehrgo.html

Java: args 数组（main 方法参数）
来源：http://hz.zdqjudy.top/gtwhcdvfri.html

Go:   os.Args[1:]
来源：http://hz.birdmap.top/gtjdjaidiv.html

Ruby: ARGV
来源：http://hz.zhongyouzk.top/gthzwcgdxd.html

C#:   args 数组（Main 方法参数）
来源：http://hz.cheryme.top/gtcrllojks.html

[M02] 读取环境变量
来源：http://hz.zhengqikj.top/gtwonojghc.html

Py:   os.environ.get("HOME")
来源：http://hz.xinyue.icu/gtmkatwzjq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.nanxuanxn.top/gtagsfomun.html

JS:   process.env.HOME
来源：http://hz.guowangkeji.top/gtriaynmjj.html

TS:   process.env.HOME
来源：http://hz.nwbrower.top/gtsdufojzf.html

Java: System.getenv("HOME")
来源：http://hz.feifeiyinyue.top/gtpsiuedfe.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.cqqwz.cn/gtasinbohe.html

Ruby: ENV["HOME"]
来源：http://hz.ybcxt.top/gtdfrxzcen.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shuidangran.top/gtpxhflzyg.html

[M03] 执行外部命令
来源：http://hz.jqgufenzy.top/gtaeyvuesu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xziqi.cn/gtnuitffqd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.chenjidiqi.icu/gttfnzggwg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yuanzhike.top/gtuyxqepzs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.cashguo.top/gtfypkpmmx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.sysykeji.top/gtenkwqkbm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hongshengwenyu.top/gtcuzovdmg.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jinghuilouyu.cn/gtlwqetnao.html

C#:   Process.Start("ls", "-l");
来源：http://hz.quarkkingdee.top/gtpndssfmn.html

[M04] 获取当前工作目录
来源：http://hz.pengpengdd.cyou/gtxqhtbmus.html

Py:   os.getcwd()
来源：http://hz.sxryk.cn/gteacybybw.html

PHP:  getcwd();
来源：http://hz.vqdsnc.cn/gtaioktwhj.html

JS:   process.cwd()
来源：http://hz.cheryme.top/gtzqovqnhz.html

TS:   process.cwd()
来源：http://hz.jyoumei.cn/gtxucyyexd.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ybcxt.top/gteqwxbwnj.html

Go:   os.Getwd()
来源：http://hz.cheryme.top/gtgqdjqkdb.html

Ruby: Dir.pwd
来源：http://hz.shuidangran.top/gtemarfkhw.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yueranfly.top/gtihyphque.html

[M05] 设置退出码
来源：http://hz.guannengcc.top/gtvpgugwmy.html

Py:   sys.exit(1)
来源：http://hz.xylfe.cn/gtyvacxejh.html

PHP:  exit(1);
来源：http://hz.snrcjt.cn/gthojwzldc.html

JS:   process.exit(1)
来源：http://hz.jiagoushi.top/gtqfnvfidr.html

TS:   process.exit(1)
来源：http://hz.hongshengwenyu.top/gtxmzejidv.html

Java: System.exit(1)
来源：http://hz.yj20258888.top/gttsejvwmc.html

Go:   os.Exit(1)
来源：http://hz.zhiwuduotai.top/gtkhnewjkh.html

Ruby: exit 1
来源：http://hz.nanxuanxn.top/gtgwjhosdk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yueranfly.top/gthgomiqyx.html

[M06] 向标准错误输出
来源：http://hz.jlsjyb.cn/gtgergiced.html

Py:   print("err", file=sys.stderr)
来源：http://hz.chenzaomai.com/gtucqtgpdj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yanxiufei.cn/gtynzppegs.html

JS:   console.error("err")
来源：http://hz.52xcode.cn/gtwauwfaua.html

TS:   console.error("err")
来源：http://hz.yangfankeji.com/gtndwosfqr.html

Java: System.err.println("err")
来源：http://hz.gotoacloud.top/gtmzjxodqu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.quarkkingdee.top/gtmcddoqjx.html

Ruby: warn "err"
来源：http://hz.gzhubu.top/gtkwcleqrv.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jinqigfzy.top/gtamxmpopd.html

[M07] 判断是否为主入口
来源：http://hz.hnxiangtu.top/gtktxwdxrh.html

Py:   if __name__ == "__main__":
来源：http://hz.316326.xyz/gtdshcsxmu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhongyouzk.top/gtpiayieob.html

JS:   require.main === module
来源：http://hz.cashguo.top/gthobstzkg.html

TS:   require.main === module
来源：http://hz.yvedp.cn/gtmqttovqr.html

Java: public static void main(String[] args)
来源：http://hz.jiagoushi.top/gtpodxylge.html

Go:   func main()
来源：http://hz.jqgfzy.top/gtbzndsyvq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ivvv.top/gtcyybnese.html

C#:   static void Main(string[] args)
来源：http://hz.gogol.net.cn/gtddujumaa.html

[M08] 获取系统与运行时信息
来源：http://hz.316326.xyz/gttdnqtllw.html

Py:   platform.system();  platform.python_version()
来源：http://hz.tian-w.cn/gtucnlluvx.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yanxiufei.cn/gtodqfklxq.html

JS:   process.platform;  process.version
来源：http://hz.tian-w.cn/gtmkpsodlj.html

TS:   process.platform;  process.version
来源：http://hz.gotoacloud.top/gtwvlgmard.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.shuidangran.top/gtnhbtjuao.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.gaohongyu789.top/gtqousdxpi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.tanke756.top/gtpukiwblf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.dianchejie.cn/gtpbduyfmw.html

================================================================================
来源：http://hz.zycfv.cn/gtgcujoelr.html

N. 数据结构与算法
来源：http://hz.cheryme.top/gttnsvfsdy.html

================================================================================
来源：http://hz.ehwqpu.com/gtsyqgtsxy.html

[N01] 二分查找（有序数组）
来源：http://hz.pengpengdd.cyou/gttgktuqgy.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ydjk.org.cn/gtuzidxzzh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.wangdashe.top/gtzpvupjdm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sufxvd.cn/gtvmarrhxn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinghuilouyu.cn/gtfottgmgp.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jlsjyb.cn/gtnqdvjrrh.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yj20258888.top/gtiejdnnny.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.aibaodan.cn/gthzomulcq.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.shangyingyoupin.top/gtitqomhzo.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.iojbl.cn/gtunxvxveq.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.daria6918.cn/gtefnhavef.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.sxryk.cn/gtulxaykjm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhengqikj.top/gtkoyuurgz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.bjfxy.top/gtqfkpmkwa.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.aizwys.cn/gtxvsoawyg.html

Go:   slices.Sort(arr)
来源：http://hz.bjfxy.top/gtntkaqafn.html

Ruby: arr.sort
来源：http://hz.tianlin.xyz/gtmrbmctak.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.52xcode.cn/gtmpsdlnna.html

[N03] 快速排序（分治示例）
来源：http://hz.shuidangran.top/gtejmytaou.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.gzhubu.top/gtxqqrddav.html

PHP:  // 递归实现，或用 usort
来源：http://hz.daxiang520.top/gtrmetlnjh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hongshengwenyu.top/gtsqcryiiu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xuetiantiany.cn/gtqlqfhwsp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jyoumei.cn/gtpenkszen.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yj20258.top/gtrktdpjfq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.dashuyun.cn/gtcbnglptt.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.vqdsnc.cn/gtpbuhqrim.html

[N04] 斐波那契数列
来源：http://hz.meibo888.top/gtziwxcxow.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jiagoushi.top/gtrxifbwyh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.havefunace.top/gtopgmzoso.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cheryme.top/gttvaquvck.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xuanzx.com/gtvqrqjhaw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zhengqikj.top/gtscdrgwwv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hnxiangtu.top/gtwihqhfvt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.wangdashe.top/gtngwwjmsz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.sxryk.cn/gttrzdabrz.html


<!-- 参考信息 -->