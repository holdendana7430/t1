代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.shanyushiyangkeji.top/gtxvgkklan.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yj202588.top/gtqunxeujv.html

[J09] 时区处理
来源：http://hz.sxryk.cn/gtrizvyjzf.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xziqi.cn/gtlfjjqwws.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.xingfuxueyuan.xyz/gtngohbuzm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj20258888.top/gtzrumgdcr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.bjfxy.top/gthaxhliew.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ehwqpu.com/gtrthfsftk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.nwbrower.top/gtuuidnprj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yangfankeji.com/gtixpwqign.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.sysykeji.top/gtztpmrjje.html

[J10] 取今天 / 本月第一天
来源：http://hz.xuanzx.com/gtgiocrkmv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hywenlv.cn/gtetdhlvib.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.shangyingyoupin.top/gtsostpcqt.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.iojbl.cn/gtjaqvyzzr.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.fzhhl.top/gttnqiyksp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.sysykeji.top/gtrrlqccpq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.pycfn.com/gtehkifqca.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yuanzhike.top/gtgiaywivp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yuanzhike.top/gtsqjfhfys.html

================================================================================
来源：http://hz.snrcjt.cn/gtpggbpmde.html

K. JSON 与序列化
来源：http://hz.yueranfly.top/gtarcjnuol.html

================================================================================
来源：http://hz.hywenlv.cn/gtfrotoqpz.html

[K01] 对象转 JSON 字符串
来源：http://hz.quarkkingdee.top/gtojxbpjem.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.guannengcc.top/gtgjyjwfuy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jinyuanbaomall.cn/gtuezxshmn.html

JS:   JSON.stringify(obj)
来源：http://hz.jinqigfzy.top/gtjzcnzibo.html

TS:   JSON.stringify(obj)
来源：http://hz.xylfe.cn/gtvmbnczys.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.iojbl.cn/gtwgyveocn.html

Go:   json.Marshal(obj)
来源：http://hz.cheryme.top/gtuawanuqa.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.aibaodan.cn/gtgkkdbiyl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.52xcode.cn/gtmmznujzd.html

[K02] JSON 字符串转对象
来源：http://hz.tian-w.cn/gttootifxh.html

Py:   json.loads(s)
来源：http://hz.ydjk.org.cn/gtcmfpigxz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.shuidangran.top/gtqqrnejss.html

JS:   JSON.parse(s)
来源：http://hz.jlsjyb.cn/gtiuyjayol.html

TS:   JSON.parse(s)
来源：http://hz.xuetiantiany.cn/gtxarieumk.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.ehwqpu.com/gtpeifpjyz.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.sweek.top/gtssiotozz.html

Ruby: JSON.parse(s)
来源：http://hz.sxryk.cn/gtjwaxofuv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jiagoushi.top/gtmznoomti.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.chenlongwang.top/gtyvyntebt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.feifeiyinyue.top/gtfrifgqlr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yj20258888.top/gthujgchxw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yueranfly.top/gtuxtsfotc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zdqjudy.top/gtqcrlwpvg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.xingfuxueyuan.xyz/gtuqmrnadb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ivvv.top/gtojilifpu.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.havefunace.top/gtixaxmcki.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jinyuanbaomall.cn/gtgymbefvq.html

[K04] 读取 JSON 文件
来源：http://hz.kuanghao11.cn/gtsrqfanif.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.nwbrower.top/gthasszxqf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jinqigfzy.top/gtsxpmtcan.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gaohongyu789.top/gtxudxtcws.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.nanxinkj.top/gtqfeysgqi.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.shangyingyoupin.top/gtvnfezumx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hywenlv.cn/gtrfhphlsj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yanxiufei.cn/gtprlxwiyy.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jinqigfzy.top/gtckygvtgs.html

[K05] 深拷贝对象
来源：http://hz.xuanzx.com/gtxgdhdqso.html

Py:   copy.deepcopy(obj)
来源：http://hz.andypj.xyz/gtlilhjdfh.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jinghuilouyu.cn/gtvpztznea.html

JS:   structuredClone(obj)
来源：http://hz.sufxvd.cn/gtduzfmlsw.html

TS:   structuredClone(obj)
来源：http://hz.jyoumei.cn/gtixflprcr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.sufxvd.cn/gtifsprsgr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.mhx1999.top/gtqxsmeicw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jinyuanbaomall.cn/gtliliogzc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.xylfe.cn/gtygxedgqp.html

[K06] 解析 URL 查询串
来源：http://hz.yangfankeji.com/gtjlvrkjpv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ivvv.top/gtqautrhxh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.shanyushiyangkeji.top/gtfasepvwt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shanyushiyangtech.top/gthadshfaz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.pengpengdd.cyou/gtgftwyvwj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.iojbl.cn/gtjsuacofe.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.snrcjt.cn/gtqwqkqdxv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.nwbrower.top/gtqjveyvbs.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.sufxvd.cn/gteanpfzce.html

[K07] 进制转换
来源：http://hz.xuanzx.com/gtizkpbckd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ppjwa.cn/gtcnghmbzc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yuxming.cn/gtwklemifc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shzxlz.cn/gtxtecflhv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.fzhhl.top/gteukmyyhz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.wangshuangyany.cn/gtdjefhzwr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yueranfly.top/gtwqjcfpmr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xinyue.icu/gtzjsnuhgj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.gotoacloud.top/gtkgorugpk.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yuanzhike.top/gtfunudgdm.html

Py:   pickle.dumps(obj)
来源：http://hz.52xcode.cn/gtyxovhtxz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jlsjyb.cn/gtantmeoif.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.gogol.net.cn/gtkssjaxbm.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.gaohongyu789.top/gtxcosqlby.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yueranfly.top/gteddnzozx.html

Go:   encoding/gob
来源：http://hz.tanke756.top/gtqlyzyxdi.html

Ruby: Marshal.dump(obj)
来源：http://hz.guannengcc.top/gtmiuzkabi.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.mhx1999.top/gttkpsicpy.html

================================================================================
来源：http://hz.yvedp.cn/gtrwqzrpvf.html

L. 网络请求
来源：http://hz.jiagoushi.top/gtemmwsebx.html

================================================================================
来源：http://hz.xylfe.cn/gtwaexxani.html

[L01] 发送 GET 请求
来源：http://hz.hnqzz.top/gtegiwoazp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.quarkkingdee.top/gttjvtkkgy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.xuanzx.com/gtgfentfpe.html

JS:   await fetch(url)
来源：http://hz.xylfe.cn/gthbwxqjyn.html

TS:   await fetch(url)
来源：http://hz.wangdashe.top/gtuqlxkhuz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yonumen.top/gtjokqyhwu.html

Go:   resp, err := http.Get(url)
来源：http://hz.snrcjt.cn/gtnynfimwr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cdnleiting.top/gtoockqemn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.cheryme.top/gtqftaqmhi.html

[L02] 发送 POST JSON
来源：http://hz.ehwqpu.com/gtnvqrznwb.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.sweek.top/gteonxavfy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.c1oappe.top/gtadajmoek.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cdnleiting.top/gtrstygubw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.fzhhl.top/gtjcxkmnnp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.dashuyun.cn/gtuthrsaly.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.dashuyun.cn/gtjeiarzln.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.gotoacloud.top/gtviqtszmq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ydjk.org.cn/gtfboqlghf.html

[L03] 设置自定义请求头
来源：http://hz.gogol.net.cn/gtqkgcmtiy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hysaishi.cn/gtjsajghlb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.cqqwz.cn/gtgcsqnzas.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cheryme.top/gtadkipzos.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ehwqpu.com/gtxziqrxfr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jianghu66.top/gteanwvybi.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.sysykeji.top/gtavfhnsre.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jinghuilouyu.cn/gtmkmwuixf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jqgufenzy.top/gtyeviqroi.html

[L04] 设置超时
来源：http://hz.jqgfzy.top/gtsjnnealr.html

Py:   requests.get(url, timeout=5)
来源：http://hz.tian-w.cn/gtnbzcumzw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ppjwa.cn/gtbsdloovm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jqgfzy.top/gtfapzmsmd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhijiandao.cn/gtpcyjmepk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jqgufenzy.top/gtjvkhdljb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.316326.xyz/gtlaudxldx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.shuidangran.top/gtsanfudlq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hongshengwenyu.top/gtwxjhrtlj.html

[L05] 上传文件（multipart）
来源：http://hz.gotoacloud.top/gtglidnqje.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.gotoacloud.top/gtdqodlsdh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.redwolf501.top/gthnnqosbt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.gaohongyu789.top/gteszzplfh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.guannengcc.top/gtbjfedboc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.svipenyu.cn/gtsgyltzrb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.hywenlv.cn/gtxmcagdyh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yuanzhike.top/gtdrxawkok.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.xinyue.icu/gtxovzspsb.html

[L06] 解析响应为 JSON
来源：http://hz.nanxuanxn.top/gtauvlqehi.html

Py:   resp.json()
来源：http://hz.zhoulong.xyz/gtstnnbtvu.html

PHP:  json_decode($body, true);
来源：http://hz.gzhubu.top/gtzojnvyao.html

JS:   await resp.json()
来源：http://hz.xuetiantiany.cn/gtfmnksfqi.html

TS:   await resp.json()
来源：http://hz.cheryme.top/gtdvvgekls.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.quarkkingdee.top/gtsnborzsa.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.fengsongda.top/gtpycdjnuq.html

Ruby: JSON.parse(resp.body)
来源：http://hz.c1oappe.top/gtjpinhtht.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.fzhhl.top/gtylxyyfif.html

[L07] 处理 HTTP 状态码
来源：http://hz.yonumen.top/gtryzafglp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.sufxvd.cn/gtpakjyomd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hnxiangtu.top/gtrdmkdbdp.html

JS:   resp.ok;  resp.status
来源：http://hz.wangshuangyany.cn/gtxkoplxvh.html

TS:   resp.ok;  resp.status
来源：http://hz.yuxming.cn/gtibrylqaz.html

Java: resp.statusCode()
来源：http://hz.xziqi.cn/gttuovogic.html

Go:   resp.StatusCode
来源：http://hz.zhiwuduotai.top/gtkiwynhnu.html

Ruby: resp.code.to_i
来源：http://hz.aibaodan.cn/gtdzaldnbf.html

C#:   (int)resp.StatusCode
来源：http://hz.smart0.xyz/gtqluodunb.html

[L08] 并发请求多个地址
来源：http://hz.feifeiyinyue.top/gtspeqncqi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.pycfn.com/gtucfmtumv.html

PHP:  curl_multi_init() 系列
来源：http://hz.hywenlv.cn/gtbcsqfoie.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tian-w.cn/gtfmjoadgd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenlongwang.top/gtdyeoyfjl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.vqdsnc.cn/gtemfeqkjf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.chenzaomai.com/gtdmuipkbs.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.sweek.top/gtwtxxjxtw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhixingplan.top/gtlsnnybmr.html

================================================================================
来源：http://hz.zhoulong.xyz/gtnataiqpn.html

M. 命令行 / 进程 / 环境
来源：http://hz.cucudq.cn/gtrtzjdhrf.html

================================================================================
来源：http://hz.havefunace.top/gtxfweynqi.html

[M01] 读取命令行参数
来源：http://hz.sxryk.cn/gtxpstmukg.html

Py:   sys.argv[1:]
来源：http://hz.snrcjt.cn/gtvnkhjopb.html

PHP:  $argv;  $argc;
来源：http://hz.dashuyun.cn/gthyktpztl.html

JS:   process.argv.slice(2)
来源：http://hz.quarkkingdee.top/gtioqmoall.html

TS:   process.argv.slice(2)
来源：http://hz.yangfankeji.com/gtwcqypsap.html

Java: args 数组（main 方法参数）
来源：http://hz.cdnleiting.top/gtbjcwvujs.html

Go:   os.Args[1:]
来源：http://hz.52xcode.cn/gtxhcntvfn.html

Ruby: ARGV
来源：http://hz.hongshengwenyu.top/gtxfqecthy.html

C#:   args 数组（Main 方法参数）
来源：http://hz.dianchejie.cn/gtgnrwwhee.html

[M02] 读取环境变量
来源：http://hz.cheryme.top/gtuyuaspqx.html

Py:   os.environ.get("HOME")
来源：http://hz.gogol.net.cn/gtietstuzf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yueranfly.top/gtsjdikbgs.html

JS:   process.env.HOME
来源：http://hz.shzxlz.cn/gtqcojzxls.html

TS:   process.env.HOME
来源：http://hz.yanxiufei.cn/gthkqoobah.html

Java: System.getenv("HOME")
来源：http://hz.shzxlz.cn/gtmxbuynvi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.mhx1999.top/gtkpjopzla.html

Ruby: ENV["HOME"]
来源：http://hz.zycfv.cn/gtgcgruluj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shzxlz.cn/gtqhdwofrp.html

[M03] 执行外部命令
来源：http://hz.316326.xyz/gtkhzsixkl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.shanyushiyangtech.top/gtyhmtvzfz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hammf.cn/gtocwewxhh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.shanyushiyangtech.top/gtmkrmjvxo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shanyushiyangtech.top/gtjrjmdkqg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hnxiangtu.top/gtmiozkvti.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.tianlin.xyz/gtzdlwqfid.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.kuanghao11.cn/gtrqetxafg.html

C#:   Process.Start("ls", "-l");
来源：http://hz.sysykeji.top/gtdeqlyfuv.html

[M04] 获取当前工作目录
来源：http://hz.xylfe.cn/gtrmypxxhg.html

Py:   os.getcwd()
来源：http://hz.yj20258.top/gtpefgepbg.html

PHP:  getcwd();
来源：http://hz.aizwys.cn/gtiuzecbev.html

JS:   process.cwd()
来源：http://hz.daxiang520.top/gtmxnmgohh.html

TS:   process.cwd()
来源：http://hz.ydzc1.top/gtbkezsebr.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhijiandao.cn/gtajuzzzoe.html

Go:   os.Getwd()
来源：http://hz.zhiwuduotai.top/gtzcayywsr.html

Ruby: Dir.pwd
来源：http://hz.ydjk.org.cn/gtfxhvhcsj.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.gotoacloud.top/gtajqevial.html

[M05] 设置退出码
来源：http://hz.hammf.cn/gtpppngqqs.html

Py:   sys.exit(1)
来源：http://hz.gotoacloud.top/gtipzxdqdn.html

PHP:  exit(1);
来源：http://hz.fzhhl.top/gtbuehppas.html

JS:   process.exit(1)
来源：http://hz.xuetiantiany.cn/gtvdlewsrx.html

TS:   process.exit(1)
来源：http://hz.shangyingyoupin.top/gthsffxyze.html

Java: System.exit(1)
来源：http://hz.ppjwa.cn/gtvuzpefmk.html

Go:   os.Exit(1)
来源：http://hz.hammf.cn/gtnlqlhfws.html

Ruby: exit 1
来源：http://hz.kuanghao11.cn/gtkkzdgrlo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.0kj1m.cn/gtxzcmqnhk.html

[M06] 向标准错误输出
来源：http://hz.jqgufenzy.top/gtlxgsnjzh.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xylfe.cn/gtdfrriaif.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.gogol.net.cn/gtwyddulbp.html

JS:   console.error("err")
来源：http://hz.havefunace.top/gtvfngenvq.html

TS:   console.error("err")
来源：http://hz.meibo888.top/gtvwmcqgri.html

Java: System.err.println("err")
来源：http://hz.xylfe.cn/gtjoloimin.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xuetiantiany.cn/gtbrtdbevb.html

Ruby: warn "err"
来源：http://hz.zhaomingkeji.xyz/gtptqidmkw.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ydzc1.top/gtrjsxapcf.html

[M07] 判断是否为主入口
来源：http://hz.jqgufenzy.top/gtlpizzacb.html

Py:   if __name__ == "__main__":
来源：http://hz.yonumen.top/gtqwguelsb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ywan-chungtsiang.top/gtibzskiqv.html

JS:   require.main === module
来源：http://hz.wangshuangyany.cn/gtpftdxbdo.html

TS:   require.main === module
来源：http://hz.shuidangran.top/gtzepiisdi.html

Java: public static void main(String[] args)
来源：http://hz.fzhhl.top/gtgvokvfro.html

Go:   func main()
来源：http://hz.jinqigufen.top/gtitllqxks.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jinghuilouyu.cn/gtiepvjmgo.html

C#:   static void Main(string[] args)
来源：http://hz.sufxvd.cn/gtvlgjqtsd.html

[M08] 获取系统与运行时信息
来源：http://hz.hywenlv.cn/gtxdawstoq.html

Py:   platform.system();  platform.python_version()
来源：http://hz.xuetiantiany.cn/gtrmrzxyhn.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhijiandao.cn/gtfkxuzxgj.html

JS:   process.platform;  process.version
来源：http://hz.zhoulong.xyz/gtsxobqzxe.html

TS:   process.platform;  process.version
来源：http://hz.hfpthk.cn/gtijehtstv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hfpthk.cn/gtmlvxxclh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yonumen.top/gtyswvcrrk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cashguo.top/gtasjdwbjj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.sweek.top/gtnzyjvhqn.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtxdnzlxmv.html

N. 数据结构与算法
来源：http://hz.jqgfzy.top/gtzwtlvuey.html

================================================================================
来源：http://hz.dianchejie.cn/gtnxiungbz.html

[N01] 二分查找（有序数组）
来源：http://hz.jqgufenzy.top/gtslfryqml.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.shanyushiyangtech.top/gtqsagmbhn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.haohaochexian.top/gtsvmtyrmf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zdqjudy.top/gtidnkmnpd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.feifeiyinyue.top/gtagoryolq.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hongshengwenyu.top/gtkplsganu.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jyoumei.cn/gtpfsiunij.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yuanzhike.top/gtugsltilt.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zhiwuduotai.top/gtvtlfjsvk.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.tian-w.cn/gtpjoftxvm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.daria6918.cn/gtvaqcstzg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.svipenyu.cn/gtiinlwsza.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinyuanbaomall.cn/gtgmtjorfa.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.redwolf501.top/gtsizktdxk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ivvv.top/gtneyzgdwm.html

Go:   slices.Sort(arr)
来源：http://hz.cdnleiting.top/gtbszljxze.html

Ruby: arr.sort
来源：http://hz.cqqwz.cn/gtvstmqjgr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.snrcjt.cn/gtcnkezbdc.html

[N03] 快速排序（分治示例）
来源：http://hz.pycfn.com/gtgvnbhpmh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.sufxvd.cn/gtrypjjehy.html

PHP:  // 递归实现，或用 usort
来源：http://hz.sweek.top/gthlwqmgre.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cdnleiting.top/gtwuuhlhdw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hywenlv.cn/gtjkhthhob.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.iojbl.cn/gtxxyjbgvi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhixingplan.top/gtpnlhfojq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.tanke756.top/gtupaqrcwg.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.gotoacloud.top/gtlmevispg.html

[N04] 斐波那契数列
来源：http://hz.aizwys.cn/gttlnaaetr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xuetiantiany.cn/gtaxrkcndq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.aibaodan.cn/gtrljlesey.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.0kj1m.cn/gttpfzobsc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.redwolf501.top/gtovpfschf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.hnqzz.top/gtdumegyjf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hywenlv.cn/gtywwcsdzi.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.wangdashe.top/gtgyvbwdvf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yonumen.top/gtyygjhwog.html

[N05] 最大公约数
来源：http://hz.nanxuanxn.top/gtgkeonmue.html

Py:   math.gcd(a, b)
来源：http://hz.sweek.top/gtccvkhpep.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hammf.cn/gtuiimohef.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shanyushiyangkeji.top/gtfclbrwox.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ivvv.top/gtdzupdqhp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yuanzhike.top/gtumckrioa.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.xylfe.cn/gtvbholuqr.html

Ruby: a.gcd(b)
来源：http://hz.nwbrower.top/gtsvdutqrr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yonumen.top/gtiulkluld.html

[N06] 判断回文字符串
来源：http://hz.pycfn.com/gtxvjqgfvw.html

Py:   s == s[::-1]
来源：http://hz.snrcjt.cn/gtuuvpeloz.html

PHP:  $s === strrev($s);
来源：http://hz.zhongyouzk.top/gtjmngxepl.html

JS:   s === [...s].reverse().join("")
来源：http://hz.gotoacloud.top/gtzhmsefrm.html

TS:   s === [...s].reverse().join("")
来源：http://hz.gogol.net.cn/gtjgpkobmx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.nanxuanxn.top/gthowdtjie.html

Go:   // 双指针从两端比较
来源：http://hz.yj20258888.top/gtntwfybvc.html


<!-- 参考信息 -->