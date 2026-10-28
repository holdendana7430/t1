代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.redwolf501.top/gtwutsgqtl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.mhx1999.top/gtvhryqzem.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jiagoushi.top/gtxopliubn.html

[K05] 深拷贝对象
来源：http://hz.hnqzz.top/gtkjfkryqf.html

Py:   copy.deepcopy(obj)
来源：http://hz.meibo888.top/gtvanllacq.html

PHP:  unserialize(serialize($obj));
来源：http://hz.aibaodan.cn/gtbvgeyerp.html

JS:   structuredClone(obj)
来源：http://hz.zhaomingkeji.xyz/gtztyvvhaj.html

TS:   structuredClone(obj)
来源：http://hz.bjfxy.top/gtlbsbetxl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.shanyushiyangtech.top/gtjkofgwac.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hysaishi.cn/gteqqlmysm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.guannengcc.top/gtuhgfplee.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yanxiufei.cn/gtjmqbvjqz.html

[K06] 解析 URL 查询串
来源：http://hz.fengsongda.top/gtlsdiqgdv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.bjfxy.top/gtxjqghfks.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.smart0.xyz/gtkfcjrwtw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xziqi.cn/gtvovthven.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.iojbl.cn/gtmhvfssac.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.bjfxy.top/gtwvpmzagj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yueranfly.top/gtmfiyieri.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.pycfn.com/gtntbqcbjw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.svipenyu.cn/gtepwzfnjn.html

[K07] 进制转换
来源：http://hz.chenlongwang.top/gtaajpbpvt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.9152youxi.cn/gtdogynlqf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.haohaochexian.top/gtqwnjpuiq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.daria6918.cn/gtrorbswla.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yj202588.top/gtrpuxolqw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.shanyushiyangkeji.top/gtwusvpkwq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhengqikj.top/gtfgvzyokl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.tanke756.top/gtheebhrad.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhixingplan.top/gtuarcrgqf.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhaomingkeji.xyz/gtgvtuavpk.html

Py:   pickle.dumps(obj)
来源：http://hz.0kj1m.cn/gtapjypbpj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hysaishi.cn/gtyagwubrw.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhongyouzk.top/gtuepllzze.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ivvv.top/gtvbysftlr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ywan-chungtsiang.top/gtwxnhdgqy.html

Go:   encoding/gob
来源：http://hz.vqdsnc.cn/gteutmrzra.html

Ruby: Marshal.dump(obj)
来源：http://hz.haohaochexian.top/gtbwaoadnk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yuxming.cn/gtwoftzcuz.html

================================================================================
来源：http://hz.dianchejie.cn/gtjezmhaav.html

L. 网络请求
来源：http://hz.ivvv.top/gtirezplmi.html

================================================================================
来源：http://hz.hfpthk.cn/gtpdusxvip.html

[L01] 发送 GET 请求
来源：http://hz.andypj.xyz/gtbpvfwfdt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.gogol.net.cn/gtnmypyfmp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhoulong.xyz/gtbyeaznwe.html

JS:   await fetch(url)
来源：http://hz.wangshuangyany.cn/gtetzqvhby.html

TS:   await fetch(url)
来源：http://hz.xziqi.cn/gthftxalms.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ybcxt.top/gtrdwmbxbg.html

Go:   resp, err := http.Get(url)
来源：http://hz.yuanzhike.top/gtknlmksii.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yanxiufei.cn/gthkmggche.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.sweek.top/gtzhktcymr.html

[L02] 发送 POST JSON
来源：http://hz.cashguo.top/gtpbaixmfr.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hywenlv.cn/gtkvvespgq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.shzxlz.cn/gtpmcdiuqf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xylfe.cn/gttmqmcfrv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.0kj1m.cn/gtattapkoo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.chenjidiqi.icu/gtbbtcdixo.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.tanke756.top/gtgnvpxmuy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhiwuduotai.top/gtrczuazbn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.smart0.xyz/gtatcqustk.html

[L03] 设置自定义请求头
来源：http://hz.zhengqikj.top/gttrdtubgk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.chenjidiqi.icu/gtzyxsgecx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.cucudq.cn/gtzazaqyrv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nanxuanxn.top/gtlbukvthz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ivvv.top/gtyhjydaqj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhengqikj.top/gtlpepfuao.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.tanke756.top/gtisoxlpyx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.cqqwz.cn/gtxkefpnbg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.mhx1999.top/gtvwdzmbqs.html

[L04] 设置超时
来源：http://hz.52xcode.cn/gtbywstnns.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hysaishi.cn/gtvhhhaaxf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.gogol.net.cn/gtpjsllfpp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.daxiang520.top/gtnppbbzuw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.dianchejie.cn/gtxosgxwbr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhongyouzk.top/gtgjhybsjm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zycfv.cn/gtkxypvdov.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.gogol.net.cn/gtxtygfpqq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hammf.cn/gtcojubmta.html

[L05] 上传文件（multipart）
来源：http://hz.meibo888.top/gtlsbvcllg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.havefunace.top/gtiyjonaio.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.smart0.xyz/gtbprotwhp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.kuanghao11.cn/gtjiamsihw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.fzhhl.top/gtxhkvwolb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xylfe.cn/gtcxpnfbet.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhongyouzk.top/gtdyeemlev.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.hongshengwenyu.top/gtkvsltlov.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.aibaodan.cn/gtwarrgtyr.html

[L06] 解析响应为 JSON
来源：http://hz.jyoumei.cn/gtdpdkthzr.html

Py:   resp.json()
来源：http://hz.hongshengwenyu.top/gtuiqtgdxa.html

PHP:  json_decode($body, true);
来源：http://hz.xylfe.cn/gtsicllful.html

JS:   await resp.json()
来源：http://hz.ywan-chungtsiang.top/gtpqixcdlr.html

TS:   await resp.json()
来源：http://hz.havefunace.top/gtinhkemvw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.bjfxy.top/gtaropiubi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.c1oappe.top/gttnkhfcri.html

Ruby: JSON.parse(resp.body)
来源：http://hz.gzhubu.top/gtwffftvcb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.dashuyun.cn/gtwlbpinoe.html

[L07] 处理 HTTP 状态码
来源：http://hz.yuanzhike.top/gtakjegvgv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hysaishi.cn/gtykihcnlh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yangfankeji.com/gtqzcucmyq.html

JS:   resp.ok;  resp.status
来源：http://hz.ehwqpu.com/gtliokhbli.html

TS:   resp.ok;  resp.status
来源：http://hz.nanxuanxn.top/gtsvepakst.html

Java: resp.statusCode()
来源：http://hz.gotoacloud.top/gtdtqbqmbt.html

Go:   resp.StatusCode
来源：http://hz.chenlongwang.top/gtxyvqozes.html

Ruby: resp.code.to_i
来源：http://hz.quarkkingdee.top/gtnntaoqeu.html

C#:   (int)resp.StatusCode
来源：http://hz.fengsongda.top/gtijltodfu.html

[L08] 并发请求多个地址
来源：http://hz.zhijiandao.cn/gtkaxxprxk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.daxiang520.top/gtccfntakf.html

PHP:  curl_multi_init() 系列
来源：http://hz.xinyue.icu/gturbdvdkh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.wangshuangyany.cn/gtxytfzazv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nwbrower.top/gtawtybvld.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.gzhubu.top/gtefkzlszp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jinghuilouyu.cn/gtbjljosts.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hnxiangtu.top/gtejgkfrjm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.sweek.top/gtrrvxdxoo.html

================================================================================
来源：http://hz.kuanghao11.cn/gtrvyhrxek.html

M. 命令行 / 进程 / 环境
来源：http://hz.52xcode.cn/gtiingzpsr.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtjqozpquy.html

[M01] 读取命令行参数
来源：http://hz.zhixingplan.top/gtimmliqgc.html

Py:   sys.argv[1:]
来源：http://hz.xziqi.cn/gtitxecemx.html

PHP:  $argv;  $argc;
来源：http://hz.cqqwz.cn/gtekeoywzb.html

JS:   process.argv.slice(2)
来源：http://hz.cheryme.top/gtmaxklrmr.html

TS:   process.argv.slice(2)
来源：http://hz.hammf.cn/gtiqupuyyp.html

Java: args 数组（main 方法参数）
来源：http://hz.xylfe.cn/gtwnrlsfap.html

Go:   os.Args[1:]
来源：http://hz.zycfv.cn/gtxcwaicuo.html

Ruby: ARGV
来源：http://hz.quarkkingdee.top/gtubfewnoe.html

C#:   args 数组（Main 方法参数）
来源：http://hz.sweek.top/gtlerzmiiv.html

[M02] 读取环境变量
来源：http://hz.zhengqikj.top/gtmrjdelvl.html

Py:   os.environ.get("HOME")
来源：http://hz.gotoacloud.top/gtvqeddjbt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jinghuilouyu.cn/gtxzkjlhpr.html

JS:   process.env.HOME
来源：http://hz.dianchejie.cn/gtfdmyluaa.html

TS:   process.env.HOME
来源：http://hz.shanyushiyangkeji.top/gthaaieejr.html

Java: System.getenv("HOME")
来源：http://hz.jqgufenzy.top/gtptuzrzhi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.chenjidiqi.icu/gtbsfzvprb.html

Ruby: ENV["HOME"]
来源：http://hz.hywenlv.cn/gtlismlgga.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.daxiang520.top/gttxwrmosm.html

[M03] 执行外部命令
来源：http://hz.yonumen.top/gtttyvdenv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.dianchejie.cn/gtisuxopma.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yuxming.cn/gtpyojzjfo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.guowangkeji.top/gttwobblkb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.aibaodan.cn/gtvcrcrlgt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.iojbl.cn/gttybptxhu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.bjfxy.top/gthipjmrcq.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jinqigufen.top/gtmochdpew.html

C#:   Process.Start("ls", "-l");
来源：http://hz.vqdsnc.cn/gtzjuipsop.html

[M04] 获取当前工作目录
来源：http://hz.chenjidiqi.icu/gtgsplknaq.html

Py:   os.getcwd()
来源：http://hz.yj20258888.top/gtfguwjpla.html

PHP:  getcwd();
来源：http://hz.52xcode.cn/gtodxsnlwu.html

JS:   process.cwd()
来源：http://hz.yueranfly.top/gtgdrpiuhj.html

TS:   process.cwd()
来源：http://hz.hongshengwenyu.top/gtnphuxfsu.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.kuanghao11.cn/gtsudceifm.html

Go:   os.Getwd()
来源：http://hz.chenjidiqi.icu/gtgirsdkqb.html

Ruby: Dir.pwd
来源：http://hz.pengpengdd.cyou/gtbhxefzkl.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.shzxlz.cn/gtnxwiiuyb.html

[M05] 设置退出码
来源：http://hz.bjfxy.top/gtwqdhlsxc.html

Py:   sys.exit(1)
来源：http://hz.bjfxy.top/gtwbgibgfj.html

PHP:  exit(1);
来源：http://hz.fzhhl.top/gttlykaiqk.html

JS:   process.exit(1)
来源：http://hz.yonumen.top/gtkdefdszp.html

TS:   process.exit(1)
来源：http://hz.xuanzx.com/gtijcnuxgl.html

Java: System.exit(1)
来源：http://hz.gaohongyu789.top/gtdxmwvhqm.html

Go:   os.Exit(1)
来源：http://hz.nanxinkj.top/gtvkbnclcp.html

Ruby: exit 1
来源：http://hz.guowangkeji.top/gthxltfccz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yuxming.cn/gtudqezzfs.html

[M06] 向标准错误输出
来源：http://hz.zhoulong.xyz/gtcfbefpwv.html

Py:   print("err", file=sys.stderr)
来源：http://hz.dashuyun.cn/gtylgtffdq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.gogol.net.cn/gtezfgysdm.html

JS:   console.error("err")
来源：http://hz.ybcxt.top/gtfqqkducl.html

TS:   console.error("err")
来源：http://hz.aizwys.cn/gtzhmgeswg.html

Java: System.err.println("err")
来源：http://hz.shzxlz.cn/gteooxvavk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.pycfn.com/gtuqcwdqkm.html

Ruby: warn "err"
来源：http://hz.chenlongwang.top/gtcsrvyktu.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.tanke756.top/gtblswyeun.html

[M07] 判断是否为主入口
来源：http://hz.tianlin.xyz/gtpiskcyzn.html

Py:   if __name__ == "__main__":
来源：http://hz.guannengcc.top/gtvnsbiqms.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.dianchejie.cn/gtsjdlifyu.html

JS:   require.main === module
来源：http://hz.zhaomingkeji.xyz/gtyswyjzqo.html

TS:   require.main === module
来源：http://hz.hongshengwenyu.top/gtpvpmidvg.html

Java: public static void main(String[] args)
来源：http://hz.havefunace.top/gtexupdxbv.html

Go:   func main()
来源：http://hz.hongshengwenyu.top/gttgycqqzs.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cqqwz.cn/gtxpznhkyw.html

C#:   static void Main(string[] args)
来源：http://hz.ehwqpu.com/gtmbtynztt.html

[M08] 获取系统与运行时信息
来源：http://hz.aizwys.cn/gtienydacv.html

Py:   platform.system();  platform.python_version()
来源：http://hz.pengpengdd.cyou/gtgiqvocer.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.hongshengwenyu.top/gtatutropi.html

JS:   process.platform;  process.version
来源：http://hz.52xcode.cn/gtiwfyveyh.html

TS:   process.platform;  process.version
来源：http://hz.dashuyun.cn/gtrggjgogc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.cheryme.top/gtznrwaors.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.wangdashe.top/gtlyttofru.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.sysykeji.top/gtswdwivlt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.chenlongwang.top/gtbyerkxhb.html

================================================================================
来源：http://hz.fengsongda.top/gtuwhdhnnw.html

N. 数据结构与算法
来源：http://hz.redwolf501.top/gtguxzqjve.html

================================================================================
来源：http://hz.0kj1m.cn/gterlyklaj.html

[N01] 二分查找（有序数组）
来源：http://hz.havefunace.top/gtmgrgfriq.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.dianchejie.cn/gtylexrydw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hnqzz.top/gtzhlpoikp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xylfe.cn/gtgrmrjqqu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhiwuduotai.top/gtewnkeqyf.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.c1oappe.top/gtasmwgbpt.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.dashuyun.cn/gtsaraiyvy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.c1oappe.top/gtuvqbbfpv.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.svipenyu.cn/gtyeppsged.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ydzc1.top/gtifjvzved.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hfpthk.cn/gtzvwmzlsk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.xylfe.cn/gtubprbpec.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yonumen.top/gteyoysnfg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.daria6918.cn/gtkvopawzb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.tianlin.xyz/gtwztzljtn.html

Go:   slices.Sort(arr)
来源：http://hz.jqgufenzy.top/gtjohforgg.html

Ruby: arr.sort
来源：http://hz.aizwys.cn/gtlhyclrlr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.hywenlv.cn/gtsmeamant.html

[N03] 快速排序（分治示例）
来源：http://hz.yanxiufei.cn/gtkkslhwfk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xingfuxueyuan.xyz/gtqcjracak.html

PHP:  // 递归实现，或用 usort
来源：http://hz.cashguo.top/gtbkcmvzrn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shanyushiyangkeji.top/gtoejakckp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shuidangran.top/gtwkauukrq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhongyouzk.top/gtitplxqns.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.aibaodan.cn/gtfzhftwbm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hnxiangtu.top/gtjtcvitiw.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.gogol.net.cn/gtiouqebmu.html

[N04] 斐波那契数列
来源：http://hz.nwbrower.top/gtrznyffow.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.gzhubu.top/gtfpnbsfbp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.shanyushiyangtech.top/gticmxshpw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nanxuanxn.top/gtfcduhhfq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xinyue.icu/gtkxtizbvr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.9152youxi.cn/gtjyzvwybq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhiwuduotai.top/gtoerklddk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.gogol.net.cn/gtstsxmsnq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.shuidangran.top/gtakcuhvnu.html

[N05] 最大公约数
来源：http://hz.52xcode.cn/gtvpdlscux.html

Py:   math.gcd(a, b)
来源：http://hz.gotoacloud.top/gtoybkgdcx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.svipenyu.cn/gtczkdhvtp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.kuanghao11.cn/gtiznhlwxx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jianghu66.top/gtzdvnyidd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.xinyue.icu/gtyniofmvy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jlsjyb.cn/gtmnxzqqgq.html

Ruby: a.gcd(b)
来源：http://hz.xuetiantiany.cn/gthphwmuyt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.nanxinkj.top/gtauntznax.html

[N06] 判断回文字符串
来源：http://hz.aizwys.cn/gtfkegogpa.html

Py:   s == s[::-1]
来源：http://hz.daria6918.cn/gtnxrlgytq.html

PHP:  $s === strrev($s);
来源：http://hz.vqdsnc.cn/gttvatvuji.html

JS:   s === [...s].reverse().join("")
来源：http://hz.cdnleiting.top/gtilmkmhmo.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ydjk.org.cn/gtmkefrbey.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jqgfzy.top/gtcbfdmsyx.html

Go:   // 双指针从两端比较
来源：http://hz.sufxvd.cn/gtgasqrqax.html

Ruby: s == s.reverse
来源：http://hz.xuetiantiany.cn/gtmsketimk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhixingplan.top/gtvbkvsvtt.html

[N07] 两数之和（返回下标）
来源：http://hz.yangfankeji.com/gtpdeigkol.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.shanyushiyangkeji.top/gtqdsyberp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jiagoushi.top/gtskphbwnz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.guowangkeji.top/gtbupnjggl.html

TS:   // 手写 Map<string, number>
来源：http://hz.pycfn.com/gtdczhpfkp.html

Java: // 手写 HashMap
来源：http://hz.cashguo.top/gtchbltsbg.html

Go:   // 手写 map[int]int
来源：http://hz.hywenlv.cn/gtaheciobm.html

Ruby: // 手写 Hash
来源：http://hz.snrcjt.cn/gtkchofgzh.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jiagoushi.top/gtpfenjdor.html

[N08] 生成全排列
来源：http://hz.sysykeji.top/gtbvorhhlc.html

Py:   itertools.permutations(arr)
来源：http://hz.aizwys.cn/gtblcdzeep.html

PHP:  // 手写递归交换
来源：http://hz.hnqzz.top/gtbezemieh.html

JS:   // 手写回溯递归
来源：http://hz.jianghu66.top/gtalqlogaz.html

TS:   // 手写回溯递归
来源：http://hz.dashuyun.cn/gtzmsylsyu.html

Java: // 手写回溯递归
来源：http://hz.dianchejie.cn/gtngjtiruh.html

Go:   // 手写回溯递归
来源：http://hz.hammf.cn/gttrtuwsfu.html

Ruby: arr.permutation.to_a
来源：http://hz.hfpthk.cn/gtwnkcrbyb.html

C#:   // 手写回溯递归
来源：http://hz.hfpthk.cn/gtgazfrkzg.html

[N09] 栈与队列
来源：http://hz.aizwys.cn/gtxofxysnm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhijiandao.cn/gtupihdxde.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.pengpengdd.cyou/gtcvbzrtsx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.ppjwa.cn/gthfjostim.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhijiandao.cn/gttnxwtfdf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.xingfuxueyuan.xyz/gteswomvqx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.c1oappe.top/gtccwmgxxo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.ywan-chungtsiang.top/gtnmvqbiff.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.shzxlz.cn/gtdesgqwpv.html

[N10] 链表节点定义
来源：http://hz.yuxming.cn/gtopzuqtly.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yonumen.top/gtqccleeii.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yuxming.cn/gtozwhwsra.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.chenzaomai.com/gtybhkpphy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hywenlv.cn/gtmxckmgve.html

Java: class Node { int v; Node next; }
来源：http://hz.svipenyu.cn/gtsdsthikh.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.haohaochexian.top/gtyfjtbwen.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.sxryk.cn/gtzmpmaiby.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.shzxlz.cn/gtckmzfrfk.html

[N11] 二叉树中序遍历
来源：http://hz.cucudq.cn/gtxxsvesew.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.52xcode.cn/gtdnqawhst.html

PHP:  // 手写递归函数
来源：http://hz.mhx1999.top/gtkdkrsvjs.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hammf.cn/gtebobegka.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.chenjidiqi.icu/gtqlnrfjcm.html

Java: // 手写递归
来源：http://hz.havefunace.top/gtqtyjvjbn.html

Go:   // 手写递归
来源：http://hz.jlsjyb.cn/gtfycexeyz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.shanyushiyangkeji.top/gtrhtjhipe.html

C#:   // 手写递归
来源：http://hz.yonumen.top/gtsfgeqpkx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yanxiufei.cn/gtpjyutogl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.shanyushiyangtech.top/gtfvmpyscv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhijiandao.cn/gtigxnjmmd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gogol.net.cn/gtfrqvfbxu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cqqwz.cn/gtfvmttpdi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.vqdsnc.cn/gtnphnjqad.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.shuidangran.top/gtywuhijha.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.svipenyu.cn/gtdezcsmjq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gogol.net.cn/gtwccujuww.html


<!-- 参考信息 -->