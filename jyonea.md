代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.fengsongda.top/gtibkvgjlf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jqgufenzy.top/gtajxgmtpx.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.gogol.net.cn/gtunmlzgxf.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.shuidangran.top/gtmxkripps.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.c1oappe.top/gtiofmqjqd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.kuanghao11.cn/gtyxefofmw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.smart0.xyz/gtvmbfzjju.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ydjk.org.cn/gtqdsfetnj.html

================================================================================
来源：http://hz.c1oappe.top/gteoyqrlma.html

K. JSON 与序列化
来源：http://hz.kuanghao11.cn/gtbnqfimuz.html

================================================================================
来源：http://hz.dianchejie.cn/gtywsxzmxf.html

[K01] 对象转 JSON 字符串
来源：http://hz.ppjwa.cn/gtoecgwszz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.gotoacloud.top/gtawmjbgpy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.sweek.top/gtfdrevlxs.html

JS:   JSON.stringify(obj)
来源：http://hz.ppjwa.cn/gttsqaikfy.html

TS:   JSON.stringify(obj)
来源：http://hz.jinyuanbaomall.cn/gtjhfiqfre.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhixingplan.top/gtxoolselb.html

Go:   json.Marshal(obj)
来源：http://hz.9152youxi.cn/gtoyfghnzw.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.nanxuanxn.top/gtjesmexlr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yongpay.top/gtmhougste.html

[K02] JSON 字符串转对象
来源：http://hz.daxiang520.top/gtxoopkvrt.html

Py:   json.loads(s)
来源：http://hz.xingfuxueyuan.xyz/gtkypyfkdi.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hongshengwenyu.top/gtozaiczrr.html

JS:   JSON.parse(s)
来源：http://hz.0kj1m.cn/gtxvmayttw.html

TS:   JSON.parse(s)
来源：http://hz.hywenlv.cn/gtlhhtkpiu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.shuidangran.top/gtolcrynnh.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jinghuilouyu.cn/gtvjmjnwwl.html

Ruby: JSON.parse(s)
来源：http://hz.shangyingyoupin.top/gtsqfntpgn.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yj20258.top/gtnxthygrk.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hongshengwenyu.top/gtxlqcixnz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jinqigufen.top/gtgdvvksmc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jqgfzy.top/gtyaejxzwx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shanyushiyangkeji.top/gttjtvduik.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.pycfn.com/gtcxvsdzyw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jianghu66.top/gtnuvavduq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.aibaodan.cn/gttyvlhdop.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jqgufenzy.top/gthtrygcxh.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ywan-chungtsiang.top/gtkiojpcvq.html

[K04] 读取 JSON 文件
来源：http://hz.guowangkeji.top/gtdzzukcnk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zycfv.cn/gtqmjncaab.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cdnleiting.top/gtmkmtfmtk.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.0kj1m.cn/gtlbsmhwvu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jqgufenzy.top/gtctvbbdik.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hammf.cn/gtdayyrmdy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.chenjidiqi.icu/gtdtorkcca.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ywan-chungtsiang.top/gtqjiatyhi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yuxming.cn/gtemoetfbi.html

[K05] 深拷贝对象
来源：http://hz.cheryme.top/gtbhadypah.html

Py:   copy.deepcopy(obj)
来源：http://hz.yj20258.top/gtbewuzkmi.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yuanzhike.top/gtookuutwu.html

JS:   structuredClone(obj)
来源：http://hz.yj202588.top/gtgurehzvb.html

TS:   structuredClone(obj)
来源：http://hz.aizwys.cn/gtlkdadowa.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.shanyushiyangtech.top/gtpgleacoh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.vqdsnc.cn/gtxmordvrv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shanyushiyangtech.top/gtblmagawv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.kuanghao11.cn/gtfksuhnch.html

[K06] 解析 URL 查询串
来源：http://hz.dianchejie.cn/gtbjhspfdj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.daria6918.cn/gtrkqcdroo.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.guowangkeji.top/gtfpzevgvo.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xylfe.cn/gtwfteariw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yueranfly.top/gtpoykhyaw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.nanxuanxn.top/gtfxssbbqi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zycfv.cn/gtkbzptwrd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.birdmap.top/gtiwdorbqb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.tian-w.cn/gtfrpculhc.html

[K07] 进制转换
来源：http://hz.sufxvd.cn/gtdpjoweys.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.chenjidiqi.icu/gtuzxsrggb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.dianchejie.cn/gtzejplyol.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.havefunace.top/gtcuwvwekm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.havefunace.top/gtoyrqdvlg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.fzhhl.top/gtbjarwvas.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.c1oappe.top/gttmeixsui.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.wangdashe.top/gtcfitxkgu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ydzc1.top/gtmhpxxtnu.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.birdmap.top/gtkclkzcnw.html

Py:   pickle.dumps(obj)
来源：http://hz.aizwys.cn/gtrhuyffpf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.shzxlz.cn/gtfeileufl.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shanyushiyangkeji.top/gtthwfoxyq.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.kuanghao11.cn/gtevnbrtgd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.chenlongwang.top/gtltckipyd.html

Go:   encoding/gob
来源：http://hz.snrcjt.cn/gtckxsyxqq.html

Ruby: Marshal.dump(obj)
来源：http://hz.yanxiufei.cn/gttzcfahux.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.haohaochexian.top/gtnnjvobtu.html

================================================================================
来源：http://hz.bjfxy.top/gthpbbnxcn.html

L. 网络请求
来源：http://hz.cheryme.top/gtfjibizoz.html

================================================================================
来源：http://hz.tian-w.cn/gtiarqttvf.html

[L01] 发送 GET 请求
来源：http://hz.wangshuangyany.cn/gtyqajyfet.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.andypj.xyz/gtfnduqtik.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.xuanzx.com/gtyzrppyaw.html

JS:   await fetch(url)
来源：http://hz.cdnleiting.top/gtxfdnflbn.html

TS:   await fetch(url)
来源：http://hz.c1oappe.top/gtxtpfrnzf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhijiandao.cn/gtwxfbmevw.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhengqikj.top/gtqmmsxpqa.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.nwbrower.top/gtrshmbrro.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.shzxlz.cn/gtocqkuhwu.html

[L02] 发送 POST JSON
来源：http://hz.daxiang520.top/gtznjbzxnk.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hnxiangtu.top/gtnzymlnso.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.sufxvd.cn/gtfhvvdgwa.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yj20258.top/gtdduolhiv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.meibo888.top/gtfsxdymvc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.fengsongda.top/gtelijrknb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.quarkkingdee.top/gtudlqhwkh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yonumen.top/gtcjushukt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.shanyushiyangkeji.top/gttfjgmaoj.html

[L03] 设置自定义请求头
来源：http://hz.snrcjt.cn/gtzkmujmii.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hfpthk.cn/gtocsveykt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.gogol.net.cn/gtemzjkwgp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.guannengcc.top/gtwyeodhxs.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nwbrower.top/gtbeifvbid.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.tanke756.top/gtxbzdmuux.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.shangyingyoupin.top/gtalsyqtsv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.wangdashe.top/gtdfdqrmqs.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yuanzhike.top/gtzzvisufb.html

[L04] 设置超时
来源：http://hz.9152youxi.cn/gtcjpdadtr.html

Py:   requests.get(url, timeout=5)
来源：http://hz.fengsongda.top/gtukdnfkpd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.daxiang520.top/gtvwqattzn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cucudq.cn/gtvrltfmll.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.vqdsnc.cn/gtlijgnbte.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.daxiang520.top/gtdtyyjbsj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.shuidangran.top/gtmwxfkyst.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jqgfzy.top/gtgprfrhbm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ppjwa.cn/gtmcjfcdik.html

[L05] 上传文件（multipart）
来源：http://hz.kuanghao11.cn/gtjblfxjmz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhixingplan.top/gtooeopqzw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhaomingkeji.xyz/gtwtkprsqr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.fengsongda.top/gtirahuazs.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.sysykeji.top/gtuuvizzij.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.cdnleiting.top/gtoqxibuwu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.sxryk.cn/gtroykorpf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.tian-w.cn/gtttwhlsvs.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.havefunace.top/gtgqhaolkz.html

[L06] 解析响应为 JSON
来源：http://hz.kuanghao11.cn/gthfbmwdmv.html

Py:   resp.json()
来源：http://hz.chenjidiqi.icu/gtiqmjfjko.html

PHP:  json_decode($body, true);
来源：http://hz.fengsongda.top/gtcelaxmex.html

JS:   await resp.json()
来源：http://hz.nanxinkj.top/gtkprmtgev.html

TS:   await resp.json()
来源：http://hz.gaohongyu789.top/gtuwymtdag.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.pycfn.com/gtbibfhtex.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.cqqwz.cn/gtwvnnhjqt.html

Ruby: JSON.parse(resp.body)
来源：http://hz.chenjidiqi.icu/gtfqemtfgw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.sxryk.cn/gtfxyousvp.html

[L07] 处理 HTTP 状态码
来源：http://hz.hnxiangtu.top/gtixgzrhra.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.chenzaomai.com/gtayajqgag.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.9152youxi.cn/gtqsonwxmx.html

JS:   resp.ok;  resp.status
来源：http://hz.pengpengdd.cyou/gtjwdrpcbp.html

TS:   resp.ok;  resp.status
来源：http://hz.birdmap.top/gtuiklzlpo.html

Java: resp.statusCode()
来源：http://hz.zhijiandao.cn/gtvjiuqneo.html

Go:   resp.StatusCode
来源：http://hz.xuanzx.com/gtvgstscvz.html

Ruby: resp.code.to_i
来源：http://hz.9152youxi.cn/gtvijrsxso.html

C#:   (int)resp.StatusCode
来源：http://hz.jqgufenzy.top/gtuiqqphtg.html

[L08] 并发请求多个地址
来源：http://hz.xuetiantiany.cn/gtkelvdyxh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ehwqpu.com/gttjvnyouw.html

PHP:  curl_multi_init() 系列
来源：http://hz.jianghu66.top/gtyaqxbacc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinqigufen.top/gtwfouepkk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.pycfn.com/gtgevugvub.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.sufxvd.cn/gtydamaxtn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.andypj.xyz/gtofozskdl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ywan-chungtsiang.top/gtppioqopk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.shzxlz.cn/gtnuvymcmy.html

================================================================================
来源：http://hz.hfpthk.cn/gtvqwcxrjm.html

M. 命令行 / 进程 / 环境
来源：http://hz.cashguo.top/gtccddnlam.html

================================================================================
来源：http://hz.xziqi.cn/gtmehpikxf.html

[M01] 读取命令行参数
来源：http://hz.sxryk.cn/gtxrsylptc.html

Py:   sys.argv[1:]
来源：http://hz.gaohongyu789.top/gtastayxsp.html

PHP:  $argv;  $argc;
来源：http://hz.xingfuxueyuan.xyz/gtsnjcruqe.html

JS:   process.argv.slice(2)
来源：http://hz.hammf.cn/gtqxdiovsy.html

TS:   process.argv.slice(2)
来源：http://hz.shzxlz.cn/gtxbvxixaz.html

Java: args 数组（main 方法参数）
来源：http://hz.jinqigfzy.top/gtzecgunuq.html

Go:   os.Args[1:]
来源：http://hz.ppjwa.cn/gtbhnipaim.html

Ruby: ARGV
来源：http://hz.zhixingplan.top/gtiavpdwuu.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hysaishi.cn/gtqfzkmxbh.html

[M02] 读取环境变量
来源：http://hz.wangshuangyany.cn/gtbtuappji.html

Py:   os.environ.get("HOME")
来源：http://hz.dianchejie.cn/gtzcteoskx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zycfv.cn/gtkafagvmo.html

JS:   process.env.HOME
来源：http://hz.gzhubu.top/gtjqgiytie.html

TS:   process.env.HOME
来源：http://hz.hnxiangtu.top/gtetsegyms.html

Java: System.getenv("HOME")
来源：http://hz.52xcode.cn/gtmlxcxjgh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.daria6918.cn/gtbvgmfzze.html

Ruby: ENV["HOME"]
来源：http://hz.zhiwuduotai.top/gtukbmrfwx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.gotoacloud.top/gtwykevbne.html

[M03] 执行外部命令
来源：http://hz.cashguo.top/gtpaqcoesd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yvedp.cn/gtzxznvnqi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhengqikj.top/gtcuasuflo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.sysykeji.top/gtmgmmnoev.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.gogol.net.cn/gtyxmpnduk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.cqqwz.cn/gtmbfvgzce.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hongshengwenyu.top/gtlsxaiilo.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.ydjk.org.cn/gtmsaigzrr.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xinyue.icu/gtgzepzfyq.html

[M04] 获取当前工作目录
来源：http://hz.snrcjt.cn/gtxfhswsvn.html

Py:   os.getcwd()
来源：http://hz.zhiwuduotai.top/gtzoboinya.html

PHP:  getcwd();
来源：http://hz.jlsjyb.cn/gtsyiwbnkz.html

JS:   process.cwd()
来源：http://hz.yanxiufei.cn/gtymkidkqf.html

TS:   process.cwd()
来源：http://hz.shanyushiyangtech.top/gtfdikhkhk.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.shanyushiyangkeji.top/gtmdzwhnhn.html

Go:   os.Getwd()
来源：http://hz.nanxuanxn.top/gtekatwtmn.html

Ruby: Dir.pwd
来源：http://hz.zhijiandao.cn/gtrxttwykt.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhongyouzk.top/gtlnfdabyy.html

[M05] 设置退出码
来源：http://hz.gaohongyu789.top/gtujsiajhc.html

Py:   sys.exit(1)
来源：http://hz.sweek.top/gtkrareeol.html

PHP:  exit(1);
来源：http://hz.yangfankeji.com/gtbcawvyjh.html

JS:   process.exit(1)
来源：http://hz.hongshengwenyu.top/gtcwhuzuyr.html

TS:   process.exit(1)
来源：http://hz.nanxinkj.top/gtypxhmmse.html

Java: System.exit(1)
来源：http://hz.zhongyouzk.top/gtlusxvrsb.html

Go:   os.Exit(1)
来源：http://hz.pycfn.com/gtfdsxafgs.html

Ruby: exit 1
来源：http://hz.hammf.cn/gtfbfdyvfy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.fengsongda.top/gtfrhapwte.html

[M06] 向标准错误输出
来源：http://hz.dianchejie.cn/gtsebanrjs.html

Py:   print("err", file=sys.stderr)
来源：http://hz.aibaodan.cn/gtzoxudmkk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hysaishi.cn/gtchpnzyao.html

JS:   console.error("err")
来源：http://hz.shangyingyoupin.top/gteprydzhe.html

TS:   console.error("err")
来源：http://hz.52xcode.cn/gtcxoxcjdu.html

Java: System.err.println("err")
来源：http://hz.yongpay.top/gtzblhbzed.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.cqqwz.cn/gtniosylwf.html

Ruby: warn "err"
来源：http://hz.xylfe.cn/gtkkxbpfdb.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.dashuyun.cn/gtaohfjufz.html

[M07] 判断是否为主入口
来源：http://hz.hammf.cn/gtcekadvrt.html

Py:   if __name__ == "__main__":
来源：http://hz.yvedp.cn/gtbzsbdtmu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cdnleiting.top/gtnqlltpgp.html

JS:   require.main === module
来源：http://hz.shanyushiyangkeji.top/gtdgixlxlc.html

TS:   require.main === module
来源：http://hz.sweek.top/gtvycoiaim.html

Java: public static void main(String[] args)
来源：http://hz.cheryme.top/gtfwwixpkr.html

Go:   func main()
来源：http://hz.c1oappe.top/gtfqtxuyec.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.nanxuanxn.top/gtepjkrnzc.html

C#:   static void Main(string[] args)
来源：http://hz.shanyushiyangkeji.top/gtohsnisln.html

[M08] 获取系统与运行时信息
来源：http://hz.sxryk.cn/gtkbamaxba.html

Py:   platform.system();  platform.python_version()
来源：http://hz.shanyushiyangkeji.top/gtaenjmqlv.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.shangyingyoupin.top/gtpyqxhkxe.html

JS:   process.platform;  process.version
来源：http://hz.birdmap.top/gtztcxkakm.html

TS:   process.platform;  process.version
来源：http://hz.gotoacloud.top/gtjmnqdxyf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.feifeiyinyue.top/gtxtilaauh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.cucudq.cn/gtigamuqof.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yueranfly.top/gtfozifohk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.52xcode.cn/gthxhmzwnq.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtstabyimt.html

N. 数据结构与算法
来源：http://hz.c1oappe.top/gtafyyzbyr.html

================================================================================
来源：http://hz.xinyue.icu/gtjkzmeeet.html

[N01] 二分查找（有序数组）
来源：http://hz.cqqwz.cn/gtmcxzzcrj.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.cqqwz.cn/gtaavrzscl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.shanyushiyangkeji.top/gtpgqzdpnq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.c1oappe.top/gtbvixhhre.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.0kj1m.cn/gtpuwibtrd.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zycfv.cn/gtmgbgiwtn.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jianghu66.top/gthwxdzjcl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yonumen.top/gtydyzizba.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.svipenyu.cn/gtgixpmwse.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yongpay.top/gtpqdsnskh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xuanzx.com/gtwodafrmv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.guowangkeji.top/gtobzdhcax.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xuanzx.com/gtdldmxljm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shangyingyoupin.top/gtswaxqvnf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.pengpengdd.cyou/gtqzjlzizs.html

Go:   slices.Sort(arr)
来源：http://hz.zhiwuduotai.top/gthhcifyqp.html

Ruby: arr.sort
来源：http://hz.zhongyouzk.top/gtsowgfbhc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.iojbl.cn/gtmlpjhhft.html

[N03] 快速排序（分治示例）
来源：http://hz.daxiang520.top/gtgmpwkawr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.316326.xyz/gtuuzsxwxr.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jlsjyb.cn/gtchfvaihz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.sweek.top/gthoqlpeng.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yj20258.top/gtiqhfjxle.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zycfv.cn/gtxlbwbwve.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.havefunace.top/gtcuupxlyj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhoulong.xyz/gtuhddjikd.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jinghuilouyu.cn/gtevlswoke.html

[N04] 斐波那契数列
来源：http://hz.sufxvd.cn/gtqrcvfkjt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.dashuyun.cn/gtduuynhrd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.kuanghao11.cn/gtseujqhpa.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yangfankeji.com/gtkylwwyvw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.dianchejie.cn/gtcxhgpysi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.cucudq.cn/gtzqawhleb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.nanxuanxn.top/gtghdsgrwk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhongyouzk.top/gtelqjcpdm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhongyouzk.top/gtzlbetlmz.html

[N05] 最大公约数
来源：http://hz.jinqigufen.top/gtnetftgkg.html

Py:   math.gcd(a, b)
来源：http://hz.zhaomingkeji.xyz/gtrdvsmqwo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.9152youxi.cn/gtavhokukh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.tianlin.xyz/gtozyegxiz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.nwbrower.top/gtmiijjxak.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.0kj1m.cn/gtbnlzsktb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.sxryk.cn/gtcbxlfnjh.html

Ruby: a.gcd(b)
来源：http://hz.0kj1m.cn/gtpnsmfxpk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.guowangkeji.top/gtwrrnhpgl.html

[N06] 判断回文字符串
来源：http://hz.ydjk.org.cn/gtqheurtbl.html

Py:   s == s[::-1]
来源：http://hz.sxryk.cn/gtyzdlrnep.html

PHP:  $s === strrev($s);
来源：http://hz.hnqzz.top/gtankgfhnk.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhijiandao.cn/gtcoobfpfg.html

TS:   s === [...s].reverse().join("")
来源：http://hz.gzhubu.top/gtgkhowhuu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ydjk.org.cn/gtxhwwbjva.html

Go:   // 双指针从两端比较
来源：http://hz.cqqwz.cn/gtjuzfbvpi.html

Ruby: s == s.reverse
来源：http://hz.hfpthk.cn/gticsyylrt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.shanyushiyangtech.top/gtinqqsbwn.html

[N07] 两数之和（返回下标）
来源：http://hz.cdnleiting.top/gtpneowqwz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.chenlongwang.top/gtpgfvucwb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.mhx1999.top/gtnnjeoutp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xuetiantiany.cn/gtpwtzupbh.html

TS:   // 手写 Map<string, number>
来源：http://hz.chenjidiqi.icu/gtvfyizaoy.html

Java: // 手写 HashMap
来源：http://hz.tian-w.cn/gtifwrcwmv.html

Go:   // 手写 map[int]int
来源：http://hz.jqgufenzy.top/gtvtwmlvqa.html

Ruby: // 手写 Hash
来源：http://hz.yangfankeji.com/gtelfyclzq.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.smart0.xyz/gtmsxmeoom.html

[N08] 生成全排列
来源：http://hz.iojbl.cn/gttisryesx.html


<!-- 参考信息 -->