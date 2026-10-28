代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.guannengcc.top/gtksygcprk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yj202588.top/gtbfshwqwm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.aibaodan.cn/gthbuhygfj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.andypj.xyz/gtkmhqujzq.html

================================================================================
来源：http://hz.jinqigfzy.top/gtxlhakzdh.html

K. JSON 与序列化
来源：http://hz.ydzc1.top/gtncsccvpq.html

================================================================================
来源：http://hz.bjfxy.top/gtvtmyfnni.html

[K01] 对象转 JSON 字符串
来源：http://hz.xinyue.icu/gtxyllfolp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yuanzhike.top/gtftppeewr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.nanxuanxn.top/gtjfzrdtxm.html

JS:   JSON.stringify(obj)
来源：http://hz.guannengcc.top/gtgiizbxkd.html

TS:   JSON.stringify(obj)
来源：http://hz.wangdashe.top/gttsxhbprz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zycfv.cn/gtkxrczesa.html

Go:   json.Marshal(obj)
来源：http://hz.zhengqikj.top/gtohpubvjh.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shuidangran.top/gtrxwzmwgf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jyoumei.cn/gtamwuinek.html

[K02] JSON 字符串转对象
来源：http://hz.shangyingyoupin.top/gtguiraidm.html

Py:   json.loads(s)
来源：http://hz.ehwqpu.com/gtwyundivd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.sweek.top/gtlcqmvyas.html

JS:   JSON.parse(s)
来源：http://hz.andypj.xyz/gttxloyaud.html

TS:   JSON.parse(s)
来源：http://hz.cheryme.top/gtlcgglmxz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.ydjk.org.cn/gtexlvcieu.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhijiandao.cn/gtnkjspezq.html

Ruby: JSON.parse(s)
来源：http://hz.mhx1999.top/gtjvoqpyci.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.gogol.net.cn/gtxmhqmwtd.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.316326.xyz/gtyglildje.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.nanxuanxn.top/gtuhaeenpr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhengqikj.top/gtexlzubsr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ybcxt.top/gtrqltrdim.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yueranfly.top/gtcrqjnoyq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ehwqpu.com/gtdxffrbgb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yonumen.top/gtzdmzgznu.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.snrcjt.cn/gtmxykjbzh.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.tianlin.xyz/gtswvdtllj.html

[K04] 读取 JSON 文件
来源：http://hz.xinyue.icu/gtxwwebcjb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.fzhhl.top/gtikqwlpes.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.wangshuangyany.cn/gttpqqigwj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.c1oappe.top/gtmyhjjevq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shuidangran.top/gtiqhjjxfs.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhixingplan.top/gtmgneuila.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ybcxt.top/gtsynnzcfv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhiwuduotai.top/gtxfvqailz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.chenjidiqi.icu/gtrphwfpjg.html

[K05] 深拷贝对象
来源：http://hz.hnxiangtu.top/gtxyptspnj.html

Py:   copy.deepcopy(obj)
来源：http://hz.gaohongyu789.top/gtysghsdxg.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yueranfly.top/gtbjphqngp.html

JS:   structuredClone(obj)
来源：http://hz.zycfv.cn/gtladbcoov.html

TS:   structuredClone(obj)
来源：http://hz.aizwys.cn/gtwdqrbbdk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhoulong.xyz/gtavtgwajt.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.fengsongda.top/gtmsdvlhke.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.mhx1999.top/gtwqftdyyz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.xuanzx.com/gtotrlyuxc.html

[K06] 解析 URL 查询串
来源：http://hz.zhixingplan.top/gtgjaqsmqh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yangfankeji.com/gtpqqarxxl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.redwolf501.top/gtuhkylgzo.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhongyouzk.top/gtpjqmtckd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ydjk.org.cn/gtgmvhrhlm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.xziqi.cn/gtkiuyudas.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hywenlv.cn/gtqmbidtpe.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ivvv.top/gtxwqyoizn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.tian-w.cn/gtdafcckvj.html

[K07] 进制转换
来源：http://hz.zhiwuduotai.top/gttnubigge.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yanxiufei.cn/gtgchcxayu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.chenlongwang.top/gtkuctwqrr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yj202588.top/gtjduykllg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jqgufenzy.top/gtluwfwluu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.feifeiyinyue.top/gtgzpgrdgg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.birdmap.top/gtlmcytcmp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.guannengcc.top/gtxdelemwx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yangfankeji.com/gtdrdamstf.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.hammf.cn/gtdiiliaou.html

Py:   pickle.dumps(obj)
来源：http://hz.yonumen.top/gtlxonovfo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.gzhubu.top/gtahtmznvk.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.fzhhl.top/gtgiaudvep.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.aizwys.cn/gtrpjpdbtv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ydjk.org.cn/gtgusnxtvz.html

Go:   encoding/gob
来源：http://hz.zhoulong.xyz/gtymtltgex.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhaomingkeji.xyz/gtzuklzhrh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xziqi.cn/gtpwgbvxiw.html

================================================================================
来源：http://hz.yuanzhike.top/gtocbdqzaq.html

L. 网络请求
来源：http://hz.316326.xyz/gtjigkjswa.html

================================================================================
来源：http://hz.gaohongyu789.top/gteobbycox.html

[L01] 发送 GET 请求
来源：http://hz.0kj1m.cn/gtgucfmxrq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.fengsongda.top/gtmolynafk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.xinyue.icu/gtgayakybl.html

JS:   await fetch(url)
来源：http://hz.haohaochexian.top/gtwxyowtuc.html

TS:   await fetch(url)
来源：http://hz.yuxming.cn/gtunpqwvsh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.cdnleiting.top/gtpoqwyhmz.html

Go:   resp, err := http.Get(url)
来源：http://hz.chenzaomai.com/gtuqdaruaq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hnxiangtu.top/gtlavtvugt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.sufxvd.cn/gtjmvgpfru.html

[L02] 发送 POST JSON
来源：http://hz.cucudq.cn/gtgnjukcik.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhiwuduotai.top/gtabrpfrjy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.wangshuangyany.cn/gtrpivsjcd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gaohongyu789.top/gtnjaoultn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gaohongyu789.top/gtxnbufpqk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zdqjudy.top/gtduwqhyuy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.aizwys.cn/gtiqagbdhr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.tianlin.xyz/gtocaeptdo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.sysykeji.top/gtskuifnjc.html

[L03] 设置自定义请求头
来源：http://hz.cashguo.top/gtkvrjnypz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jqgufenzy.top/gtgfsddiqp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.shanyushiyangkeji.top/gtssfkfkff.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jqgufenzy.top/gtdnwydvoi.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ywan-chungtsiang.top/gtssskkucl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhoulong.xyz/gtkhqmheal.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ybcxt.top/gtrlexpllt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.daria6918.cn/gtsmstzfuq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.fengsongda.top/gtmhnfzoqg.html

[L04] 设置超时
来源：http://hz.yj20258888.top/gttidrhqlu.html

Py:   requests.get(url, timeout=5)
来源：http://hz.haohaochexian.top/gtjbuibmql.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.cheryme.top/gtmcbxpjlk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sufxvd.cn/gtohidbqrq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sufxvd.cn/gtdmulohhp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xingfuxueyuan.xyz/gteogtmjcq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jqgfzy.top/gtjnucjayv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jinqigufen.top/gtyhhabxjl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.fzhhl.top/gtrrglbdkh.html

[L05] 上传文件（multipart）
来源：http://hz.hysaishi.cn/gtzuxuwlsn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.316326.xyz/gtrvkyuuxx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xinyue.icu/gtufugdonk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.xziqi.cn/gtqpmklydw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.fzhhl.top/gtuwqcswiv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.sxryk.cn/gtxdhjacxw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.chenlongwang.top/gtjmotojzs.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ywan-chungtsiang.top/gtzesphmfb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.nwbrower.top/gtqpebwcqt.html

[L06] 解析响应为 JSON
来源：http://hz.shangyingyoupin.top/gtzwkdling.html

Py:   resp.json()
来源：http://hz.xuanzx.com/gtbcvsutdt.html

PHP:  json_decode($body, true);
来源：http://hz.zhixingplan.top/gtdstwwpif.html

JS:   await resp.json()
来源：http://hz.xuanzx.com/gtrreedkdo.html

TS:   await resp.json()
来源：http://hz.cdnleiting.top/gtkywnbwiq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.cqqwz.cn/gtxvfilucm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.cucudq.cn/gtstziczfg.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ydjk.org.cn/gtmptzwpkl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.meibo888.top/gteqbkxqkg.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhixingplan.top/gthfzhzvzs.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.daria6918.cn/gtyrttchnp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.cheryme.top/gtmahtxmgb.html

JS:   resp.ok;  resp.status
来源：http://hz.guowangkeji.top/gtfkqrvypu.html

TS:   resp.ok;  resp.status
来源：http://hz.hammf.cn/gtvieccbcb.html

Java: resp.statusCode()
来源：http://hz.cucudq.cn/gtrwaouuks.html

Go:   resp.StatusCode
来源：http://hz.yangfankeji.com/gtfqtcpgza.html

Ruby: resp.code.to_i
来源：http://hz.xuanzx.com/gtkjupsrje.html

C#:   (int)resp.StatusCode
来源：http://hz.yj20258.top/gtgpwhbmqs.html

[L08] 并发请求多个地址
来源：http://hz.sufxvd.cn/gtcwclxgmd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ppjwa.cn/gtjsskszbl.html

PHP:  curl_multi_init() 系列
来源：http://hz.shanyushiyangkeji.top/gtinvoggxm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhaomingkeji.xyz/gtkzcazqij.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ivvv.top/gtazuedxva.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xziqi.cn/gteytecxsd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.gotoacloud.top/gtawfwkxjk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.xziqi.cn/gtwyjrprfj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xingfuxueyuan.xyz/gtceaituei.html

================================================================================
来源：http://hz.xylfe.cn/gtethdopko.html

M. 命令行 / 进程 / 环境
来源：http://hz.nanxinkj.top/gtldlzbhzr.html

================================================================================
来源：http://hz.yangfankeji.com/gtomyzjfjf.html

[M01] 读取命令行参数
来源：http://hz.hywenlv.cn/gtmgkyrhem.html

Py:   sys.argv[1:]
来源：http://hz.yuanzhike.top/gtaifcwqfj.html

PHP:  $argv;  $argc;
来源：http://hz.shangyingyoupin.top/gtpquejqge.html

JS:   process.argv.slice(2)
来源：http://hz.hysaishi.cn/gtyrpzolov.html

TS:   process.argv.slice(2)
来源：http://hz.chenjidiqi.icu/gtgrwsslsi.html

Java: args 数组（main 方法参数）
来源：http://hz.dashuyun.cn/gtyfnwnobq.html

Go:   os.Args[1:]
来源：http://hz.hammf.cn/gtsnazzxlq.html

Ruby: ARGV
来源：http://hz.9152youxi.cn/gtmesrpjkv.html

C#:   args 数组（Main 方法参数）
来源：http://hz.cqqwz.cn/gtvitjmpro.html

[M02] 读取环境变量
来源：http://hz.wangshuangyany.cn/gtbgirqmqj.html

Py:   os.environ.get("HOME")
来源：http://hz.nanxinkj.top/gtealybhcl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.xylfe.cn/gtkeshlftz.html

JS:   process.env.HOME
来源：http://hz.birdmap.top/gtpyohoxyu.html

TS:   process.env.HOME
来源：http://hz.52xcode.cn/gtpedrheus.html

Java: System.getenv("HOME")
来源：http://hz.nanxuanxn.top/gtpsadteil.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jinyuanbaomall.cn/gtiabdrpqt.html

Ruby: ENV["HOME"]
来源：http://hz.tanke756.top/gtakshsnbf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.mhx1999.top/gtvptucopu.html

[M03] 执行外部命令
来源：http://hz.gzhubu.top/gtldhbvszc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.shanyushiyangtech.top/gtbtreqwfu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.pengpengdd.cyou/gtupjoexrg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yangfankeji.com/gtwneblaiz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.gaohongyu789.top/gtgnirtaqi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.gotoacloud.top/gtaxcirtiw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.iojbl.cn/gtdwmblfpb.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zycfv.cn/gtrplbucqi.html

C#:   Process.Start("ls", "-l");
来源：http://hz.nanxuanxn.top/gtxcvbtofh.html

[M04] 获取当前工作目录
来源：http://hz.sufxvd.cn/gtljmxywqr.html

Py:   os.getcwd()
来源：http://hz.xingfuxueyuan.xyz/gtdlozemcr.html

PHP:  getcwd();
来源：http://hz.ydjk.org.cn/gtepwswubt.html

JS:   process.cwd()
来源：http://hz.xingfuxueyuan.xyz/gtimejkbqa.html

TS:   process.cwd()
来源：http://hz.kuanghao11.cn/gtaotuvuhs.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yvedp.cn/gtupwjdmri.html

Go:   os.Getwd()
来源：http://hz.nanxinkj.top/gtiaurdeic.html

Ruby: Dir.pwd
来源：http://hz.nanxinkj.top/gtpdejknlt.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.xinyue.icu/gtoraqktav.html

[M05] 设置退出码
来源：http://hz.yj202588.top/gtvgskksyp.html

Py:   sys.exit(1)
来源：http://hz.yueranfly.top/gtlhapupdx.html

PHP:  exit(1);
来源：http://hz.hywenlv.cn/gtfarpcwke.html

JS:   process.exit(1)
来源：http://hz.yj202588.top/gtbxadngjg.html

TS:   process.exit(1)
来源：http://hz.fzhhl.top/gtieidacrk.html

Java: System.exit(1)
来源：http://hz.xinyue.icu/gtteryedhd.html

Go:   os.Exit(1)
来源：http://hz.gotoacloud.top/gtmabcdcye.html

Ruby: exit 1
来源：http://hz.xziqi.cn/gtixtmkhnf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.0kj1m.cn/gtljotybwx.html

[M06] 向标准错误输出
来源：http://hz.jyoumei.cn/gtaqhrlnjo.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ivvv.top/gtkgatkogl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.guannengcc.top/gtuivwcbzs.html

JS:   console.error("err")
来源：http://hz.hammf.cn/gtmcsttsyn.html

TS:   console.error("err")
来源：http://hz.yvedp.cn/gttpoxycvi.html

Java: System.err.println("err")
来源：http://hz.zhixingplan.top/gtwhjmyyqs.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhaomingkeji.xyz/gtjjsiptgd.html

Ruby: warn "err"
来源：http://hz.yangfankeji.com/gtnbjdpibj.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hammf.cn/gtexxatiod.html

[M07] 判断是否为主入口
来源：http://hz.yueranfly.top/gtcdlhmiel.html

Py:   if __name__ == "__main__":
来源：http://hz.aizwys.cn/gtxxcgtwzq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.smart0.xyz/gtcdqiqxme.html

JS:   require.main === module
来源：http://hz.jinyuanbaomall.cn/gtoylsdjgj.html

TS:   require.main === module
来源：http://hz.yonumen.top/gtcspstcoc.html

Java: public static void main(String[] args)
来源：http://hz.jqgufenzy.top/gtninepyfu.html

Go:   func main()
来源：http://hz.havefunace.top/gtnffpperh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.xinyue.icu/gtycvyxxcc.html

C#:   static void Main(string[] args)
来源：http://hz.52xcode.cn/gtuaxglvzm.html

[M08] 获取系统与运行时信息
来源：http://hz.hywenlv.cn/gtjdngppdy.html

Py:   platform.system();  platform.python_version()
来源：http://hz.nwbrower.top/gtjciyyjio.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhongyouzk.top/gtbjhlwxff.html

JS:   process.platform;  process.version
来源：http://hz.52xcode.cn/gtgxxynhyl.html

TS:   process.platform;  process.version
来源：http://hz.xylfe.cn/gtmsqwdudz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.chenzaomai.com/gtfraaiwij.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.ydjk.org.cn/gthkxlpixw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.guowangkeji.top/gtlwjjwaaf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jlsjyb.cn/gtebcjezxq.html

================================================================================
来源：http://hz.svipenyu.cn/gthzkftldu.html

N. 数据结构与算法
来源：http://hz.zycfv.cn/gttkabodnh.html

================================================================================
来源：http://hz.shuidangran.top/gturlosete.html

[N01] 二分查找（有序数组）
来源：http://hz.gzhubu.top/gtvpeatzvj.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.nanxinkj.top/gteagbkzyg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.daxiang520.top/gtvkxlgmet.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.daxiang520.top/gteyzboqmc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yuxming.cn/gtyskkbnrb.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.tianlin.xyz/gttflhferb.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.chenlongwang.top/gtcztkyvyo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.cashguo.top/gtbdxypraw.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.hnqzz.top/gtaarkdsvi.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yuxming.cn/gtrfvevvpd.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ehwqpu.com/gtqcbdftpa.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhengqikj.top/gtpucfaeye.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.snrcjt.cn/gtkppfyxty.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jyoumei.cn/gtmozkjclz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhoulong.xyz/gtkszryshg.html

Go:   slices.Sort(arr)
来源：http://hz.cashguo.top/gtydxjqwkv.html

Ruby: arr.sort
来源：http://hz.yueranfly.top/gtvjddkjfy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ivvv.top/gtqlsevmmh.html

[N03] 快速排序（分治示例）
来源：http://hz.shangyingyoupin.top/gtwktpqviy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.bjfxy.top/gtopndcqve.html

PHP:  // 递归实现，或用 usort
来源：http://hz.dianchejie.cn/gtmhajswra.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cheryme.top/gtjefwdvxj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.c1oappe.top/gtwptduikc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jiagoushi.top/gtlzsrbhra.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.0kj1m.cn/gtajkdxcvf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.quarkkingdee.top/gtxdqnklhw.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yangfankeji.com/gtzumtzlss.html

[N04] 斐波那契数列
来源：http://hz.shzxlz.cn/gtedglvajw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.kuanghao11.cn/gtlittyffw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.tian-w.cn/gthwbkmixw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zdqjudy.top/gteuxdyqlh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hammf.cn/gtzqhmcpzq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.fengsongda.top/gtnzjjfwrz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.shanyushiyangkeji.top/gtnaaiijan.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.smart0.xyz/gtkuqkxirn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hfpthk.cn/gtfkbqluwc.html

[N05] 最大公约数
来源：http://hz.sysykeji.top/gtqzvgawax.html

Py:   math.gcd(a, b)
来源：http://hz.yj20258888.top/gtnhjfciwc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zhijiandao.cn/gtveijgzni.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yangfankeji.com/gtxkncspok.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhijiandao.cn/gtzwedazyq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.xziqi.cn/gtnfdccpcv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hysaishi.cn/gtwizurstk.html

Ruby: a.gcd(b)
来源：http://hz.ywan-chungtsiang.top/gtnnjykwsn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yangfankeji.com/gtxeshlgmt.html

[N06] 判断回文字符串
来源：http://hz.xingfuxueyuan.xyz/gtvayojaxb.html

Py:   s == s[::-1]
来源：http://hz.yangfankeji.com/gtzufqbiaz.html

PHP:  $s === strrev($s);
来源：http://hz.hammf.cn/gtfvhfxitf.html

JS:   s === [...s].reverse().join("")
来源：http://hz.c1oappe.top/gtwxhabuuv.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jinqigufen.top/gtjeljbqpk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zdqjudy.top/gtbahwipgm.html

Go:   // 双指针从两端比较
来源：http://hz.xuetiantiany.cn/gtxrbhzpup.html

Ruby: s == s.reverse
来源：http://hz.wangdashe.top/gtndoqxoiu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.xinyue.icu/gtldmqyufw.html

[N07] 两数之和（返回下标）
来源：http://hz.hnxiangtu.top/gthepjbggl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.chenlongwang.top/gtpdwzyptq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.316326.xyz/gtniaagizt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.havefunace.top/gtudeidmhf.html

TS:   // 手写 Map<string, number>
来源：http://hz.yueranfly.top/gtcvnnvqvy.html

Java: // 手写 HashMap
来源：http://hz.aizwys.cn/gtvuarhczr.html

Go:   // 手写 map[int]int
来源：http://hz.gaohongyu789.top/gtxdezpwjr.html

Ruby: // 手写 Hash
来源：http://hz.xuetiantiany.cn/gthfwcelsb.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.ppjwa.cn/gtnxreivmg.html

[N08] 生成全排列
来源：http://hz.sweek.top/gtgvmkpgcg.html

Py:   itertools.permutations(arr)
来源：http://hz.redwolf501.top/gtjrmhnhgf.html

PHP:  // 手写递归交换
来源：http://hz.52xcode.cn/gtnzpvdyep.html

JS:   // 手写回溯递归
来源：http://hz.jyoumei.cn/gtdyladgrs.html

TS:   // 手写回溯递归
来源：http://hz.hnqzz.top/gtwjtoafoc.html


<!-- 参考信息 -->