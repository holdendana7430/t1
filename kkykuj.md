代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://hz.daria6918.cn/gtltfzwnzo.html

Go:   end.Sub(start).Hours()
来源：http://hz.ydjk.org.cn/gtrbqwqssi.html

Ruby: end - start                 # 返回秒数
来源：http://hz.pengpengdd.cyou/gtkuqweikb.html

C#:   (end - start).TotalSeconds
来源：http://hz.xuanzx.com/gtkibmltoq.html

[J07] 比较两个日期
来源：http://hz.jinyuanbaomall.cn/gtshsubkhu.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.chenzaomai.com/gthvhzcmfg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.kuanghao11.cn/gteyvicrce.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.meibo888.top/gtqdkwkavj.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.smart0.xyz/gtyjexgaju.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.sysykeji.top/gtksomidqy.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jinqigfzy.top/gttesrntrg.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yangfankeji.com/gtjfmzwwcv.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.52xcode.cn/gtloqrrhyu.html

[J08] 提取年月日与星期
来源：http://hz.daria6918.cn/gtmzxjccjk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.cucudq.cn/gtohoytluf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.gotoacloud.top/gthpglguya.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.gotoacloud.top/gtsgugwput.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.gaohongyu789.top/gtyudrbknr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hnxiangtu.top/gtrgirvwtc.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hfpthk.cn/gtvaopfmci.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yanxiufei.cn/gtgaxtvvxi.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.andypj.xyz/gtfebgibfq.html

[J09] 时区处理
来源：http://hz.fzhhl.top/gtrtohytft.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.quarkkingdee.top/gtbsgzspbg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhaomingkeji.xyz/gtunubqitf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shzxlz.cn/gtwzeeokss.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jiagoushi.top/gtirnunimq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.fzhhl.top/gtbqaczguw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hysaishi.cn/gtmumuozut.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.mhx1999.top/gttwlbmjle.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.gaohongyu789.top/gtpbpxsrtx.html

[J10] 取今天 / 本月第一天
来源：http://hz.hnxiangtu.top/gtmkpekpuo.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yj20258888.top/gtbkxufwxj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.kuanghao11.cn/gtttrbioex.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yuxming.cn/gtajaadfur.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.kuanghao11.cn/gtacveqdgl.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.cucudq.cn/gtukoiwllw.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.daxiang520.top/gtteorwhdj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jinqigufen.top/gtafnmbdmf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ppjwa.cn/gtbqoarrvc.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtolbevjbg.html

K. JSON 与序列化
来源：http://hz.yueranfly.top/gtflohsgfg.html

================================================================================
来源：http://hz.jinqigfzy.top/gtvyybrqii.html

[K01] 对象转 JSON 字符串
来源：http://hz.mhx1999.top/gtsbzuczub.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ywan-chungtsiang.top/gtlagowxaa.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.chenlongwang.top/gtpgfzrqfe.html

JS:   JSON.stringify(obj)
来源：http://hz.smart0.xyz/gtgvxebgbo.html

TS:   JSON.stringify(obj)
来源：http://hz.ehwqpu.com/gtxenxdxiq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jinqigfzy.top/gtvvmiuygt.html

Go:   json.Marshal(obj)
来源：http://hz.jinyuanbaomall.cn/gtdprfgglm.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shzxlz.cn/gtrvprelmh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhongyouzk.top/gtzftylrbg.html

[K02] JSON 字符串转对象
来源：http://hz.nwbrower.top/gtskajdwgz.html

Py:   json.loads(s)
来源：http://hz.316326.xyz/gtcihgfsdl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zdqjudy.top/gtfmrsqlkk.html

JS:   JSON.parse(s)
来源：http://hz.hysaishi.cn/gtxklcenbe.html

TS:   JSON.parse(s)
来源：http://hz.jqgufenzy.top/gtlisonxbc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.fzhhl.top/gtisnqbpeh.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.guannengcc.top/gtpgixduoy.html

Ruby: JSON.parse(s)
来源：http://hz.vqdsnc.cn/gtwhdafhiq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hywenlv.cn/gtmmhhdtxq.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zycfv.cn/gthapgtydq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.nwbrower.top/gtezpnjyzc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yueranfly.top/gtcienalfh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj20258888.top/gtorjnrajy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hysaishi.cn/gtxrymbspx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.gotoacloud.top/gtavuchurt.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.guowangkeji.top/gtepipaqgc.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhixingplan.top/gtpbbbpjyr.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jinqigufen.top/gtlwxhyzeu.html

[K04] 读取 JSON 文件
来源：http://hz.hfpthk.cn/gtpluieibr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.dianchejie.cn/gtnumabfxc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jinqigufen.top/gtkagqdszf.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hnxiangtu.top/gtqlhwlgwc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gotoacloud.top/gthkilqjwg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hnxiangtu.top/gtpfgwkmvs.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yj202588.top/gtuadwkpti.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hywenlv.cn/gtamohuwrx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.9152youxi.cn/gtlreqccxi.html

[K05] 深拷贝对象
来源：http://hz.snrcjt.cn/gtusjoufes.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhaomingkeji.xyz/gtjzfhhxps.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhoulong.xyz/gtdhzmgpdh.html

JS:   structuredClone(obj)
来源：http://hz.hnqzz.top/gtaparjsbb.html

TS:   structuredClone(obj)
来源：http://hz.tianlin.xyz/gtdbvyfbon.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.gogol.net.cn/gtsjtbqlvj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.fzhhl.top/gtwqhwihbg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jinyuanbaomall.cn/gthbnxmhwx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.wangdashe.top/gtrbojzmhr.html

[K06] 解析 URL 查询串
来源：http://hz.yongpay.top/gtlqjrxhli.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ybcxt.top/gtuvaehowg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yonumen.top/gtwvanqofp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinqigfzy.top/gtmtdywcfc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.chenzaomai.com/gtynodwsqt.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zycfv.cn/gtxceuamkd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.sysykeji.top/gtanknqhol.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ehwqpu.com/gtszfdtdft.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.hammf.cn/gtpqufmcje.html

[K07] 进制转换
来源：http://hz.vqdsnc.cn/gtjoiwossm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jinyuanbaomall.cn/gtfhkktbbv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jianghu66.top/gtcnagzszx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhaomingkeji.xyz/gtflqkjtgo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.quarkkingdee.top/gtrvzssodp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yuanzhike.top/gtfavyuxee.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.wangshuangyany.cn/gtceujnegc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.daxiang520.top/gtlkcmqjps.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.birdmap.top/gtugepbznr.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.sufxvd.cn/gtknsbpzpu.html

Py:   pickle.dumps(obj)
来源：http://hz.smart0.xyz/gtcrubmsyu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.sxryk.cn/gtatadaffb.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.pycfn.com/gtsitwmnxe.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ywan-chungtsiang.top/gtelmhquud.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hammf.cn/gtwicowjhq.html

Go:   encoding/gob
来源：http://hz.gaohongyu789.top/gtbfajjivy.html

Ruby: Marshal.dump(obj)
来源：http://hz.jqgufenzy.top/gtpvhhhshd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xinyue.icu/gtbltoudxk.html

================================================================================
来源：http://hz.pycfn.com/gtjtjjwejm.html

L. 网络请求
来源：http://hz.hnxiangtu.top/gtfyquqxov.html

================================================================================
来源：http://hz.mhx1999.top/gtzqbnfxcd.html

[L01] 发送 GET 请求
来源：http://hz.sufxvd.cn/gtvfokazjl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.quarkkingdee.top/gtpctstiky.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhijiandao.cn/gtqckgzhhv.html

JS:   await fetch(url)
来源：http://hz.haohaochexian.top/gtxyxbruwg.html

TS:   await fetch(url)
来源：http://hz.cqqwz.cn/gtbtnkaykg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hammf.cn/gtitdoocpb.html

Go:   resp, err := http.Get(url)
来源：http://hz.pycfn.com/gtdajuuoei.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.gogol.net.cn/gtadxgwagz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.sysykeji.top/gtsgciowoh.html

[L02] 发送 POST JSON
来源：http://hz.dianchejie.cn/gtwgtfzdol.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.mhx1999.top/gtualphhqk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.nanxuanxn.top/gtgmlamhcb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yongpay.top/gtnxzurzkt.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.nanxuanxn.top/gtwwtfdvwr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.xingfuxueyuan.xyz/gtfoyemgag.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhaomingkeji.xyz/gttckzobnq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yangfankeji.com/gtapeiswpo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.tian-w.cn/gthqofbgwi.html

[L03] 设置自定义请求头
来源：http://hz.vqdsnc.cn/gtholzrgzr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jinghuilouyu.cn/gtnkczysvn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.guowangkeji.top/gtomydlgrt.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.havefunace.top/gtriidlfgq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nwbrower.top/gtekimsbgo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.xinyue.icu/gteuiveatv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yj202588.top/gtbyunrxes.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yuanzhike.top/gtgrgamfof.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zycfv.cn/gtnieufeug.html

[L04] 设置超时
来源：http://hz.jinyuanbaomall.cn/gthcubksvs.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hywenlv.cn/gtgpykiwrv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.hfpthk.cn/gtefasivih.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jyoumei.cn/gtfezpiqmg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zycfv.cn/gtqehknjcc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zdqjudy.top/gtftxflfha.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.gzhubu.top/gticonxuje.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.bjfxy.top/gtyxrblguv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hnxiangtu.top/gtyqpkeqeu.html

[L05] 上传文件（multipart）
来源：http://hz.yj20258888.top/gtucbjaewi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.havefunace.top/gtjnwhoccx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xinyue.icu/gtfnhnpslo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.feifeiyinyue.top/gtkdkwqomr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.haohaochexian.top/gtpjewyoyu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.daria6918.cn/gtwapzcrwv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.daxiang520.top/gtybqbvvgj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.sweek.top/gtkkrgmqcs.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.guannengcc.top/gtaxvxetre.html

[L06] 解析响应为 JSON
来源：http://hz.xingfuxueyuan.xyz/gtqhkggglx.html

Py:   resp.json()
来源：http://hz.zhaomingkeji.xyz/gtmbkhpxfq.html

PHP:  json_decode($body, true);
来源：http://hz.wangdashe.top/gtqdbrosvr.html

JS:   await resp.json()
来源：http://hz.birdmap.top/gtcwpshzyr.html

TS:   await resp.json()
来源：http://hz.jinyuanbaomall.cn/gthwipkwsv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.smart0.xyz/gtjlqxvwhx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.chenjidiqi.icu/gtxqpxnirh.html

Ruby: JSON.parse(resp.body)
来源：http://hz.hfpthk.cn/gtacrqglda.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.iojbl.cn/gtzwolljou.html

[L07] 处理 HTTP 状态码
来源：http://hz.tian-w.cn/gtdikmscaq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.pengpengdd.cyou/gtxpqzziuo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jqgufenzy.top/gtdoyugmgb.html

JS:   resp.ok;  resp.status
来源：http://hz.yj20258.top/gtilyazwuw.html

TS:   resp.ok;  resp.status
来源：http://hz.dashuyun.cn/gtkjlrgscz.html

Java: resp.statusCode()
来源：http://hz.yueranfly.top/gtldsxwfxq.html

Go:   resp.StatusCode
来源：http://hz.yj20258888.top/gtbjbesrbh.html

Ruby: resp.code.to_i
来源：http://hz.kuanghao11.cn/gtgrfndkmu.html

C#:   (int)resp.StatusCode
来源：http://hz.shanyushiyangkeji.top/gtfjlzzohp.html

[L08] 并发请求多个地址
来源：http://hz.jlsjyb.cn/gtwttogiga.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.mhx1999.top/gtqdnyjoyh.html

PHP:  curl_multi_init() 系列
来源：http://hz.9152youxi.cn/gtctwjjruk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.feifeiyinyue.top/gtuexmmzrc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.52xcode.cn/gtjktjnxbj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ivvv.top/gtbmcsggcx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.gotoacloud.top/gtpbwzsvmh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ehwqpu.com/gtndmaljzx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.daxiang520.top/gttikbjmcb.html

================================================================================
来源：http://hz.ydzc1.top/gtuwawdrjp.html

M. 命令行 / 进程 / 环境
来源：http://hz.xingfuxueyuan.xyz/gtbzuzqkqy.html

================================================================================
来源：http://hz.chenzaomai.com/gttvjfokls.html

[M01] 读取命令行参数
来源：http://hz.hfpthk.cn/gtnwpqigez.html

Py:   sys.argv[1:]
来源：http://hz.dianchejie.cn/gtdennpgyi.html

PHP:  $argv;  $argc;
来源：http://hz.meibo888.top/gtabdaxsko.html

JS:   process.argv.slice(2)
来源：http://hz.tanke756.top/gtpwbpplik.html

TS:   process.argv.slice(2)
来源：http://hz.shzxlz.cn/gtdaonxqxu.html

Java: args 数组（main 方法参数）
来源：http://hz.feifeiyinyue.top/gtgkpgucfe.html

Go:   os.Args[1:]
来源：http://hz.jyoumei.cn/gtabharuyv.html

Ruby: ARGV
来源：http://hz.yangfankeji.com/gtdgpwpojx.html

C#:   args 数组（Main 方法参数）
来源：http://hz.chenlongwang.top/gtnoaonqso.html

[M02] 读取环境变量
来源：http://hz.snrcjt.cn/gtqzptxcpb.html

Py:   os.environ.get("HOME")
来源：http://hz.ydjk.org.cn/gtkoebjatu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.iojbl.cn/gtzbtdzdnz.html

JS:   process.env.HOME
来源：http://hz.jianghu66.top/gthyluxmtt.html

TS:   process.env.HOME
来源：http://hz.redwolf501.top/gtbzzlcibo.html

Java: System.getenv("HOME")
来源：http://hz.guannengcc.top/gtxnzijafs.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhongyouzk.top/gtsolilzvc.html

Ruby: ENV["HOME"]
来源：http://hz.pengpengdd.cyou/gtyggsxlbu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hongshengwenyu.top/gtlfarznhb.html

[M03] 执行外部命令
来源：http://hz.yvedp.cn/gtpinibzqe.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jqgufenzy.top/gtmmdkrwpl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.tanke756.top/gthkmrkjyo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hammf.cn/gtihyataom.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hfpthk.cn/gtltukooty.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.xuetiantiany.cn/gtjtjdvdca.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.sweek.top/gtsfemwafu.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.bjfxy.top/gtenuuzgzu.html

C#:   Process.Start("ls", "-l");
来源：http://hz.gogol.net.cn/gtdbmmlgeb.html

[M04] 获取当前工作目录
来源：http://hz.jinqigfzy.top/gtdkvbddjs.html

Py:   os.getcwd()
来源：http://hz.xingfuxueyuan.xyz/gtfhaooemj.html

PHP:  getcwd();
来源：http://hz.svipenyu.cn/gtfwkhrkwx.html

JS:   process.cwd()
来源：http://hz.zhijiandao.cn/gtqojivejd.html

TS:   process.cwd()
来源：http://hz.kuanghao11.cn/gtaxulyeoz.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.tanke756.top/gtwsosrekb.html

Go:   os.Getwd()
来源：http://hz.9152youxi.cn/gtlwphszrt.html

Ruby: Dir.pwd
来源：http://hz.gzhubu.top/gtaifmomyq.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.feifeiyinyue.top/gtcdwdvykz.html

[M05] 设置退出码
来源：http://hz.vqdsnc.cn/gtsddxbrsp.html

Py:   sys.exit(1)
来源：http://hz.havefunace.top/gtndgujucp.html

PHP:  exit(1);
来源：http://hz.zycfv.cn/gtvgacmfip.html

JS:   process.exit(1)
来源：http://hz.xingfuxueyuan.xyz/gtidvflcrx.html

TS:   process.exit(1)
来源：http://hz.yj202588.top/gtskvjeyjw.html

Java: System.exit(1)
来源：http://hz.yangfankeji.com/gtngivxrrl.html

Go:   os.Exit(1)
来源：http://hz.yuxming.cn/gtftrtbwoo.html

Ruby: exit 1
来源：http://hz.guowangkeji.top/gthhqzaual.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.havefunace.top/gtsjrbpxbv.html

[M06] 向标准错误输出
来源：http://hz.cashguo.top/gtxljtekgv.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hammf.cn/gtvcqtsxii.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.daxiang520.top/gtafdgpuaf.html

JS:   console.error("err")
来源：http://hz.xinyue.icu/gtyewrqazt.html

TS:   console.error("err")
来源：http://hz.jyoumei.cn/gtyjrxdhdl.html

Java: System.err.println("err")
来源：http://hz.shanyushiyangtech.top/gtgeahopke.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.sysykeji.top/gtopjeimmo.html

Ruby: warn "err"
来源：http://hz.zhengqikj.top/gtrriyyxap.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhengqikj.top/gtjhtbncjt.html

[M07] 判断是否为主入口
来源：http://hz.chenzaomai.com/gtacbfpqmk.html

Py:   if __name__ == "__main__":
来源：http://hz.birdmap.top/gtymgmytci.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cashguo.top/gtxmkepyuq.html

JS:   require.main === module
来源：http://hz.0kj1m.cn/gtuzfjekmn.html

TS:   require.main === module
来源：http://hz.sufxvd.cn/gtsmlddiyk.html

Java: public static void main(String[] args)
来源：http://hz.316326.xyz/gtqqfxtzym.html

Go:   func main()
来源：http://hz.zycfv.cn/gtxgeelexl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.quarkkingdee.top/gtpbifotzq.html

C#:   static void Main(string[] args)
来源：http://hz.daxiang520.top/gtrbwsutlp.html

[M08] 获取系统与运行时信息
来源：http://hz.hnqzz.top/gtaeuluwvj.html

Py:   platform.system();  platform.python_version()
来源：http://hz.quarkkingdee.top/gtoypzboti.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ppjwa.cn/gtyjbqfnse.html

JS:   process.platform;  process.version
来源：http://hz.chenlongwang.top/gtfnghqqzh.html

TS:   process.platform;  process.version
来源：http://hz.jqgufenzy.top/gtbxprqozo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.ydzc1.top/gtpweidtuq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jianghu66.top/gtidpfjmmc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ydzc1.top/gtqbimavkq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jianghu66.top/gttmrdmxjm.html

================================================================================
来源：http://hz.hnxiangtu.top/gtaymaelwq.html

N. 数据结构与算法
来源：http://hz.cdnleiting.top/gtcpibniog.html

================================================================================
来源：http://hz.ydzc1.top/gtlqhksqxe.html

[N01] 二分查找（有序数组）
来源：http://hz.chenjidiqi.icu/gtuucsrroc.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.tanke756.top/gtvgjidglm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yvedp.cn/gtcgeaivpj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ydjk.org.cn/gtoxyydyzu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ppjwa.cn/gtiotkkscb.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yj20258888.top/gtpqcsxyii.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.feifeiyinyue.top/gtpblghtda.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.bjfxy.top/gtnobtawor.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gtjyyxokoy.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ehwqpu.com/gtzwjwprgk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.quarkkingdee.top/gtlzckrfbg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yj20258888.top/gtoxjxgzcc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sweek.top/gtrhawlpdk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.pengpengdd.cyou/gthopxrekm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.tanke756.top/gtkfafvqgn.html

Go:   slices.Sort(arr)
来源：http://hz.vqdsnc.cn/gtyfbqxxvi.html

Ruby: arr.sort
来源：http://hz.316326.xyz/gtilajcifj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jinghuilouyu.cn/gtdxqjjstx.html

[N03] 快速排序（分治示例）
来源：http://hz.wangshuangyany.cn/gtoamsimpg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hywenlv.cn/gtyfnedhda.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zhaomingkeji.xyz/gtqqkdmxdb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tian-w.cn/gtpsqnihyk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.aibaodan.cn/gtdleatunz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yj202588.top/gtksnyullb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jlsjyb.cn/gtzqsareoz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.sxryk.cn/gtjgzlrhiy.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yuxming.cn/gtdrfpmyab.html

[N04] 斐波那契数列
来源：http://hz.hfpthk.cn/gtkinlhqki.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.cucudq.cn/gtlaoifwlt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.nanxuanxn.top/gtnxojzxzt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hammf.cn/gtctfbjyxp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yonumen.top/gtyjrqacgx.html


<!-- 参考信息 -->