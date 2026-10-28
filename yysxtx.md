代发 wailian999

================================================================================
来源：http://hz.hammf.cn/gtjtbdnupa.html

K. JSON 与序列化
来源：http://hz.zhoulong.xyz/gtqivizjtd.html

================================================================================
来源：http://hz.tanke756.top/gtauytvzsi.html

[K01] 对象转 JSON 字符串
来源：http://hz.andypj.xyz/gtgoxwrdxm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hongshengwenyu.top/gtygbupfne.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ydzc1.top/gtediriovv.html

JS:   JSON.stringify(obj)
来源：http://hz.wangshuangyany.cn/gthxlokbcl.html

TS:   JSON.stringify(obj)
来源：http://hz.zdqjudy.top/gtdwxuzlib.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.guannengcc.top/gtfslgqreb.html

Go:   json.Marshal(obj)
来源：http://hz.jinqigfzy.top/gttcvljocv.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.pycfn.com/gtxsmmcfpz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hywenlv.cn/gtinfwoblp.html

[K02] JSON 字符串转对象
来源：http://hz.xylfe.cn/gthccgcsru.html

Py:   json.loads(s)
来源：http://hz.chenlongwang.top/gtybdqnbcu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yj20258888.top/gtmfbenxyp.html

JS:   JSON.parse(s)
来源：http://hz.jlsjyb.cn/gtxoefswvz.html

TS:   JSON.parse(s)
来源：http://hz.ivvv.top/gtkxcahkfw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.0kj1m.cn/gtanmzobil.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.wangshuangyany.cn/gtjjbfqnce.html

Ruby: JSON.parse(s)
来源：http://hz.cashguo.top/gtwvldgkiu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.aizwys.cn/gtwpjfsqxc.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.gogol.net.cn/gtnzplacfb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.pengpengdd.cyou/gtmkirkkhj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jqgufenzy.top/gtftyvxily.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhixingplan.top/gtywdapmau.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.9152youxi.cn/gtukoonzrb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.bjfxy.top/gtewvoqkuz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zycfv.cn/gtqaunihvq.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.vqdsnc.cn/gtzgjkehiq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hnxiangtu.top/gtgdrjgpad.html

[K04] 读取 JSON 文件
来源：http://hz.yuanzhike.top/gtqatfhqiv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.feifeiyinyue.top/gtdnrejylh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.sweek.top/gthadfsksx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.316326.xyz/gtlmkicgfv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shuidangran.top/gtxufayhnm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.cashguo.top/gtyesibpyj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.316326.xyz/gtcjibskxl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.guowangkeji.top/gttwwiwzst.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.xuetiantiany.cn/gtcznewnax.html

[K05] 深拷贝对象
来源：http://hz.jiagoushi.top/gtzzskrriu.html

Py:   copy.deepcopy(obj)
来源：http://hz.redwolf501.top/gtacbbfzme.html

PHP:  unserialize(serialize($obj));
来源：http://hz.xuanzx.com/gtlxvbsyoz.html

JS:   structuredClone(obj)
来源：http://hz.fzhhl.top/gtdkdpmkir.html

TS:   structuredClone(obj)
来源：http://hz.jinyuanbaomall.cn/gtpalgsmcb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jqgufenzy.top/gtrupzsmog.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.aibaodan.cn/gtsxvmllgb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.guowangkeji.top/gthhmvkqhf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.tianlin.xyz/gthvzwzvek.html

[K06] 解析 URL 查询串
来源：http://hz.aizwys.cn/gtdshyclhs.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.cashguo.top/gtuytjpokd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.birdmap.top/gtcoxvopkm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shanyushiyangkeji.top/gtusiivauj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yvedp.cn/gtivclubfr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.dianchejie.cn/gtmasqcipu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.aibaodan.cn/gtmardtbud.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jinyuanbaomall.cn/gtyvkufnzv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yongpay.top/gtqlyjslsj.html

[K07] 进制转换
来源：http://hz.yangfankeji.com/gtpxdhbklh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.xinyue.icu/gtiipcbwly.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jyoumei.cn/gtfrclemcc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yj20258.top/gtilekvlge.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.chenlongwang.top/gtdctndzov.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xuanzx.com/gthncquspb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hnqzz.top/gtmmpowvdh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.daria6918.cn/gtdqpmqwfe.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ivvv.top/gthcdmcnli.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zycfv.cn/gtvapwunck.html

Py:   pickle.dumps(obj)
来源：http://hz.aizwys.cn/gtdwficrmi.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.birdmap.top/gtwsnbhrvy.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.redwolf501.top/gtofxhnrqn.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.cheryme.top/gtevfqgwru.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.cucudq.cn/gtzanlhnpf.html

Go:   encoding/gob
来源：http://hz.guowangkeji.top/gtrokqximv.html

Ruby: Marshal.dump(obj)
来源：http://hz.jqgfzy.top/gtxxasbxmw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.hammf.cn/gtkzckxizo.html

================================================================================
来源：http://hz.guowangkeji.top/gtdksgxqlx.html

L. 网络请求
来源：http://hz.ybcxt.top/gtblspflse.html

================================================================================
来源：http://hz.ivvv.top/gtpgsdfevx.html

[L01] 发送 GET 请求
来源：http://hz.zdqjudy.top/gtoeicqtmr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.svipenyu.cn/gtmedktkcg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.wangdashe.top/gtbxmxnzky.html

JS:   await fetch(url)
来源：http://hz.guowangkeji.top/gtdxkjpzcj.html

TS:   await fetch(url)
来源：http://hz.hongshengwenyu.top/gtvlsumbnj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.sufxvd.cn/gttcrwhcer.html

Go:   resp, err := http.Get(url)
来源：http://hz.yuxming.cn/gtswntcqud.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.0kj1m.cn/gtiwwhdkcl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jinqigufen.top/gtglkurafr.html

[L02] 发送 POST JSON
来源：http://hz.hnxiangtu.top/gtpjjcfhtj.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zycfv.cn/gtczickmnt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.meibo888.top/gtbbolktub.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.guowangkeji.top/gtcfvfjnnz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xuetiantiany.cn/gtqvjzxvja.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hnqzz.top/gtxkzhrsfg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jiagoushi.top/gtoynriptn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yj20258.top/gtdrwqffet.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.bjfxy.top/gteptfanar.html

[L03] 设置自定义请求头
来源：http://hz.chenjidiqi.icu/gtyrgufibc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.c1oappe.top/gtzzcxemjj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zhiwuduotai.top/gtpmbifdja.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ivvv.top/gtudokffjl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhiwuduotai.top/gtaoxylwkq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.meibo888.top/gtigzxrzfh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.gaohongyu789.top/gtufqjrprs.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.bjfxy.top/gtjjmonqna.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.gotoacloud.top/gtnnsbmjcr.html

[L04] 设置超时
来源：http://hz.ybcxt.top/gtidyvfokp.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yonumen.top/gtuvvmifkm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.tanke756.top/gtrvjubmpj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinqigfzy.top/gtkjclaivc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nwbrower.top/gtjtykvywr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yangfankeji.com/gtvbfzytyq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.cdnleiting.top/gtezfcvhmu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.daria6918.cn/gttzxizkvb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ehwqpu.com/gtesndulfw.html

[L05] 上传文件（multipart）
来源：http://hz.cucudq.cn/gtlvnbflwz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.ehwqpu.com/gtinupniah.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xuetiantiany.cn/gtdhmnwpvm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ybcxt.top/gtiyznwamh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.sysykeji.top/gtreypdwnx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.haohaochexian.top/gtbfrsyusi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jqgfzy.top/gtsikgcnie.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jiagoushi.top/gtqmokgvar.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.haohaochexian.top/gtgqqcykbv.html

[L06] 解析响应为 JSON
来源：http://hz.yvedp.cn/gthrzovovb.html

Py:   resp.json()
来源：http://hz.zhoulong.xyz/gtpsgmowus.html

PHP:  json_decode($body, true);
来源：http://hz.cheryme.top/gthjydbniz.html

JS:   await resp.json()
来源：http://hz.kuanghao11.cn/gtcnjaavfl.html

TS:   await resp.json()
来源：http://hz.sxryk.cn/gtaosofkqk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.andypj.xyz/gtxjhwgnlz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.tianlin.xyz/gtaqtucquc.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jqgufenzy.top/gtpboftayp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ydzc1.top/gtmalcivpn.html

[L07] 处理 HTTP 状态码
来源：http://hz.shzxlz.cn/gtkdcxadmv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.9152youxi.cn/gtjfyqqmwn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.shuidangran.top/gtehddamia.html

JS:   resp.ok;  resp.status
来源：http://hz.ppjwa.cn/gtfounomrq.html

TS:   resp.ok;  resp.status
来源：http://hz.316326.xyz/gtsfylnocz.html

Java: resp.statusCode()
来源：http://hz.daxiang520.top/gtyxmxvixu.html

Go:   resp.StatusCode
来源：http://hz.dashuyun.cn/gtpcucdgia.html

Ruby: resp.code.to_i
来源：http://hz.feifeiyinyue.top/gtfskflohd.html

C#:   (int)resp.StatusCode
来源：http://hz.ydzc1.top/gtnfacalgy.html

[L08] 并发请求多个地址
来源：http://hz.aizwys.cn/gtyygrapnf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yj20258.top/gtwyubhdnm.html

PHP:  curl_multi_init() 系列
来源：http://hz.shanyushiyangkeji.top/gtoeiuvohh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhiwuduotai.top/gtiawjkxyv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.aizwys.cn/gtiteglqir.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jinghuilouyu.cn/gtstinrdyp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.andypj.xyz/gtnmxgvbie.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhijiandao.cn/gtoxcspslj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.iojbl.cn/gtoqfiepyf.html

================================================================================
来源：http://hz.xuetiantiany.cn/gthvpxvgtz.html

M. 命令行 / 进程 / 环境
来源：http://hz.nanxuanxn.top/gtmscljcgh.html

================================================================================
来源：http://hz.chenlongwang.top/gttfibzgwi.html

[M01] 读取命令行参数
来源：http://hz.tianlin.xyz/gttjcqdpzy.html

Py:   sys.argv[1:]
来源：http://hz.aizwys.cn/gtbbdwywwf.html

PHP:  $argv;  $argc;
来源：http://hz.cheryme.top/gtenlosete.html

JS:   process.argv.slice(2)
来源：http://hz.nwbrower.top/gtgfsehdhu.html

TS:   process.argv.slice(2)
来源：http://hz.yuanzhike.top/gtpkuqanci.html

Java: args 数组（main 方法参数）
来源：http://hz.tanke756.top/gtqgfeaowc.html

Go:   os.Args[1:]
来源：http://hz.52xcode.cn/gtljjwjegt.html

Ruby: ARGV
来源：http://hz.zhaomingkeji.xyz/gtmkrcjzhm.html

C#:   args 数组（Main 方法参数）
来源：http://hz.vqdsnc.cn/gtkapiklbv.html

[M02] 读取环境变量
来源：http://hz.kuanghao11.cn/gtdtgjbjms.html

Py:   os.environ.get("HOME")
来源：http://hz.gotoacloud.top/gtjundbzdi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hammf.cn/gtfemfbnnf.html

JS:   process.env.HOME
来源：http://hz.redwolf501.top/gttqeneunw.html

TS:   process.env.HOME
来源：http://hz.cashguo.top/gtfxixyymp.html

Java: System.getenv("HOME")
来源：http://hz.kuanghao11.cn/gtttnanxnb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.tianlin.xyz/gtkzfzqpro.html

Ruby: ENV["HOME"]
来源：http://hz.hnxiangtu.top/gtliuhclwv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yongpay.top/gtjxobrmxe.html

[M03] 执行外部命令
来源：http://hz.pengpengdd.cyou/gtiltcoptb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.cheryme.top/gtwlpphkdy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.aizwys.cn/gtjtotjsxx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.quarkkingdee.top/gtnzscvlxo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.aibaodan.cn/gtkkmpclmd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zycfv.cn/gtamfgoteu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ydjk.org.cn/gtvcbcutup.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jinghuilouyu.cn/gtwzxoxmok.html

C#:   Process.Start("ls", "-l");
来源：http://hz.sxryk.cn/gttpjkeonl.html

[M04] 获取当前工作目录
来源：http://hz.tian-w.cn/gtdbkfxlqo.html

Py:   os.getcwd()
来源：http://hz.xziqi.cn/gtzubhywxg.html

PHP:  getcwd();
来源：http://hz.jinghuilouyu.cn/gtgdozezdd.html

JS:   process.cwd()
来源：http://hz.yonumen.top/gtcmhghige.html

TS:   process.cwd()
来源：http://hz.xylfe.cn/gtybxkxcdl.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.chenzaomai.com/gtvqhjivvv.html

Go:   os.Getwd()
来源：http://hz.daria6918.cn/gtwjjkzyun.html

Ruby: Dir.pwd
来源：http://hz.ppjwa.cn/gtdytwjevh.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hammf.cn/gtnuovfkgw.html

[M05] 设置退出码
来源：http://hz.yangfankeji.com/gttavtegya.html

Py:   sys.exit(1)
来源：http://hz.gzhubu.top/gtroplwarz.html

PHP:  exit(1);
来源：http://hz.tianlin.xyz/gtvkzbxipg.html

JS:   process.exit(1)
来源：http://hz.ppjwa.cn/gtuhqlvpha.html

TS:   process.exit(1)
来源：http://hz.jqgfzy.top/gtqwfjkfve.html

Java: System.exit(1)
来源：http://hz.nwbrower.top/gtexhplwzz.html

Go:   os.Exit(1)
来源：http://hz.daxiang520.top/gttlptblxj.html

Ruby: exit 1
来源：http://hz.hammf.cn/gtazrwexrz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jinqigufen.top/gtkcmnbzzi.html

[M06] 向标准错误输出
来源：http://hz.yuxming.cn/gtvvocqgyg.html

Py:   print("err", file=sys.stderr)
来源：http://hz.0kj1m.cn/gtqinclyzh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yangfankeji.com/gtvhecbuye.html

JS:   console.error("err")
来源：http://hz.feifeiyinyue.top/gtbmnamodk.html

TS:   console.error("err")
来源：http://hz.jyoumei.cn/gtcdchouwb.html

Java: System.err.println("err")
来源：http://hz.kuanghao11.cn/gtlbgjoefi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.snrcjt.cn/gtxwfyyufy.html

Ruby: warn "err"
来源：http://hz.c1oappe.top/gtyabnrcgh.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhijiandao.cn/gthgxdtgar.html

[M07] 判断是否为主入口
来源：http://hz.redwolf501.top/gtwndxlyqc.html

Py:   if __name__ == "__main__":
来源：http://hz.yonumen.top/gtoewbpxzl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.hnxiangtu.top/gtusbbmvop.html

JS:   require.main === module
来源：http://hz.nanxinkj.top/gtokceeusj.html

TS:   require.main === module
来源：http://hz.gogol.net.cn/gtpzxaramt.html

Java: public static void main(String[] args)
来源：http://hz.andypj.xyz/gtumcvnwys.html

Go:   func main()
来源：http://hz.redwolf501.top/gtsxoejolj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jinqigufen.top/gtvrnywgwv.html

C#:   static void Main(string[] args)
来源：http://hz.hongshengwenyu.top/gtcemvnshw.html

[M08] 获取系统与运行时信息
来源：http://hz.jinghuilouyu.cn/gtzdrxuypt.html

Py:   platform.system();  platform.python_version()
来源：http://hz.birdmap.top/gtejtzukhx.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.shangyingyoupin.top/gtursijkdk.html

JS:   process.platform;  process.version
来源：http://hz.pycfn.com/gtdzmbbrwq.html

TS:   process.platform;  process.version
来源：http://hz.xziqi.cn/gtwdwoowui.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jqgufenzy.top/gtimlczoxn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xingfuxueyuan.xyz/gtiuboyvpt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jinghuilouyu.cn/gtyjcofbhp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.dianchejie.cn/gtkkcoyfmd.html

================================================================================
来源：http://hz.xylfe.cn/gthetzamgx.html

N. 数据结构与算法
来源：http://hz.bjfxy.top/gtqwydkidj.html

================================================================================
来源：http://hz.vqdsnc.cn/gtrtnaaknf.html

[N01] 二分查找（有序数组）
来源：http://hz.sweek.top/gtljdnbufi.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xziqi.cn/gteqxzpvcl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hywenlv.cn/gtozaefoln.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xingfuxueyuan.xyz/gturangaao.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yonumen.top/gtxdocbcqq.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.chenlongwang.top/gtdipmdefm.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cucudq.cn/gtbmkodtbv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ydjk.org.cn/gtwbwqffsh.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jiagoushi.top/gtwidzltsm.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.cheryme.top/gtjsbuioir.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gotoacloud.top/gtcbjzrqxl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.cashguo.top/gtmcuqniib.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gzhubu.top/gtbbhzaczy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.pycfn.com/gtxsglnyfu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.fengsongda.top/gtblrrvfhv.html

Go:   slices.Sort(arr)
来源：http://hz.svipenyu.cn/gtyucxheob.html

Ruby: arr.sort
来源：http://hz.yongpay.top/gtbptgnbxa.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.gzhubu.top/gtlipeubso.html

[N03] 快速排序（分治示例）
来源：http://hz.ivvv.top/gtpbyulxfe.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ivvv.top/gtfffenghd.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yvedp.cn/gtwtdhnknr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ydjk.org.cn/gtltjbwhmm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.dianchejie.cn/gtjbozmfzq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.tianlin.xyz/gtknwlkkxa.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.cucudq.cn/gtsyvcdsjy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.c1oappe.top/gtsfmghpln.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yj202588.top/gtdhbcymva.html

[N04] 斐波那契数列
来源：http://hz.sufxvd.cn/gtwmlsetvg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jiagoushi.top/gtbrirunjs.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.316326.xyz/gtcbydqraq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hnxiangtu.top/gtatunujwh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj202588.top/gtkrgeopvp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.mhx1999.top/gtdtqrxbtm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.tianlin.xyz/gtjnlbiera.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.chenjidiqi.icu/gtsdwmiozp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hysaishi.cn/gtiaudhnyq.html

[N05] 最大公约数
来源：http://hz.birdmap.top/gtoputxrjy.html

Py:   math.gcd(a, b)
来源：http://hz.yuxming.cn/gtnmtfrigy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yanxiufei.cn/gtkzlpvocn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ywan-chungtsiang.top/gtmioxnncg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.haohaochexian.top/gtlqsbswir.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hnxiangtu.top/gtcgfndwum.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.kuanghao11.cn/gtkduhdurr.html

Ruby: a.gcd(b)
来源：http://hz.c1oappe.top/gtvsdhkyxc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jlsjyb.cn/gtwsgzsgez.html

[N06] 判断回文字符串
来源：http://hz.jqgfzy.top/gtxivnldba.html

Py:   s == s[::-1]
来源：http://hz.hongshengwenyu.top/gtkkfrgkcz.html

PHP:  $s === strrev($s);
来源：http://hz.iojbl.cn/gttjmdhchv.html

JS:   s === [...s].reverse().join("")
来源：http://hz.sxryk.cn/gteodsacuy.html

TS:   s === [...s].reverse().join("")
来源：http://hz.shanyushiyangtech.top/gtjajvygbw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.guowangkeji.top/gtuqtfudsf.html

Go:   // 双指针从两端比较
来源：http://hz.zycfv.cn/gtdgsqbzei.html

Ruby: s == s.reverse
来源：http://hz.jiagoushi.top/gtrmhvsqjk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.quarkkingdee.top/gtcddqmato.html

[N07] 两数之和（返回下标）
来源：http://hz.yj20258888.top/gtufaigffy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.bjfxy.top/gtaewsjbfr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jinqigufen.top/gtzqzxvlme.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.hnqzz.top/gtdstadqhb.html

TS:   // 手写 Map<string, number>
来源：http://hz.yongpay.top/gtksnmofit.html

Java: // 手写 HashMap
来源：http://hz.yueranfly.top/gtqmmnvjnb.html

Go:   // 手写 map[int]int
来源：http://hz.andypj.xyz/gtjvyjzbgh.html

Ruby: // 手写 Hash
来源：http://hz.316326.xyz/gtipybxphs.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.bjfxy.top/gtcuflpzyv.html

[N08] 生成全排列
来源：http://hz.gogol.net.cn/gtpeakjoyk.html

Py:   itertools.permutations(arr)
来源：http://hz.tianlin.xyz/gthjbobvxb.html

PHP:  // 手写递归交换
来源：http://hz.shanyushiyangtech.top/gtcggdccem.html

JS:   // 手写回溯递归
来源：http://hz.ydjk.org.cn/gtzpxrrmon.html

TS:   // 手写回溯递归
来源：http://hz.yongpay.top/gttbolusze.html

Java: // 手写回溯递归
来源：http://hz.cashguo.top/gtlyhrpoqw.html

Go:   // 手写回溯递归
来源：http://hz.jqgfzy.top/gtgnyqfrwc.html

Ruby: arr.permutation.to_a
来源：http://hz.shuidangran.top/gtekkrdmaa.html

C#:   // 手写回溯递归
来源：http://hz.yueranfly.top/gtxqyuglkg.html


<!-- 参考信息 -->