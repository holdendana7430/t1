代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yongpay.top/gtawdykaey.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yj202588.top/gtnysarwbv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhixingplan.top/gtharrwivt.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.cucudq.cn/gtldvfcpgc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.gotoacloud.top/gtcszisefc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.cucudq.cn/gtndumcpuo.html

[J09] 时区处理
来源：http://hz.jinqigfzy.top/gtntgwsqer.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ydzc1.top/gtjvwpbbis.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.redwolf501.top/gtfhgmaeim.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zycfv.cn/gtctihgtwz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.birdmap.top/gtqughprlh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ydzc1.top/gtnilsfrtw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xylfe.cn/gtlfketmbc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.iojbl.cn/gtetmbpued.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zdqjudy.top/gtbachuxlr.html

[J10] 取今天 / 本月第一天
来源：http://hz.yvedp.cn/gtamlosgma.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.tianlin.xyz/gtecteklot.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yanxiufei.cn/gtngsdowzh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yangfankeji.com/gtczsckoqw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.guannengcc.top/gtnsngumrl.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.gogol.net.cn/gtzvyfmvhg.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhaomingkeji.xyz/gtmjlryiqs.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.cdnleiting.top/gtkxovajvt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.dashuyun.cn/gtvbrqqucj.html

================================================================================
来源：http://hz.cashguo.top/gtnndliagb.html

K. JSON 与序列化
来源：http://hz.0kj1m.cn/gtbpkgwlqk.html

================================================================================
来源：http://hz.cucudq.cn/gtawgbvdbp.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhijiandao.cn/gthiivhtvf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ybcxt.top/gttdboxstu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yonumen.top/gtisphpmii.html

JS:   JSON.stringify(obj)
来源：http://hz.chenlongwang.top/gtiftaoccl.html

TS:   JSON.stringify(obj)
来源：http://hz.cqqwz.cn/gtoxoabshk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.bjfxy.top/gttufyocmb.html

Go:   json.Marshal(obj)
来源：http://hz.yuxming.cn/gtajiblcxy.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cheryme.top/gtywfyjnoy.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhoulong.xyz/gtcmkvfmru.html

[K02] JSON 字符串转对象
来源：http://hz.yuxming.cn/gthvaezxzg.html

Py:   json.loads(s)
来源：http://hz.hfpthk.cn/gtoqaxnbvd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yonumen.top/gtqgfctxpr.html

JS:   JSON.parse(s)
来源：http://hz.pycfn.com/gtsouorise.html

TS:   JSON.parse(s)
来源：http://hz.9152youxi.cn/gtbtetrhiz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.shzxlz.cn/gtachkpwza.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yueranfly.top/gtaqvebobg.html

Ruby: JSON.parse(s)
来源：http://hz.yj202588.top/gthvqoepqp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.316326.xyz/gtwefwccki.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.52xcode.cn/gtytaakirz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.tanke756.top/gtlmffnoav.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.sxryk.cn/gtzaodwcuy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yanxiufei.cn/gtmnbcnfep.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yueranfly.top/gtqcfedpud.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.nanxinkj.top/gtbioxtrqn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.316326.xyz/gtqoooicnd.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yj202588.top/gtfhljvdlg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xuanzx.com/gtzlunehyc.html

[K04] 读取 JSON 文件
来源：http://hz.zhixingplan.top/gtlziziqsj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zhijiandao.cn/gtnnbwtvph.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.sufxvd.cn/gttlqtocjs.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cqqwz.cn/gtftfnnaxe.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.aibaodan.cn/gtbkgitiwy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.gogol.net.cn/gtmordhcey.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.quarkkingdee.top/gtinkmdzei.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.kuanghao11.cn/gtuxpoiazc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.xingfuxueyuan.xyz/gtwajlbali.html

[K05] 深拷贝对象
来源：http://hz.guowangkeji.top/gthzmcbpdh.html

Py:   copy.deepcopy(obj)
来源：http://hz.haohaochexian.top/gtofmhorzz.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cashguo.top/gtjmwkyiuc.html

JS:   structuredClone(obj)
来源：http://hz.jqgfzy.top/gtovamtbsr.html

TS:   structuredClone(obj)
来源：http://hz.jlsjyb.cn/gtcrscnugh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.cashguo.top/gtlymawkzv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.wangshuangyany.cn/gtxwkytcki.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.pycfn.com/gthhyfzocc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.cheryme.top/gtvwuhixxl.html

[K06] 解析 URL 查询串
来源：http://hz.ehwqpu.com/gtklqkrllc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.svipenyu.cn/gtkcqdclji.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xingfuxueyuan.xyz/gtxqtreydz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.aizwys.cn/gtvxhdctoz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jiagoushi.top/gtznsrpenc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.gogol.net.cn/gtcaoqhlgf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.ybcxt.top/gtiparchfa.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.redwolf501.top/gtqjbnhiep.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cashguo.top/gtnppgjngr.html

[K07] 进制转换
来源：http://hz.shzxlz.cn/gtbnrkegde.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hammf.cn/gtofcplhvc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xinyue.icu/gtmxbhqcvi.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jiagoushi.top/gtoskuufqr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.chenjidiqi.icu/gtoqhlsvhp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.316326.xyz/gtgspvlgqw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yonumen.top/gtecmvbgyc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.vqdsnc.cn/gtnvuhwinm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ywan-chungtsiang.top/gttyhlegiq.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhongyouzk.top/gtlnxbggax.html

Py:   pickle.dumps(obj)
来源：http://hz.xuetiantiany.cn/gtrovldkgo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jinyuanbaomall.cn/gtscvsburl.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhoulong.xyz/gtzsfdkbqu.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhoulong.xyz/gtcyezwyhx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yuxming.cn/gtfeubeqfj.html

Go:   encoding/gob
来源：http://hz.andypj.xyz/gtlvwtmbgn.html

Ruby: Marshal.dump(obj)
来源：http://hz.daxiang520.top/gtyvtubitg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhijiandao.cn/gtggvjcgwm.html

================================================================================
来源：http://hz.tian-w.cn/gtthwrbmhq.html

L. 网络请求
来源：http://hz.meibo888.top/gtjikufccn.html

================================================================================
来源：http://hz.c1oappe.top/gtxyzvcupt.html

[L01] 发送 GET 请求
来源：http://hz.jqgfzy.top/gtbjheqfoo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.ydjk.org.cn/gtfjpffpqb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.guowangkeji.top/gtfizhudah.html

JS:   await fetch(url)
来源：http://hz.zhengqikj.top/gtstypxrsq.html

TS:   await fetch(url)
来源：http://hz.xylfe.cn/gtmdusnziy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ydzc1.top/gtfofmkrco.html

Go:   resp, err := http.Get(url)
来源：http://hz.c1oappe.top/gtsvewjrrf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.tian-w.cn/gtnhamnnja.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.xingfuxueyuan.xyz/gtkvbslvxp.html

[L02] 发送 POST JSON
来源：http://hz.ivvv.top/gtvhiwyraf.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.dianchejie.cn/gtfphiobkz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jqgfzy.top/gtncipavhm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shanyushiyangtech.top/gtarqpxcgr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.redwolf501.top/gtfnchurme.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.52xcode.cn/gtqieimikb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hnqzz.top/gtftxdeakj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.hnqzz.top/gthqrinwml.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hnqzz.top/gtyrxkzifz.html

[L03] 设置自定义请求头
来源：http://hz.havefunace.top/gtubtjyape.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hywenlv.cn/gttjlaaimw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.0kj1m.cn/gtqhisylgb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jqgfzy.top/gttypochqd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.guannengcc.top/gtfbkfwtxo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.cucudq.cn/gtazsyvkhf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jqgfzy.top/gtuodfgrph.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.haohaochexian.top/gtvrosbsbr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.tanke756.top/gtjspwomsp.html

[L04] 设置超时
来源：http://hz.xylfe.cn/gtybqhauen.html

Py:   requests.get(url, timeout=5)
来源：http://hz.nanxinkj.top/gtyiyralla.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.daxiang520.top/gtmbmcvykw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.andypj.xyz/gthncjrajf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.bjfxy.top/gtlizuuyej.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zycfv.cn/gtreqcxpws.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.gogol.net.cn/gtzgekwbcz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.feifeiyinyue.top/gtkrrowfkt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hywenlv.cn/gttjkchfox.html

[L05] 上传文件（multipart）
来源：http://hz.xziqi.cn/gtpnvpfwxh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hfpthk.cn/gtlgcdkrvb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yj202588.top/gtgwtnbxfh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.xylfe.cn/gtngbxecpv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.nanxuanxn.top/gtjdnivntn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zycfv.cn/gtfivmfaah.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.hywenlv.cn/gtkpzowtby.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yj20258888.top/gtyevxmxil.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jinqigufen.top/gtuvygvyjk.html

[L06] 解析响应为 JSON
来源：http://hz.redwolf501.top/gtpggdhmyi.html

Py:   resp.json()
来源：http://hz.jiagoushi.top/gtruawkmiu.html

PHP:  json_decode($body, true);
来源：http://hz.dianchejie.cn/gtcrfcrftn.html

JS:   await resp.json()
来源：http://hz.xinyue.icu/gtkphmkmra.html

TS:   await resp.json()
来源：http://hz.hysaishi.cn/gtjohgrolk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yj20258888.top/gtetnvcwdy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.ydzc1.top/gtwhbtjiuz.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yj20258.top/gtqyplpxlr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.pycfn.com/gtlhbkivza.html

[L07] 处理 HTTP 状态码
来源：http://hz.hfpthk.cn/gtywnlhdaq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.shanyushiyangkeji.top/gtrlhqnqaq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhijiandao.cn/gtcrpzifcr.html

JS:   resp.ok;  resp.status
来源：http://hz.zhoulong.xyz/gtxjacttjp.html

TS:   resp.ok;  resp.status
来源：http://hz.bjfxy.top/gtmfgxowkz.html

Java: resp.statusCode()
来源：http://hz.dianchejie.cn/gtptkvrbaj.html

Go:   resp.StatusCode
来源：http://hz.ivvv.top/gtiooobpvp.html

Ruby: resp.code.to_i
来源：http://hz.nwbrower.top/gtisanewnn.html

C#:   (int)resp.StatusCode
来源：http://hz.cashguo.top/gtrxdakgba.html

[L08] 并发请求多个地址
来源：http://hz.jiagoushi.top/gtaecccgpr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jinqigufen.top/gtsmrtphql.html

PHP:  curl_multi_init() 系列
来源：http://hz.shanyushiyangtech.top/gtdxvfcuuf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hfpthk.cn/gtfinxmaol.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.birdmap.top/gtvkqiezer.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhaomingkeji.xyz/gttvxqyegh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.cqqwz.cn/gttnvkytyt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zdqjudy.top/gttmdhbcak.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.shuidangran.top/gtojljaylf.html

================================================================================
来源：http://hz.yj202588.top/gttlhslkum.html

M. 命令行 / 进程 / 环境
来源：http://hz.ivvv.top/gtrnehjphd.html

================================================================================
来源：http://hz.yj20258888.top/gtpjxpypwk.html

[M01] 读取命令行参数
来源：http://hz.jlsjyb.cn/gtnoqrtfet.html

Py:   sys.argv[1:]
来源：http://hz.vqdsnc.cn/gtglocfxvy.html

PHP:  $argv;  $argc;
来源：http://hz.zhoulong.xyz/gtgpobzduu.html

JS:   process.argv.slice(2)
来源：http://hz.havefunace.top/gtqpkklzgj.html

TS:   process.argv.slice(2)
来源：http://hz.hongshengwenyu.top/gtamqpdrwa.html

Java: args 数组（main 方法参数）
来源：http://hz.yongpay.top/gtuldphjif.html

Go:   os.Args[1:]
来源：http://hz.mhx1999.top/gtclyxipjv.html

Ruby: ARGV
来源：http://hz.dashuyun.cn/gtaniwdfbl.html

C#:   args 数组（Main 方法参数）
来源：http://hz.smart0.xyz/gtigvbxrlj.html

[M02] 读取环境变量
来源：http://hz.cashguo.top/gthrtbgthr.html

Py:   os.environ.get("HOME")
来源：http://hz.pycfn.com/gtgjutdzmd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.andypj.xyz/gtexijzwxx.html

JS:   process.env.HOME
来源：http://hz.yj20258.top/gtbvnkxmvc.html

TS:   process.env.HOME
来源：http://hz.zhaomingkeji.xyz/gtxxdaxshf.html

Java: System.getenv("HOME")
来源：http://hz.shanyushiyangtech.top/gtyrhrvmdl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jiagoushi.top/gtzdsjecoi.html

Ruby: ENV["HOME"]
来源：http://hz.zhijiandao.cn/gtvgadcwqx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hfpthk.cn/gtbyvntsla.html

[M03] 执行外部命令
来源：http://hz.zhiwuduotai.top/gtxxqvswpw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yvedp.cn/gtfbsyxrqn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ywan-chungtsiang.top/gtxbadbyxy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinghuilouyu.cn/gthnlydrsc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xylfe.cn/gtuyjjcjki.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.0kj1m.cn/gtchvufyhw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yuxming.cn/gtftdkvhja.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yuxming.cn/gtvvqedxri.html

C#:   Process.Start("ls", "-l");
来源：http://hz.dianchejie.cn/gtovlkpqax.html

[M04] 获取当前工作目录
来源：http://hz.jinghuilouyu.cn/gtofedlfou.html

Py:   os.getcwd()
来源：http://hz.shanyushiyangtech.top/gtpjkjouom.html

PHP:  getcwd();
来源：http://hz.sxryk.cn/gtnimpjiro.html

JS:   process.cwd()
来源：http://hz.cheryme.top/gtrqpetzpm.html

TS:   process.cwd()
来源：http://hz.pengpengdd.cyou/gtppeqnorn.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.chenlongwang.top/gttjksobpd.html

Go:   os.Getwd()
来源：http://hz.andypj.xyz/gtvtzrhpbo.html

Ruby: Dir.pwd
来源：http://hz.yanxiufei.cn/gticiyplpz.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hfpthk.cn/gtnqlcermj.html

[M05] 设置退出码
来源：http://hz.xingfuxueyuan.xyz/gtpmjlwgwl.html

Py:   sys.exit(1)
来源：http://hz.gzhubu.top/gthukkvwht.html

PHP:  exit(1);
来源：http://hz.chenzaomai.com/gtswfuwadz.html

JS:   process.exit(1)
来源：http://hz.nanxinkj.top/gtdlunwuvw.html

TS:   process.exit(1)
来源：http://hz.52xcode.cn/gtrlgsxoty.html

Java: System.exit(1)
来源：http://hz.dianchejie.cn/gtbknmashg.html

Go:   os.Exit(1)
来源：http://hz.hywenlv.cn/gtrrfppbix.html

Ruby: exit 1
来源：http://hz.nanxinkj.top/gtaebcnnez.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.redwolf501.top/gtsbqncqhf.html

[M06] 向标准错误输出
来源：http://hz.pengpengdd.cyou/gtmxptmivp.html

Py:   print("err", file=sys.stderr)
来源：http://hz.guannengcc.top/gtbuutrnby.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yvedp.cn/gtpovifenw.html

JS:   console.error("err")
来源：http://hz.tanke756.top/gtkbmpteut.html

TS:   console.error("err")
来源：http://hz.chenjidiqi.icu/gtyspwkjzr.html

Java: System.err.println("err")
来源：http://hz.shanyushiyangtech.top/gtzefsgeef.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.cdnleiting.top/gtsgwerjry.html

Ruby: warn "err"
来源：http://hz.shangyingyoupin.top/gtfctcpsca.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hnqzz.top/gtcyeqzumo.html

[M07] 判断是否为主入口
来源：http://hz.9152youxi.cn/gtfyptykgd.html

Py:   if __name__ == "__main__":
来源：http://hz.jlsjyb.cn/gtoyceqpoe.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yuanzhike.top/gtzwrdajzz.html

JS:   require.main === module
来源：http://hz.redwolf501.top/gtmkgolbjd.html

TS:   require.main === module
来源：http://hz.zhoulong.xyz/gtvohgvtlf.html

Java: public static void main(String[] args)
来源：http://hz.yvedp.cn/gtpsxfpobd.html

Go:   func main()
来源：http://hz.sysykeji.top/gtiwuqgxnl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cheryme.top/gtckeidmyn.html

C#:   static void Main(string[] args)
来源：http://hz.yanxiufei.cn/gtmyjghskz.html

[M08] 获取系统与运行时信息
来源：http://hz.jyoumei.cn/gtvxvqgnvw.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yuxming.cn/gtjhqznpnt.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.iojbl.cn/gtrtvizmve.html

JS:   process.platform;  process.version
来源：http://hz.9152youxi.cn/gtafwrvbkr.html

TS:   process.platform;  process.version
来源：http://hz.hnqzz.top/gthabavdgu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zycfv.cn/gtfxomkxjt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yongpay.top/gthihpkpuc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zycfv.cn/gtrjfdzorx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.meibo888.top/gturvvfhvz.html

================================================================================
来源：http://hz.nanxuanxn.top/gtrlagolts.html

N. 数据结构与算法
来源：http://hz.jiagoushi.top/gtlqacjfra.html

================================================================================
来源：http://hz.wangdashe.top/gtudrzqciz.html

[N01] 二分查找（有序数组）
来源：http://hz.kuanghao11.cn/gtukykaqwv.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jinyuanbaomall.cn/gtxjdjpsrz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.xingfuxueyuan.xyz/gtpwayooeh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.daria6918.cn/gtzbyapqpl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.aizwys.cn/gttxlvoypn.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.xziqi.cn/gtcixknzjn.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.gzhubu.top/gtdkypcily.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.snrcjt.cn/gtaxlhoyyg.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.sweek.top/gtrnxnnjzn.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ybcxt.top/gtxrwhgrpg.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.aibaodan.cn/gtoilrwdyl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.shangyingyoupin.top/gtrzyuckis.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.kuanghao11.cn/gtzpprqpgg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhixingplan.top/gtyjyyexas.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.aibaodan.cn/gtjmvttgrj.html

Go:   slices.Sort(arr)
来源：http://hz.hysaishi.cn/gtxminlxvc.html

Ruby: arr.sort
来源：http://hz.chenzaomai.com/gtiozwzjte.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yj20258888.top/gtvpadljes.html

[N03] 快速排序（分治示例）
来源：http://hz.gogol.net.cn/gtmeuxhwef.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.sweek.top/gtihavwqlt.html

PHP:  // 递归实现，或用 usort
来源：http://hz.svipenyu.cn/gtipoooqcr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yj202588.top/gtyeqkigqj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.bjfxy.top/gtkwdkjxzh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.hnxiangtu.top/gtdyfrzdyg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.gaohongyu789.top/gtxxlowuym.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.aizwys.cn/gtoahdzziz.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.aizwys.cn/gtlohpnlfp.html

[N04] 斐波那契数列
来源：http://hz.zhengqikj.top/gthqjpvhuo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.cashguo.top/gtaqskxdti.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhoulong.xyz/gtqonexioj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jqgufenzy.top/gtrmikqhqg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.tian-w.cn/gtfnrbgqgf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.gzhubu.top/gtavfybhkc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.cucudq.cn/gtvxugvjha.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.bjfxy.top/gtasugkgzv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yueranfly.top/gtdyfkwqmu.html

[N05] 最大公约数
来源：http://hz.zycfv.cn/gtjfabcbxw.html

Py:   math.gcd(a, b)
来源：http://hz.vqdsnc.cn/gtprcarmjk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.fzhhl.top/gtxgyopaqq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.fzhhl.top/gtotblehuy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.c1oappe.top/gtohadviff.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jinyuanbaomall.cn/gtgyfaqjkk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.vqdsnc.cn/gtufuyphvb.html

Ruby: a.gcd(b)
来源：http://hz.quarkkingdee.top/gtgxjdhpih.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.gzhubu.top/gtagtwldan.html

[N06] 判断回文字符串
来源：http://hz.hnqzz.top/gtdprzuksw.html

Py:   s == s[::-1]
来源：http://hz.chenjidiqi.icu/gtnijoeezc.html

PHP:  $s === strrev($s);
来源：http://hz.jinqigufen.top/gtjpoicxzq.html


<!-- 参考信息 -->