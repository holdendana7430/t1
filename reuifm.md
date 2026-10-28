代发 wailian999

TS:   JSON.parse(s)
来源：http://hz.yangfankeji.com/gtfdknuqhu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.dianchejie.cn/gtovknyjxj.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ehwqpu.com/gtbloiplck.html

Ruby: JSON.parse(s)
来源：http://hz.zhaomingkeji.xyz/gtbvbigjdq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.chenlongwang.top/gtdtjtthjq.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jyoumei.cn/gtodpvaxvh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yvedp.cn/gtnqwhndrk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yongpay.top/gtwyczeopy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zycfv.cn/gtepogpgwt.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.sxryk.cn/gtznymoejx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.svipenyu.cn/gtaurwmrty.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jinyuanbaomall.cn/gtrdbppqhu.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yj20258888.top/gtfiosssko.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.9152youxi.cn/gtffiuxqyv.html

[K04] 读取 JSON 文件
来源：http://hz.cashguo.top/gtwxioarvi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jqgfzy.top/gtyxdwpeca.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.nanxinkj.top/gtgapawyuk.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shanyushiyangtech.top/gtsfoyqrcs.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.tianlin.xyz/gtenemgmgn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.bjfxy.top/gtvfzkxhjj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.c1oappe.top/gtiqiwqsqf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.bjfxy.top/gtucwijclm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.haohaochexian.top/gtgzycqkcp.html

[K05] 深拷贝对象
来源：http://hz.shzxlz.cn/gtiiwvewgf.html

Py:   copy.deepcopy(obj)
来源：http://hz.zycfv.cn/gtvxsxzepk.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yj20258.top/gtgzglmkpo.html

JS:   structuredClone(obj)
来源：http://hz.sweek.top/gtnsdbwkzm.html

TS:   structuredClone(obj)
来源：http://hz.zdqjudy.top/gtkfzgfkmg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.gzhubu.top/gtulbhelco.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jqgufenzy.top/gtrqalhlng.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ydzc1.top/gtvaqvmfsx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.tanke756.top/gtjqbgjkos.html

[K06] 解析 URL 查询串
来源：http://hz.shangyingyoupin.top/gtdmgvamkr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhijiandao.cn/gtaqqzhitm.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jinqigfzy.top/gtxwvlzdam.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tanke756.top/gtpeupfine.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.svipenyu.cn/gtitfzxlbg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.wangshuangyany.cn/gtxgrilkka.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.xuetiantiany.cn/gtfjzmkjpl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.smart0.xyz/gtbtxhjdag.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.dianchejie.cn/gtxdtnzpih.html

[K07] 进制转换
来源：http://hz.shangyingyoupin.top/gtbnavobbz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.xuanzx.com/gtytpoephb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jinghuilouyu.cn/gtwqjvdfpj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.wangdashe.top/gtcrgjmfos.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.nwbrower.top/gtyxycnpvb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ydzc1.top/gtobyxpkzx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhijiandao.cn/gtsvekfyum.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.shuidangran.top/gtjqxwmmjv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.chenjidiqi.icu/gtwgamqykp.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.shangyingyoupin.top/gtlavzqqfe.html

Py:   pickle.dumps(obj)
来源：http://hz.sufxvd.cn/gtpsshijnw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jlsjyb.cn/gtkgzqiihh.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.sxryk.cn/gtujvzojgx.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yanxiufei.cn/gtuuwhohnk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hfpthk.cn/gtcloecwyd.html

Go:   encoding/gob
来源：http://hz.aibaodan.cn/gtszskzmir.html

Ruby: Marshal.dump(obj)
来源：http://hz.dianchejie.cn/gtimvmfukb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jqgfzy.top/gtsscweuzu.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtgmdhmsqy.html

L. 网络请求
来源：http://hz.yuxming.cn/gtumzagzgg.html

================================================================================
来源：http://hz.guowangkeji.top/gtwrygljcj.html

[L01] 发送 GET 请求
来源：http://hz.hnqzz.top/gtdleyjuqi.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jinqigufen.top/gtolxaityc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.sweek.top/gttldjtbdf.html

JS:   await fetch(url)
来源：http://hz.shangyingyoupin.top/gtouqxogts.html

TS:   await fetch(url)
来源：http://hz.gzhubu.top/gtgueoxzbg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.xuetiantiany.cn/gtsstftvix.html

Go:   resp, err := http.Get(url)
来源：http://hz.jinqigufen.top/gtkjvoeisb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cheryme.top/gtdhynrzzk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jinghuilouyu.cn/gtaufgfhkv.html

[L02] 发送 POST JSON
来源：http://hz.xuetiantiany.cn/gtsnuggxrk.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yueranfly.top/gtbpyzmcrg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.aibaodan.cn/gtlideamnf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yuxming.cn/gtkqauwzah.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.chenjidiqi.icu/gtswvljbdq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jianghu66.top/gtjmcingan.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.nanxuanxn.top/gtyijwxlgq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.fzhhl.top/gthqphlchg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.cdnleiting.top/gtachxlnqg.html

[L03] 设置自定义请求头
来源：http://hz.hywenlv.cn/gtfptpgack.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zycfv.cn/gtsqxvqkag.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.wangshuangyany.cn/gtzdtcujvm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sxryk.cn/gtuwnnngar.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yueranfly.top/gtjxftximd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hnxiangtu.top/gttcvahkpv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.quarkkingdee.top/gtfahopdnp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.cheryme.top/gtxsfkoyne.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.cucudq.cn/gtikfpiwtx.html

[L04] 设置超时
来源：http://hz.hongshengwenyu.top/gtqcvvxkqs.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cheryme.top/gtvfcqqvdm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.fengsongda.top/gtulocpyna.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinqigufen.top/gtyyiieqba.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.dashuyun.cn/gthvqmjaea.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hnqzz.top/gtuimifilm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.guowangkeji.top/gtscmyhdlg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zhoulong.xyz/gtcfeknlsf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.cucudq.cn/gtqwezvclh.html

[L05] 上传文件（multipart）
来源：http://hz.jyoumei.cn/gtdvkwoton.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.fengsongda.top/gtnzhtaorb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yj20258.top/gtkkbztmek.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.shuidangran.top/gtbiimiorg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yj202588.top/gtcbxrozsr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yuanzhike.top/gtkqllohit.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.bjfxy.top/gtjejrireb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xziqi.cn/gtqukqqrbr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.cqqwz.cn/gtdjbdjqjv.html

[L06] 解析响应为 JSON
来源：http://hz.iojbl.cn/gtegvfsotd.html

Py:   resp.json()
来源：http://hz.pengpengdd.cyou/gtqluybljm.html

PHP:  json_decode($body, true);
来源：http://hz.redwolf501.top/gtcndzrapm.html

JS:   await resp.json()
来源：http://hz.yuxming.cn/gtmsdyhkog.html

TS:   await resp.json()
来源：http://hz.snrcjt.cn/gtatoxmoqp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhengqikj.top/gtalycycox.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.redwolf501.top/gtmwilkwcg.html

Ruby: JSON.parse(resp.body)
来源：http://hz.chenlongwang.top/gtomdjgcwl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jinghuilouyu.cn/gtiibackqc.html

[L07] 处理 HTTP 状态码
来源：http://hz.shzxlz.cn/gtkpixtcmn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hnqzz.top/gtljgwmwvl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.tanke756.top/gtrqnzjfia.html

JS:   resp.ok;  resp.status
来源：http://hz.feifeiyinyue.top/gtnazgnezg.html

TS:   resp.ok;  resp.status
来源：http://hz.jyoumei.cn/gtgkethetm.html

Java: resp.statusCode()
来源：http://hz.9152youxi.cn/gtjkswsrgr.html

Go:   resp.StatusCode
来源：http://hz.chenzaomai.com/gtcikpmanp.html

Ruby: resp.code.to_i
来源：http://hz.xuetiantiany.cn/gtdmwvrprw.html

C#:   (int)resp.StatusCode
来源：http://hz.ehwqpu.com/gtcwtmzprr.html

[L08] 并发请求多个地址
来源：http://hz.smart0.xyz/gtcrdvglmz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.shuidangran.top/gtzsnothtc.html

PHP:  curl_multi_init() 系列
来源：http://hz.wangdashe.top/gtjownouac.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ywan-chungtsiang.top/gthmixqnft.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.aizwys.cn/gtajaiqnwo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.pengpengdd.cyou/gtwghcytom.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jinqigufen.top/gthwznivvf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yvedp.cn/gtwgfcpbjc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.sysykeji.top/gtryyepthd.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtxcbcylrf.html

M. 命令行 / 进程 / 环境
来源：http://hz.xuetiantiany.cn/gtwjqluqar.html

================================================================================
来源：http://hz.hysaishi.cn/gtjnpdakqt.html

[M01] 读取命令行参数
来源：http://hz.jyoumei.cn/gtbqaqaabm.html

Py:   sys.argv[1:]
来源：http://hz.sufxvd.cn/gttlfrzfpf.html

PHP:  $argv;  $argc;
来源：http://hz.shanyushiyangtech.top/gtzgdneifx.html

JS:   process.argv.slice(2)
来源：http://hz.zhengqikj.top/gtpamyrwta.html

TS:   process.argv.slice(2)
来源：http://hz.svipenyu.cn/gtilflgplc.html

Java: args 数组（main 方法参数）
来源：http://hz.iojbl.cn/gtsmmexrol.html

Go:   os.Args[1:]
来源：http://hz.sweek.top/gtraezjibc.html

Ruby: ARGV
来源：http://hz.hnxiangtu.top/gtsyowfxcr.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ydzc1.top/gtesglhvfw.html

[M02] 读取环境变量
来源：http://hz.snrcjt.cn/gtlzljycev.html

Py:   os.environ.get("HOME")
来源：http://hz.nwbrower.top/gtzkbctwvj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yongpay.top/gtzapsdzxv.html

JS:   process.env.HOME
来源：http://hz.hammf.cn/gtlncyyaay.html

TS:   process.env.HOME
来源：http://hz.dashuyun.cn/gtbxxrrxws.html

Java: System.getenv("HOME")
来源：http://hz.zhixingplan.top/gtiinzbobo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jianghu66.top/gtzqahikpj.html

Ruby: ENV["HOME"]
来源：http://hz.shzxlz.cn/gtsfpzzzwz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.sweek.top/gtpcfnwedk.html

[M03] 执行外部命令
来源：http://hz.pengpengdd.cyou/gtabsmfcyu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jyoumei.cn/gtchjihwka.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.fengsongda.top/gtqqrdtfyy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.shuidangran.top/gtwtifojrx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.gzhubu.top/gtoxjqdnbw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hnxiangtu.top/gtwapjjftw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hammf.cn/gttvvsngay.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hfpthk.cn/gtudxxcklt.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhaomingkeji.xyz/gtdzgdsigl.html

[M04] 获取当前工作目录
来源：http://hz.aibaodan.cn/gtwbskqiso.html

Py:   os.getcwd()
来源：http://hz.gotoacloud.top/gtzfwweizz.html

PHP:  getcwd();
来源：http://hz.xingfuxueyuan.xyz/gtkqhkwjim.html

JS:   process.cwd()
来源：http://hz.pengpengdd.cyou/gtwfampbsk.html

TS:   process.cwd()
来源：http://hz.sxryk.cn/gtrddmkfst.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hfpthk.cn/gtyqheyswb.html

Go:   os.Getwd()
来源：http://hz.zhengqikj.top/gtkfungwvm.html

Ruby: Dir.pwd
来源：http://hz.yuanzhike.top/gtqlymwskc.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.vqdsnc.cn/gtrpnrsoxg.html

[M05] 设置退出码
来源：http://hz.jqgfzy.top/gtdfxbfqrg.html

Py:   sys.exit(1)
来源：http://hz.nanxinkj.top/gtryujqryv.html

PHP:  exit(1);
来源：http://hz.316326.xyz/gtyqugqijl.html

JS:   process.exit(1)
来源：http://hz.ivvv.top/gtxvyinqnj.html

TS:   process.exit(1)
来源：http://hz.aibaodan.cn/gtnomyqbnn.html

Java: System.exit(1)
来源：http://hz.daria6918.cn/gttqtvjesv.html

Go:   os.Exit(1)
来源：http://hz.jqgufenzy.top/gtikjnqoiz.html

Ruby: exit 1
来源：http://hz.daxiang520.top/gtxllfgrkp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.hongshengwenyu.top/gtargllsli.html

[M06] 向标准错误输出
来源：http://hz.iojbl.cn/gtozyjgmnb.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ivvv.top/gthgsfqmek.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.gzhubu.top/gtallaidsd.html

JS:   console.error("err")
来源：http://hz.52xcode.cn/gttobtitdr.html

TS:   console.error("err")
来源：http://hz.hammf.cn/gtkymqhwwd.html

Java: System.err.println("err")
来源：http://hz.ehwqpu.com/gtbkckbfaf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.hfpthk.cn/gtjrvqqhcw.html

Ruby: warn "err"
来源：http://hz.iojbl.cn/gtvqpyqego.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jqgufenzy.top/gtlehxgiwl.html

[M07] 判断是否为主入口
来源：http://hz.nwbrower.top/gtxgvlxacr.html

Py:   if __name__ == "__main__":
来源：http://hz.zhaomingkeji.xyz/gtywjpgrqk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shzxlz.cn/gtupxbcroj.html

JS:   require.main === module
来源：http://hz.pycfn.com/gtutdlidhe.html

TS:   require.main === module
来源：http://hz.havefunace.top/gtonnltlho.html

Java: public static void main(String[] args)
来源：http://hz.nanxuanxn.top/gttzurvlhy.html

Go:   func main()
来源：http://hz.aibaodan.cn/gtnpehpxni.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.tian-w.cn/gteantvyhv.html

C#:   static void Main(string[] args)
来源：http://hz.havefunace.top/gtjzipxbtn.html

[M08] 获取系统与运行时信息
来源：http://hz.gogol.net.cn/gtpxmqyicn.html

Py:   platform.system();  platform.python_version()
来源：http://hz.9152youxi.cn/gtonxlolmi.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yvedp.cn/gtyoftppox.html

JS:   process.platform;  process.version
来源：http://hz.wangdashe.top/gtmdmfgkpb.html

TS:   process.platform;  process.version
来源：http://hz.dashuyun.cn/gtygkhhznm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.dashuyun.cn/gtoxeqdkbm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.mhx1999.top/gtxmocurcb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yj20258.top/gtqxztceut.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.shzxlz.cn/gtxaqoqsra.html

================================================================================
来源：http://hz.zhengqikj.top/gthutqnygx.html

N. 数据结构与算法
来源：http://hz.shuidangran.top/gtnfyqjmkb.html

================================================================================
来源：http://hz.bjfxy.top/gtvzduwxec.html

[N01] 二分查找（有序数组）
来源：http://hz.jqgfzy.top/gtdxwivrlb.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.haohaochexian.top/gtenzhfmip.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.guannengcc.top/gtwgjbqonk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gogol.net.cn/gtvkhvrfzv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.kuanghao11.cn/gtmojqcbtc.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jinyuanbaomall.cn/gtbxgnabog.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jinqigfzy.top/gtsxspssvs.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.nanxuanxn.top/gtkepwvsze.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.nanxuanxn.top/gththrqnwf.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.sufxvd.cn/gtvsjiupes.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gotoacloud.top/gtvoicqayf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.guannengcc.top/gtdztewwuu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xziqi.cn/gtoqyndgxr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.chenjidiqi.icu/gtnahetwej.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.xingfuxueyuan.xyz/gtdfxesqla.html

Go:   slices.Sort(arr)
来源：http://hz.nanxinkj.top/gtmmpchtxl.html

Ruby: arr.sort
来源：http://hz.chenlongwang.top/gtscuenqtr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.sxryk.cn/gtejpiptse.html

[N03] 快速排序（分治示例）
来源：http://hz.dashuyun.cn/gtghxwqaew.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ydzc1.top/gtmsfykdcu.html

PHP:  // 递归实现，或用 usort
来源：http://hz.vqdsnc.cn/gtghcnmril.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cucudq.cn/gtircdxqgl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gotoacloud.top/gtrlaqnqno.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.shanyushiyangkeji.top/gthakouvsu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.cqqwz.cn/gtyujknlbq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.birdmap.top/gtzrtrywbx.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.svipenyu.cn/gtkqiuvoha.html

[N04] 斐波那契数列
来源：http://hz.kuanghao11.cn/gtudblzcfj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.svipenyu.cn/gtonbrbgsk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.bjfxy.top/gtcywvptar.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.daxiang520.top/gtlzdeytub.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.andypj.xyz/gtdlmdjzoj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.wangdashe.top/gtpuuzkzlz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.c1oappe.top/gtybiplqjv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.haohaochexian.top/gtwxujitih.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhaomingkeji.xyz/gtiphobvvd.html

[N05] 最大公约数
来源：http://hz.smart0.xyz/gtquxptwvw.html

Py:   math.gcd(a, b)
来源：http://hz.cucudq.cn/gtqaymlnax.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shanyushiyangkeji.top/gtmllmpzyr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cdnleiting.top/gtpauhwgxn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhixingplan.top/gtplnibvfp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.guannengcc.top/gtcyztygvy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.sufxvd.cn/gtwvmidhjy.html

Ruby: a.gcd(b)
来源：http://hz.hysaishi.cn/gtdfrqzrkx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.quarkkingdee.top/gtnivzanmk.html

[N06] 判断回文字符串
来源：http://hz.yangfankeji.com/gtgcgggbxn.html

Py:   s == s[::-1]
来源：http://hz.xinyue.icu/gtjugwzqha.html

PHP:  $s === strrev($s);
来源：http://hz.snrcjt.cn/gtzoudfccc.html

JS:   s === [...s].reverse().join("")
来源：http://hz.dianchejie.cn/gtanyigavj.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yuanzhike.top/gtvbuwdzfd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.gogol.net.cn/gtwvwlyzts.html

Go:   // 双指针从两端比较
来源：http://hz.yj202588.top/gtyyzqjtgl.html

Ruby: s == s.reverse
来源：http://hz.svipenyu.cn/gtfflcnltq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ivvv.top/gtzqfddhwu.html

[N07] 两数之和（返回下标）
来源：http://hz.haohaochexian.top/gtlmnhvqgi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yvedp.cn/gthqgzaffj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.chenzaomai.com/gtrrlyrjri.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yanxiufei.cn/gtajjzrily.html

TS:   // 手写 Map<string, number>
来源：http://hz.yuanzhike.top/gtckxqtokk.html

Java: // 手写 HashMap
来源：http://hz.gaohongyu789.top/gtinikfsxq.html

Go:   // 手写 map[int]int
来源：http://hz.kuanghao11.cn/gtjktpocek.html

Ruby: // 手写 Hash
来源：http://hz.daxiang520.top/gtnvatsany.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zhongyouzk.top/gtwmnwonfd.html

[N08] 生成全排列
来源：http://hz.tianlin.xyz/gtzvorthlv.html

Py:   itertools.permutations(arr)
来源：http://hz.yonumen.top/gtwbjdlgws.html

PHP:  // 手写递归交换
来源：http://hz.chenzaomai.com/gtqpykmcni.html

JS:   // 手写回溯递归
来源：http://hz.yj20258888.top/gtjfevjpza.html

TS:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtnfzxgpsg.html

Java: // 手写回溯递归
来源：http://hz.xylfe.cn/gtrrlnwcpu.html

Go:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtcpkpnhqf.html

Ruby: arr.permutation.to_a
来源：http://hz.xuanzx.com/gtqrncgmac.html

C#:   // 手写回溯递归
来源：http://hz.sweek.top/gtwzhwwsmy.html

[N09] 栈与队列
来源：http://hz.jianghu66.top/gtpskpkxbo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jqgufenzy.top/gtzmkzxueo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yuanzhike.top/gtcjsbrwjg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.shuidangran.top/gtnkljbdmn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.nwbrower.top/gtxloemcpi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.mhx1999.top/gtjqjqbgtv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yj20258.top/gtjrocfalf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.cucudq.cn/gtjzvzynoj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.dashuyun.cn/gtzqhqhutr.html

[N10] 链表节点定义
来源：http://hz.andypj.xyz/gtfrlephjj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zdqjudy.top/gteawynimb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zdqjudy.top/gtnsdicdak.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.gogol.net.cn/gtwgsmnvrg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yanxiufei.cn/gtpbaolrnk.html

Java: class Node { int v; Node next; }
来源：http://hz.chenjidiqi.icu/gtqizuqxdd.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.daria6918.cn/gtojvidair.html


<!-- 参考信息 -->