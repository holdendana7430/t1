代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yueranfly.top/gtmunscjrp.html

Go:   json.Marshal(obj)
来源：http://hz.nanxinkj.top/gtvgiujhjz.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.ydjk.org.cn/gteaenblid.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhongyouzk.top/gtoprakaai.html

[K02] JSON 字符串转对象
来源：http://hz.aizwys.cn/gtjsqpmntj.html

Py:   json.loads(s)
来源：http://hz.snrcjt.cn/gtvsfrpkjp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.c1oappe.top/gthdgspaxq.html

JS:   JSON.parse(s)
来源：http://hz.jianghu66.top/gthtcmwiam.html

TS:   JSON.parse(s)
来源：http://hz.dashuyun.cn/gtqwekllxf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hnqzz.top/gtfuiizpat.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.bjfxy.top/gtgbssuufn.html

Ruby: JSON.parse(s)
来源：http://hz.zhiwuduotai.top/gtaozxukuh.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.shanyushiyangtech.top/gtixjqekjr.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.guannengcc.top/gtmdthwnov.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.sysykeji.top/gtsjquxxei.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.nanxinkj.top/gthtyhxuty.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhiwuduotai.top/gtfvnqtnsf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jqgufenzy.top/gtngbcptel.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hammf.cn/gtxqpcfhuu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.shuidangran.top/gtibotdrox.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.aizwys.cn/gthcsxvwhj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hammf.cn/gtmxvjhyps.html

[K04] 读取 JSON 文件
来源：http://hz.nanxuanxn.top/gtiidquptn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yuxming.cn/gtvriuaykj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cheryme.top/gthcjoixtr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cqqwz.cn/gtweldfnce.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.redwolf501.top/gtasauikwk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hammf.cn/gtcnswwmtk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hongshengwenyu.top/gtilopljmr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.vqdsnc.cn/gtemwiwwnx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.redwolf501.top/gtzjujxogq.html

[K05] 深拷贝对象
来源：http://hz.ybcxt.top/gtbhjgsfzl.html

Py:   copy.deepcopy(obj)
来源：http://hz.shzxlz.cn/gtwvdibbwe.html

PHP:  unserialize(serialize($obj));
来源：http://hz.vqdsnc.cn/gtbsrjikcg.html

JS:   structuredClone(obj)
来源：http://hz.chenzaomai.com/gtxcafwuas.html

TS:   structuredClone(obj)
来源：http://hz.gotoacloud.top/gtoxffsnjs.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.aizwys.cn/gtiwpwwglw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xingfuxueyuan.xyz/gtmtmucfdw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.c1oappe.top/gtitljcwji.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ybcxt.top/gtlfnnzzqj.html

[K06] 解析 URL 查询串
来源：http://hz.jinqigufen.top/gtwvxggock.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xuetiantiany.cn/gtpzoowhdl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.ybcxt.top/gtjapacdcb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj20258888.top/gtfjncbthc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinyuanbaomall.cn/gtvfupvncw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ywan-chungtsiang.top/gtcohwbpkv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jinqigufen.top/gtfrdwezeo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.aizwys.cn/gtyftifbpp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cashguo.top/gtogjkdpqq.html

[K07] 进制转换
来源：http://hz.fzhhl.top/gtcrwyzkrj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jianghu66.top/gtxlrkwsdx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jqgfzy.top/gtrsuuyrzy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.aizwys.cn/gtphacylyh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yueranfly.top/gtddsoaynk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xuetiantiany.cn/gtnocykexz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xinyue.icu/gthpbwggwc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.vqdsnc.cn/gtsbbhmlot.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ppjwa.cn/gtrarukcdi.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yongpay.top/gtihfeqsqq.html

Py:   pickle.dumps(obj)
来源：http://hz.gogol.net.cn/gtrukfnmmv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.sxryk.cn/gtrzrdxugi.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ivvv.top/gtccrpghcd.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.birdmap.top/gtxxruqpdz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jinyuanbaomall.cn/gtbctgiuap.html

Go:   encoding/gob
来源：http://hz.hysaishi.cn/gtnuswjeau.html

Ruby: Marshal.dump(obj)
来源：http://hz.shanyushiyangkeji.top/gtbywznupg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.nwbrower.top/gtymuusckc.html

================================================================================
来源：http://hz.yuanzhike.top/gtzxirozmn.html

L. 网络请求
来源：http://hz.pycfn.com/gtyaavtafd.html

================================================================================
来源：http://hz.zdqjudy.top/gtzhqwtjcn.html

[L01] 发送 GET 请求
来源：http://hz.dianchejie.cn/gtldqeguje.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jinyuanbaomall.cn/gthxotuktp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jyoumei.cn/gtozgnedwy.html

JS:   await fetch(url)
来源：http://hz.jqgfzy.top/gthnnwrprk.html

TS:   await fetch(url)
来源：http://hz.quarkkingdee.top/gtconvgmhs.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.gaohongyu789.top/gtnawfqmoc.html

Go:   resp, err := http.Get(url)
来源：http://hz.aibaodan.cn/gtncxdgnle.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhiwuduotai.top/gthmztdtev.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ydzc1.top/gthjwsnkru.html

[L02] 发送 POST JSON
来源：http://hz.aizwys.cn/gtwrrnhbng.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.meibo888.top/gtgdqtpfuy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.aibaodan.cn/gthkxuesrs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yvedp.cn/gtwntndnkf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.nanxuanxn.top/gtxqramnjv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.pycfn.com/gttzfurabt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhixingplan.top/gtblhfpckh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.pycfn.com/gthjrluwjv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.chenlongwang.top/gtexbsxxwp.html

[L03] 设置自定义请求头
来源：http://hz.c1oappe.top/gtgfpmgaty.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.quarkkingdee.top/gtwqudhxha.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ydjk.org.cn/gtezkqfyqn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yongpay.top/gtsdbsqark.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cashguo.top/gtreserjjz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.316326.xyz/gtuimbmvhe.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jyoumei.cn/gtsgypcnsf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.pengpengdd.cyou/gtlkogjfsd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hywenlv.cn/gtsfgprysg.html

[L04] 设置超时
来源：http://hz.jianghu66.top/gtczuditgx.html

Py:   requests.get(url, timeout=5)
来源：http://hz.shanyushiyangkeji.top/gtxwkznxct.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jianghu66.top/gtcpdzqnxr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shzxlz.cn/gtjbsfbcds.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xziqi.cn/gtujhyordv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zdqjudy.top/gtzdixlrzu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hywenlv.cn/gtdulyjuek.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.dashuyun.cn/gtbjuwhcmb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hnxiangtu.top/gtzlocfixz.html

[L05] 上传文件（multipart）
来源：http://hz.316326.xyz/gtvrevtknb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zycfv.cn/gtcyxcstzs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.nwbrower.top/gttbzwgugz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ybcxt.top/gtsjawbzmq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.wangdashe.top/gtpbzfzpfm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.tianlin.xyz/gtzlgqydyd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.chenlongwang.top/gtrwszqgtz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zdqjudy.top/gttmrqlcnl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.smart0.xyz/gtnlbpiexy.html

[L06] 解析响应为 JSON
来源：http://hz.tian-w.cn/gtjhqxukzb.html

Py:   resp.json()
来源：http://hz.ywan-chungtsiang.top/gtuczczhhr.html

PHP:  json_decode($body, true);
来源：http://hz.vqdsnc.cn/gtguwhrjui.html

JS:   await resp.json()
来源：http://hz.cashguo.top/gtuinmuifh.html

TS:   await resp.json()
来源：http://hz.smart0.xyz/gtggmtecae.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.c1oappe.top/gtszwjberz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.tianlin.xyz/gtpnfpbtfb.html

Ruby: JSON.parse(resp.body)
来源：http://hz.pengpengdd.cyou/gtsygoycxs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hnqzz.top/gtbjkwewex.html

[L07] 处理 HTTP 状态码
来源：http://hz.sxryk.cn/gtepotbtai.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.pycfn.com/gtgbhgyffm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.dianchejie.cn/gtxkupzdfy.html

JS:   resp.ok;  resp.status
来源：http://hz.aizwys.cn/gtwrsnfyby.html

TS:   resp.ok;  resp.status
来源：http://hz.shanyushiyangtech.top/gthzwyhpjv.html

Java: resp.statusCode()
来源：http://hz.guowangkeji.top/gtztzscokc.html

Go:   resp.StatusCode
来源：http://hz.gogol.net.cn/gtsvqduhbl.html

Ruby: resp.code.to_i
来源：http://hz.shanyushiyangtech.top/gtxudwufel.html

C#:   (int)resp.StatusCode
来源：http://hz.gogol.net.cn/gtvwqlcctc.html

[L08] 并发请求多个地址
来源：http://hz.andypj.xyz/gtcfmcbmls.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.feifeiyinyue.top/gtljnsgjvc.html

PHP:  curl_multi_init() 系列
来源：http://hz.nanxuanxn.top/gtwncmfrry.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xuetiantiany.cn/gtworgkdhl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.havefunace.top/gtyzhusezy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yuanzhike.top/gtoqzgtdno.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.smart0.xyz/gtivhuhvjz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hnqzz.top/gtvalokywd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.wangdashe.top/gtrpefgpae.html

================================================================================
来源：http://hz.ivvv.top/gtwfmqyrsf.html

M. 命令行 / 进程 / 环境
来源：http://hz.xylfe.cn/gtdncisvvy.html

================================================================================
来源：http://hz.ivvv.top/gtacwoadcv.html

[M01] 读取命令行参数
来源：http://hz.aizwys.cn/gtxscyiwbo.html

Py:   sys.argv[1:]
来源：http://hz.yuanzhike.top/gtinhgixba.html

PHP:  $argv;  $argc;
来源：http://hz.mhx1999.top/gtrlvfatsr.html

JS:   process.argv.slice(2)
来源：http://hz.haohaochexian.top/gtkbokwdrt.html

TS:   process.argv.slice(2)
来源：http://hz.yj20258.top/gtyhrowobd.html

Java: args 数组（main 方法参数）
来源：http://hz.dianchejie.cn/gtyjsesaox.html

Go:   os.Args[1:]
来源：http://hz.nwbrower.top/gtekqlvmav.html

Ruby: ARGV
来源：http://hz.bjfxy.top/gtombtsogc.html

C#:   args 数组（Main 方法参数）
来源：http://hz.shanyushiyangkeji.top/gtixnuiejq.html

[M02] 读取环境变量
来源：http://hz.pycfn.com/gtxmddfqho.html

Py:   os.environ.get("HOME")
来源：http://hz.hnqzz.top/gtsciqowbz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jiagoushi.top/gtjncblulm.html

JS:   process.env.HOME
来源：http://hz.zhengqikj.top/gtaoyotqul.html

TS:   process.env.HOME
来源：http://hz.ivvv.top/gtyajtsasy.html

Java: System.getenv("HOME")
来源：http://hz.cdnleiting.top/gtvjxjgbtb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yuxming.cn/gtsnlqwbrw.html

Ruby: ENV["HOME"]
来源：http://hz.tanke756.top/gtyqhbvfhe.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.nanxinkj.top/gtphmbzkkb.html

[M03] 执行外部命令
来源：http://hz.zhaomingkeji.xyz/gtytppgokq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.c1oappe.top/gtiplphkrp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.pengpengdd.cyou/gtpjtpyiyl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.meibo888.top/gtoxragjjy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.chenzaomai.com/gtztovnraj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhengqikj.top/gtsyazpmaq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.sysykeji.top/gtgclkxfoz.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.cucudq.cn/gtfznvfrmj.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jiagoushi.top/gtkgvpymhd.html

[M04] 获取当前工作目录
来源：http://hz.yanxiufei.cn/gtacmnypwz.html

Py:   os.getcwd()
来源：http://hz.cucudq.cn/gtnsbphlgp.html

PHP:  getcwd();
来源：http://hz.smart0.xyz/gthfzuhasf.html

JS:   process.cwd()
来源：http://hz.redwolf501.top/gtonltvpxi.html

TS:   process.cwd()
来源：http://hz.zhoulong.xyz/gtqplvxruo.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zycfv.cn/gtqccuvqfh.html

Go:   os.Getwd()
来源：http://hz.fzhhl.top/gttjnzwtfh.html

Ruby: Dir.pwd
来源：http://hz.xziqi.cn/gtzgmgrynt.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.iojbl.cn/gthoxsrihd.html

[M05] 设置退出码
来源：http://hz.gzhubu.top/gtqdhjsenh.html

Py:   sys.exit(1)
来源：http://hz.hongshengwenyu.top/gtqznomhji.html

PHP:  exit(1);
来源：http://hz.ivvv.top/gtzmqkqvjq.html

JS:   process.exit(1)
来源：http://hz.jlsjyb.cn/gtjcfywsvs.html

TS:   process.exit(1)
来源：http://hz.gaohongyu789.top/gtlvvwelvz.html

Java: System.exit(1)
来源：http://hz.cucudq.cn/gtjkpilzsi.html

Go:   os.Exit(1)
来源：http://hz.jinyuanbaomall.cn/gtlqopqopd.html

Ruby: exit 1
来源：http://hz.ydzc1.top/gtvpesxtnh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.snrcjt.cn/gtgfjqorle.html

[M06] 向标准错误输出
来源：http://hz.hfpthk.cn/gthmupxcvh.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yvedp.cn/gtqokgvuvl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.c1oappe.top/gtlckicrru.html

JS:   console.error("err")
来源：http://hz.yvedp.cn/gtsuvplczg.html

TS:   console.error("err")
来源：http://hz.redwolf501.top/gtomrdjgdi.html

Java: System.err.println("err")
来源：http://hz.cdnleiting.top/gtzoroqzgq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zycfv.cn/gtztztnmzz.html

Ruby: warn "err"
来源：http://hz.shanyushiyangkeji.top/gttdvroypw.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.nanxinkj.top/gtprcmbzed.html

[M07] 判断是否为主入口
来源：http://hz.zhoulong.xyz/gtelvkatmh.html

Py:   if __name__ == "__main__":
来源：http://hz.tanke756.top/gtqmqvbmxb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.hongshengwenyu.top/gtuqyeutcv.html

JS:   require.main === module
来源：http://hz.vqdsnc.cn/gtsejbdnru.html

TS:   require.main === module
来源：http://hz.yangfankeji.com/gtgasblvfd.html

Java: public static void main(String[] args)
来源：http://hz.cdnleiting.top/gtmgvtysnk.html

Go:   func main()
来源：http://hz.haohaochexian.top/gtwvpocqzp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.gzhubu.top/gtcpyaykji.html

C#:   static void Main(string[] args)
来源：http://hz.hnqzz.top/gtzmooiotj.html

[M08] 获取系统与运行时信息
来源：http://hz.shangyingyoupin.top/gtbpnbeaqh.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jiagoushi.top/gtixlzxcbo.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.chenjidiqi.icu/gtyjdpntos.html

JS:   process.platform;  process.version
来源：http://hz.mhx1999.top/gtqnnzrmrr.html

TS:   process.platform;  process.version
来源：http://hz.ppjwa.cn/gtdfgdwxpi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.fengsongda.top/gtrdczkdei.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.wangdashe.top/gtsyrvblat.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.xziqi.cn/gtlahngdxj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jinqigufen.top/gtofyvkvym.html

================================================================================
来源：http://hz.yvedp.cn/gtzppokijj.html

N. 数据结构与算法
来源：http://hz.guannengcc.top/gtdsvgqtao.html

================================================================================
来源：http://hz.pycfn.com/gtkqvhnxqd.html

[N01] 二分查找（有序数组）
来源：http://hz.nwbrower.top/gtxtplhsvx.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhoulong.xyz/gtxarfrkok.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jinyuanbaomall.cn/gtlyzesksk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yonumen.top/gtaaeahrnu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.chenzaomai.com/gtkbyhseoe.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.quarkkingdee.top/gtisxjddic.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yanxiufei.cn/gtzvouayzo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yvedp.cn/gtqierrlxf.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.tanke756.top/gtrfifkunv.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.shangyingyoupin.top/gtfmddmcrh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhongyouzk.top/gtjhkbjrpr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.gaohongyu789.top/gtqrxqczzp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zdqjudy.top/gterbduubd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.quarkkingdee.top/gtpcraqmst.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yangfankeji.com/gtuquanoyf.html

Go:   slices.Sort(arr)
来源：http://hz.316326.xyz/gtpmdfkwqa.html

Ruby: arr.sort
来源：http://hz.guannengcc.top/gtkxnmvhma.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.guannengcc.top/gtcezdjswz.html

[N03] 快速排序（分治示例）
来源：http://hz.daria6918.cn/gtecriekkx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.chenjidiqi.icu/gtkweercwl.html

PHP:  // 递归实现，或用 usort
来源：http://hz.chenzaomai.com/gtaacvnnng.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shangyingyoupin.top/gtfepyscax.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.dashuyun.cn/gtthxkvxwn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.hammf.cn/gtsroucfoq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.ivvv.top/gtrdseinhs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jinyuanbaomall.cn/gtkxpnhdtm.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jlsjyb.cn/gtqknwemdc.html

[N04] 斐波那契数列
来源：http://hz.aibaodan.cn/gtodjpedzd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yj202588.top/gtbaeysakw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.cashguo.top/gtwrxyrads.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.birdmap.top/gtfyygzfnf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.meibo888.top/gtegvlhspk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.gzhubu.top/gtlsvidomp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.mhx1999.top/gtbnxtnotf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yj202588.top/gtedcnnsyo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.nanxinkj.top/gtanqtyhpg.html

[N05] 最大公约数
来源：http://hz.tanke756.top/gtfmlimkhg.html

Py:   math.gcd(a, b)
来源：http://hz.bjfxy.top/gtpuzgqmlk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hfpthk.cn/gtvapehdnh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhijiandao.cn/gthocwcpwr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xuanzx.com/gtayzvodjy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.haohaochexian.top/gtfhvzdazy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.haohaochexian.top/gtyltrvghe.html

Ruby: a.gcd(b)
来源：http://hz.zhijiandao.cn/gtwtuxdpwx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.9152youxi.cn/gtbdjmxnia.html

[N06] 判断回文字符串
来源：http://hz.ivvv.top/gtwbatkxux.html

Py:   s == s[::-1]
来源：http://hz.zdqjudy.top/gtokmxcupe.html

PHP:  $s === strrev($s);
来源：http://hz.ppjwa.cn/gtabmmmlzz.html

JS:   s === [...s].reverse().join("")
来源：http://hz.ydjk.org.cn/gtvlcmvdpz.html

TS:   s === [...s].reverse().join("")
来源：http://hz.pycfn.com/gtiskgebue.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.gotoacloud.top/gtreqhmnzg.html

Go:   // 双指针从两端比较
来源：http://hz.zhiwuduotai.top/gtsifiixen.html

Ruby: s == s.reverse
来源：http://hz.shzxlz.cn/gtnfdotehr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.svipenyu.cn/gtxifefdqi.html

[N07] 两数之和（返回下标）
来源：http://hz.zhaomingkeji.xyz/gtxnceoygs.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.mhx1999.top/gtjgdhtrom.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yuanzhike.top/gtshzdvgjs.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.quarkkingdee.top/gttkrlldjx.html

TS:   // 手写 Map<string, number>
来源：http://hz.sysykeji.top/gtknytuude.html

Java: // 手写 HashMap
来源：http://hz.jiagoushi.top/gtalsseejg.html

Go:   // 手写 map[int]int
来源：http://hz.smart0.xyz/gtinqkqisa.html

Ruby: // 手写 Hash
来源：http://hz.gzhubu.top/gtkrxeeaou.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yangfankeji.com/gtrloeyhji.html

[N08] 生成全排列
来源：http://hz.zhoulong.xyz/gtnbkpkwng.html

Py:   itertools.permutations(arr)
来源：http://hz.ehwqpu.com/gtkcfnwiyw.html

PHP:  // 手写递归交换
来源：http://hz.havefunace.top/gtkkszwcxn.html

JS:   // 手写回溯递归
来源：http://hz.chenjidiqi.icu/gtdfurqsym.html

TS:   // 手写回溯递归
来源：http://hz.pycfn.com/gtsfxxgzsx.html

Java: // 手写回溯递归
来源：http://hz.zhongyouzk.top/gtxpqlnqhv.html

Go:   // 手写回溯递归
来源：http://hz.gzhubu.top/gtxceylzsm.html

Ruby: arr.permutation.to_a
来源：http://hz.zhoulong.xyz/gtkfuitbqq.html

C#:   // 手写回溯递归
来源：http://hz.zdqjudy.top/gtyjadbooi.html

[N09] 栈与队列
来源：http://hz.jiagoushi.top/gthbbnxbza.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.chenzaomai.com/gtsgngvnfl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.nanxuanxn.top/gtjsooezri.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.wangdashe.top/gthzxtsrav.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.xinyue.icu/gtbloumach.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yuanzhike.top/gtuwhyzryn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jyoumei.cn/gtkhrpxkqk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.ydjk.org.cn/gtajbbyhnr.html


<!-- 参考信息 -->