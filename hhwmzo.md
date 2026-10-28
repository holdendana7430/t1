代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.aibaodan.cn/gtudifegvh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sweek.top/gtiieryovl.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhaomingkeji.xyz/gtgwlueboz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hnqzz.top/gtrgpshvim.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.svipenyu.cn/gtjtgdfgos.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhongyouzk.top/gtemjmfzga.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.tian-w.cn/gtqvxkoqyi.html

[J10] 取今天 / 本月第一天
来源：http://hz.yj202588.top/gtiyygvryj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ybcxt.top/gtzkvvpcmx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.quarkkingdee.top/gtgvxthrbn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.cucudq.cn/gttqbrwzmo.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ivvv.top/gtqbyvfuxg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.hongshengwenyu.top/gtulhzgill.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.guowangkeji.top/gtiayienav.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zdqjudy.top/gtgyjporsl.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ywan-chungtsiang.top/gtejlxrgan.html

================================================================================
来源：http://hz.mhx1999.top/gtsmnwofbi.html

K. JSON 与序列化
来源：http://hz.ydjk.org.cn/gtawfysekg.html

================================================================================
来源：http://hz.wangdashe.top/gtsbnkzlwb.html

[K01] 对象转 JSON 字符串
来源：http://hz.bjfxy.top/gticyytzoq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.daria6918.cn/gtzqsypojx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.cdnleiting.top/gtgidsjrpp.html

JS:   JSON.stringify(obj)
来源：http://hz.52xcode.cn/gtactwzouo.html

TS:   JSON.stringify(obj)
来源：http://hz.aibaodan.cn/gtfunvqxcg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.daxiang520.top/gtehxjlbpl.html

Go:   json.Marshal(obj)
来源：http://hz.jiagoushi.top/gtpkpixbnn.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.feifeiyinyue.top/gtovvnmysi.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.bjfxy.top/gtbmvchpyr.html

[K02] JSON 字符串转对象
来源：http://hz.jiagoushi.top/gtoeczxnmh.html

Py:   json.loads(s)
来源：http://hz.cheryme.top/gtwyapklpb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jyoumei.cn/gtoydwlgui.html

JS:   JSON.parse(s)
来源：http://hz.hammf.cn/gtclyrqpkd.html

TS:   JSON.parse(s)
来源：http://hz.dianchejie.cn/gtfdygmkid.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.meibo888.top/gthewfcehk.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.chenlongwang.top/gtihafxlpp.html

Ruby: JSON.parse(s)
来源：http://hz.hfpthk.cn/gtduihfypj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.aizwys.cn/gtxgdvgmtz.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.havefunace.top/gtmsaficbq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.0kj1m.cn/gtnxemimdq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.cheryme.top/gtpvspputf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.bjfxy.top/gtmchnakpc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jlsjyb.cn/gtoqbiumal.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.tanke756.top/gtarwpvswx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhiwuduotai.top/gtilmnqyax.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hnxiangtu.top/gttxpbdmiz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.chenlongwang.top/gtgdrfaitd.html

[K04] 读取 JSON 文件
来源：http://hz.yonumen.top/gtvbttkwny.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.vqdsnc.cn/gtvafdxhvt.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.gzhubu.top/gtdugcqrih.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.fengsongda.top/gtxbfdokti.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ehwqpu.com/gtioghmaof.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jqgufenzy.top/gtknhdngle.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jinyuanbaomall.cn/gthaovfdam.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.shzxlz.cn/gtghwedxgt.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jinqigufen.top/gtifdgqpoy.html

[K05] 深拷贝对象
来源：http://hz.daria6918.cn/gtkylczmsi.html

Py:   copy.deepcopy(obj)
来源：http://hz.dianchejie.cn/gtcfxlofdm.html

PHP:  unserialize(serialize($obj));
来源：http://hz.tianlin.xyz/gtpyiayrtt.html

JS:   structuredClone(obj)
来源：http://hz.wangshuangyany.cn/gtwgxxfcdi.html

TS:   structuredClone(obj)
来源：http://hz.ivvv.top/gteinohmva.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.haohaochexian.top/gtdqjdtyjr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jinqigufen.top/gtezqdqqlp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.nanxuanxn.top/gtxjjjyecd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.redwolf501.top/gtitrznhxx.html

[K06] 解析 URL 查询串
来源：http://hz.redwolf501.top/gtcqmjyzhp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jinqigfzy.top/gtrimhsbwt.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hysaishi.cn/gtuhpjstlk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cqqwz.cn/gtldiursog.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gotoacloud.top/gtkdcowgny.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jlsjyb.cn/gtjzegzjvv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.haohaochexian.top/gteiqkhhly.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hfpthk.cn/gtvfhroxnu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.hywenlv.cn/gtjykldiup.html

[K07] 进制转换
来源：http://hz.sxryk.cn/gtegirruhb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.sysykeji.top/gtufefdhxm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.feifeiyinyue.top/gtadvuadsk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.dashuyun.cn/gtizbtqxkw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.mhx1999.top/gtrxmtpxub.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhijiandao.cn/gtdvpzdtma.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xziqi.cn/gtsqqwycck.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.sufxvd.cn/gtzzpbeexa.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.gaohongyu789.top/gtffbkhrtw.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.chenjidiqi.icu/gtzpqedwbm.html

Py:   pickle.dumps(obj)
来源：http://hz.shzxlz.cn/gtnwesgkdk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zhengqikj.top/gtlpibeufg.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.9152youxi.cn/gtepabhuqv.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.birdmap.top/gtdspvgrla.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jinqigfzy.top/gtrokjktlz.html

Go:   encoding/gob
来源：http://hz.feifeiyinyue.top/gtfkjxpnxd.html

Ruby: Marshal.dump(obj)
来源：http://hz.yuanzhike.top/gthxlashai.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ehwqpu.com/gtbksutspb.html

================================================================================
来源：http://hz.ydzc1.top/gtwxjwryor.html

L. 网络请求
来源：http://hz.ivvv.top/gtoqkcltlb.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtpmmhplpo.html

[L01] 发送 GET 请求
来源：http://hz.smart0.xyz/gtgmqdzwyf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.xinyue.icu/gtauiubwsb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.mhx1999.top/gtfarpppqs.html

JS:   await fetch(url)
来源：http://hz.xylfe.cn/gtzqyiwouf.html

TS:   await fetch(url)
来源：http://hz.ppjwa.cn/gtwuxwkvqq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.smart0.xyz/gtowfervih.html

Go:   resp, err := http.Get(url)
来源：http://hz.haohaochexian.top/gtnjdxbgyb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jqgfzy.top/gtatazipny.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.316326.xyz/gtsjdaoczf.html

[L02] 发送 POST JSON
来源：http://hz.9152youxi.cn/gtccyhfiec.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.shuidangran.top/gtkebxkdbe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yongpay.top/gtlarshwem.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tianlin.xyz/gtdprfszal.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhoulong.xyz/gtneabpfot.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.pycfn.com/gtotukslnk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hammf.cn/gtvgvvylhp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jiagoushi.top/gtspyzjwer.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jlsjyb.cn/gthquixcrf.html

[L03] 设置自定义请求头
来源：http://hz.ppjwa.cn/gtqqvfhmat.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.nanxinkj.top/gtecynvvel.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.aibaodan.cn/gtxownxuwo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.quarkkingdee.top/gtpmwoyjtj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gaohongyu789.top/gttvtcpntg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.shzxlz.cn/gtwynbxkwk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.xinyue.icu/gtfyhpwqov.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.daxiang520.top/gtyedticyd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.pycfn.com/gtfzulyxrb.html

[L04] 设置超时
来源：http://hz.shzxlz.cn/gtmziquqew.html

Py:   requests.get(url, timeout=5)
来源：http://hz.mhx1999.top/gtpolnamcy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.xingfuxueyuan.xyz/gtnoayyshh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.52xcode.cn/gtdtuhxket.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.dashuyun.cn/gtwmyupawt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhixingplan.top/gtxeffxkwx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.andypj.xyz/gtvdbqmoov.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.guannengcc.top/gtxmibjjwa.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.nanxuanxn.top/gtenscelqg.html

[L05] 上传文件（multipart）
来源：http://hz.fzhhl.top/gtqxlgmhho.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.tanke756.top/gtpampurkd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.sufxvd.cn/gtuwwswtpo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.sysykeji.top/gtuksujrhh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.iojbl.cn/gtkanmykgu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.iojbl.cn/gtpouwxool.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xuetiantiany.cn/gtaumvhrhp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.dashuyun.cn/gtlbimjsyl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yj20258.top/gttauiagkt.html

[L06] 解析响应为 JSON
来源：http://hz.xylfe.cn/gtbbngqhvg.html

Py:   resp.json()
来源：http://hz.gzhubu.top/gtvajnxmza.html

PHP:  json_decode($body, true);
来源：http://hz.daxiang520.top/gtvttrmyun.html

JS:   await resp.json()
来源：http://hz.gogol.net.cn/gtsxlzuhgh.html

TS:   await resp.json()
来源：http://hz.jqgufenzy.top/gtcyqzeace.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.daria6918.cn/gtqfcqtesi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.gogol.net.cn/gthvrogctw.html

Ruby: JSON.parse(resp.body)
来源：http://hz.wangdashe.top/gtofxaduyy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhixingplan.top/gtnplcydzb.html

[L07] 处理 HTTP 状态码
来源：http://hz.yonumen.top/gtjppgwyco.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xingfuxueyuan.xyz/gtdpraljfa.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.shuidangran.top/gtgkkehugo.html

JS:   resp.ok;  resp.status
来源：http://hz.jinghuilouyu.cn/gtgdhxxyov.html

TS:   resp.ok;  resp.status
来源：http://hz.hnqzz.top/gtbmupagol.html

Java: resp.statusCode()
来源：http://hz.pycfn.com/gthtzndbgp.html

Go:   resp.StatusCode
来源：http://hz.birdmap.top/gtpfowxirs.html

Ruby: resp.code.to_i
来源：http://hz.sysykeji.top/gtfzzwaxzq.html

C#:   (int)resp.StatusCode
来源：http://hz.shuidangran.top/gtsrvetwmy.html

[L08] 并发请求多个地址
来源：http://hz.hongshengwenyu.top/gtxaddtkdu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.c1oappe.top/gtfdjviqje.html

PHP:  curl_multi_init() 系列
来源：http://hz.yueranfly.top/gtzectacjp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.0kj1m.cn/gtvdubqkww.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinqigufen.top/gtnwvmfxup.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hammf.cn/gtlzwnnyul.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yueranfly.top/gteuwjguab.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ivvv.top/gtqzwfhfxg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhiwuduotai.top/gtfabnrkkj.html

================================================================================
来源：http://hz.gzhubu.top/gtzdjyyxoe.html

M. 命令行 / 进程 / 环境
来源：http://hz.cheryme.top/gtffokufhk.html

================================================================================
来源：http://hz.havefunace.top/gtydylmgzi.html

[M01] 读取命令行参数
来源：http://hz.tian-w.cn/gtvyngbziy.html

Py:   sys.argv[1:]
来源：http://hz.snrcjt.cn/gttjdncnca.html

PHP:  $argv;  $argc;
来源：http://hz.yongpay.top/gtcweiwnot.html

JS:   process.argv.slice(2)
来源：http://hz.xuanzx.com/gtprieoqci.html

TS:   process.argv.slice(2)
来源：http://hz.aizwys.cn/gtysuwsmea.html

Java: args 数组（main 方法参数）
来源：http://hz.snrcjt.cn/gtxdzlbohg.html

Go:   os.Args[1:]
来源：http://hz.fzhhl.top/gtjbuoouxs.html

Ruby: ARGV
来源：http://hz.aizwys.cn/gtaopiqlmn.html

C#:   args 数组（Main 方法参数）
来源：http://hz.tianlin.xyz/gtghskhjcp.html

[M02] 读取环境变量
来源：http://hz.sweek.top/gtbbfjfxrc.html

Py:   os.environ.get("HOME")
来源：http://hz.bjfxy.top/gtjizafgjv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.0kj1m.cn/gtgpvldyyv.html

JS:   process.env.HOME
来源：http://hz.hysaishi.cn/gtwmmsdedc.html

TS:   process.env.HOME
来源：http://hz.yj20258888.top/gtibqayryo.html

Java: System.getenv("HOME")
来源：http://hz.yongpay.top/gtrbkyvbhh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.iojbl.cn/gtldqkohyc.html

Ruby: ENV["HOME"]
来源：http://hz.dianchejie.cn/gtqdwvulbq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.wangshuangyany.cn/gtqjkrwuws.html

[M03] 执行外部命令
来源：http://hz.birdmap.top/gtiheiczka.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.52xcode.cn/gtnwfbmeug.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.nanxuanxn.top/gtttfnqqmh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.daria6918.cn/gtgwmmzlis.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shanyushiyangkeji.top/gtzfrwkskp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.andypj.xyz/gtciittbjj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jlsjyb.cn/gtcvvidwql.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.xinyue.icu/gtgwuljdcx.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xylfe.cn/gtccsvrzgn.html

[M04] 获取当前工作目录
来源：http://hz.snrcjt.cn/gtzdtzukrm.html

Py:   os.getcwd()
来源：http://hz.jqgufenzy.top/gtyztduotm.html

PHP:  getcwd();
来源：http://hz.xuanzx.com/gtmeikgknf.html

JS:   process.cwd()
来源：http://hz.tian-w.cn/gtnigjfpyt.html

TS:   process.cwd()
来源：http://hz.jinqigfzy.top/gtevgychdh.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xuetiantiany.cn/gtoddybfdi.html

Go:   os.Getwd()
来源：http://hz.yanxiufei.cn/gtvysiorbj.html

Ruby: Dir.pwd
来源：http://hz.vqdsnc.cn/gtckyrdecn.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhixingplan.top/gtdoxcpuaq.html

[M05] 设置退出码
来源：http://hz.dianchejie.cn/gtnwcbiawx.html

Py:   sys.exit(1)
来源：http://hz.guannengcc.top/gtgssqxcbb.html

PHP:  exit(1);
来源：http://hz.0kj1m.cn/gtlrjqtfft.html

JS:   process.exit(1)
来源：http://hz.bjfxy.top/gtfupbpcbj.html

TS:   process.exit(1)
来源：http://hz.vqdsnc.cn/gtmlxmytaw.html

Java: System.exit(1)
来源：http://hz.haohaochexian.top/gtmdgkoqma.html

Go:   os.Exit(1)
来源：http://hz.ehwqpu.com/gtivctdjgp.html

Ruby: exit 1
来源：http://hz.haohaochexian.top/gtkkpigips.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.gzhubu.top/gtijapefzj.html

[M06] 向标准错误输出
来源：http://hz.sxryk.cn/gtzdngimtq.html

Py:   print("err", file=sys.stderr)
来源：http://hz.tianlin.xyz/gtfukrjogy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yvedp.cn/gtrcrvcdnu.html

JS:   console.error("err")
来源：http://hz.jqgfzy.top/gtzxovriom.html

TS:   console.error("err")
来源：http://hz.sufxvd.cn/gtjogwkvzr.html

Java: System.err.println("err")
来源：http://hz.hnxiangtu.top/gtnbdafkjw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.nanxuanxn.top/gtamlhcyga.html

Ruby: warn "err"
来源：http://hz.yongpay.top/gtebshyoqh.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.snrcjt.cn/gtsbtpxbxj.html

[M07] 判断是否为主入口
来源：http://hz.daria6918.cn/gtoqfnzwbp.html

Py:   if __name__ == "__main__":
来源：http://hz.sufxvd.cn/gtvfrbetfz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.sweek.top/gtlqyduwew.html

JS:   require.main === module
来源：http://hz.snrcjt.cn/gtzbuqerbo.html

TS:   require.main === module
来源：http://hz.yj202588.top/gtbkatqduc.html

Java: public static void main(String[] args)
来源：http://hz.shanyushiyangtech.top/gtlktxylze.html

Go:   func main()
来源：http://hz.fengsongda.top/gtbiamgpfk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yvedp.cn/gtfpamhatu.html

C#:   static void Main(string[] args)
来源：http://hz.yanxiufei.cn/gteabcpluh.html

[M08] 获取系统与运行时信息
来源：http://hz.hywenlv.cn/gtmvdintmc.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zdqjudy.top/gttwtfllcd.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.cheryme.top/gttlooblfm.html

JS:   process.platform;  process.version
来源：http://hz.zycfv.cn/gtfrsktlgk.html

TS:   process.platform;  process.version
来源：http://hz.aibaodan.cn/gtbgaxjisp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.smart0.xyz/gtsixkmrqb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yuxming.cn/gtehaztzwt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yuxming.cn/gtwdpnjivr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hywenlv.cn/gtzjmawnht.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtltzuqmox.html

N. 数据结构与算法
来源：http://hz.cashguo.top/gtzmanfplu.html

================================================================================
来源：http://hz.bjfxy.top/gtvlallyky.html

[N01] 二分查找（有序数组）
来源：http://hz.sufxvd.cn/gtaltcdren.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ywan-chungtsiang.top/gtwxxdvcbf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yonumen.top/gtvxftluvn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yonumen.top/gtutmgowle.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yueranfly.top/gtezjikerj.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.shzxlz.cn/gtnjoskhui.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.vqdsnc.cn/gtrhwfdtwy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hnqzz.top/gtwbykgsuq.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jinqigfzy.top/gtayrrffwb.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.52xcode.cn/gtjpqxklgx.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.kuanghao11.cn/gtmovnlazs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zycfv.cn/gtdvhbhhgv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cheryme.top/gtkpvlkvbm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.bjfxy.top/gtqrzfytoq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.daria6918.cn/gttcyoenju.html

Go:   slices.Sort(arr)
来源：http://hz.jiagoushi.top/gtqalpajqu.html

Ruby: arr.sort
来源：http://hz.ppjwa.cn/gtbvhycikh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jyoumei.cn/gtrrvysavl.html

[N03] 快速排序（分治示例）
来源：http://hz.sweek.top/gtrbsyjcjq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.shanyushiyangtech.top/gtbgaxdolh.html

PHP:  // 递归实现，或用 usort
来源：http://hz.meibo888.top/gtqmveyizt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jianghu66.top/gtjdmoxokg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.bjfxy.top/gtcgzludmp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.wangshuangyany.cn/gtwvjponwn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zdqjudy.top/gtqktvryrb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.chenlongwang.top/gtfrnwyxdo.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.shanyushiyangkeji.top/gtthriokwa.html

[N04] 斐波那契数列
来源：http://hz.pengpengdd.cyou/gtafvnucnc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.c1oappe.top/gthleojits.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhongyouzk.top/gtaebsjtrk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sysykeji.top/gterxwnmul.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cucudq.cn/gtmjcwhzwd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.c1oappe.top/gtvcgyqfvq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yj20258.top/gtevjjlecl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.pycfn.com/gtcaijzveq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yuxming.cn/gtildkzkkb.html

[N05] 最大公约数
来源：http://hz.316326.xyz/gtdpxmwezt.html

Py:   math.gcd(a, b)
来源：http://hz.52xcode.cn/gtpmnmfiik.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jinghuilouyu.cn/gtsnbtythq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jyoumei.cn/gtznyegzhc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hywenlv.cn/gtyindnecf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yuanzhike.top/gtqkhkbpmp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.fzhhl.top/gthevtkmfi.html

Ruby: a.gcd(b)
来源：http://hz.yongpay.top/gtkwacilwl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.smart0.xyz/gttqbbacrw.html

[N06] 判断回文字符串
来源：http://hz.jqgufenzy.top/gtwrfqwzxx.html

Py:   s == s[::-1]
来源：http://hz.vqdsnc.cn/gtganwpybz.html

PHP:  $s === strrev($s);
来源：http://hz.yonumen.top/gtsdqiprpm.html

JS:   s === [...s].reverse().join("")
来源：http://hz.52xcode.cn/gtdhpmdxno.html

TS:   s === [...s].reverse().join("")
来源：http://hz.haohaochexian.top/gtgpedjgfq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.hnxiangtu.top/gtgksfglji.html

Go:   // 双指针从两端比较
来源：http://hz.52xcode.cn/gtcbmtqkph.html

Ruby: s == s.reverse
来源：http://hz.zhongyouzk.top/gtauokafxa.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hnqzz.top/gtnilrlvwo.html

[N07] 两数之和（返回下标）
来源：http://hz.gogol.net.cn/gtfzkfmcjz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.dianchejie.cn/gtcrcdelnx.html


<!-- 参考信息 -->