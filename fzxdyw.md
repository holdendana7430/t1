代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://hz.nwbrower.top/gthqvtlcmi.html

[J08] 提取年月日与星期
来源：http://hz.sufxvd.cn/gtbhdtfjcz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jinghuilouyu.cn/gtidsurisl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.redwolf501.top/gtozptjkny.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.kuanghao11.cn/gthngefjms.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.316326.xyz/gthcbddvbm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.cqqwz.cn/gtmrsxcfmi.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hnqzz.top/gtqfaadpyg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.c1oappe.top/gtnflnjmzf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.snrcjt.cn/gtjsmljjvc.html

[J09] 时区处理
来源：http://hz.havefunace.top/gtnxdeqiij.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.sxryk.cn/gtbettnhem.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.aizwys.cn/gtewbsaald.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.andypj.xyz/gtclfrqjjr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.redwolf501.top/gtajokebmb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.havefunace.top/gtpycjnxur.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.iojbl.cn/gtckrlcebl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.chenlongwang.top/gtplzmgmji.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.xuetiantiany.cn/gttvibwfur.html

[J10] 取今天 / 本月第一天
来源：http://hz.ehwqpu.com/gtuohnlcus.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yuxming.cn/gtpkvsrnnm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hfpthk.cn/gtmkqowegm.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.dashuyun.cn/gtdwnvcwmp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cheryme.top/gtmsqkkwmw.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.316326.xyz/gtqpdwbctm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhijiandao.cn/gtsarklpeg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.shanyushiyangkeji.top/gtyhsjnrna.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ywan-chungtsiang.top/gttqjyozuv.html

================================================================================
来源：http://hz.ppjwa.cn/gtovhkollw.html

K. JSON 与序列化
来源：http://hz.jqgfzy.top/gtpvyllbtn.html

================================================================================
来源：http://hz.yvedp.cn/gtkvpnrqol.html

[K01] 对象转 JSON 字符串
来源：http://hz.quarkkingdee.top/gtsygjtpof.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shanyushiyangkeji.top/gtrkqutump.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.pengpengdd.cyou/gtpsulitvg.html

JS:   JSON.stringify(obj)
来源：http://hz.daria6918.cn/gtkxpudaqa.html

TS:   JSON.stringify(obj)
来源：http://hz.gotoacloud.top/gtlprrduor.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhixingplan.top/gtstevaxnj.html

Go:   json.Marshal(obj)
来源：http://hz.pycfn.com/gthehvrojm.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shanyushiyangtech.top/gtxaohlpzj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhijiandao.cn/gtcyqouuem.html

[K02] JSON 字符串转对象
来源：http://hz.cqqwz.cn/gtorkkhqtq.html

Py:   json.loads(s)
来源：http://hz.pycfn.com/gtscburvdu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.redwolf501.top/gtumdlpubr.html

JS:   JSON.parse(s)
来源：http://hz.fzhhl.top/gtcatmonhy.html

TS:   JSON.parse(s)
来源：http://hz.xingfuxueyuan.xyz/gtwftovzvp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jinyuanbaomall.cn/gttgssiggh.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ywan-chungtsiang.top/gtuxditeny.html

Ruby: JSON.parse(s)
来源：http://hz.mhx1999.top/gtdrgjmwvs.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xuanzx.com/gtkbkrvfee.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jinghuilouyu.cn/gtqgnfaccb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yongpay.top/gtwctjusfh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.cashguo.top/gtipsnoeri.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hysaishi.cn/gthwkyzqpt.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yangfankeji.com/gthqqwlshs.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yongpay.top/gtnxkaswje.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hfpthk.cn/gtcpagcuyj.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jqgufenzy.top/gtidjgqiqx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.smart0.xyz/gtssbbamdy.html

[K04] 读取 JSON 文件
来源：http://hz.shanyushiyangtech.top/gtucvybiij.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.sxryk.cn/gttqttilcg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhoulong.xyz/gtryeycmtp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xinyue.icu/gtfnrkjxfd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yongpay.top/gtmtiyoxak.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ppjwa.cn/gtukzrevzb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.dianchejie.cn/gtvkjjblbj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.gotoacloud.top/gtcnlakvmj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.cqqwz.cn/gtvpdkyezj.html

[K05] 深拷贝对象
来源：http://hz.haohaochexian.top/gtqteafxhd.html

Py:   copy.deepcopy(obj)
来源：http://hz.jlsjyb.cn/gthoswxidc.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cheryme.top/gtnrnjekqo.html

JS:   structuredClone(obj)
来源：http://hz.havefunace.top/gtzlllkzvw.html

TS:   structuredClone(obj)
来源：http://hz.havefunace.top/gtcaulqnan.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.chenjidiqi.icu/gtqhkjrvsb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yj20258.top/gtascnvkfl.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhijiandao.cn/gtatuwwshx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ydzc1.top/gtvmrftgbu.html

[K06] 解析 URL 查询串
来源：http://hz.cheryme.top/gtxfzafrpw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.smart0.xyz/gtzbkcupwf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhengqikj.top/gtcuazbyhv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yuanzhike.top/gtabpmtjou.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.andypj.xyz/gtbbzgqsju.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhoulong.xyz/gthyavseuu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.c1oappe.top/gtevyflwqx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.mhx1999.top/gtmxgmpecu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.guowangkeji.top/gtkmiquwnl.html

[K07] 进制转换
来源：http://hz.guannengcc.top/gtoobwnjgg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhixingplan.top/gttzgncylu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.shzxlz.cn/gtwhrpcgdd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xylfe.cn/gtxakuwotm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ppjwa.cn/gtepkcbhjm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.9152youxi.cn/gtcjjyeiur.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hnxiangtu.top/gtruqxvktt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jqgufenzy.top/gtqhtkbwep.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ehwqpu.com/gtddvruazl.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.hfpthk.cn/gttyacoklh.html

Py:   pickle.dumps(obj)
来源：http://hz.redwolf501.top/gtuarwtnqq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hongshengwenyu.top/gtappiishk.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.mhx1999.top/gtoxoifjvm.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhongyouzk.top/gtpxppbgwv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.shuidangran.top/gtlullqozf.html

Go:   encoding/gob
来源：http://hz.haohaochexian.top/gtknfeddbo.html

Ruby: Marshal.dump(obj)
来源：http://hz.havefunace.top/gtlofffzsx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.52xcode.cn/gtjgajlpoy.html

================================================================================
来源：http://hz.fzhhl.top/gtppexmfte.html

L. 网络请求
来源：http://hz.hfpthk.cn/gtevnfubmu.html

================================================================================
来源：http://hz.snrcjt.cn/gtmhhduhpi.html

[L01] 发送 GET 请求
来源：http://hz.jinqigufen.top/gtqfnronhg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.havefunace.top/gtlfrifcaw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.xylfe.cn/gtiiuckibd.html

JS:   await fetch(url)
来源：http://hz.tian-w.cn/gtfzlhuffv.html

TS:   await fetch(url)
来源：http://hz.birdmap.top/gtceleuiho.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.shanyushiyangkeji.top/gtstkgyjmp.html

Go:   resp, err := http.Get(url)
来源：http://hz.redwolf501.top/gtvnplkalh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.shanyushiyangtech.top/gtbsftucqp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.tian-w.cn/gteaaagiha.html

[L02] 发送 POST JSON
来源：http://hz.jinyuanbaomall.cn/gtdpteammv.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.fzhhl.top/gtqyldzbtv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.cucudq.cn/gtlvusnbuj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhijiandao.cn/gtgdnzcaej.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.wangdashe.top/gtmobjrkih.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yuxming.cn/gtgkijtido.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.fengsongda.top/gtlwesaish.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yuxming.cn/gtezcxlusq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yvedp.cn/gtzpqzfdlc.html

[L03] 设置自定义请求头
来源：http://hz.mhx1999.top/gthperbxpt.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.quarkkingdee.top/gtesyryklm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ywan-chungtsiang.top/gtdyfwzanc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.quarkkingdee.top/gtsykleuhh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.redwolf501.top/gtaaosdsyh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yvedp.cn/gtqirnnrsc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hfpthk.cn/gtpnozjfnm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jinqigufen.top/gtluhqeqic.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ppjwa.cn/gtwyvrxrje.html

[L04] 设置超时
来源：http://hz.guowangkeji.top/gtxdjnsfap.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cashguo.top/gtmjzvtgbw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yj202588.top/gtdlzsdfmq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.vqdsnc.cn/gtwebezvti.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.guannengcc.top/gtozlqhjmp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.chenlongwang.top/gtvtohmmbh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.mhx1999.top/gtvqzynrzx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jyoumei.cn/gtrsquuvql.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.kuanghao11.cn/gtafhdzkuf.html

[L05] 上传文件（multipart）
来源：http://hz.ywan-chungtsiang.top/gtugoqyhzs.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhixingplan.top/gtpiknxtpy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.hysaishi.cn/gtglntlcrs.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yvedp.cn/gtfmyfnkny.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.birdmap.top/gtlgcpzgxh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.shanyushiyangkeji.top/gtkmwyiaag.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.hysaishi.cn/gtkjwcacme.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.guowangkeji.top/gtzucbnbuv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zdqjudy.top/gtrwflxvzj.html

[L06] 解析响应为 JSON
来源：http://hz.ydzc1.top/gtmdlimini.html

Py:   resp.json()
来源：http://hz.yvedp.cn/gthegbbdzv.html

PHP:  json_decode($body, true);
来源：http://hz.hammf.cn/gtvyqcnebs.html

JS:   await resp.json()
来源：http://hz.mhx1999.top/gtijzvszia.html

TS:   await resp.json()
来源：http://hz.daxiang520.top/gtgqjahkmg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.fengsongda.top/gtdabaxozs.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xuetiantiany.cn/gtqmrabiml.html

Ruby: JSON.parse(resp.body)
来源：http://hz.chenjidiqi.icu/gtfwdxxzym.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hammf.cn/gtssbkmvfm.html

[L07] 处理 HTTP 状态码
来源：http://hz.zdqjudy.top/gtwjmibewn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.316326.xyz/gthlajlkwd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.xylfe.cn/gtoofphelm.html

JS:   resp.ok;  resp.status
来源：http://hz.xuetiantiany.cn/gtwwcvqrsb.html

TS:   resp.ok;  resp.status
来源：http://hz.316326.xyz/gtgixftkht.html

Java: resp.statusCode()
来源：http://hz.cashguo.top/gtuczzxskr.html

Go:   resp.StatusCode
来源：http://hz.feifeiyinyue.top/gtbjsiirwk.html

Ruby: resp.code.to_i
来源：http://hz.yj202588.top/gtzlmtdoge.html

C#:   (int)resp.StatusCode
来源：http://hz.jyoumei.cn/gtqrybvzzj.html

[L08] 并发请求多个地址
来源：http://hz.ehwqpu.com/gtciijjggx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hongshengwenyu.top/gtvcoygghz.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhengqikj.top/gtqsrvorra.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinyuanbaomall.cn/gtmzraidyr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ydzc1.top/gtxaebfmso.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.chenlongwang.top/gthzmjrslh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhoulong.xyz/gtklzmftig.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.fengsongda.top/gtzldacbtt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.fengsongda.top/gtqtqsbkkz.html

================================================================================
来源：http://hz.andypj.xyz/gtalccehwh.html

M. 命令行 / 进程 / 环境
来源：http://hz.nanxinkj.top/gtcajkcyar.html

================================================================================
来源：http://hz.yonumen.top/gttucxtxcp.html

[M01] 读取命令行参数
来源：http://hz.chenlongwang.top/gteftlitje.html

Py:   sys.argv[1:]
来源：http://hz.havefunace.top/gtwdqgbxgw.html

PHP:  $argv;  $argc;
来源：http://hz.dianchejie.cn/gtpmvkhgbp.html

JS:   process.argv.slice(2)
来源：http://hz.meibo888.top/gtklywuacp.html

TS:   process.argv.slice(2)
来源：http://hz.meibo888.top/gtzgwuviav.html

Java: args 数组（main 方法参数）
来源：http://hz.haohaochexian.top/gtzekxwttf.html

Go:   os.Args[1:]
来源：http://hz.jinyuanbaomall.cn/gtvoqmzlhz.html

Ruby: ARGV
来源：http://hz.yueranfly.top/gtudnecvxr.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhiwuduotai.top/gtzyyicuqd.html

[M02] 读取环境变量
来源：http://hz.vqdsnc.cn/gtdmycwyqz.html

Py:   os.environ.get("HOME")
来源：http://hz.snrcjt.cn/gtoyhwusdc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zhiwuduotai.top/gtgtwkksfv.html

JS:   process.env.HOME
来源：http://hz.haohaochexian.top/gtktgghimq.html

TS:   process.env.HOME
来源：http://hz.jianghu66.top/gtpymknqqr.html

Java: System.getenv("HOME")
来源：http://hz.bjfxy.top/gtvqmhexsu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hammf.cn/gttmefcbek.html

Ruby: ENV["HOME"]
来源：http://hz.guowangkeji.top/gtznwfrvmd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hywenlv.cn/gtuuroujoy.html

[M03] 执行外部命令
来源：http://hz.ybcxt.top/gtxetpfhoo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.316326.xyz/gtbzyrqidd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.dashuyun.cn/gtvjjfnuhj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.52xcode.cn/gtipktgvqw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.quarkkingdee.top/gtixftjera.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.havefunace.top/gtzvqzpthk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.meibo888.top/gtupcdefth.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jlsjyb.cn/gtsxgutmtx.html

C#:   Process.Start("ls", "-l");
来源：http://hz.shuidangran.top/gtgngshlju.html

[M04] 获取当前工作目录
来源：http://hz.sxryk.cn/gtxkfbryno.html

Py:   os.getcwd()
来源：http://hz.ybcxt.top/gtocffjgaw.html

PHP:  getcwd();
来源：http://hz.guannengcc.top/gtljwjcwfs.html

JS:   process.cwd()
来源：http://hz.9152youxi.cn/gtkercdmpu.html

TS:   process.cwd()
来源：http://hz.birdmap.top/gtfpdknewf.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhengqikj.top/gtjiyswclv.html

Go:   os.Getwd()
来源：http://hz.chenjidiqi.icu/gtbwsxatzr.html

Ruby: Dir.pwd
来源：http://hz.0kj1m.cn/gtuhhzagll.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.redwolf501.top/gtutdvamkj.html

[M05] 设置退出码
来源：http://hz.ppjwa.cn/gtxnmalsvd.html

Py:   sys.exit(1)
来源：http://hz.jlsjyb.cn/gtsgnhnnmj.html

PHP:  exit(1);
来源：http://hz.cheryme.top/gtmaaiuknz.html

JS:   process.exit(1)
来源：http://hz.cashguo.top/gtpyafqcur.html

TS:   process.exit(1)
来源：http://hz.kuanghao11.cn/gtylmlyojm.html

Java: System.exit(1)
来源：http://hz.ydzc1.top/gtlfrjmafg.html

Go:   os.Exit(1)
来源：http://hz.hongshengwenyu.top/gtanbhqukt.html

Ruby: exit 1
来源：http://hz.sufxvd.cn/gtsapvkxgc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yj20258888.top/gttytrrzrz.html

[M06] 向标准错误输出
来源：http://hz.aibaodan.cn/gtbidjpisk.html

Py:   print("err", file=sys.stderr)
来源：http://hz.cashguo.top/gtieasksun.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.0kj1m.cn/gtpaedvivy.html

JS:   console.error("err")
来源：http://hz.jlsjyb.cn/gtxfbopldv.html

TS:   console.error("err")
来源：http://hz.jyoumei.cn/gtclvrsshz.html

Java: System.err.println("err")
来源：http://hz.haohaochexian.top/gtwocsiqvb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.fzhhl.top/gtvsaldlba.html

Ruby: warn "err"
来源：http://hz.xingfuxueyuan.xyz/gtxpvbwimg.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.gzhubu.top/gtryatlixk.html

[M07] 判断是否为主入口
来源：http://hz.wangdashe.top/gtzofaegne.html

Py:   if __name__ == "__main__":
来源：http://hz.hammf.cn/gtnksayrgu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.vqdsnc.cn/gtudrvhxnt.html

JS:   require.main === module
来源：http://hz.zhengqikj.top/gtqedhrjwl.html

TS:   require.main === module
来源：http://hz.cdnleiting.top/gtqgzxmwus.html

Java: public static void main(String[] args)
来源：http://hz.sweek.top/gtsvarixkg.html

Go:   func main()
来源：http://hz.cashguo.top/gtclttjyhb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.chenjidiqi.icu/gtroxugney.html

C#:   static void Main(string[] args)
来源：http://hz.svipenyu.cn/gtlnjfbsex.html

[M08] 获取系统与运行时信息
来源：http://hz.nwbrower.top/gtypkostff.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yonumen.top/gttdkoivwi.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zdqjudy.top/gtetaexgoz.html

JS:   process.platform;  process.version
来源：http://hz.jianghu66.top/gtmcinpmdw.html

TS:   process.platform;  process.version
来源：http://hz.chenjidiqi.icu/gtqxvjsgvj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.vqdsnc.cn/gtimmsqufh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jqgfzy.top/gticnodozq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.bjfxy.top/gtntfbkmmf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.birdmap.top/gtcalsxkuc.html

================================================================================
来源：http://hz.c1oappe.top/gtlgnktgmm.html

N. 数据结构与算法
来源：http://hz.316326.xyz/gtbdczosbh.html

================================================================================
来源：http://hz.ppjwa.cn/gtjokqcbmo.html

[N01] 二分查找（有序数组）
来源：http://hz.chenjidiqi.icu/gtrubyfovc.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jiagoushi.top/gtnulssjff.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yonumen.top/gtfqtrebar.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.svipenyu.cn/gtdusjhhkh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xuetiantiany.cn/gtcpqlsqbr.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.gzhubu.top/gtnqexotio.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jinqigufen.top/gtdongajeh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.fzhhl.top/gtuztftvgk.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.cdnleiting.top/gtkahecenr.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jinyuanbaomall.cn/gtiktmtpji.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yj20258.top/gtrlzwtsbl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jyoumei.cn/gtjfaomrol.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.tianlin.xyz/gtmzbrflms.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.iojbl.cn/gtxkbntqzr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.bjfxy.top/gtvrrdbrar.html

Go:   slices.Sort(arr)
来源：http://hz.chenjidiqi.icu/gtbqkqwxdz.html

Ruby: arr.sort
来源：http://hz.zhengqikj.top/gtkunpoblj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ydzc1.top/gtdspearea.html

[N03] 快速排序（分治示例）
来源：http://hz.andypj.xyz/gtsubnpctz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.shanyushiyangkeji.top/gteiucaokr.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yanxiufei.cn/gtucyskbao.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xuetiantiany.cn/gtmhfecveq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.sweek.top/gtolomxvcz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zdqjudy.top/gtuayclvgt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.fzhhl.top/gtsndwitjd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yvedp.cn/gtyvujetnw.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yanxiufei.cn/gtbrhezjbd.html

[N04] 斐波那契数列
来源：http://hz.shangyingyoupin.top/gtayxknbtc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ehwqpu.com/gtohgohpli.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jiagoushi.top/gtwlxraank.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.havefunace.top/gtddfqnpgl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yonumen.top/gtmyjwutof.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.52xcode.cn/gtzwuhzfvv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhengqikj.top/gtjmruvewi.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.tianlin.xyz/gtryjohwgk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.birdmap.top/gtgirmkpwh.html

[N05] 最大公约数
来源：http://hz.nanxuanxn.top/gtklzkogxf.html

Py:   math.gcd(a, b)
来源：http://hz.jianghu66.top/gttsmduwso.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.daxiang520.top/gtefydwxqq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.feifeiyinyue.top/gtsxnmcokr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jlsjyb.cn/gtgpgjrpoi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.meibo888.top/gtirtjydiu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jqgfzy.top/gtrklmtzmo.html

Ruby: a.gcd(b)
来源：http://hz.hnqzz.top/gtluvtrmns.html


<!-- 参考信息 -->