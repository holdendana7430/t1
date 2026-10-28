代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.316326.xyz/gtnjxfxghc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jiagoushi.top/gtsxtnwhtv.html

JS:   JSON.stringify(obj)
来源：http://hz.c1oappe.top/gtqzsvmgve.html

TS:   JSON.stringify(obj)
来源：http://hz.jinqigufen.top/gtvjhblacz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.ivvv.top/gtfueurykq.html

Go:   json.Marshal(obj)
来源：http://hz.ydzc1.top/gtrgnzdbnx.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shuidangran.top/gttvyenxwp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.guowangkeji.top/gtfcydqmwu.html

[K02] JSON 字符串转对象
来源：http://hz.yangfankeji.com/gtppvjnhdk.html

Py:   json.loads(s)
来源：http://hz.quarkkingdee.top/gttgzhkoou.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.pycfn.com/gtujxcrizy.html

JS:   JSON.parse(s)
来源：http://hz.xinyue.icu/gtimmucmkr.html

TS:   JSON.parse(s)
来源：http://hz.dashuyun.cn/gtvoweoolr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.gogol.net.cn/gtpjmmboxi.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.shanyushiyangtech.top/gtzjygeqgf.html

Ruby: JSON.parse(s)
来源：http://hz.sysykeji.top/gtgynmbhcv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhixingplan.top/gtuvmbblqk.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhiwuduotai.top/gtwtbvpbpi.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yuxming.cn/gtyggndpsi.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.sweek.top/gtzsvpsngc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shzxlz.cn/gtifvirysh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.gaohongyu789.top/gthxuleonm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.sufxvd.cn/gthmekatze.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yj202588.top/gtkxblbvrz.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jinghuilouyu.cn/gtguifpidx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ivvv.top/gtlawnregr.html

[K04] 读取 JSON 文件
来源：http://hz.jqgufenzy.top/gtmatrjzoa.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.guannengcc.top/gtdwzhzxja.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.xingfuxueyuan.xyz/gtgergsemt.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yueranfly.top/gtaelbfpjr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.feifeiyinyue.top/gtzfyekzfp.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.birdmap.top/gtdajwoaqu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yanxiufei.cn/gtpbvlqeeh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jianghu66.top/gttyprcfhv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.shuidangran.top/gtvotlttxu.html

[K05] 深拷贝对象
来源：http://hz.cheryme.top/gtzzalqghz.html

Py:   copy.deepcopy(obj)
来源：http://hz.quarkkingdee.top/gtcqslzlcw.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jiagoushi.top/gtgpljusyi.html

JS:   structuredClone(obj)
来源：http://hz.andypj.xyz/gtipinwwne.html

TS:   structuredClone(obj)
来源：http://hz.hammf.cn/gtmpacjegy.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jinyuanbaomall.cn/gtvbxwtycp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.quarkkingdee.top/gtlbmohgwl.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.gaohongyu789.top/gtbawndmuk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yuxming.cn/gtytklllsi.html

[K06] 解析 URL 查询串
来源：http://hz.meibo888.top/gtqbqsctsc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.dianchejie.cn/gtwcevvssh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.316326.xyz/gtdafpqmmf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.dianchejie.cn/gtimzlzztm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cdnleiting.top/gtnqcwonet.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.dianchejie.cn/gtyewbrzfx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.shuidangran.top/gtwplipyjn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.52xcode.cn/gtafowqjze.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.wangdashe.top/gttmwrwmli.html

[K07] 进制转换
来源：http://hz.yj20258888.top/gtenonjgye.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.guannengcc.top/gttlgvwptp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ybcxt.top/gtvwllnovh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jinghuilouyu.cn/gtqdwmcdqb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jinqigfzy.top/gtytadiany.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.aizwys.cn/gttqvwfsgb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.gotoacloud.top/gtyshbqbvi.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ppjwa.cn/gttsnqgbpv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.bjfxy.top/gtanydiclo.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.shanyushiyangkeji.top/gtybmpgbfa.html

Py:   pickle.dumps(obj)
来源：http://hz.jinqigufen.top/gtllpkevmm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hywenlv.cn/gtgyxrfttw.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.havefunace.top/gtvrnpczem.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ppjwa.cn/gtqyobhxsk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.gogol.net.cn/gtohlatpwr.html

Go:   encoding/gob
来源：http://hz.xingfuxueyuan.xyz/gtnimltsaa.html

Ruby: Marshal.dump(obj)
来源：http://hz.shanyushiyangtech.top/gtiocpbqbu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yangfankeji.com/gttwafamwq.html

================================================================================
来源：http://hz.hammf.cn/gtopaoxwgo.html

L. 网络请求
来源：http://hz.birdmap.top/gttkvmirdo.html

================================================================================
来源：http://hz.zhengqikj.top/gtykugpglj.html

[L01] 发送 GET 请求
来源：http://hz.quarkkingdee.top/gtccbvdtjo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.shuidangran.top/gtegvbkvuy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhoulong.xyz/gtnejjgtqc.html

JS:   await fetch(url)
来源：http://hz.wangdashe.top/gtbhewabby.html

TS:   await fetch(url)
来源：http://hz.316326.xyz/gtjyurffio.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.xziqi.cn/gtiruxkuru.html

Go:   resp, err := http.Get(url)
来源：http://hz.jlsjyb.cn/gtvotpqaby.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.shuidangran.top/gtrhvxoowv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.c1oappe.top/gttatnkaba.html

[L02] 发送 POST JSON
来源：http://hz.wangshuangyany.cn/gtskngfqbd.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.pycfn.com/gtjkmpyajc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhixingplan.top/gtqckqwmch.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hywenlv.cn/gtxxweyoss.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhixingplan.top/gtyzxtesum.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.cheryme.top/gtksefaufi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.sxryk.cn/gtsftswlyt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.hysaishi.cn/gtkfzswnrd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.cashguo.top/gtvikbepro.html

[L03] 设置自定义请求头
来源：http://hz.yuxming.cn/gtmirbnbsm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.wangdashe.top/gtokxlhyjy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.tian-w.cn/gtfmjtchmr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jianghu66.top/gttfhbcmtf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hywenlv.cn/gtojhflwzo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jinghuilouyu.cn/gtesqsshrq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.svipenyu.cn/gtnusyltpk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yj202588.top/gtfnkltcjb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.sxryk.cn/gtxsnufwcv.html

[L04] 设置超时
来源：http://hz.feifeiyinyue.top/gtdoacasso.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xuetiantiany.cn/gtougejpgt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.wangshuangyany.cn/gtnjmnglqw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhaomingkeji.xyz/gtnndnhqay.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.feifeiyinyue.top/gtbugeuhnc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xylfe.cn/gtqkphztaf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jinqigufen.top/gtttmiommu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jinyuanbaomall.cn/gtupzsecqj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hfpthk.cn/gtpvqvwotn.html

[L05] 上传文件（multipart）
来源：http://hz.pycfn.com/gteftvygvi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.sufxvd.cn/gtfxpditwi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.pengpengdd.cyou/gtbznwigaq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenlongwang.top/gtsufxhwxz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.sxryk.cn/gtloisuofo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jqgfzy.top/gtjuqpovhk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yj20258888.top/gtgjemhzap.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhongyouzk.top/gtzpetzxjj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.mhx1999.top/gtiqybugdn.html

[L06] 解析响应为 JSON
来源：http://hz.dashuyun.cn/gtpwiymdln.html

Py:   resp.json()
来源：http://hz.dashuyun.cn/gtmokuvwyp.html

PHP:  json_decode($body, true);
来源：http://hz.kuanghao11.cn/gtfrivzlsq.html

JS:   await resp.json()
来源：http://hz.yonumen.top/gtqwzhjsiv.html

TS:   await resp.json()
来源：http://hz.ywan-chungtsiang.top/gthowavwjd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhiwuduotai.top/gtjngjtcjo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xylfe.cn/gtjbixrcfr.html

Ruby: JSON.parse(resp.body)
来源：http://hz.snrcjt.cn/gteilcwqgv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.kuanghao11.cn/gtwjppbfzl.html

[L07] 处理 HTTP 状态码
来源：http://hz.bjfxy.top/gtejggjfzv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yonumen.top/gtnxucspoy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.9152youxi.cn/gtrbxiuutr.html

JS:   resp.ok;  resp.status
来源：http://hz.ybcxt.top/gtybaobqva.html

TS:   resp.ok;  resp.status
来源：http://hz.xziqi.cn/gtxwmnbnbo.html

Java: resp.statusCode()
来源：http://hz.daxiang520.top/gtfeiqgroo.html

Go:   resp.StatusCode
来源：http://hz.zycfv.cn/gtwvksqzra.html

Ruby: resp.code.to_i
来源：http://hz.andypj.xyz/gtwnmtuvbu.html

C#:   (int)resp.StatusCode
来源：http://hz.cqqwz.cn/gtuanlsjsv.html

[L08] 并发请求多个地址
来源：http://hz.jiagoushi.top/gtoiefbteq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yongpay.top/gtooabhkuf.html

PHP:  curl_multi_init() 系列
来源：http://hz.ppjwa.cn/gtbqqvzljv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.vqdsnc.cn/gtcjerdnac.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jlsjyb.cn/gtdgegerqo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xylfe.cn/gtzslymswe.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.gaohongyu789.top/gtyjnnzxam.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.birdmap.top/gtdrowezpv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.wangdashe.top/gtasfsymsx.html

================================================================================
来源：http://hz.svipenyu.cn/gtbaappoqe.html

M. 命令行 / 进程 / 环境
来源：http://hz.jiagoushi.top/gtevprxbyu.html

================================================================================
来源：http://hz.sysykeji.top/gthkjgwsrf.html

[M01] 读取命令行参数
来源：http://hz.cheryme.top/gtxexmrdem.html

Py:   sys.argv[1:]
来源：http://hz.quarkkingdee.top/gtbeebcesr.html

PHP:  $argv;  $argc;
来源：http://hz.ydzc1.top/gtxacdfobz.html

JS:   process.argv.slice(2)
来源：http://hz.smart0.xyz/gtrxxdpxax.html

TS:   process.argv.slice(2)
来源：http://hz.snrcjt.cn/gttmsottps.html

Java: args 数组（main 方法参数）
来源：http://hz.jyoumei.cn/gtxuysgnuy.html

Go:   os.Args[1:]
来源：http://hz.yongpay.top/gtwmqwrzpw.html

Ruby: ARGV
来源：http://hz.zhixingplan.top/gtityoojja.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhongyouzk.top/gtcuviyjms.html

[M02] 读取环境变量
来源：http://hz.dianchejie.cn/gtpjymwcbp.html

Py:   os.environ.get("HOME")
来源：http://hz.nanxinkj.top/gtnvligrdj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hnqzz.top/gtczrcwdod.html

JS:   process.env.HOME
来源：http://hz.mhx1999.top/gtdpnvqkfm.html

TS:   process.env.HOME
来源：http://hz.guowangkeji.top/gtdsgbounz.html

Java: System.getenv("HOME")
来源：http://hz.hywenlv.cn/gtulfupaij.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.daxiang520.top/gtaowqzurk.html

Ruby: ENV["HOME"]
来源：http://hz.sweek.top/gtrwoeeaum.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.svipenyu.cn/gtofozsapb.html

[M03] 执行外部命令
来源：http://hz.gzhubu.top/gtngcekihc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.gotoacloud.top/gtxotmforr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.fzhhl.top/gtabxvwgwl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ydjk.org.cn/gtimqjgjob.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xingfuxueyuan.xyz/gtjwdxsogb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.sweek.top/gtwlkakbri.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yongpay.top/gtentuugna.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.sweek.top/gtwwsjptol.html

C#:   Process.Start("ls", "-l");
来源：http://hz.sxryk.cn/gtoscqxzlp.html

[M04] 获取当前工作目录
来源：http://hz.316326.xyz/gtqxpbcabj.html

Py:   os.getcwd()
来源：http://hz.shuidangran.top/gtemkabzqa.html

PHP:  getcwd();
来源：http://hz.snrcjt.cn/gtlvxskrss.html

JS:   process.cwd()
来源：http://hz.hnqzz.top/gtazmcrgor.html

TS:   process.cwd()
来源：http://hz.xuetiantiany.cn/gtlqmowmfe.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhaomingkeji.xyz/gtqjllirxt.html

Go:   os.Getwd()
来源：http://hz.jqgfzy.top/gtrkadukmt.html

Ruby: Dir.pwd
来源：http://hz.nanxinkj.top/gttmmakgra.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.sysykeji.top/gtsywngwxy.html

[M05] 设置退出码
来源：http://hz.aibaodan.cn/gtxyzqrtan.html

Py:   sys.exit(1)
来源：http://hz.hysaishi.cn/gtikhpcplk.html

PHP:  exit(1);
来源：http://hz.xylfe.cn/gttopfsplm.html

JS:   process.exit(1)
来源：http://hz.ydjk.org.cn/gtdmhcicpl.html

TS:   process.exit(1)
来源：http://hz.ehwqpu.com/gtsszixmhh.html

Java: System.exit(1)
来源：http://hz.hongshengwenyu.top/gtghwqsogh.html

Go:   os.Exit(1)
来源：http://hz.zhixingplan.top/gtwtmxaxmv.html

Ruby: exit 1
来源：http://hz.cheryme.top/gtlpxnpqgo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yvedp.cn/gtedazwprk.html

[M06] 向标准错误输出
来源：http://hz.gogol.net.cn/gtknoutvtw.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ivvv.top/gtjzxclxxs.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.cucudq.cn/gtlqwymuzj.html

JS:   console.error("err")
来源：http://hz.haohaochexian.top/gtmxhdgutq.html

TS:   console.error("err")
来源：http://hz.ybcxt.top/gtelnnqgkx.html

Java: System.err.println("err")
来源：http://hz.yj20258.top/gtbyjwcoff.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ybcxt.top/gtbndjskgb.html

Ruby: warn "err"
来源：http://hz.gotoacloud.top/gthxuyryde.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ydzc1.top/gthtvpehaj.html

[M07] 判断是否为主入口
来源：http://hz.andypj.xyz/gtnlayjxoi.html

Py:   if __name__ == "__main__":
来源：http://hz.gotoacloud.top/gtgphwsrsl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.gaohongyu789.top/gtgqwiwnkl.html

JS:   require.main === module
来源：http://hz.316326.xyz/gtlfqmqbpu.html

TS:   require.main === module
来源：http://hz.jqgufenzy.top/gtxhueldzd.html

Java: public static void main(String[] args)
来源：http://hz.xuanzx.com/gtyahrezzy.html

Go:   func main()
来源：http://hz.wangdashe.top/gtrpyerycj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.aibaodan.cn/gtenmxapfl.html

C#:   static void Main(string[] args)
来源：http://hz.sysykeji.top/gtljyqquri.html

[M08] 获取系统与运行时信息
来源：http://hz.cheryme.top/gtjsysvdjz.html

Py:   platform.system();  platform.python_version()
来源：http://hz.pengpengdd.cyou/gtarcovpnq.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.aibaodan.cn/gtvuglddgu.html

JS:   process.platform;  process.version
来源：http://hz.yueranfly.top/gtymucjanr.html

TS:   process.platform;  process.version
来源：http://hz.yuxming.cn/gtujplpujb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.cucudq.cn/gtdvtnuyhp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.chenjidiqi.icu/gtvmcwpymo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.0kj1m.cn/gtiyncaich.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.xuetiantiany.cn/gtommdhdns.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtstdogjal.html

N. 数据结构与算法
来源：http://hz.hfpthk.cn/gtvrsibadr.html

================================================================================
来源：http://hz.cashguo.top/gtgdubktck.html

[N01] 二分查找（有序数组）
来源：http://hz.hfpthk.cn/gtlxnwtfbw.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.gogol.net.cn/gtmhkjdyrn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.haohaochexian.top/gtsoozuqsn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.daria6918.cn/gtyblbaniu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ybcxt.top/gtkrsjtkow.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.ppjwa.cn/gtvgvqqzqu.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.andypj.xyz/gtqrptmtej.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xuetiantiany.cn/gtsdzlklst.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yonumen.top/gtpnfjlbrl.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.xuanzx.com/gtjpmzyjxf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.pengpengdd.cyou/gtirhpzkwl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.sysykeji.top/gtlgjyvlwr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.vqdsnc.cn/gtdxguvepd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.aizwys.cn/gtupuzowcn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.fengsongda.top/gttphihysl.html

Go:   slices.Sort(arr)
来源：http://hz.jlsjyb.cn/gtjtzpaocr.html

Ruby: arr.sort
来源：http://hz.hnxiangtu.top/gtcnqlkvea.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhixingplan.top/gtsolzzxqn.html

[N03] 快速排序（分治示例）
来源：http://hz.ybcxt.top/gtsqdwidjk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yj202588.top/gtoksihkye.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jinqigufen.top/gtjkffgakl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ybcxt.top/gtpgvbhjjd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhixingplan.top/gtomvlwvjv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.ydjk.org.cn/gtgcnygsxu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.gzhubu.top/gtpdcpxage.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.c1oappe.top/gtsewiicrx.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jyoumei.cn/gtratbczqf.html

[N04] 斐波那契数列
来源：http://hz.tianlin.xyz/gtzehvngec.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.havefunace.top/gtuqfgopnu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.gzhubu.top/gtxxxqyyyu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj20258888.top/gtaysjudvs.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yonumen.top/gtvjvisota.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.hammf.cn/gtqpygtqke.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.chenlongwang.top/gtyxftaysx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jlsjyb.cn/gtjyuqqooy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.sufxvd.cn/gtsqlwxdhi.html

[N05] 最大公约数
来源：http://hz.nanxinkj.top/gtgywhzorg.html

Py:   math.gcd(a, b)
来源：http://hz.9152youxi.cn/gtjinxtnnh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.0kj1m.cn/gtwclyklak.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yj20258.top/gtgjxwapam.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ybcxt.top/gtrvfholil.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zycfv.cn/gtphhxskcu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yongpay.top/gtlgddgzsq.html

Ruby: a.gcd(b)
来源：http://hz.ywan-chungtsiang.top/gteocxgdve.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.cashguo.top/gtujswwuji.html

[N06] 判断回文字符串
来源：http://hz.ydjk.org.cn/gtlodvnlqb.html

Py:   s == s[::-1]
来源：http://hz.dianchejie.cn/gtdcnejdsd.html

PHP:  $s === strrev($s);
来源：http://hz.ivvv.top/gtbsyiogms.html

JS:   s === [...s].reverse().join("")
来源：http://hz.nanxinkj.top/gtzxpwnmya.html

TS:   s === [...s].reverse().join("")
来源：http://hz.9152youxi.cn/gtroxuosur.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.nanxinkj.top/gtzycpnwgx.html

Go:   // 双指针从两端比较
来源：http://hz.c1oappe.top/gtubphkyhy.html

Ruby: s == s.reverse
来源：http://hz.shanyushiyangkeji.top/gtidsddefi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yanxiufei.cn/gtswgibjxk.html

[N07] 两数之和（返回下标）
来源：http://hz.yuanzhike.top/gtbpzqnclz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hnqzz.top/gtpmxgyajc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.guowangkeji.top/gtuawpyffz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jyoumei.cn/gteilxvbdp.html

TS:   // 手写 Map<string, number>
来源：http://hz.aibaodan.cn/gtqqfkgxxf.html

Java: // 手写 HashMap
来源：http://hz.ydzc1.top/gtgtobczly.html

Go:   // 手写 map[int]int
来源：http://hz.sweek.top/gtjwcwgviq.html

Ruby: // 手写 Hash
来源：http://hz.daxiang520.top/gtjdsanfmx.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yongpay.top/gtkzmlyafl.html

[N08] 生成全排列
来源：http://hz.jyoumei.cn/gtimtjmzyy.html

Py:   itertools.permutations(arr)
来源：http://hz.daria6918.cn/gtcicntenu.html

PHP:  // 手写递归交换
来源：http://hz.ydzc1.top/gtcjofuivx.html

JS:   // 手写回溯递归
来源：http://hz.c1oappe.top/gtmunnmkze.html

TS:   // 手写回溯递归
来源：http://hz.smart0.xyz/gtobqkzakq.html

Java: // 手写回溯递归
来源：http://hz.yangfankeji.com/gtgilsytuh.html

Go:   // 手写回溯递归
来源：http://hz.xinyue.icu/gtycitukhh.html

Ruby: arr.permutation.to_a
来源：http://hz.jlsjyb.cn/gtxpywcssy.html

C#:   // 手写回溯递归
来源：http://hz.yangfankeji.com/gtcndqiiaf.html

[N09] 栈与队列
来源：http://hz.zhongyouzk.top/gtjtavkkec.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.xylfe.cn/gtxsgwykrr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.bjfxy.top/gtzaxobtko.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.9152youxi.cn/gtnfpsuqoq.html


<!-- 参考信息 -->