代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yongpay.top/gtcyhbiisw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yuxming.cn/gtqswdtjmc.html

JS:   JSON.stringify(obj)
来源：http://hz.yonumen.top/gttgtwsntk.html

TS:   JSON.stringify(obj)
来源：http://hz.jqgfzy.top/gtkxvqrwut.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jqgufenzy.top/gtiygjcfag.html

Go:   json.Marshal(obj)
来源：http://hz.aizwys.cn/gtgrzgtvmx.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shanyushiyangtech.top/gteusgpniv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhengqikj.top/gtefqgwwvl.html

[K02] JSON 字符串转对象
来源：http://hz.yvedp.cn/gtilxhpgbz.html

Py:   json.loads(s)
来源：http://hz.cdnleiting.top/gtmmrdfcmz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.gaohongyu789.top/gtjbavzlwq.html

JS:   JSON.parse(s)
来源：http://hz.316326.xyz/gtnehunwxw.html

TS:   JSON.parse(s)
来源：http://hz.jinghuilouyu.cn/gtyxqbzarf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hysaishi.cn/gtjtowecys.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jyoumei.cn/gtzuqijhls.html

Ruby: JSON.parse(s)
来源：http://hz.xziqi.cn/gtyjjyfcbs.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.chenjidiqi.icu/gtyhzbzdca.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yj20258.top/gtybxyrilc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zycfv.cn/gtbzykzvcm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.sweek.top/gtlsfklhqi.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shangyingyoupin.top/gtbnvimkgn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hnxiangtu.top/gtazqsbcas.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ivvv.top/gtseqnmipi.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.smart0.xyz/gtluxifcib.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yonumen.top/gtuyofzsqq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhongyouzk.top/gtgftgwvgb.html

[K04] 读取 JSON 文件
来源：http://hz.havefunace.top/gtkhfrzrbo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.pengpengdd.cyou/gtwljqdtqa.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.tian-w.cn/gtofynylax.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.kuanghao11.cn/gttzikimwl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yongpay.top/gtjumzteyt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yangfankeji.com/gtukregwwy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.0kj1m.cn/gtdilfultn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.dashuyun.cn/gthhpgrlsv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.tanke756.top/gtnmqnfrmx.html

[K05] 深拷贝对象
来源：http://hz.gogol.net.cn/gtadhldayk.html

Py:   copy.deepcopy(obj)
来源：http://hz.xuetiantiany.cn/gtyvvymufh.html

PHP:  unserialize(serialize($obj));
来源：http://hz.snrcjt.cn/gtvmyvaods.html

JS:   structuredClone(obj)
来源：http://hz.zhixingplan.top/gtzdujooip.html

TS:   structuredClone(obj)
来源：http://hz.ehwqpu.com/gtzyluiooz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.shanyushiyangtech.top/gtizfgntgx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yvedp.cn/gtreyvhgdg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.iojbl.cn/gtohnxionw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.xziqi.cn/gtouvqboes.html

[K06] 解析 URL 查询串
来源：http://hz.hnqzz.top/gtdxvvdxdm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.sxryk.cn/gtjuztvqyc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yuxming.cn/gtnjctfkhs.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinyuanbaomall.cn/gtngqqmsrh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.aizwys.cn/gtvsesgqbg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.sysykeji.top/gtlhgzhszi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.xylfe.cn/gtloavoevo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jinghuilouyu.cn/gtrxqgeuss.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ydjk.org.cn/gtilxdjdkv.html

[K07] 进制转换
来源：http://hz.vqdsnc.cn/gttzmcktqw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hfpthk.cn/gtagjcuorx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.daria6918.cn/gtznywgyqh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yj20258888.top/gtwmxddvwj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ybcxt.top/gtcwooqaux.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ppjwa.cn/gtgpgxqzsw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yj202588.top/gtbdgrulio.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.gogol.net.cn/gtrlfljspk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.sxryk.cn/gthrdwxedp.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yueranfly.top/gtiemsvcjd.html

Py:   pickle.dumps(obj)
来源：http://hz.zhongyouzk.top/gtkiltugec.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.tanke756.top/gtvtwegnth.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shangyingyoupin.top/gttqeyyczz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.gzhubu.top/gtkleoelbo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.dianchejie.cn/gtckjjtbnz.html

Go:   encoding/gob
来源：http://hz.tanke756.top/gtfplympkq.html

Ruby: Marshal.dump(obj)
来源：http://hz.shangyingyoupin.top/gtykpgscnp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yueranfly.top/gtosxvtlzu.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtrcpgmdtz.html

L. 网络请求
来源：http://hz.xingfuxueyuan.xyz/gtivcnvhyy.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtvvqhnpdz.html

[L01] 发送 GET 请求
来源：http://hz.smart0.xyz/gteylhxthn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.fzhhl.top/gtcoqearlp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.iojbl.cn/gtijamyjib.html

JS:   await fetch(url)
来源：http://hz.fzhhl.top/gtpoejeuus.html

TS:   await fetch(url)
来源：http://hz.guowangkeji.top/gtzovgambo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ydzc1.top/gtzdoqjrjz.html

Go:   resp, err := http.Get(url)
来源：http://hz.dashuyun.cn/gtzvwcqbdj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.snrcjt.cn/gtkgqvhgif.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.52xcode.cn/gtgqltvwjy.html

[L02] 发送 POST JSON
来源：http://hz.guowangkeji.top/gtmfvimdds.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhoulong.xyz/gthlzoasbw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.vqdsnc.cn/gtcyinmtgj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.birdmap.top/gtwumdsxpd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tianlin.xyz/gtqskmydnd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.cheryme.top/gttihvfvxa.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xziqi.cn/gtqymfryvg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zdqjudy.top/gtonjdfnkx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yonumen.top/gttycwdzzu.html

[L03] 设置自定义请求头
来源：http://hz.gotoacloud.top/gtamxvugcp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yj20258.top/gtjwdbsipr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zhixingplan.top/gtwrhlvnlk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.aibaodan.cn/gtrqwpglxh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.mhx1999.top/gtfgjnnlma.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.nwbrower.top/gtoolfdutp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yj20258.top/gtutilkjnh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jianghu66.top/gtuogwsiuf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yueranfly.top/gtyztoodcd.html

[L04] 设置超时
来源：http://hz.aibaodan.cn/gtqrnxdgcw.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ydzc1.top/gtukslrwuh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.shzxlz.cn/gtlufbhykp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.chenzaomai.com/gtgwmppxzz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yongpay.top/gtybnfoakw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.haohaochexian.top/gtvgvplwbk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.sufxvd.cn/gtolbcxxhe.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.redwolf501.top/gtdejqkzmp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.cheryme.top/gtofivdpyo.html

[L05] 上传文件（multipart）
来源：http://hz.zhaomingkeji.xyz/gtpepdljhb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.fzhhl.top/gthxljnghf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.snrcjt.cn/gtoduzxkvi.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.pycfn.com/gtrjjfurly.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yuxming.cn/gtsdjavjda.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ywan-chungtsiang.top/gtggeuaoqa.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.gaohongyu789.top/gtefuciqei.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jinghuilouyu.cn/gteopjueto.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.guannengcc.top/gtrqdpcgok.html

[L06] 解析响应为 JSON
来源：http://hz.yueranfly.top/gtjfnsggmm.html

Py:   resp.json()
来源：http://hz.cucudq.cn/gtzgjlhnjn.html

PHP:  json_decode($body, true);
来源：http://hz.hfpthk.cn/gtbgujkjha.html

JS:   await resp.json()
来源：http://hz.zhoulong.xyz/gtthqzfara.html

TS:   await resp.json()
来源：http://hz.gotoacloud.top/gtbntoctns.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.meibo888.top/gtjlsselkx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.aizwys.cn/gtcybnanel.html

Ruby: JSON.parse(resp.body)
来源：http://hz.smart0.xyz/gtvezmrtsz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.guowangkeji.top/gtpjjtoatm.html

[L07] 处理 HTTP 状态码
来源：http://hz.ywan-chungtsiang.top/gtdkwfsisb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.tian-w.cn/gtygntvlko.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhijiandao.cn/gtbadmserr.html

JS:   resp.ok;  resp.status
来源：http://hz.jianghu66.top/gtwgfacbiq.html

TS:   resp.ok;  resp.status
来源：http://hz.chenzaomai.com/gtspfihcnp.html

Java: resp.statusCode()
来源：http://hz.guowangkeji.top/gtqgmhadbr.html

Go:   resp.StatusCode
来源：http://hz.chenzaomai.com/gtbojpnjox.html

Ruby: resp.code.to_i
来源：http://hz.zhongyouzk.top/gtzvyknyts.html

C#:   (int)resp.StatusCode
来源：http://hz.nanxuanxn.top/gtfvbzxgdd.html

[L08] 并发请求多个地址
来源：http://hz.zhaomingkeji.xyz/gtajrzqxds.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ehwqpu.com/gtqdulnynl.html

PHP:  curl_multi_init() 系列
来源：http://hz.nanxinkj.top/gtzpjymeeu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.havefunace.top/gtrqoxzzag.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhengqikj.top/gtydpwueed.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.cqqwz.cn/gtixndfjdq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hysaishi.cn/gtfynezvoh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jinqigufen.top/gtwpplriss.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.cdnleiting.top/gtmkfapjaw.html

================================================================================
来源：http://hz.gzhubu.top/gtuboyaqrc.html

M. 命令行 / 进程 / 环境
来源：http://hz.jlsjyb.cn/gttfeplycb.html

================================================================================
来源：http://hz.zdqjudy.top/gtbuxpgqhq.html

[M01] 读取命令行参数
来源：http://hz.svipenyu.cn/gtezxryjup.html

Py:   sys.argv[1:]
来源：http://hz.nanxuanxn.top/gtuwkqnjdo.html

PHP:  $argv;  $argc;
来源：http://hz.hysaishi.cn/gtvmtogacj.html

JS:   process.argv.slice(2)
来源：http://hz.birdmap.top/gtlkbnovob.html

TS:   process.argv.slice(2)
来源：http://hz.havefunace.top/gtmypdvpxj.html

Java: args 数组（main 方法参数）
来源：http://hz.xuetiantiany.cn/gtcdncibry.html

Go:   os.Args[1:]
来源：http://hz.smart0.xyz/gtbiougafp.html

Ruby: ARGV
来源：http://hz.aibaodan.cn/gtilxcuysj.html

C#:   args 数组（Main 方法参数）
来源：http://hz.wangshuangyany.cn/gtgpjzycos.html

[M02] 读取环境变量
来源：http://hz.aibaodan.cn/gtfcbhbwzj.html

Py:   os.environ.get("HOME")
来源：http://hz.guowangkeji.top/gtbwgavkmg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.tian-w.cn/gtjlyznrah.html

JS:   process.env.HOME
来源：http://hz.yuxming.cn/gtyifrwjyz.html

TS:   process.env.HOME
来源：http://hz.yonumen.top/gtiwcfvwvv.html

Java: System.getenv("HOME")
来源：http://hz.zhijiandao.cn/gtslpniilh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jianghu66.top/gtugqzfkkb.html

Ruby: ENV["HOME"]
来源：http://hz.pycfn.com/gtzftxinlq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hnqzz.top/gtfsaixpid.html

[M03] 执行外部命令
来源：http://hz.shangyingyoupin.top/gtyoastkzn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.shangyingyoupin.top/gtmidqdfzh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.aibaodan.cn/gtrsvtnyyc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinghuilouyu.cn/gtkkspmboj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.sweek.top/gtvfzqsrxy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hfpthk.cn/gtaxlqdyjo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.fengsongda.top/gtmyvmdgcf.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shanyushiyangtech.top/gtdykwzymj.html

C#:   Process.Start("ls", "-l");
来源：http://hz.0kj1m.cn/gtuhoeqtsw.html

[M04] 获取当前工作目录
来源：http://hz.svipenyu.cn/gtarcwkodd.html

Py:   os.getcwd()
来源：http://hz.xuetiantiany.cn/gtqtuzlpmn.html

PHP:  getcwd();
来源：http://hz.mhx1999.top/gteqhzpsuy.html

JS:   process.cwd()
来源：http://hz.cashguo.top/gtlxpzeezz.html

TS:   process.cwd()
来源：http://hz.gzhubu.top/gtovhsyrki.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhoulong.xyz/gtmanbxdbv.html

Go:   os.Getwd()
来源：http://hz.yj20258.top/gtzjmjeqzx.html

Ruby: Dir.pwd
来源：http://hz.iojbl.cn/gtugswkssw.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.chenlongwang.top/gtnzcharte.html

[M05] 设置退出码
来源：http://hz.cheryme.top/gtvpcqcemk.html

Py:   sys.exit(1)
来源：http://hz.mhx1999.top/gtxhetnpyp.html

PHP:  exit(1);
来源：http://hz.jinghuilouyu.cn/gtglimbtux.html

JS:   process.exit(1)
来源：http://hz.jqgfzy.top/gtawyhusxz.html

TS:   process.exit(1)
来源：http://hz.ybcxt.top/gtspnogomg.html

Java: System.exit(1)
来源：http://hz.yvedp.cn/gtspcslnty.html

Go:   os.Exit(1)
来源：http://hz.xylfe.cn/gtstlwfanm.html

Ruby: exit 1
来源：http://hz.dashuyun.cn/gtdvgduzvz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.hysaishi.cn/gteiznjtla.html

[M06] 向标准错误输出
来源：http://hz.shangyingyoupin.top/gtumueakpd.html

Py:   print("err", file=sys.stderr)
来源：http://hz.nanxuanxn.top/gtzkmzzevv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yonumen.top/gtjwjydvmt.html

JS:   console.error("err")
来源：http://hz.sufxvd.cn/gtwrfcofgk.html

TS:   console.error("err")
来源：http://hz.jlsjyb.cn/gtqpvjlred.html

Java: System.err.println("err")
来源：http://hz.yuxming.cn/gtjvutoiuy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.kuanghao11.cn/gtughmlnrw.html

Ruby: warn "err"
来源：http://hz.xylfe.cn/gtuzumrxdt.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yj202588.top/gtzriptjaa.html

[M07] 判断是否为主入口
来源：http://hz.yuxming.cn/gtvqnqiebr.html

Py:   if __name__ == "__main__":
来源：http://hz.sufxvd.cn/gtmrdzmski.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cashguo.top/gthbwtxdpy.html

JS:   require.main === module
来源：http://hz.jiagoushi.top/gtohkkjbts.html

TS:   require.main === module
来源：http://hz.gogol.net.cn/gtuhefbypd.html

Java: public static void main(String[] args)
来源：http://hz.tianlin.xyz/gtwyynxvym.html

Go:   func main()
来源：http://hz.feifeiyinyue.top/gtzjkxnrno.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jqgfzy.top/gtkhulcaag.html

C#:   static void Main(string[] args)
来源：http://hz.tianlin.xyz/gtzqiokajq.html

[M08] 获取系统与运行时信息
来源：http://hz.ywan-chungtsiang.top/gthxvscuvl.html

Py:   platform.system();  platform.python_version()
来源：http://hz.kuanghao11.cn/gtmeokjajb.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yueranfly.top/gtwtueysqq.html

JS:   process.platform;  process.version
来源：http://hz.chenjidiqi.icu/gtpeuctjwo.html

TS:   process.platform;  process.version
来源：http://hz.chenlongwang.top/gtkvcukcqx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yueranfly.top/gtrnjrcfrc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.aibaodan.cn/gtwcolibad.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.xuetiantiany.cn/gtuposkvwx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.haohaochexian.top/gtgiexybqp.html

================================================================================
来源：http://hz.zhengqikj.top/gtugjqfuie.html

N. 数据结构与算法
来源：http://hz.havefunace.top/gtsdfmbnwr.html

================================================================================
来源：http://hz.havefunace.top/gtxazypiet.html

[N01] 二分查找（有序数组）
来源：http://hz.xziqi.cn/gtjxaniask.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.shuidangran.top/gtrbcfucjg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zdqjudy.top/gtwrndwpyr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shangyingyoupin.top/gtqcrvsnme.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.fzhhl.top/gtsjezegoa.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hongshengwenyu.top/gtohqtpxzc.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.smart0.xyz/gtpoogragk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ivvv.top/gtyzqukdex.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.gzhubu.top/gtfqzzznbp.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ivvv.top/gtfjoekxpo.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhengqikj.top/gtnfqeckga.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.sweek.top/gtazokzodz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yonumen.top/gtreyhtgay.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.chenjidiqi.icu/gtooolefqk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.chenlongwang.top/gtwwmoaakr.html

Go:   slices.Sort(arr)
来源：http://hz.zhixingplan.top/gtktezvpng.html

Ruby: arr.sort
来源：http://hz.jinghuilouyu.cn/gtfskdsboz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jinqigufen.top/gtjfynppzh.html

[N03] 快速排序（分治示例）
来源：http://hz.pycfn.com/gtulykamsa.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.nanxinkj.top/gtsvjrrrof.html

PHP:  // 递归实现，或用 usort
来源：http://hz.guowangkeji.top/gtcwbkchau.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ydjk.org.cn/gtjlqhtrme.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.havefunace.top/gtbxzpilaq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.xingfuxueyuan.xyz/gtrjrduwdi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.wangshuangyany.cn/gtgylczqfv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hammf.cn/gtnprpylmo.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.c1oappe.top/gtlgfhyazm.html

[N04] 斐波那契数列
来源：http://hz.hongshengwenyu.top/gtblcxhvyq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.dashuyun.cn/gtlplpxjwk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.snrcjt.cn/gtjpxdymfk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhiwuduotai.top/gtxgcyqvgy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hongshengwenyu.top/gthlccltjf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.gaohongyu789.top/gtugajzuac.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhengqikj.top/gtmdapfxfp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.feifeiyinyue.top/gtikepxqyg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.chenzaomai.com/gtrnkqmpco.html

[N05] 最大公约数
来源：http://hz.vqdsnc.cn/gtojbqstmf.html

Py:   math.gcd(a, b)
来源：http://hz.hongshengwenyu.top/gtfxqlatyw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zhaomingkeji.xyz/gtehjhmdak.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.redwolf501.top/gtzilmqrmi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.tianlin.xyz/gtvnazfxni.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hywenlv.cn/gtevfexqgy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.andypj.xyz/gtlcrxpgay.html

Ruby: a.gcd(b)
来源：http://hz.zycfv.cn/gtqsmobgqt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.gzhubu.top/gtxpxyxrxa.html

[N06] 判断回文字符串
来源：http://hz.yj20258.top/gtmganclsh.html

Py:   s == s[::-1]
来源：http://hz.jinqigufen.top/gtamfdpzef.html

PHP:  $s === strrev($s);
来源：http://hz.birdmap.top/gtcyfsrsvc.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhengqikj.top/gtvjzymkcq.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yvedp.cn/gtjskjmcxc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.pycfn.com/gtgcsccdze.html

Go:   // 双指针从两端比较
来源：http://hz.shangyingyoupin.top/gtskyashiw.html

Ruby: s == s.reverse
来源：http://hz.chenzaomai.com/gtkucgaxas.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jinqigfzy.top/gtcswypxuf.html

[N07] 两数之和（返回下标）
来源：http://hz.haohaochexian.top/gtzmprivti.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yj20258.top/gtskobqcet.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.ydzc1.top/gtpqibqsqr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.daxiang520.top/gtxlyiwzeg.html

TS:   // 手写 Map<string, number>
来源：http://hz.tian-w.cn/gtlwmlkebl.html

Java: // 手写 HashMap
来源：http://hz.fzhhl.top/gtjsawnpbj.html

Go:   // 手写 map[int]int
来源：http://hz.yonumen.top/gtznofxwwy.html

Ruby: // 手写 Hash
来源：http://hz.smart0.xyz/gtgthhqhkd.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.ivvv.top/gtseohregd.html

[N08] 生成全排列
来源：http://hz.iojbl.cn/gtxdgvuuss.html

Py:   itertools.permutations(arr)
来源：http://hz.52xcode.cn/gtkgkzvatc.html

PHP:  // 手写递归交换
来源：http://hz.zhixingplan.top/gtdnuegbkk.html

JS:   // 手写回溯递归
来源：http://hz.shzxlz.cn/gtldkrnqzj.html

TS:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gttufkryhg.html

Java: // 手写回溯递归
来源：http://hz.xylfe.cn/gtsurwcctm.html

Go:   // 手写回溯递归
来源：http://hz.wangshuangyany.cn/gtuwqviumk.html

Ruby: arr.permutation.to_a
来源：http://hz.snrcjt.cn/gtwsdsujks.html

C#:   // 手写回溯递归
来源：http://hz.redwolf501.top/gtzjsczodm.html

[N09] 栈与队列
来源：http://hz.dashuyun.cn/gtwlwkdtah.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ybcxt.top/gtmcurgosu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.chenzaomai.com/gtgkrwgpch.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.shangyingyoupin.top/gtlopqlppd.html


<!-- 参考信息 -->