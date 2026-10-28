代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yj202588.top/gtgqizcivj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hfpthk.cn/gtshlsylyv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.aizwys.cn/gtkltucptt.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jinqigufen.top/gtjzoaqdlc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yanxiufei.cn/gtjdcpijxa.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hnxiangtu.top/gtazpphndr.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ppjwa.cn/gtfbtkswni.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zycfv.cn/gtjbgfskkl.html

================================================================================
来源：http://hz.jiagoushi.top/gtmggtjjgs.html

K. JSON 与序列化
来源：http://hz.ehwqpu.com/gtebcpgopv.html

================================================================================
来源：http://hz.chenlongwang.top/gtsurjpogx.html

[K01] 对象转 JSON 字符串
来源：http://hz.yueranfly.top/gtqgpkgfgk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.chenzaomai.com/gtlxsneeer.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.cdnleiting.top/gtnvkikisb.html

JS:   JSON.stringify(obj)
来源：http://hz.gaohongyu789.top/gtmbhbmsmw.html

TS:   JSON.stringify(obj)
来源：http://hz.yonumen.top/gtgetwftzf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.vqdsnc.cn/gtotertqwj.html

Go:   json.Marshal(obj)
来源：http://hz.316326.xyz/gtghunpqlb.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.chenlongwang.top/gtjxgaveeq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.pengpengdd.cyou/gtliomzsom.html

[K02] JSON 字符串转对象
来源：http://hz.nwbrower.top/gtfbeqhbdn.html

Py:   json.loads(s)
来源：http://hz.yj202588.top/gtpjxruegg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yj202588.top/gthbacjuyn.html

JS:   JSON.parse(s)
来源：http://hz.ivvv.top/gtfupuaatd.html

TS:   JSON.parse(s)
来源：http://hz.fengsongda.top/gtekikuppo.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.gzhubu.top/gtivvgpqeq.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.cucudq.cn/gtilzlxvir.html

Ruby: JSON.parse(s)
来源：http://hz.redwolf501.top/gtnqqpbvbk.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.nanxuanxn.top/gtewneeulg.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.sufxvd.cn/gthegzqfmf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.cqqwz.cn/gtbsfiihdw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jinqigufen.top/gtdtlacdwv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xuanzx.com/gtkpdqofkm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yongpay.top/gtlsjmviru.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jianghu66.top/gtykzqzzvu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ehwqpu.com/gtpaihwkky.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.daxiang520.top/gttydafxyh.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ydzc1.top/gtxlchtpak.html

[K04] 读取 JSON 文件
来源：http://hz.tanke756.top/gtwwuuvvqd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hywenlv.cn/gtuqxyyzbe.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cucudq.cn/gtcjwpjnuq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.guowangkeji.top/gtncdnmotc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zycfv.cn/gtdiqewwhb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.sxryk.cn/gtzxbqyukg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.daxiang520.top/gtcqzkuyqw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.xylfe.cn/gtslrnxekc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.snrcjt.cn/gtrhiwsogf.html

[K05] 深拷贝对象
来源：http://hz.yueranfly.top/gtljodwwtu.html

Py:   copy.deepcopy(obj)
来源：http://hz.redwolf501.top/gtzoahpcnj.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ydzc1.top/gtqdnnazku.html

JS:   structuredClone(obj)
来源：http://hz.yvedp.cn/gtkxhjdgpb.html

TS:   structuredClone(obj)
来源：http://hz.sxryk.cn/gtuqhabzoq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.smart0.xyz/gtnhjritlf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.andypj.xyz/gtdoracloc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.smart0.xyz/gtakatzqzf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.dashuyun.cn/gtissbwscy.html

[K06] 解析 URL 查询串
来源：http://hz.ybcxt.top/gtjaiwalmu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jianghu66.top/gtfaaqivcy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yuanzhike.top/gtgeufovde.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yanxiufei.cn/gtohmjoqlc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jiagoushi.top/gttzzmecjn.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hnqzz.top/gtphzekwrk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.ywan-chungtsiang.top/gtodedwekc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.sysykeji.top/gtqmncqlcm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.0kj1m.cn/gtbwnznqsr.html

[K07] 进制转换
来源：http://hz.zycfv.cn/gtyvwbrrar.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yuanzhike.top/gtwwrwddcb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.chenzaomai.com/gtfxnytheb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hfpthk.cn/gtyjqaioui.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhengqikj.top/gtrwtstbel.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ivvv.top/gtsjkprfrh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jianghu66.top/gteyeualxv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.pycfn.com/gtzfiyhubi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.aizwys.cn/gtxjvabbdf.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhijiandao.cn/gtmqpouhlp.html

Py:   pickle.dumps(obj)
来源：http://hz.jqgfzy.top/gtyqesjfcj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yonumen.top/gtlmrdlfhd.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.wangshuangyany.cn/gtdourwvif.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yvedp.cn/gtahffzgcv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.smart0.xyz/gtukjiyfzm.html

Go:   encoding/gob
来源：http://hz.guowangkeji.top/gtevgaduqk.html

Ruby: Marshal.dump(obj)
来源：http://hz.nanxuanxn.top/gtcrxelnxp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.smart0.xyz/gtxmepojov.html

================================================================================
来源：http://hz.sufxvd.cn/gtfaqcgptw.html

L. 网络请求
来源：http://hz.9152youxi.cn/gtubmbptjs.html

================================================================================
来源：http://hz.c1oappe.top/gtszwigysn.html

[L01] 发送 GET 请求
来源：http://hz.zdqjudy.top/gtsiulzgke.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jyoumei.cn/gtxsjbwqpy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.sufxvd.cn/gtehaogxxj.html

JS:   await fetch(url)
来源：http://hz.guowangkeji.top/gtcqclxemt.html

TS:   await fetch(url)
来源：http://hz.jianghu66.top/gtlvxmcjor.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.nanxinkj.top/gtfgdgsvbu.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhengqikj.top/gteppvuzhu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cheryme.top/gtspzhhhuz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.chenjidiqi.icu/gtilrsskoa.html

[L02] 发送 POST JSON
来源：http://hz.ydjk.org.cn/gthdfwzqeb.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.birdmap.top/gtvgmyftuz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yueranfly.top/gttwehohza.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gogol.net.cn/gtbnozemiu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.snrcjt.cn/gtzcdqfort.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yuanzhike.top/gtywupvngj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.svipenyu.cn/gtlrzgquyo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhixingplan.top/gtewsurtar.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jqgufenzy.top/gtnoixwwpm.html

[L03] 设置自定义请求头
来源：http://hz.ehwqpu.com/gtxsevsptd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.quarkkingdee.top/gtqvovnymy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.tian-w.cn/gthjscbpxb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.daria6918.cn/gthlvouayx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sweek.top/gtwpwtwhws.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.cucudq.cn/gtnywwzege.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hnqzz.top/gtmjmzwmhh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ydjk.org.cn/gtlvfrgpni.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhengqikj.top/gtbtmdkafg.html

[L04] 设置超时
来源：http://hz.ydzc1.top/gtofashiof.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hfpthk.cn/gtjavibowx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zhijiandao.cn/gtyrujesqp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.guowangkeji.top/gtlnvittfl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ywan-chungtsiang.top/gtcwrdsfeb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zycfv.cn/gtukvjloeh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.haohaochexian.top/gtsxpaunln.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zhaomingkeji.xyz/gtnodwyvif.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.shangyingyoupin.top/gtcbpeasca.html

[L05] 上传文件（multipart）
来源：http://hz.cashguo.top/gtiyjdqsoc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.gzhubu.top/gtmzsinwpp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.tianlin.xyz/gtzhbzigyo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.haohaochexian.top/gtvtsnyrqq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.guowangkeji.top/gtbeeeffpd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.cdnleiting.top/gtqhyczhks.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.chenjidiqi.icu/gtuxsyurpw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jiagoushi.top/gtwxfjdklf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.gotoacloud.top/gtzjlnhqbw.html

[L06] 解析响应为 JSON
来源：http://hz.zycfv.cn/gtkcmxnyue.html

Py:   resp.json()
来源：http://hz.pycfn.com/gtizkbflvb.html

PHP:  json_decode($body, true);
来源：http://hz.aizwys.cn/gtlupjlvcr.html

JS:   await resp.json()
来源：http://hz.chenlongwang.top/gtkvignhmy.html

TS:   await resp.json()
来源：http://hz.yj20258888.top/gtmrjxmxed.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.9152youxi.cn/gtolqcjwri.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yj20258.top/gtwvwiyqen.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ivvv.top/gtataxmpwv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yuanzhike.top/gtqgzeopez.html

[L07] 处理 HTTP 状态码
来源：http://hz.gzhubu.top/gtovmkirso.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.fzhhl.top/gteantxkow.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.sysykeji.top/gtttwqyxwb.html

JS:   resp.ok;  resp.status
来源：http://hz.sufxvd.cn/gteoxpjfon.html

TS:   resp.ok;  resp.status
来源：http://hz.shangyingyoupin.top/gtneetnnlf.html

Java: resp.statusCode()
来源：http://hz.shanyushiyangkeji.top/gtevdgbagu.html

Go:   resp.StatusCode
来源：http://hz.hnqzz.top/gtocgbzhdz.html

Ruby: resp.code.to_i
来源：http://hz.zhaomingkeji.xyz/gtgyiyzcfc.html

C#:   (int)resp.StatusCode
来源：http://hz.yvedp.cn/gtukmymfgp.html

[L08] 并发请求多个地址
来源：http://hz.shuidangran.top/gtowknevbn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.tian-w.cn/gtlrajlvxw.html

PHP:  curl_multi_init() 系列
来源：http://hz.vqdsnc.cn/gtfikfobke.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yueranfly.top/gtzjzzjgjq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zdqjudy.top/gtdtruvoxi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hnqzz.top/gtzvckqctb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.shuidangran.top/gtkvomskpk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yonumen.top/gtstfgrcpv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.dianchejie.cn/gtvzxexkix.html

================================================================================
来源：http://hz.yongpay.top/gtsdmhfczs.html

M. 命令行 / 进程 / 环境
来源：http://hz.gogol.net.cn/gtjdebkxua.html

================================================================================
来源：http://hz.zhixingplan.top/gtfkgajbxp.html

[M01] 读取命令行参数
来源：http://hz.shuidangran.top/gtknyaobup.html

Py:   sys.argv[1:]
来源：http://hz.52xcode.cn/gtkfoudlwq.html

PHP:  $argv;  $argc;
来源：http://hz.sufxvd.cn/gtlnftaple.html

JS:   process.argv.slice(2)
来源：http://hz.daria6918.cn/gtrxpgvjnd.html

TS:   process.argv.slice(2)
来源：http://hz.dianchejie.cn/gthnhfntyb.html

Java: args 数组（main 方法参数）
来源：http://hz.hysaishi.cn/gtyuktaycd.html

Go:   os.Args[1:]
来源：http://hz.c1oappe.top/gteqregitd.html

Ruby: ARGV
来源：http://hz.jinqigufen.top/gtpiaazcan.html

C#:   args 数组（Main 方法参数）
来源：http://hz.nanxinkj.top/gtetcazsov.html

[M02] 读取环境变量
来源：http://hz.zycfv.cn/gtctmpymxn.html

Py:   os.environ.get("HOME")
来源：http://hz.daria6918.cn/gtppyifpju.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.kuanghao11.cn/gtzrcpxizn.html

JS:   process.env.HOME
来源：http://hz.cdnleiting.top/gtxobhhpot.html

TS:   process.env.HOME
来源：http://hz.yvedp.cn/gtkwupsjhc.html

Java: System.getenv("HOME")
来源：http://hz.shanyushiyangtech.top/gtbzgrooef.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.iojbl.cn/gtqyjzdzmd.html

Ruby: ENV["HOME"]
来源：http://hz.haohaochexian.top/gtrecsmmqc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jqgufenzy.top/gtpvhepslk.html

[M03] 执行外部命令
来源：http://hz.jlsjyb.cn/gtifupbuix.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.tanke756.top/gtfppphuhg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.bjfxy.top/gtcatefmke.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.vqdsnc.cn/gtauczwzdw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.52xcode.cn/gtmxkcsqha.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.dashuyun.cn/gtxlwbzqei.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hnqzz.top/gtcxtkdmaa.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.guannengcc.top/gtzbjdxpol.html

C#:   Process.Start("ls", "-l");
来源：http://hz.gotoacloud.top/gtcbbpqjji.html

[M04] 获取当前工作目录
来源：http://hz.havefunace.top/gtmdztqiwx.html

Py:   os.getcwd()
来源：http://hz.daxiang520.top/gtunxbphpd.html

PHP:  getcwd();
来源：http://hz.nanxinkj.top/gtojxxohlm.html

JS:   process.cwd()
来源：http://hz.yueranfly.top/gtyyhstbmh.html

TS:   process.cwd()
来源：http://hz.yj20258888.top/gtcfvlugkm.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jlsjyb.cn/gtwbiqykkm.html

Go:   os.Getwd()
来源：http://hz.sxryk.cn/gtlckzozja.html

Ruby: Dir.pwd
来源：http://hz.yvedp.cn/gtcltujdwf.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.guannengcc.top/gtxrfokkbc.html

[M05] 设置退出码
来源：http://hz.hywenlv.cn/gtytkfmxss.html

Py:   sys.exit(1)
来源：http://hz.jinqigufen.top/gtkmoqfonr.html

PHP:  exit(1);
来源：http://hz.gzhubu.top/gtcmkwmuio.html

JS:   process.exit(1)
来源：http://hz.wangdashe.top/gtvwribzqk.html

TS:   process.exit(1)
来源：http://hz.nwbrower.top/gthtzqaqtf.html

Java: System.exit(1)
来源：http://hz.hnxiangtu.top/gtoavqwmvt.html

Go:   os.Exit(1)
来源：http://hz.yj202588.top/gtrhipxxbo.html

Ruby: exit 1
来源：http://hz.nanxuanxn.top/gtrrhdowen.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.hnxiangtu.top/gtrteibows.html

[M06] 向标准错误输出
来源：http://hz.yuanzhike.top/gtcucgqwpp.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jqgufenzy.top/gtfbblthtz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.pycfn.com/gtmmsdqyoj.html

JS:   console.error("err")
来源：http://hz.haohaochexian.top/gtcqpozuek.html

TS:   console.error("err")
来源：http://hz.hywenlv.cn/gtrdsaxnxc.html

Java: System.err.println("err")
来源：http://hz.sweek.top/gtwyrjsrxi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.vqdsnc.cn/gtbdlyfejy.html

Ruby: warn "err"
来源：http://hz.yj202588.top/gtdieekyix.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.feifeiyinyue.top/gtbyufbxjp.html

[M07] 判断是否为主入口
来源：http://hz.fengsongda.top/gtokukjgyv.html

Py:   if __name__ == "__main__":
来源：http://hz.wangdashe.top/gturotlidn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhixingplan.top/gtecouyybc.html

JS:   require.main === module
来源：http://hz.birdmap.top/gtykbtiefh.html

TS:   require.main === module
来源：http://hz.9152youxi.cn/gtiupnuflf.html

Java: public static void main(String[] args)
来源：http://hz.zhoulong.xyz/gtkqxgzzpe.html

Go:   func main()
来源：http://hz.fzhhl.top/gtfqjftruy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zycfv.cn/gtanhwlwxy.html

C#:   static void Main(string[] args)
来源：http://hz.zhixingplan.top/gtimtevaqu.html

[M08] 获取系统与运行时信息
来源：http://hz.hongshengwenyu.top/gtzaipxraa.html

Py:   platform.system();  platform.python_version()
来源：http://hz.xinyue.icu/gtwkhvhtlt.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.cashguo.top/gttqyudfkq.html

JS:   process.platform;  process.version
来源：http://hz.xingfuxueyuan.xyz/gtufkazxec.html

TS:   process.platform;  process.version
来源：http://hz.zycfv.cn/gtijiwpqaz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.nanxinkj.top/gtwkgdsmch.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.pengpengdd.cyou/gtdujdnpws.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jlsjyb.cn/gtlwshnsfc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhijiandao.cn/gteisbnykg.html

================================================================================
来源：http://hz.wangdashe.top/gtivtyyess.html

N. 数据结构与算法
来源：http://hz.c1oappe.top/gtdvsvftfe.html

================================================================================
来源：http://hz.dashuyun.cn/gtlpqbycld.html

[N01] 二分查找（有序数组）
来源：http://hz.jianghu66.top/gtbdyyvqey.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.nanxinkj.top/gtlisixgui.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ehwqpu.com/gtnrsfgxsk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhaomingkeji.xyz/gtlcerjkvy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yueranfly.top/gtoadcnrtv.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jinqigufen.top/gtigoxhofq.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ywan-chungtsiang.top/gtqehizrqc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.svipenyu.cn/gtfbxffshe.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.birdmap.top/gtrrdtqcfz.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.fzhhl.top/gtpigklpef.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gogol.net.cn/gtzeabrllo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.shanyushiyangtech.top/gtqyagjzmt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sxryk.cn/gtkxgxgrsf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.snrcjt.cn/gtttvucgxu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhaomingkeji.xyz/gtoygdwfmq.html

Go:   slices.Sort(arr)
来源：http://hz.jqgfzy.top/gtkmqkmpot.html

Ruby: arr.sort
来源：http://hz.mhx1999.top/gtldoqmwww.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jinghuilouyu.cn/gtqcwqoqlj.html

[N03] 快速排序（分治示例）
来源：http://hz.sweek.top/gtcwtgqtxm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hammf.cn/gtutgfmbvs.html

PHP:  // 递归实现，或用 usort
来源：http://hz.shanyushiyangtech.top/gthfwfwpbw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhixingplan.top/gtcmrdtnnd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhaomingkeji.xyz/gtnrxjyutx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.gogol.net.cn/gtzkbnuuqj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yongpay.top/gtkczbvtjn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhoulong.xyz/gtfjnqhshv.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ivvv.top/gtvxvbhgrg.html

[N04] 斐波那契数列
来源：http://hz.ywan-chungtsiang.top/gtuohmcbep.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.daria6918.cn/gtpmnnzlhn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.fzhhl.top/gttjdyiyiz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shzxlz.cn/gtwndkkvax.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sufxvd.cn/gtpyipsdul.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.quarkkingdee.top/gtxzavjndh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.pengpengdd.cyou/gttvxvulbf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ppjwa.cn/gtugnieeyl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jinqigufen.top/gtibgkjvrb.html

[N05] 最大公约数
来源：http://hz.jqgufenzy.top/gtgqtkvppg.html

Py:   math.gcd(a, b)
来源：http://hz.ywan-chungtsiang.top/gtiuysbujb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zdqjudy.top/gtnzajcvss.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhaomingkeji.xyz/gtlkzfpxtz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ybcxt.top/gtzrqzqneb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.tianlin.xyz/gtuspniqxi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhengqikj.top/gtwxbnawgj.html

Ruby: a.gcd(b)
来源：http://hz.smart0.xyz/gtlilyejjm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhengqikj.top/gthunbmewq.html

[N06] 判断回文字符串
来源：http://hz.hongshengwenyu.top/gtctchvshw.html

Py:   s == s[::-1]
来源：http://hz.jqgufenzy.top/gtqcipxdwx.html

PHP:  $s === strrev($s);
来源：http://hz.ehwqpu.com/gtytvwprkq.html

JS:   s === [...s].reverse().join("")
来源：http://hz.dianchejie.cn/gtogvqwuxd.html

TS:   s === [...s].reverse().join("")
来源：http://hz.cashguo.top/gtzhsaizol.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.aibaodan.cn/gtbxtoxvam.html

Go:   // 双指针从两端比较
来源：http://hz.52xcode.cn/gtqdfubxbt.html

Ruby: s == s.reverse
来源：http://hz.hnqzz.top/gtquiyybig.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.tian-w.cn/gtocjwhigs.html

[N07] 两数之和（返回下标）
来源：http://hz.yj202588.top/gtqbzqngal.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.gzhubu.top/gtpjrjlyyw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hongshengwenyu.top/gtudvluerl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ehwqpu.com/gttyuiqpua.html

TS:   // 手写 Map<string, number>
来源：http://hz.xuanzx.com/gtjswqzudd.html

Java: // 手写 HashMap
来源：http://hz.hnxiangtu.top/gtlkrfnfsf.html

Go:   // 手写 map[int]int
来源：http://hz.chenjidiqi.icu/gtiromafxo.html

Ruby: // 手写 Hash
来源：http://hz.cdnleiting.top/gtgfcwqloo.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.ybcxt.top/gtwbsdpydb.html

[N08] 生成全排列
来源：http://hz.havefunace.top/gtzottwwde.html


<!-- 参考信息 -->