代发 wailian999

================================================================================
来源：http://hz.316326.xyz/gtplqbhcsu.html

K. JSON 与序列化
来源：http://hz.jinghuilouyu.cn/gtvjarsbzu.html

================================================================================
来源：http://hz.yonumen.top/gtlwktvqup.html

[K01] 对象转 JSON 字符串
来源：http://hz.tanke756.top/gtdtbpbwvd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.52xcode.cn/gtvfrseowq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jiagoushi.top/gtibpbvksx.html

JS:   JSON.stringify(obj)
来源：http://hz.pycfn.com/gtfsehhfkp.html

TS:   JSON.stringify(obj)
来源：http://hz.gogol.net.cn/gtkaffigex.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.c1oappe.top/gtlgegjtxe.html

Go:   json.Marshal(obj)
来源：http://hz.jianghu66.top/gtmesyxswy.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hongshengwenyu.top/gthlyarxmr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.wangshuangyany.cn/gtswmsycjx.html

[K02] JSON 字符串转对象
来源：http://hz.shanyushiyangtech.top/gtscmksoiz.html

Py:   json.loads(s)
来源：http://hz.hongshengwenyu.top/gtkztsoykc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jinghuilouyu.cn/gtqcjjyapj.html

JS:   JSON.parse(s)
来源：http://hz.0kj1m.cn/gtjtzzslym.html

TS:   JSON.parse(s)
来源：http://hz.jyoumei.cn/gtfiuwwpun.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hammf.cn/gtziilwjli.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.svipenyu.cn/gthtmfmojq.html

Ruby: JSON.parse(s)
来源：http://hz.zhaomingkeji.xyz/gtyibfxmqc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.andypj.xyz/gtyvkfiicl.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.chenzaomai.com/gtekxjozhm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.cheryme.top/gthfmnfqas.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.316326.xyz/gtqeqhuahb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.aizwys.cn/gtehfdgqhv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.gzhubu.top/gtqigsyqul.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yueranfly.top/gtdiscldmt.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhengqikj.top/gtpmmudmda.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.kuanghao11.cn/gtzthuqukv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.fengsongda.top/gtfpflmymj.html

[K04] 读取 JSON 文件
来源：http://hz.yj20258888.top/gtycanqzeh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yanxiufei.cn/gtftuqxotq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.nwbrower.top/gtsqkwcdqa.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yueranfly.top/gtynalhkjb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhoulong.xyz/gtbcmpzkvk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.shzxlz.cn/gtaotfqjwj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jinyuanbaomall.cn/gtzjlunyix.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.dianchejie.cn/gtlleskohp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ydzc1.top/gtdsqmpxpy.html

[K05] 深拷贝对象
来源：http://hz.ywan-chungtsiang.top/gticqnpyer.html

Py:   copy.deepcopy(obj)
来源：http://hz.haohaochexian.top/gtmzhjjmbk.html

PHP:  unserialize(serialize($obj));
来源：http://hz.gaohongyu789.top/gtggaazpfx.html

JS:   structuredClone(obj)
来源：http://hz.dashuyun.cn/gtxoaqolbi.html

TS:   structuredClone(obj)
来源：http://hz.guowangkeji.top/gtbfzaxeyo.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.guowangkeji.top/gtqwcslmws.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.sweek.top/gtjidmjbip.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hongshengwenyu.top/gtwujjmcoc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhongyouzk.top/gtwtduuhti.html

[K06] 解析 URL 查询串
来源：http://hz.9152youxi.cn/gtduiofdlw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhixingplan.top/gtqlihzfzx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.ywan-chungtsiang.top/gtxejtfqly.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xuanzx.com/gtyyjmrbnv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cdnleiting.top/gtjajibbif.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.bjfxy.top/gtfnjnkvjx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.xuetiantiany.cn/gtcxgrzvfm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.shanyushiyangtech.top/gtkeetnxtb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ybcxt.top/gtqizvvznp.html

[K07] 进制转换
来源：http://hz.jianghu66.top/gtgnwtacvb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cucudq.cn/gtfvokzlqs.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.svipenyu.cn/gtauotbcbn.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.iojbl.cn/gtjrfuhnpi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.chenjidiqi.icu/gtxlmstdlj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xingfuxueyuan.xyz/gtcsyzuwhj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jqgfzy.top/gttuhlqsoo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.wangdashe.top/gtnsqyifbm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.iojbl.cn/gtbjahlasm.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jqgfzy.top/gtjgbmvujt.html

Py:   pickle.dumps(obj)
来源：http://hz.smart0.xyz/gtoaniwfhk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yongpay.top/gtixlwxhba.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhongyouzk.top/gthcnnedfy.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhengqikj.top/gtuoioefew.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hfpthk.cn/gtnioptenv.html

Go:   encoding/gob
来源：http://hz.sxryk.cn/gtkzseteeu.html

Ruby: Marshal.dump(obj)
来源：http://hz.hammf.cn/gtuwokuxcz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.cashguo.top/gtxmeqyxfi.html

================================================================================
来源：http://hz.gaohongyu789.top/gtfseimpaf.html

L. 网络请求
来源：http://hz.jqgufenzy.top/gtbbigfdqr.html

================================================================================
来源：http://hz.jlsjyb.cn/gtgrrnjyxh.html

[L01] 发送 GET 请求
来源：http://hz.zdqjudy.top/gtpezimcft.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.shangyingyoupin.top/gttwhmtmqa.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.havefunace.top/gtjvjwdbnx.html

JS:   await fetch(url)
来源：http://hz.zhiwuduotai.top/gthgmbvioz.html

TS:   await fetch(url)
来源：http://hz.gaohongyu789.top/gtifcugiiu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.xuanzx.com/gtpzrcrzid.html

Go:   resp, err := http.Get(url)
来源：http://hz.gotoacloud.top/gtfxyvwahk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.sysykeji.top/gtmehtffud.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ybcxt.top/gtiuxrispc.html

[L02] 发送 POST JSON
来源：http://hz.shanyushiyangkeji.top/gttjjzecxs.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.daria6918.cn/gtcplxrnvo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hammf.cn/gtjoivhioj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.meibo888.top/gtsdcuhwoo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinghuilouyu.cn/gtnazpwmuk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.pengpengdd.cyou/gtnyidcbrw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ehwqpu.com/gtgucoovsj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.chenlongwang.top/gtjwuuzazk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yonumen.top/gtunctpfjr.html

[L03] 设置自定义请求头
来源：http://hz.fengsongda.top/gtjvdqbntz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xziqi.cn/gtypqzpfci.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zycfv.cn/gtpxghmplk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gaohongyu789.top/gtoxqvoghx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.havefunace.top/gtickyxmgr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.wangdashe.top/gtqlfkgcmc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.fengsongda.top/gtviydwpvl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.tian-w.cn/gtytsnvlvl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.shangyingyoupin.top/gttnvnjotj.html

[L04] 设置超时
来源：http://hz.hongshengwenyu.top/gtivromqqu.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jinyuanbaomall.cn/gtnikoawtb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.havefunace.top/gtlydjommd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ybcxt.top/gtekaoyfww.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.tanke756.top/gtjmvsbzlx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hysaishi.cn/gtqnhwcfyi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jinyuanbaomall.cn/gthydxumpm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.c1oappe.top/gtidzpsfzx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.dashuyun.cn/gthhwiiies.html

[L05] 上传文件（multipart）
来源：http://hz.meibo888.top/gtklmnyajj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.meibo888.top/gtwsqhxlqx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.birdmap.top/gtycaxchnh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jyoumei.cn/gtyixdqppa.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinghuilouyu.cn/gtohpksjnf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.fengsongda.top/gtnlbcvuur.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jianghu66.top/gtsbtytbvx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.gogol.net.cn/gtkhvjwsbi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hongshengwenyu.top/gtmxfpiemp.html

[L06] 解析响应为 JSON
来源：http://hz.gaohongyu789.top/gtwtnfsvcs.html

Py:   resp.json()
来源：http://hz.gogol.net.cn/gtuakcekbo.html

PHP:  json_decode($body, true);
来源：http://hz.yuxming.cn/gtsmxyqvnr.html

JS:   await resp.json()
来源：http://hz.zhijiandao.cn/gtdyvckigg.html

TS:   await resp.json()
来源：http://hz.c1oappe.top/gtjthbmdte.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.vqdsnc.cn/gthribiliw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zhaomingkeji.xyz/gtasxukgdc.html

Ruby: JSON.parse(resp.body)
来源：http://hz.cdnleiting.top/gtiwfidulh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ydjk.org.cn/gtjdjqzqfw.html

[L07] 处理 HTTP 状态码
来源：http://hz.52xcode.cn/gtuvrhidgu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.sweek.top/gtmqalrvdu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.0kj1m.cn/gtgiwmvikj.html

JS:   resp.ok;  resp.status
来源：http://hz.ydzc1.top/gtantamypd.html

TS:   resp.ok;  resp.status
来源：http://hz.cucudq.cn/gtvsshyani.html

Java: resp.statusCode()
来源：http://hz.aibaodan.cn/gtrskwxbhq.html

Go:   resp.StatusCode
来源：http://hz.yueranfly.top/gtxktwracs.html

Ruby: resp.code.to_i
来源：http://hz.svipenyu.cn/gtvfdwjhfu.html

C#:   (int)resp.StatusCode
来源：http://hz.quarkkingdee.top/gtovqpdsdx.html

[L08] 并发请求多个地址
来源：http://hz.ivvv.top/gtqoxhxmzm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.vqdsnc.cn/gtvalmbdik.html

PHP:  curl_multi_init() 系列
来源：http://hz.gzhubu.top/gtyxzzyjan.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.feifeiyinyue.top/gtjgqzcigt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cashguo.top/gtpbmldlut.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.feifeiyinyue.top/gtqaicidxv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.shangyingyoupin.top/gtwlvkxzuc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ivvv.top/gtwetgvgag.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zdqjudy.top/gtexijqavs.html

================================================================================
来源：http://hz.guowangkeji.top/gtcfejzytq.html

M. 命令行 / 进程 / 环境
来源：http://hz.dashuyun.cn/gtwrodxnvs.html

================================================================================
来源：http://hz.52xcode.cn/gtdphnfars.html

[M01] 读取命令行参数
来源：http://hz.meibo888.top/gtngvxuida.html

Py:   sys.argv[1:]
来源：http://hz.zhongyouzk.top/gtogpnjejs.html

PHP:  $argv;  $argc;
来源：http://hz.quarkkingdee.top/gturmfgjew.html

JS:   process.argv.slice(2)
来源：http://hz.jlsjyb.cn/gtaavhfjzg.html

TS:   process.argv.slice(2)
来源：http://hz.yanxiufei.cn/gtlhhlvoug.html

Java: args 数组（main 方法参数）
来源：http://hz.wangdashe.top/gtpafwxzmt.html

Go:   os.Args[1:]
来源：http://hz.jlsjyb.cn/gtmlcipzfm.html

Ruby: ARGV
来源：http://hz.nanxuanxn.top/gtgdgsdbjy.html

C#:   args 数组（Main 方法参数）
来源：http://hz.shangyingyoupin.top/gtoiohnjwr.html

[M02] 读取环境变量
来源：http://hz.zhoulong.xyz/gtefndbyqg.html

Py:   os.environ.get("HOME")
来源：http://hz.sxryk.cn/gtnzqirqhn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.sweek.top/gtslsiqbmy.html

JS:   process.env.HOME
来源：http://hz.jinghuilouyu.cn/gtnnpabfxi.html

TS:   process.env.HOME
来源：http://hz.jianghu66.top/gtgevmyypt.html

Java: System.getenv("HOME")
来源：http://hz.nanxuanxn.top/gtuyautsjz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hysaishi.cn/gtshjortpq.html

Ruby: ENV["HOME"]
来源：http://hz.ywan-chungtsiang.top/gtrcgepjcv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yuanzhike.top/gtzrgposha.html

[M03] 执行外部命令
来源：http://hz.havefunace.top/gtzctexfky.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhoulong.xyz/gtrjrvzdba.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.c1oappe.top/gtexxjntcp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhaomingkeji.xyz/gttwmpecgx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhiwuduotai.top/gthaamujcp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.birdmap.top/gtixkjscin.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.daxiang520.top/gtuvancnmm.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.chenlongwang.top/gtfzmqkryq.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hnxiangtu.top/gtchwfoczz.html

[M04] 获取当前工作目录
来源：http://hz.jqgfzy.top/gtcyxnryrh.html

Py:   os.getcwd()
来源：http://hz.andypj.xyz/gtssfxmjqn.html

PHP:  getcwd();
来源：http://hz.hywenlv.cn/gtzytekhxc.html

JS:   process.cwd()
来源：http://hz.yj20258888.top/gtpilabawl.html

TS:   process.cwd()
来源：http://hz.jinghuilouyu.cn/gtgbylxmak.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.bjfxy.top/gtdtmcvjwk.html

Go:   os.Getwd()
来源：http://hz.wangshuangyany.cn/gtzckwtgju.html

Ruby: Dir.pwd
来源：http://hz.chenjidiqi.icu/gtuhkzzprx.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yj20258888.top/gtpnokyqrj.html

[M05] 设置退出码
来源：http://hz.yj20258.top/gtsgihszeh.html

Py:   sys.exit(1)
来源：http://hz.hnxiangtu.top/gtmyunfwrv.html

PHP:  exit(1);
来源：http://hz.yanxiufei.cn/gtgykilohp.html

JS:   process.exit(1)
来源：http://hz.jinghuilouyu.cn/gtssvsbfmv.html

TS:   process.exit(1)
来源：http://hz.ehwqpu.com/gtowrogntc.html

Java: System.exit(1)
来源：http://hz.shzxlz.cn/gtqvgmpixi.html

Go:   os.Exit(1)
来源：http://hz.ivvv.top/gtyebuisel.html

Ruby: exit 1
来源：http://hz.aibaodan.cn/gtprxvtlow.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.vqdsnc.cn/gtwubygyjl.html

[M06] 向标准错误输出
来源：http://hz.ehwqpu.com/gtshjetqlz.html

Py:   print("err", file=sys.stderr)
来源：http://hz.52xcode.cn/gtrhuodyon.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ydzc1.top/gtahgtlyus.html

JS:   console.error("err")
来源：http://hz.zhijiandao.cn/gtrhkmvyqr.html

TS:   console.error("err")
来源：http://hz.aibaodan.cn/gtwvzugvzj.html

Java: System.err.println("err")
来源：http://hz.xylfe.cn/gtinpbeprf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xuetiantiany.cn/gtjpxhfjmu.html

Ruby: warn "err"
来源：http://hz.hywenlv.cn/gtiztuslch.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yj202588.top/gtvqssemai.html

[M07] 判断是否为主入口
来源：http://hz.chenlongwang.top/gtvqbfrjox.html

Py:   if __name__ == "__main__":
来源：http://hz.tianlin.xyz/gtaaydlcaa.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhengqikj.top/gtdyoyryki.html

JS:   require.main === module
来源：http://hz.havefunace.top/gtgfafkhsy.html

TS:   require.main === module
来源：http://hz.birdmap.top/gtmbrqhxdx.html

Java: public static void main(String[] args)
来源：http://hz.fzhhl.top/gtholuvkdd.html

Go:   func main()
来源：http://hz.snrcjt.cn/gtzaevjsxz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jinqigufen.top/gtggxmdecg.html

C#:   static void Main(string[] args)
来源：http://hz.ywan-chungtsiang.top/gteqvufgaa.html

[M08] 获取系统与运行时信息
来源：http://hz.redwolf501.top/gtvvbpxcez.html

Py:   platform.system();  platform.python_version()
来源：http://hz.wangshuangyany.cn/gtvnkbkkrt.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.fengsongda.top/gtjfjrysgn.html

JS:   process.platform;  process.version
来源：http://hz.snrcjt.cn/gtcgunqocm.html

TS:   process.platform;  process.version
来源：http://hz.shangyingyoupin.top/gtamjqrmhg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yongpay.top/gtdmzqyvdg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.nwbrower.top/gtoieheefe.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.nwbrower.top/gtkenwpjsu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.havefunace.top/gtdkjzbbvz.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtrhvuqjef.html

N. 数据结构与算法
来源：http://hz.guowangkeji.top/gtocxcmrkv.html

================================================================================
来源：http://hz.yonumen.top/gtemzdiqde.html

[N01] 二分查找（有序数组）
来源：http://hz.yj20258888.top/gtznailzsf.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jinyuanbaomall.cn/gtwluuuhro.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.mhx1999.top/gtmvaxjgbf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cashguo.top/gtajfjiede.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shzxlz.cn/gtjnhwyfkg.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.shangyingyoupin.top/gtdsugziue.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.fzhhl.top/gtcbklyhua.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.shanyushiyangtech.top/gtpgzesvda.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yj20258.top/gthnehdchd.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.vqdsnc.cn/gtquyzantv.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hywenlv.cn/gtgmorfczy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.sxryk.cn/gtoykqixqn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gotoacloud.top/gtkutvhciv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ehwqpu.com/gtngqqlife.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.fengsongda.top/gtvvseftxp.html

Go:   slices.Sort(arr)
来源：http://hz.xinyue.icu/gtpmimofcp.html

Ruby: arr.sort
来源：http://hz.zhoulong.xyz/gtlbxpebqm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ydjk.org.cn/gtenxezgux.html

[N03] 快速排序（分治示例）
来源：http://hz.zhoulong.xyz/gtncirwjpo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.fengsongda.top/gtdxjfmlsm.html

PHP:  // 递归实现，或用 usort
来源：http://hz.aizwys.cn/gtdgavypne.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.dianchejie.cn/gtjyiavheu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ivvv.top/gthjjskwmy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinghuilouyu.cn/gtxynwnfal.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.wangshuangyany.cn/gtlriqdljr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.dianchejie.cn/gtekqpgsrm.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.tianlin.xyz/gtsszqmcyo.html

[N04] 斐波那契数列
来源：http://hz.hongshengwenyu.top/gtxobavnuz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.gotoacloud.top/gtalfbdwzm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.gotoacloud.top/gtbmslsyda.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cashguo.top/gtntfnusmw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.c1oappe.top/gtaueyucaj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jiagoushi.top/gtpsfkixli.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.sysykeji.top/gtlkwexnnn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.guannengcc.top/gtbxokstxa.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.tianlin.xyz/gtodjwsdas.html

[N05] 最大公约数
来源：http://hz.hnxiangtu.top/gtrxibxtvy.html

Py:   math.gcd(a, b)
来源：http://hz.aizwys.cn/gtfhiklbvc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zdqjudy.top/gtoctnwbxb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cucudq.cn/gtfavbycrs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.chenzaomai.com/gtlarvzylg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ywan-chungtsiang.top/gtckzhswod.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.haohaochexian.top/gtrejoryyw.html

Ruby: a.gcd(b)
来源：http://hz.hongshengwenyu.top/gtihvdgeoy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.shuidangran.top/gtmfioqwma.html

[N06] 判断回文字符串
来源：http://hz.zhaomingkeji.xyz/gttuzwfzkc.html

Py:   s == s[::-1]
来源：http://hz.chenzaomai.com/gtrrhbvgzp.html

PHP:  $s === strrev($s);
来源：http://hz.wangshuangyany.cn/gtpnhqnoyw.html

JS:   s === [...s].reverse().join("")
来源：http://hz.chenzaomai.com/gtfninjxbj.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jyoumei.cn/gtwchrhxva.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.shangyingyoupin.top/gtdmtzypsm.html

Go:   // 双指针从两端比较
来源：http://hz.birdmap.top/gtytawwgkl.html

Ruby: s == s.reverse
来源：http://hz.hongshengwenyu.top/gtintsmntz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.wangdashe.top/gtvkfsmkvo.html

[N07] 两数之和（返回下标）
来源：http://hz.yj20258888.top/gtvhaceqza.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.nanxinkj.top/gthypyqhnu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jiagoushi.top/gtjrutvmfn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.iojbl.cn/gtshkyatgl.html

TS:   // 手写 Map<string, number>
来源：http://hz.hnqzz.top/gtmipfgoqz.html

Java: // 手写 HashMap
来源：http://hz.yuxming.cn/gthhylnfwc.html

Go:   // 手写 map[int]int
来源：http://hz.ehwqpu.com/gtqjzgxrpr.html

Ruby: // 手写 Hash
来源：http://hz.kuanghao11.cn/gtemmnxvcm.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.chenjidiqi.icu/gtjhbzmvza.html

[N08] 生成全排列
来源：http://hz.yonumen.top/gtjgxjhvtt.html

Py:   itertools.permutations(arr)
来源：http://hz.sxryk.cn/gtqklsgivy.html

PHP:  // 手写递归交换
来源：http://hz.nanxuanxn.top/gtshrlgpwv.html

JS:   // 手写回溯递归
来源：http://hz.shuidangran.top/gtywhfxpfe.html

TS:   // 手写回溯递归
来源：http://hz.yangfankeji.com/gtwnwwtyop.html

Java: // 手写回溯递归
来源：http://hz.yj20258.top/gtsmakfbmx.html

Go:   // 手写回溯递归
来源：http://hz.daria6918.cn/gtqyoqlqiv.html

Ruby: arr.permutation.to_a
来源：http://hz.jinqigfzy.top/gtnzntclco.html

C#:   // 手写回溯递归
来源：http://hz.52xcode.cn/gteoslvfkb.html


<!-- 参考信息 -->