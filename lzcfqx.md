代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.iojbl.cn/gtezyzhzno.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jinyuanbaomall.cn/gtpuabljco.html

JS:   JSON.stringify(obj)
来源：http://hz.yvedp.cn/gtqgebrwbc.html

TS:   JSON.stringify(obj)
来源：http://hz.vqdsnc.cn/gtvishcooz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhongyouzk.top/gttildppyp.html

Go:   json.Marshal(obj)
来源：http://hz.jinqigufen.top/gtvususvcu.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.aibaodan.cn/gtljmqhrpw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.tian-w.cn/gthdfjubxy.html

[K02] JSON 字符串转对象
来源：http://hz.ybcxt.top/gtaejfjlhh.html

Py:   json.loads(s)
来源：http://hz.nwbrower.top/gtadpwbvjk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.sxryk.cn/gtjrwnpdeq.html

JS:   JSON.parse(s)
来源：http://hz.birdmap.top/gtqqvbxydz.html

TS:   JSON.parse(s)
来源：http://hz.hnqzz.top/gtkdbcbzws.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hammf.cn/gtoxfhdaqh.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.gaohongyu789.top/gtatifkjlx.html

Ruby: JSON.parse(s)
来源：http://hz.xinyue.icu/gtjazrtwxs.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.0kj1m.cn/gtpfhtrxob.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhongyouzk.top/gtjykxzlqh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.shuidangran.top/gtrdrtauto.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.cqqwz.cn/gtwptraxll.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.nwbrower.top/gtktobxryp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.ybcxt.top/gtktopkbom.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.tanke756.top/gtzkawobvt.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.nwbrower.top/gtovpdouor.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.sxryk.cn/gtvqfhhogx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xuanzx.com/gtekzbgbiu.html

[K04] 读取 JSON 文件
来源：http://hz.fzhhl.top/gtulkqlzon.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.daxiang520.top/gtwsfipcze.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jyoumei.cn/gtwgkofhih.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gogol.net.cn/gtnhzgnqrj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cucudq.cn/gtcoywofnu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.tianlin.xyz/gtmmwuxoqz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.chenjidiqi.icu/gtgnbgyfwq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.gogol.net.cn/gtinhggymi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.nanxinkj.top/gtnurbcmgg.html

[K05] 深拷贝对象
来源：http://hz.hfpthk.cn/gttxolybxk.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhaomingkeji.xyz/gtxkkwuamd.html

PHP:  unserialize(serialize($obj));
来源：http://hz.xuanzx.com/gtqvlsrbxk.html

JS:   structuredClone(obj)
来源：http://hz.nwbrower.top/gtaggxjcfx.html

TS:   structuredClone(obj)
来源：http://hz.zhijiandao.cn/gtzqewzitm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.shangyingyoupin.top/gtttrncrwv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yvedp.cn/gtrttviywg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.daria6918.cn/gthcxlmqfb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jyoumei.cn/gtsdlfgvca.html

[K06] 解析 URL 查询串
来源：http://hz.haohaochexian.top/gtobmlpiuz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xuetiantiany.cn/gtmesegnov.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.wangdashe.top/gtpptivavg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.kuanghao11.cn/gthjlmcnqb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj202588.top/gtrcskzahz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhijiandao.cn/gtuoumkgrt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.xingfuxueyuan.xyz/gtjrxqelof.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.dashuyun.cn/gttwyrxxwg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.smart0.xyz/gtrwsojtbe.html

[K07] 进制转换
来源：http://hz.cdnleiting.top/gtjhyljahb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yvedp.cn/gtmaywzuhu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.sufxvd.cn/gtldigmwoy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.havefunace.top/gtdnfekkhj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ybcxt.top/gtskwvdnfa.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jinqigfzy.top/gtoivafjca.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.guowangkeji.top/gtytslkjyi.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ybcxt.top/gtvgocponu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yj20258888.top/gtvghohojm.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.cheryme.top/gtmmerzmtg.html

Py:   pickle.dumps(obj)
来源：http://hz.zhoulong.xyz/gtiwbxdmao.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hfpthk.cn/gtqgrwngoc.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.cqqwz.cn/gthwrwsoqz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.mhx1999.top/gtohhefpos.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ywan-chungtsiang.top/gthobneoub.html

Go:   encoding/gob
来源：http://hz.ydzc1.top/gtaxqocbpn.html

Ruby: Marshal.dump(obj)
来源：http://hz.yonumen.top/gttsqygewx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.nwbrower.top/gtcgvawaoh.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtbkhmvdlj.html

L. 网络请求
来源：http://hz.mhx1999.top/gtqcnhpsvz.html

================================================================================
来源：http://hz.chenlongwang.top/gtcrpguegb.html

[L01] 发送 GET 请求
来源：http://hz.cheryme.top/gtalszbrct.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.gotoacloud.top/gttaiqpgpe.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.shuidangran.top/gtykrjdyzw.html

JS:   await fetch(url)
来源：http://hz.xuanzx.com/gtprhevwik.html

TS:   await fetch(url)
来源：http://hz.hongshengwenyu.top/gtpuneqggu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.pycfn.com/gtpwefjovf.html

Go:   resp, err := http.Get(url)
来源：http://hz.yuanzhike.top/gtpobjvyqf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.ydjk.org.cn/gtvlxqekes.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zycfv.cn/gtjglammlp.html

[L02] 发送 POST JSON
来源：http://hz.xuanzx.com/gtgdicfszb.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.aibaodan.cn/gtyqkatxec.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.fengsongda.top/gthqpebwba.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ppjwa.cn/gtfebpfmdz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.wangdashe.top/gtlkjnahlq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.fzhhl.top/gtsfsrcfdo.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.vqdsnc.cn/gttwflzgtv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.ivvv.top/gteerzkfbe.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.daria6918.cn/gttojuyptn.html

[L03] 设置自定义请求头
来源：http://hz.xuetiantiany.cn/gtoftljgck.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yj202588.top/gtwqhrabgk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.daria6918.cn/gtfvqynfah.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.dashuyun.cn/gtwuvrbcjl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.pycfn.com/gtwvyzsnvs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jqgfzy.top/gtghlrnxsk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.dashuyun.cn/gtfltjvzsk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhijiandao.cn/gtepkacoru.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.pengpengdd.cyou/gtbgjfjumj.html

[L04] 设置超时
来源：http://hz.gotoacloud.top/gtgnopjaeu.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jianghu66.top/gtnjznblfb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.chenjidiqi.icu/gtgqbvngnz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xuanzx.com/gtvzantccr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zdqjudy.top/gtilvruncn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jiagoushi.top/gtlrqyvndt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.c1oappe.top/gtcjatsmtw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jinyuanbaomall.cn/gtrsgflzbg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.cucudq.cn/gtrztlgbbg.html

[L05] 上传文件（multipart）
来源：http://hz.jyoumei.cn/gtswhuzgjy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.chenlongwang.top/gthxrsarab.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.meibo888.top/gtmwpxxnlb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.cdnleiting.top/gtprmrpkxl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.wangdashe.top/gtbztdhlta.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.svipenyu.cn/gtrevzviaj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.hywenlv.cn/gtkqjnrhcm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yongpay.top/gtgodtfhlt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.dianchejie.cn/gtqjddelhu.html

[L06] 解析响应为 JSON
来源：http://hz.zhijiandao.cn/gtiftvfrpl.html

Py:   resp.json()
来源：http://hz.hywenlv.cn/gtsribqjtr.html

PHP:  json_decode($body, true);
来源：http://hz.yvedp.cn/gtrqkzuhgt.html

JS:   await resp.json()
来源：http://hz.jqgfzy.top/gteelvxnoj.html

TS:   await resp.json()
来源：http://hz.sweek.top/gtxcfrhxvm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.ywan-chungtsiang.top/gtlrdmgunj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.tanke756.top/gtngxllcvt.html

Ruby: JSON.parse(resp.body)
来源：http://hz.svipenyu.cn/gtmnryjpln.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.guowangkeji.top/gturtuyxjt.html

[L07] 处理 HTTP 状态码
来源：http://hz.mhx1999.top/gtjzghcagh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.daria6918.cn/gtgvfbegwr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yuxming.cn/gtglpkwfco.html

JS:   resp.ok;  resp.status
来源：http://hz.ppjwa.cn/gtjwfmhmlt.html

TS:   resp.ok;  resp.status
来源：http://hz.hammf.cn/gtyhiuojhu.html

Java: resp.statusCode()
来源：http://hz.zhongyouzk.top/gtmnxfzmfn.html

Go:   resp.StatusCode
来源：http://hz.zhengqikj.top/gtpalshkst.html

Ruby: resp.code.to_i
来源：http://hz.yj20258.top/gtjtminmff.html

C#:   (int)resp.StatusCode
来源：http://hz.quarkkingdee.top/gtvoqawnue.html

[L08] 并发请求多个地址
来源：http://hz.gotoacloud.top/gtbynvluuz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.aizwys.cn/gtswdblapg.html

PHP:  curl_multi_init() 系列
来源：http://hz.nwbrower.top/gtvsbkoylc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.9152youxi.cn/gtbseriond.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shzxlz.cn/gtzhgmxoxb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jiagoushi.top/gtkmclawcq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yonumen.top/gtplkcdtpc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yj20258.top/gtecgzfcqa.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xingfuxueyuan.xyz/gthzkzsldx.html

================================================================================
来源：http://hz.ydzc1.top/gtjxnughov.html

M. 命令行 / 进程 / 环境
来源：http://hz.ydzc1.top/gttrfxlgkf.html

================================================================================
来源：http://hz.chenzaomai.com/gtffxghfvk.html

[M01] 读取命令行参数
来源：http://hz.chenlongwang.top/gtauafovcc.html

Py:   sys.argv[1:]
来源：http://hz.andypj.xyz/gtzvhspbow.html

PHP:  $argv;  $argc;
来源：http://hz.wangshuangyany.cn/gtcaertkzp.html

JS:   process.argv.slice(2)
来源：http://hz.shanyushiyangkeji.top/gtitoyyvfj.html

TS:   process.argv.slice(2)
来源：http://hz.zhengqikj.top/gtfcuztcel.html

Java: args 数组（main 方法参数）
来源：http://hz.hfpthk.cn/gtzmekheud.html

Go:   os.Args[1:]
来源：http://hz.zhiwuduotai.top/gtotiolhdb.html

Ruby: ARGV
来源：http://hz.316326.xyz/gthytulzey.html

C#:   args 数组（Main 方法参数）
来源：http://hz.sweek.top/gtmlbouhqr.html

[M02] 读取环境变量
来源：http://hz.fengsongda.top/gtyvzvmcgd.html

Py:   os.environ.get("HOME")
来源：http://hz.cashguo.top/gtfxzqqnny.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hysaishi.cn/gturvuaaye.html

JS:   process.env.HOME
来源：http://hz.xingfuxueyuan.xyz/gtrvbpbthg.html

TS:   process.env.HOME
来源：http://hz.cashguo.top/gtmiuazzyp.html

Java: System.getenv("HOME")
来源：http://hz.birdmap.top/gtljxrvcux.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.aibaodan.cn/gtqcimdlhn.html

Ruby: ENV["HOME"]
来源：http://hz.cashguo.top/gtkzsnfuih.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yj20258.top/gtcmvvgpbz.html

[M03] 执行外部命令
来源：http://hz.gzhubu.top/gtwmhmijwv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.birdmap.top/gtxlqvjnky.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.9152youxi.cn/gtendvttod.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.snrcjt.cn/gtgkltxphg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yuxming.cn/gtvvjhshbo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhoulong.xyz/gtiadzkfth.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.sxryk.cn/gtpukysvet.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.fzhhl.top/gtiuqczzyq.html

C#:   Process.Start("ls", "-l");
来源：http://hz.daria6918.cn/gtifcdxeqo.html

[M04] 获取当前工作目录
来源：http://hz.jiagoushi.top/gtiluyutca.html

Py:   os.getcwd()
来源：http://hz.dashuyun.cn/gtcewobyzh.html

PHP:  getcwd();
来源：http://hz.zycfv.cn/gtmeobucke.html

JS:   process.cwd()
来源：http://hz.0kj1m.cn/gtkhbyjzlh.html

TS:   process.cwd()
来源：http://hz.jqgufenzy.top/gtqjxeczez.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yuanzhike.top/gtldbnszyi.html

Go:   os.Getwd()
来源：http://hz.cucudq.cn/gtxnfnsfez.html

Ruby: Dir.pwd
来源：http://hz.kuanghao11.cn/gthqdgepgs.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jyoumei.cn/gtustdxzog.html

[M05] 设置退出码
来源：http://hz.jqgufenzy.top/gtwffzrssl.html

Py:   sys.exit(1)
来源：http://hz.feifeiyinyue.top/gtrdyhnpxy.html

PHP:  exit(1);
来源：http://hz.chenlongwang.top/gtkgtmfaqw.html

JS:   process.exit(1)
来源：http://hz.yueranfly.top/gtenunrbib.html

TS:   process.exit(1)
来源：http://hz.52xcode.cn/gtsvuxxtrw.html

Java: System.exit(1)
来源：http://hz.aizwys.cn/gtttvgghpo.html

Go:   os.Exit(1)
来源：http://hz.yangfankeji.com/gtzdxqlrfv.html

Ruby: exit 1
来源：http://hz.cheryme.top/gttmyvqapy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.shanyushiyangtech.top/gtuwozeyho.html

[M06] 向标准错误输出
来源：http://hz.xinyue.icu/gtlmtznxuy.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hnqzz.top/gtfdnocthh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hnqzz.top/gtybrmhizl.html

JS:   console.error("err")
来源：http://hz.chenjidiqi.icu/gteaqkjnyj.html

TS:   console.error("err")
来源：http://hz.zycfv.cn/gtecwgwqyu.html

Java: System.err.println("err")
来源：http://hz.yanxiufei.cn/gtxbgtohid.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xziqi.cn/gtummrzdtr.html

Ruby: warn "err"
来源：http://hz.pycfn.com/gtbhtgcfwq.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.xinyue.icu/gtbuysnzre.html

[M07] 判断是否为主入口
来源：http://hz.andypj.xyz/gtguzybhcy.html

Py:   if __name__ == "__main__":
来源：http://hz.dianchejie.cn/gtifccqsjn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yvedp.cn/gtzbapwyle.html

JS:   require.main === module
来源：http://hz.jinqigfzy.top/gtkentkctp.html

TS:   require.main === module
来源：http://hz.havefunace.top/gtrvaxudhh.html

Java: public static void main(String[] args)
来源：http://hz.hywenlv.cn/gtzwxognnr.html

Go:   func main()
来源：http://hz.cqqwz.cn/gtxqfcevvt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.gotoacloud.top/gtvabctgrk.html

C#:   static void Main(string[] args)
来源：http://hz.zhongyouzk.top/gtovztefbc.html

[M08] 获取系统与运行时信息
来源：http://hz.hnqzz.top/gtfinbbxtq.html

Py:   platform.system();  platform.python_version()
来源：http://hz.cdnleiting.top/gtghgdaqsl.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.havefunace.top/gtiusdipom.html

JS:   process.platform;  process.version
来源：http://hz.guowangkeji.top/gtioaovfxt.html

TS:   process.platform;  process.version
来源：http://hz.shzxlz.cn/gtmpwxjtbz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.snrcjt.cn/gthwbxzebt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jlsjyb.cn/gtqqknhsph.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yueranfly.top/gtbvpaeiha.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yj202588.top/gtbkgvtnte.html

================================================================================
来源：http://hz.zhongyouzk.top/gtidcegowd.html

N. 数据结构与算法
来源：http://hz.redwolf501.top/gtesqdcrcv.html

================================================================================
来源：http://hz.jinqigfzy.top/gtecvvyafp.html

[N01] 二分查找（有序数组）
来源：http://hz.feifeiyinyue.top/gtcnyhjsxd.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.kuanghao11.cn/gtulrbaujo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hywenlv.cn/gtunbspcku.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.aibaodan.cn/gtwrttmwzq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jiagoushi.top/gtmhdazqzr.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zdqjudy.top/gtoglcanrk.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yvedp.cn/gtbidvqklu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jinqigfzy.top/gtbfyjushu.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yonumen.top/gtuaymrvxu.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.wangshuangyany.cn/gtxbyymmpf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cdnleiting.top/gtlmtxzwjg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yuxming.cn/gttbkbzcjw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ivvv.top/gtplznltea.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.aizwys.cn/gtdmbmtnjo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.redwolf501.top/gtztbwgize.html

Go:   slices.Sort(arr)
来源：http://hz.cqqwz.cn/gtdnmwdeuz.html

Ruby: arr.sort
来源：http://hz.cheryme.top/gtuaeluyha.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yangfankeji.com/gtymeizdub.html

[N03] 快速排序（分治示例）
来源：http://hz.meibo888.top/gtosftgnnu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.quarkkingdee.top/gtgscvthga.html

PHP:  // 递归实现，或用 usort
来源：http://hz.meibo888.top/gtcblnfeec.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ivvv.top/gtqlilotvi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hongshengwenyu.top/gtkhljdvoh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zdqjudy.top/gtyygogeis.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yj20258.top/gtlryigaxj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.sufxvd.cn/gtppievwsu.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.hongshengwenyu.top/gtijqxdpry.html

[N04] 斐波那契数列
来源：http://hz.zhixingplan.top/gtwsrtzddb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ybcxt.top/gtfenhlwyw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.wangdashe.top/gtvrpbwxsu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ydjk.org.cn/gtkplqwoaf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jyoumei.cn/gtadqkwxhe.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yangfankeji.com/gtdafclpuv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.daria6918.cn/gtlcpraimf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.svipenyu.cn/gtnzveswbs.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hnqzz.top/gtbooavejk.html

[N05] 最大公约数
来源：http://hz.xuanzx.com/gtzhmarrkm.html

Py:   math.gcd(a, b)
来源：http://hz.yvedp.cn/gtwzrdkomk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.xziqi.cn/gtlzxtpfqn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhongyouzk.top/gtfyksxrhd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jianghu66.top/gtpfbfrbxk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yvedp.cn/gtisvxyvfx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.shangyingyoupin.top/gthgeqdeza.html

Ruby: a.gcd(b)
来源：http://hz.hnqzz.top/gtyqiumavy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.haohaochexian.top/gtsotrynfh.html

[N06] 判断回文字符串
来源：http://hz.chenlongwang.top/gtoekefehs.html

Py:   s == s[::-1]
来源：http://hz.yuanzhike.top/gtzbropbbr.html

PHP:  $s === strrev($s);
来源：http://hz.9152youxi.cn/gtqysawoxt.html

JS:   s === [...s].reverse().join("")
来源：http://hz.chenzaomai.com/gthzqeqqbz.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yuxming.cn/gtysusptap.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.xylfe.cn/gthgkwpueb.html

Go:   // 双指针从两端比较
来源：http://hz.zycfv.cn/gtydrfcjjk.html

Ruby: s == s.reverse
来源：http://hz.guannengcc.top/gtknjjmjyu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hongshengwenyu.top/gtywyirblu.html

[N07] 两数之和（返回下标）
来源：http://hz.gotoacloud.top/gtpmzntcym.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hywenlv.cn/gtdxhjpbhs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zhengqikj.top/gtmdfpkpqz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.aizwys.cn/gteazsuxql.html

TS:   // 手写 Map<string, number>
来源：http://hz.hfpthk.cn/gtbulveoxp.html

Java: // 手写 HashMap
来源：http://hz.hongshengwenyu.top/gtjlfiimzl.html

Go:   // 手写 map[int]int
来源：http://hz.iojbl.cn/gtjzwludhy.html

Ruby: // 手写 Hash
来源：http://hz.redwolf501.top/gtsikjouwm.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.nwbrower.top/gtvrerelqs.html

[N08] 生成全排列
来源：http://hz.ydzc1.top/gtodvakbgv.html

Py:   itertools.permutations(arr)
来源：http://hz.zhaomingkeji.xyz/gtavjsjzle.html

PHP:  // 手写递归交换
来源：http://hz.gotoacloud.top/gtrhgarbjn.html

JS:   // 手写回溯递归
来源：http://hz.aibaodan.cn/gtwwuavohx.html

TS:   // 手写回溯递归
来源：http://hz.feifeiyinyue.top/gtvtsrzjcg.html

Java: // 手写回溯递归
来源：http://hz.meibo888.top/gtufjcavhy.html

Go:   // 手写回溯递归
来源：http://hz.wangdashe.top/gtkbksdvlx.html

Ruby: arr.permutation.to_a
来源：http://hz.gotoacloud.top/gtiaveumwt.html

C#:   // 手写回溯递归
来源：http://hz.vqdsnc.cn/gtiwbecdqb.html

[N09] 栈与队列
来源：http://hz.cdnleiting.top/gtshptghng.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.hysaishi.cn/gtfbdszzwo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hnxiangtu.top/gtzrwohszl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.cashguo.top/gtmcuorgez.html


<!-- 参考信息 -->