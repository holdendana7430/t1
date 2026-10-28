代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.ydjk.org.cn/gtmzrqnwhr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.smart0.xyz/gtuaglrkom.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.vqdsnc.cn/gtdghpeooj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.fzhhl.top/gtvwgxrcux.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.sweek.top/gtzyutfgwr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.shangyingyoupin.top/gtymzxmgeq.html

[J09] 时区处理
来源：http://hz.yj20258.top/gtyrqrysvs.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shanyushiyangkeji.top/gtprophqbi.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.wangshuangyany.cn/gttdhjfgft.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj202588.top/gtbhzmzbsy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ydjk.org.cn/gtvyhqluhb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hongshengwenyu.top/gtsqynedwy.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jinghuilouyu.cn/gtztqczxdw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jinyuanbaomall.cn/gtljkikqcl.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.9152youxi.cn/gtqfnymuac.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhijiandao.cn/gttwiptrsq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.chenjidiqi.icu/gtdlhyegoh.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yanxiufei.cn/gtauvnuyai.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.daria6918.cn/gtrtlyamaj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.snrcjt.cn/gtctrsitvl.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhengqikj.top/gthhybuhkc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.cqqwz.cn/gtymcvueqh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.c1oappe.top/gtlztfcsym.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.cashguo.top/gtidcqzwfw.html

================================================================================
来源：http://hz.guannengcc.top/gtqbvdamyd.html

K. JSON 与序列化
来源：http://hz.zhixingplan.top/gtwfhmcljn.html

================================================================================
来源：http://hz.jinqigufen.top/gtsfwgvgpu.html

[K01] 对象转 JSON 字符串
来源：http://hz.aizwys.cn/gtyvniavlv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jlsjyb.cn/gtgyeoxkdz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.kuanghao11.cn/gtsqdjqopk.html

JS:   JSON.stringify(obj)
来源：http://hz.haohaochexian.top/gtpkyeugmp.html

TS:   JSON.stringify(obj)
来源：http://hz.xuanzx.com/gtwkkkpvim.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.haohaochexian.top/gtemabdvzi.html

Go:   json.Marshal(obj)
来源：http://hz.cdnleiting.top/gtuwkudiqk.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.9152youxi.cn/gtuxbglmzc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.nanxuanxn.top/gtkbnquuge.html

[K02] JSON 字符串转对象
来源：http://hz.52xcode.cn/gtioegkfbq.html

Py:   json.loads(s)
来源：http://hz.yongpay.top/gtbxouepvj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.havefunace.top/gtrmnwxxgq.html

JS:   JSON.parse(s)
来源：http://hz.guowangkeji.top/gtlkcsdygf.html

TS:   JSON.parse(s)
来源：http://hz.ppjwa.cn/gtfkxumczi.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.shangyingyoupin.top/gtbcmkpojs.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jinyuanbaomall.cn/gtlczfapev.html

Ruby: JSON.parse(s)
来源：http://hz.snrcjt.cn/gthhxzqpeg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ivvv.top/gtvrrjufwm.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yuanzhike.top/gtxfixqyby.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ydzc1.top/gtbjqzucgq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.chenzaomai.com/gtuvhqyofp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.nwbrower.top/gtozmlzsyx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.sxryk.cn/gtexarkmpi.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ivvv.top/gthikfejkw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.tian-w.cn/gtqxrgnpbw.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhiwuduotai.top/gtffcqflpn.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cheryme.top/gtposvqwlo.html

[K04] 读取 JSON 文件
来源：http://hz.0kj1m.cn/gtqpozznwi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jinqigufen.top/gtispxursc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.dashuyun.cn/gtdpylpbof.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gogol.net.cn/gtwnpopoku.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cdnleiting.top/gtbxgisosc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.nwbrower.top/gtnwjpnfsu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xziqi.cn/gtdcjsdpft.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.mhx1999.top/gtyfvejego.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.kuanghao11.cn/gtsirpekrh.html

[K05] 深拷贝对象
来源：http://hz.yanxiufei.cn/gtexmypnnf.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhongyouzk.top/gtpdnrfdom.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ivvv.top/gtjndggxit.html

JS:   structuredClone(obj)
来源：http://hz.0kj1m.cn/gtcvwydaiz.html

TS:   structuredClone(obj)
来源：http://hz.ywan-chungtsiang.top/gteyzezfdt.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.birdmap.top/gttsygmofd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yj20258.top/gtmcpnkqzp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shzxlz.cn/gtcxdrifgl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ywan-chungtsiang.top/gttkcgawmv.html

[K06] 解析 URL 查询串
来源：http://hz.zhoulong.xyz/gtegouxyrr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.cucudq.cn/gtjznqqujn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.fzhhl.top/gtjfwlyxjr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.316326.xyz/gtxhskjzsc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yuanzhike.top/gtbnmrddik.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.dianchejie.cn/gtwnlytqxs.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.c1oappe.top/gtitnkbozh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhengqikj.top/gtkctevmdg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.shuidangran.top/gtrofuhzfp.html

[K07] 进制转换
来源：http://hz.guannengcc.top/gtbbuaatmy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.pengpengdd.cyou/gtrnvzqena.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ydjk.org.cn/gtykebeshi.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.meibo888.top/gtmkxcpohh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.cdnleiting.top/gtgzecdhnt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhaomingkeji.xyz/gtwdqwskcc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yanxiufei.cn/gtxjscjdyd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.quarkkingdee.top/gtqqhuhkuc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.cheryme.top/gtsnzppjsi.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.daxiang520.top/gttdnkovjz.html

Py:   pickle.dumps(obj)
来源：http://hz.chenjidiqi.icu/gtcszqzhkb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.gogol.net.cn/gtwvznkmbl.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhongyouzk.top/gttiisykga.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.tanke756.top/gtdwcqxcyl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.cheryme.top/gtxdirtcjk.html

Go:   encoding/gob
来源：http://hz.hnqzz.top/gtqsmcfcnm.html

Ruby: Marshal.dump(obj)
来源：http://hz.jianghu66.top/gtvbhvwarp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zycfv.cn/gtfnngxwsy.html

================================================================================
来源：http://hz.bjfxy.top/gttrjgowue.html

L. 网络请求
来源：http://hz.gzhubu.top/gtuvpgictz.html

================================================================================
来源：http://hz.bjfxy.top/gtncfylwrp.html

[L01] 发送 GET 请求
来源：http://hz.ydjk.org.cn/gtptqezywy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cheryme.top/gtmekhqswx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.shanyushiyangkeji.top/gtbzuvgtcp.html

JS:   await fetch(url)
来源：http://hz.aizwys.cn/gtqcvuckqq.html

TS:   await fetch(url)
来源：http://hz.yueranfly.top/gtogoikeei.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.svipenyu.cn/gtdiodkhgj.html

Go:   resp, err := http.Get(url)
来源：http://hz.ehwqpu.com/gtoizzorgq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.9152youxi.cn/gtjbsxnpwn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.pengpengdd.cyou/gtkcurkkvf.html

[L02] 发送 POST JSON
来源：http://hz.yongpay.top/gtpjyuirdc.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.fzhhl.top/gtslqtrien.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.wangdashe.top/gtmlqgiqcz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yj20258.top/gtfdbddxsi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yueranfly.top/gtwdxukkpd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.shuidangran.top/gtxethxiuk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ehwqpu.com/gtlrochyar.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.sxryk.cn/gtjappbwsl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zhiwuduotai.top/gtypvazwir.html

[L03] 设置自定义请求头
来源：http://hz.xingfuxueyuan.xyz/gttodartnm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.andypj.xyz/gtiqpoxucd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.shangyingyoupin.top/gtaendwspm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jyoumei.cn/gtltgslxdp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhijiandao.cn/gtyngorjos.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.fengsongda.top/gtiohfrmzv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.0kj1m.cn/gtpbrepwpl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.meibo888.top/gtvhtcyzit.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.dianchejie.cn/gthevfgmve.html

[L04] 设置超时
来源：http://hz.jinqigufen.top/gtklxsdjiz.html

Py:   requests.get(url, timeout=5)
来源：http://hz.wangdashe.top/gtrhqqsvle.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jiagoushi.top/gtmnfkkimj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yueranfly.top/gtrmwddjbo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj20258.top/gtquqrldsx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jianghu66.top/gtukeszyme.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jlsjyb.cn/gtkscncrow.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jlsjyb.cn/gtriiitfei.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.snrcjt.cn/gtagdfktgv.html

[L05] 上传文件（multipart）
来源：http://hz.316326.xyz/gtuqkrluvy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.0kj1m.cn/gttefilyux.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.aibaodan.cn/gtdbgctjhq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.shangyingyoupin.top/gtsptmxpak.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yj202588.top/gtiyjqpcrm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yj20258.top/gtjovdcrbh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.shzxlz.cn/gtiaqawrud.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.iojbl.cn/gtzptdwwye.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.tian-w.cn/gtxouffufj.html

[L06] 解析响应为 JSON
来源：http://hz.fengsongda.top/gtcnlhlbrx.html

Py:   resp.json()
来源：http://hz.zhixingplan.top/gtewkecpos.html

PHP:  json_decode($body, true);
来源：http://hz.nanxinkj.top/gtzmywkpjp.html

JS:   await resp.json()
来源：http://hz.snrcjt.cn/gtlckrxbam.html

TS:   await resp.json()
来源：http://hz.jinqigfzy.top/gtgtyqfsue.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.havefunace.top/gtoscemust.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jinqigfzy.top/gtyolgluuz.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yonumen.top/gtpitrejsv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.cheryme.top/gtkpkuhzhi.html

[L07] 处理 HTTP 状态码
来源：http://hz.zdqjudy.top/gtkumqrtcp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.nanxuanxn.top/gtyriahewp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jianghu66.top/gtuzwaeguz.html

JS:   resp.ok;  resp.status
来源：http://hz.zhijiandao.cn/gtfyknehso.html

TS:   resp.ok;  resp.status
来源：http://hz.pengpengdd.cyou/gtledrwfpg.html

Java: resp.statusCode()
来源：http://hz.yonumen.top/gtwqddccmj.html

Go:   resp.StatusCode
来源：http://hz.jinqigfzy.top/gtuiydiara.html

Ruby: resp.code.to_i
来源：http://hz.chenlongwang.top/gtkbuyygit.html

C#:   (int)resp.StatusCode
来源：http://hz.hywenlv.cn/gtvlykuzje.html

[L08] 并发请求多个地址
来源：http://hz.sweek.top/gtnpwiavmx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jyoumei.cn/gtqwrnxezu.html

PHP:  curl_multi_init() 系列
来源：http://hz.hongshengwenyu.top/gtdhrjdeqj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xingfuxueyuan.xyz/gtixaqiwba.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.52xcode.cn/gtizfojchg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.svipenyu.cn/gtstxzjnzl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhaomingkeji.xyz/gtjkainvzo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhijiandao.cn/gtgmfqhrwf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.kuanghao11.cn/gtwlhozvdb.html

================================================================================
来源：http://hz.sysykeji.top/gtqqxomubd.html

M. 命令行 / 进程 / 环境
来源：http://hz.yuxming.cn/gtmqhpnefg.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtftmixiho.html

[M01] 读取命令行参数
来源：http://hz.daria6918.cn/gtqudrtcqf.html

Py:   sys.argv[1:]
来源：http://hz.xuanzx.com/gtgclyrthq.html

PHP:  $argv;  $argc;
来源：http://hz.cashguo.top/gtkildjzvk.html

JS:   process.argv.slice(2)
来源：http://hz.ydjk.org.cn/gtqkscelxk.html

TS:   process.argv.slice(2)
来源：http://hz.yangfankeji.com/gtlpycezaf.html

Java: args 数组（main 方法参数）
来源：http://hz.tanke756.top/gtlaisbjtp.html

Go:   os.Args[1:]
来源：http://hz.daria6918.cn/gtwisjvdca.html

Ruby: ARGV
来源：http://hz.ywan-chungtsiang.top/gttlietffw.html

C#:   args 数组（Main 方法参数）
来源：http://hz.316326.xyz/gtybivndnh.html

[M02] 读取环境变量
来源：http://hz.chenjidiqi.icu/gthwiexkld.html

Py:   os.environ.get("HOME")
来源：http://hz.jlsjyb.cn/gtpcueoesp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.pycfn.com/gtsepxwmyp.html

JS:   process.env.HOME
来源：http://hz.hnqzz.top/gtxzfblfcf.html

TS:   process.env.HOME
来源：http://hz.dashuyun.cn/gtkfgaotps.html

Java: System.getenv("HOME")
来源：http://hz.jqgfzy.top/gtesobwpzc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zdqjudy.top/gtclxtgass.html

Ruby: ENV["HOME"]
来源：http://hz.jinqigfzy.top/gtablewzpd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xylfe.cn/gtzgusmfim.html

[M03] 执行外部命令
来源：http://hz.jinyuanbaomall.cn/gtjlzkgamr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.cheryme.top/gtwonhyrdr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jiagoushi.top/gtiysnkfpi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.andypj.xyz/gtherfgcdt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jqgfzy.top/gtjunfrsar.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.daria6918.cn/gtieorfqsg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.316326.xyz/gtkvftihzp.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.fzhhl.top/gtcwufodha.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xinyue.icu/gtrzhebdvc.html

[M04] 获取当前工作目录
来源：http://hz.chenjidiqi.icu/gtxvjwmkqy.html

Py:   os.getcwd()
来源：http://hz.tanke756.top/gtsajhcnlw.html

PHP:  getcwd();
来源：http://hz.aibaodan.cn/gtmtpkgpax.html

JS:   process.cwd()
来源：http://hz.hysaishi.cn/gtoiuojalu.html

TS:   process.cwd()
来源：http://hz.hnqzz.top/gtqslmpwgu.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.nwbrower.top/gtrijpnjon.html

Go:   os.Getwd()
来源：http://hz.jinyuanbaomall.cn/gtobgexbaf.html

Ruby: Dir.pwd
来源：http://hz.ydjk.org.cn/gtqygvhutm.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.havefunace.top/gtkyhdargo.html

[M05] 设置退出码
来源：http://hz.316326.xyz/gtcxnokerq.html

Py:   sys.exit(1)
来源：http://hz.jinqigufen.top/gtzbmawotw.html

PHP:  exit(1);
来源：http://hz.yuanzhike.top/gtjqinityp.html

JS:   process.exit(1)
来源：http://hz.hfpthk.cn/gtetndtbam.html

TS:   process.exit(1)
来源：http://hz.chenlongwang.top/gtquaumlxk.html

Java: System.exit(1)
来源：http://hz.chenlongwang.top/gtkrkvfjdy.html

Go:   os.Exit(1)
来源：http://hz.yuxming.cn/gtrrbpnapt.html

Ruby: exit 1
来源：http://hz.chenzaomai.com/gtnycynvxj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.tianlin.xyz/gtaugvlarj.html

[M06] 向标准错误输出
来源：http://hz.zdqjudy.top/gtmxqljxud.html

Py:   print("err", file=sys.stderr)
来源：http://hz.pengpengdd.cyou/gtxvikdupw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yangfankeji.com/gthrhnlsxm.html

JS:   console.error("err")
来源：http://hz.gogol.net.cn/gthxuzjgfy.html

TS:   console.error("err")
来源：http://hz.gzhubu.top/gtocokqoyn.html

Java: System.err.println("err")
来源：http://hz.c1oappe.top/gtrmhxavki.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.svipenyu.cn/gtzbigtjla.html

Ruby: warn "err"
来源：http://hz.ywan-chungtsiang.top/gtmwynblnj.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.cashguo.top/gtihvifpok.html

[M07] 判断是否为主入口
来源：http://hz.iojbl.cn/gtnxqwgiim.html

Py:   if __name__ == "__main__":
来源：http://hz.jqgufenzy.top/gtqlpafehx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.daria6918.cn/gtundsnpzd.html

JS:   require.main === module
来源：http://hz.xingfuxueyuan.xyz/gtpyijgneb.html

TS:   require.main === module
来源：http://hz.hnxiangtu.top/gtnejclbvk.html

Java: public static void main(String[] args)
来源：http://hz.zhijiandao.cn/gtbwraefhm.html

Go:   func main()
来源：http://hz.316326.xyz/gtoefurqtf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.0kj1m.cn/gtrdkfcicj.html

C#:   static void Main(string[] args)
来源：http://hz.yuanzhike.top/gtoqxykrgf.html

[M08] 获取系统与运行时信息
来源：http://hz.sufxvd.cn/gtitmosjqb.html

Py:   platform.system();  platform.python_version()
来源：http://hz.c1oappe.top/gtuosjbtuz.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ywan-chungtsiang.top/gtxcuqtlpb.html

JS:   process.platform;  process.version
来源：http://hz.cucudq.cn/gtqjbnueih.html

TS:   process.platform;  process.version
来源：http://hz.52xcode.cn/gtyoyoylno.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhixingplan.top/gtmdybbevi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.vqdsnc.cn/gtxnswtpqk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.xingfuxueyuan.xyz/gtozeysylg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.pengpengdd.cyou/gtztyisanu.html

================================================================================
来源：http://hz.gotoacloud.top/gtvarfbjto.html

N. 数据结构与算法
来源：http://hz.hywenlv.cn/gtcruanpln.html

================================================================================
来源：http://hz.vqdsnc.cn/gtlgyepzlw.html

[N01] 二分查找（有序数组）
来源：http://hz.ydzc1.top/gthkoyboxk.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.aizwys.cn/gtvuosiyks.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ywan-chungtsiang.top/gttitwcour.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.haohaochexian.top/gtbweskofx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hfpthk.cn/gtegwodufl.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.316326.xyz/gtsedsgqan.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ybcxt.top/gtkrhtarzn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.shangyingyoupin.top/gtxiotfula.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.meibo888.top/gtwjcltlgj.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jqgfzy.top/gtuitqumxu.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shangyingyoupin.top/gtdiramsab.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.dashuyun.cn/gtpkevktaw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.smart0.xyz/gtfrwjekkp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hfpthk.cn/gtznwxmjeo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yuxming.cn/gtwgjmuumc.html

Go:   slices.Sort(arr)
来源：http://hz.dashuyun.cn/gtwmlyryfp.html

Ruby: arr.sort
来源：http://hz.snrcjt.cn/gttigsamgu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ydjk.org.cn/gtjgyfzqak.html

[N03] 快速排序（分治示例）
来源：http://hz.vqdsnc.cn/gtarmglgfd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yueranfly.top/gtehsctmnp.html

PHP:  // 递归实现，或用 usort
来源：http://hz.gotoacloud.top/gtsmejmyih.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ybcxt.top/gtyddjgroq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gogol.net.cn/gtrbhkfhea.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinqigfzy.top/gtexlrando.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.quarkkingdee.top/gtuwbrwvat.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jqgfzy.top/gtgechskws.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.shanyushiyangtech.top/gtgacxwlyv.html

[N04] 斐波那契数列
来源：http://hz.fzhhl.top/gtxmsftwkg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.9152youxi.cn/gtuqihochp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.tian-w.cn/gtatvrlvmd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nanxuanxn.top/gtinajfiab.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj20258888.top/gtapfsvrqz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.xuetiantiany.cn/gtaxxcbaur.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhijiandao.cn/gtqlqqejdy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hnxiangtu.top/gtqffzrart.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.gaohongyu789.top/gtwfmpvbgb.html

[N05] 最大公约数
来源：http://hz.hywenlv.cn/gtxmknwowm.html

Py:   math.gcd(a, b)
来源：http://hz.cqqwz.cn/gthlmzsqux.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zhijiandao.cn/gtoarmeosa.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hammf.cn/gtdjntiskx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.redwolf501.top/gtdaxwcibz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.feifeiyinyue.top/gtsfttbsnb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hywenlv.cn/gtmyeormwh.html

Ruby: a.gcd(b)
来源：http://hz.hnqzz.top/gtzhxlsuqj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.smart0.xyz/gtppcaoyok.html

[N06] 判断回文字符串
来源：http://hz.xinyue.icu/gtnaeiynsg.html

Py:   s == s[::-1]
来源：http://hz.jinghuilouyu.cn/gtzyeburzh.html

PHP:  $s === strrev($s);
来源：http://hz.smart0.xyz/gtygrlnfdv.html


<!-- 参考信息 -->