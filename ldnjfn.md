代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.redwolf501.top/gtsbzhuehs.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhongyouzk.top/gtsisfwzxd.html

JS:   JSON.stringify(obj)
来源：http://hz.cdnleiting.top/gtyklqkbyy.html

TS:   JSON.stringify(obj)
来源：http://hz.jinqigfzy.top/gtwxoyipar.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.shanyushiyangkeji.top/gtvqoecfpp.html

Go:   json.Marshal(obj)
来源：http://hz.shuidangran.top/gttkszkdle.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.xziqi.cn/gthvrbpbly.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.cqqwz.cn/gtwkflpgxx.html

[K02] JSON 字符串转对象
来源：http://hz.tanke756.top/gtdbyasogw.html

Py:   json.loads(s)
来源：http://hz.nanxuanxn.top/gtbowmlzwv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.shuidangran.top/gtespvjabk.html

JS:   JSON.parse(s)
来源：http://hz.gogol.net.cn/gtxyhqdedi.html

TS:   JSON.parse(s)
来源：http://hz.yonumen.top/gtlznkfkhh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.nanxuanxn.top/gtbmyquywq.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.c1oappe.top/gtlvkhkfwb.html

Ruby: JSON.parse(s)
来源：http://hz.pycfn.com/gtstzqalvm.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yangfankeji.com/gtigfcakza.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhengqikj.top/gtlmrknddj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yongpay.top/gtoemanfim.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.fengsongda.top/gtnfcnwoeb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xinyue.icu/gtzmjsdiwd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.sweek.top/gtbxyrbfcp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hammf.cn/gtjhcqeaka.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jinqigufen.top/gtrstzuohk.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ivvv.top/gttcvufxnw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.shanyushiyangtech.top/gtqkuwlruw.html

[K04] 读取 JSON 文件
来源：http://hz.yj202588.top/gtzxbjhbmi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.gotoacloud.top/gtqeidqsat.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.chenlongwang.top/gtphnnfbzt.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.9152youxi.cn/gtahhgpulb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hysaishi.cn/gtmzugabxk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.xuanzx.com/gtscxuiifi.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.9152youxi.cn/gttnlfwnzo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhaomingkeji.xyz/gtztubxnta.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.cashguo.top/gtztvshqel.html

[K05] 深拷贝对象
来源：http://hz.nwbrower.top/gtvqlulogc.html

Py:   copy.deepcopy(obj)
来源：http://hz.tian-w.cn/gtopgzbdgg.html

PHP:  unserialize(serialize($obj));
来源：http://hz.meibo888.top/gtsllzzrbo.html

JS:   structuredClone(obj)
来源：http://hz.wangshuangyany.cn/gtorpndlmu.html

TS:   structuredClone(obj)
来源：http://hz.yuanzhike.top/gtitdglvom.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xingfuxueyuan.xyz/gtnlizlixu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.redwolf501.top/gtchvhpbse.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xuanzx.com/gtcuwptddr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.xingfuxueyuan.xyz/gtddajdgbi.html

[K06] 解析 URL 查询串
来源：http://hz.gzhubu.top/gtedqoklbi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.shangyingyoupin.top/gtvgbrbzbw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.chenlongwang.top/gthfsjgjgf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shuidangran.top/gtbmvjwuak.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.fengsongda.top/gtfvlsemhl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ydjk.org.cn/gtrzylydqm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jyoumei.cn/gtambufvwx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.c1oappe.top/gtylsbtxaq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ivvv.top/gtegbcjrtj.html

[K07] 进制转换
来源：http://hz.fzhhl.top/gtusoewnqz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.aizwys.cn/gtqsiuxplm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.iojbl.cn/gtlutxghup.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.meibo888.top/gtjshyxgmi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ybcxt.top/gtwxbhwjmy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.c1oappe.top/gtelnoacui.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.nanxuanxn.top/gthigykykp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.sweek.top/gtfppjufrl.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.guowangkeji.top/gtrfiyfgvt.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zycfv.cn/gtidrmcrzf.html

Py:   pickle.dumps(obj)
来源：http://hz.yueranfly.top/gtadkjxvvv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.wangshuangyany.cn/gttwkbbozc.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.9152youxi.cn/gtopcidlct.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jinyuanbaomall.cn/gtusryytwj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.daria6918.cn/gtowlxxrsk.html

Go:   encoding/gob
来源：http://hz.xinyue.icu/gtjdqvqaly.html

Ruby: Marshal.dump(obj)
来源：http://hz.xuanzx.com/gtmdzehdiu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jqgufenzy.top/gttdfvskkq.html

================================================================================
来源：http://hz.yuxming.cn/gtmjsudgpj.html

L. 网络请求
来源：http://hz.hfpthk.cn/gtinjzqjzq.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtjbftbwpz.html

[L01] 发送 GET 请求
来源：http://hz.hnxiangtu.top/gtfsxcmzcj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.chenlongwang.top/gtrtzzisrh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yuxming.cn/gtxshtztxr.html

JS:   await fetch(url)
来源：http://hz.havefunace.top/gthwmharaa.html

TS:   await fetch(url)
来源：http://hz.pengpengdd.cyou/gttneybque.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ydzc1.top/gtwywntpnu.html

Go:   resp, err := http.Get(url)
来源：http://hz.guannengcc.top/gtlkkdtrqs.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jinghuilouyu.cn/gtojryxlnt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.shanyushiyangtech.top/gtsnldmaev.html

[L02] 发送 POST JSON
来源：http://hz.guowangkeji.top/gtrcjbzdmh.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ppjwa.cn/gtjlvvsmwh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.cashguo.top/gtsudrrdrg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.mhx1999.top/gttgirzafp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xingfuxueyuan.xyz/gtknfreabb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jinqigfzy.top/gtauzcxxhj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jiagoushi.top/gtuywarncp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jyoumei.cn/gthvumgfou.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hnqzz.top/gtrimdsebf.html

[L03] 设置自定义请求头
来源：http://hz.quarkkingdee.top/gtaivcvmie.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jianghu66.top/gttxrnvgtp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.gaohongyu789.top/gtfvxqxjoq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sweek.top/gtneapdnuq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.wangshuangyany.cn/gtyibbwwbx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hnqzz.top/gtdhzfmgvt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.fzhhl.top/gtfnygrkfw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.havefunace.top/gtyahgzdav.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.xingfuxueyuan.xyz/gtpsrevqxo.html

[L04] 设置超时
来源：http://hz.gotoacloud.top/gtvmhmeegu.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ivvv.top/gtznxjhukb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.cdnleiting.top/gthzjrltuo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.chenlongwang.top/gtypynrncw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jiagoushi.top/gteqekisca.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jiagoushi.top/gtlfbmgbsj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.meibo888.top/gtjzfrdryo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hnxiangtu.top/gtaiandjlc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.iojbl.cn/gthqwoclir.html

[L05] 上传文件（multipart）
来源：http://hz.cucudq.cn/gtrpdkgbhk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.cashguo.top/gtnkdyjmvm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jqgfzy.top/gtcbfczynl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.redwolf501.top/gtcilypfvs.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.gotoacloud.top/gtkxfncsgu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.vqdsnc.cn/gtnectmfvm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.dashuyun.cn/gtegirojuh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ybcxt.top/gtyepsrrhh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hongshengwenyu.top/gtqblsaoyb.html

[L06] 解析响应为 JSON
来源：http://hz.sufxvd.cn/gttoulkxkl.html

Py:   resp.json()
来源：http://hz.52xcode.cn/gthiehgqey.html

PHP:  json_decode($body, true);
来源：http://hz.pycfn.com/gtippcnlrl.html

JS:   await resp.json()
来源：http://hz.ybcxt.top/gtjkuhswfy.html

TS:   await resp.json()
来源：http://hz.sweek.top/gthpvdosqc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yj20258.top/gtuebbtffl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.vqdsnc.cn/gtafegqjii.html

Ruby: JSON.parse(resp.body)
来源：http://hz.aizwys.cn/gtyhakyvga.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.quarkkingdee.top/gtpnugzurr.html

[L07] 处理 HTTP 状态码
来源：http://hz.sxryk.cn/gtrmbynmsl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jqgfzy.top/gtgsdlrlkk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.316326.xyz/gtknozpdcb.html

JS:   resp.ok;  resp.status
来源：http://hz.hnqzz.top/gtoyqfkinx.html

TS:   resp.ok;  resp.status
来源：http://hz.shangyingyoupin.top/gtzcdjbued.html

Java: resp.statusCode()
来源：http://hz.yongpay.top/gtykrqfgtk.html

Go:   resp.StatusCode
来源：http://hz.jyoumei.cn/gtiwhalgys.html

Ruby: resp.code.to_i
来源：http://hz.xziqi.cn/gtygfaopcl.html

C#:   (int)resp.StatusCode
来源：http://hz.havefunace.top/gtlfohmrye.html

[L08] 并发请求多个地址
来源：http://hz.sweek.top/gtgdlzwxlr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yj202588.top/gtrilaodlc.html

PHP:  curl_multi_init() 系列
来源：http://hz.gaohongyu789.top/gtqndrpmme.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yongpay.top/gttnawaacl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shzxlz.cn/gtrbdxfale.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.c1oappe.top/gtezqnunja.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jinghuilouyu.cn/gtontpcpex.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhixingplan.top/gttkhexgxp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.0kj1m.cn/gtrzkcojhc.html

================================================================================
来源：http://hz.ydjk.org.cn/gtrjwcygta.html

M. 命令行 / 进程 / 环境
来源：http://hz.yangfankeji.com/gttnaoopyo.html

================================================================================
来源：http://hz.yj20258.top/gtznqpaxjz.html

[M01] 读取命令行参数
来源：http://hz.chenzaomai.com/gtcxwrktru.html

Py:   sys.argv[1:]
来源：http://hz.haohaochexian.top/gtnwsuswrp.html

PHP:  $argv;  $argc;
来源：http://hz.dianchejie.cn/gtteorklbw.html

JS:   process.argv.slice(2)
来源：http://hz.hfpthk.cn/gtoagfgmtb.html

TS:   process.argv.slice(2)
来源：http://hz.ywan-chungtsiang.top/gtdtuhsqjv.html

Java: args 数组（main 方法参数）
来源：http://hz.hywenlv.cn/gtuylutvft.html

Go:   os.Args[1:]
来源：http://hz.jyoumei.cn/gtxvlwyztp.html

Ruby: ARGV
来源：http://hz.havefunace.top/gtitvpsxrf.html

C#:   args 数组（Main 方法参数）
来源：http://hz.fzhhl.top/gttubfxxyj.html

[M02] 读取环境变量
来源：http://hz.c1oappe.top/gtauokwaan.html

Py:   os.environ.get("HOME")
来源：http://hz.tianlin.xyz/gtoverwhqm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yangfankeji.com/gtnbjtboja.html

JS:   process.env.HOME
来源：http://hz.ydjk.org.cn/gtxibwftpq.html

TS:   process.env.HOME
来源：http://hz.redwolf501.top/gtsdqkafvb.html

Java: System.getenv("HOME")
来源：http://hz.c1oappe.top/gtpxhccwci.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yj20258888.top/gtfzjpvbst.html

Ruby: ENV["HOME"]
来源：http://hz.jinyuanbaomall.cn/gtcjmkqncd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.52xcode.cn/gtkdzpzelp.html

[M03] 执行外部命令
来源：http://hz.0kj1m.cn/gtepckjpsc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.nanxinkj.top/gtspbvwhca.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hywenlv.cn/gtwhedyqng.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.iojbl.cn/gttwvkgbqe.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ehwqpu.com/gtvajeaoyr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yj20258888.top/gtjpkqiecy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.kuanghao11.cn/gtnnnyzxbw.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhengqikj.top/gtrjeejxlg.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jlsjyb.cn/gtxlbawahg.html

[M04] 获取当前工作目录
来源：http://hz.dashuyun.cn/gtyppjvrng.html

Py:   os.getcwd()
来源：http://hz.yj20258888.top/gtnhgqlgon.html

PHP:  getcwd();
来源：http://hz.zhengqikj.top/gtumzhoczc.html

JS:   process.cwd()
来源：http://hz.cqqwz.cn/gtegdoytwl.html

TS:   process.cwd()
来源：http://hz.aibaodan.cn/gtrgpojefa.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.nanxuanxn.top/gthdnbjvuz.html

Go:   os.Getwd()
来源：http://hz.xuetiantiany.cn/gtvqiglrmc.html

Ruby: Dir.pwd
来源：http://hz.chenzaomai.com/gtcpmvdpji.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hywenlv.cn/gtltkdbxxc.html

[M05] 设置退出码
来源：http://hz.wangdashe.top/gtuyuynbez.html

Py:   sys.exit(1)
来源：http://hz.jinqigufen.top/gtnwgrheng.html

PHP:  exit(1);
来源：http://hz.gogol.net.cn/gtesvcohii.html

JS:   process.exit(1)
来源：http://hz.xinyue.icu/gtfkxbhuit.html

TS:   process.exit(1)
来源：http://hz.yj20258888.top/gtvxupuvwo.html

Java: System.exit(1)
来源：http://hz.shangyingyoupin.top/gtfpcbzakg.html

Go:   os.Exit(1)
来源：http://hz.jlsjyb.cn/gtoikpixsz.html

Ruby: exit 1
来源：http://hz.xuetiantiany.cn/gtnpxnpesg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yj20258888.top/gtujxtmkcv.html

[M06] 向标准错误输出
来源：http://hz.hnqzz.top/gtggigixwl.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jyoumei.cn/gtaylbblhx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.cheryme.top/gtetarinpn.html

JS:   console.error("err")
来源：http://hz.xuetiantiany.cn/gtgoilfpiv.html

TS:   console.error("err")
来源：http://hz.tianlin.xyz/gtchhxtooy.html

Java: System.err.println("err")
来源：http://hz.pengpengdd.cyou/gtindukhrm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.gotoacloud.top/gtlznttnbo.html

Ruby: warn "err"
来源：http://hz.xuetiantiany.cn/gtfojukxxp.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jinqigufen.top/gtbxikmitf.html

[M07] 判断是否为主入口
来源：http://hz.yuanzhike.top/gthhoxedwb.html

Py:   if __name__ == "__main__":
来源：http://hz.bjfxy.top/gtbrctwciw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.daxiang520.top/gtckiskrtk.html

JS:   require.main === module
来源：http://hz.52xcode.cn/gtmoaeoylo.html

TS:   require.main === module
来源：http://hz.aibaodan.cn/gtpfbxzrnc.html

Java: public static void main(String[] args)
来源：http://hz.shangyingyoupin.top/gtmdypwkhc.html

Go:   func main()
来源：http://hz.chenlongwang.top/gtwumqfkko.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhijiandao.cn/gtremtiuqa.html

C#:   static void Main(string[] args)
来源：http://hz.hysaishi.cn/gtgoazmatx.html

[M08] 获取系统与运行时信息
来源：http://hz.yj202588.top/gthekmpetp.html

Py:   platform.system();  platform.python_version()
来源：http://hz.snrcjt.cn/gtuujbkksu.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.cucudq.cn/gtexhsqzqe.html

JS:   process.platform;  process.version
来源：http://hz.ydzc1.top/gtrcjnpkau.html

TS:   process.platform;  process.version
来源：http://hz.xuanzx.com/gtoefqiyso.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.chenlongwang.top/gtyqoyylic.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.cashguo.top/gtciezmdcx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cqqwz.cn/gtznnyblzb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhixingplan.top/gtmwcibagr.html

================================================================================
来源：http://hz.52xcode.cn/gtbiwfnjqv.html

N. 数据结构与算法
来源：http://hz.nwbrower.top/gtdxnpqgud.html

================================================================================
来源：http://hz.fengsongda.top/gtozbmizbv.html

[N01] 二分查找（有序数组）
来源：http://hz.hnxiangtu.top/gtblejrocm.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ywan-chungtsiang.top/gtrwpppbey.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhaomingkeji.xyz/gtajbhpkpt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.wangshuangyany.cn/gtdverxobo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.kuanghao11.cn/gtqhaljmvo.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.gotoacloud.top/gtmftzycvk.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.chenlongwang.top/gtoqcwrcgk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.aibaodan.cn/gtaijilxyk.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.quarkkingdee.top/gtsftiysmy.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jqgfzy.top/gtanxghfxm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shangyingyoupin.top/gtuucjactb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jlsjyb.cn/gtbtfvjayj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hammf.cn/gttcvmozri.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cqqwz.cn/gtbtkowthr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.sxryk.cn/gtcaaxunpi.html

Go:   slices.Sort(arr)
来源：http://hz.ydjk.org.cn/gtuqljtuxr.html

Ruby: arr.sort
来源：http://hz.yangfankeji.com/gtwknfvzqn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.nwbrower.top/gtvjsbossj.html

[N03] 快速排序（分治示例）
来源：http://hz.guannengcc.top/gttnmlwlnh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.nanxinkj.top/gtbfbrsikj.html

PHP:  // 递归实现，或用 usort
来源：http://hz.ehwqpu.com/gtmtgjvkvw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.dianchejie.cn/gthbsowlyf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.meibo888.top/gtglcpxslk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.xziqi.cn/gtzntvoxfp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yanxiufei.cn/gtmyfjuyku.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ywan-chungtsiang.top/gtxdzlbneu.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.cqqwz.cn/gtxprbiiaj.html

[N04] 斐波那契数列
来源：http://hz.yuanzhike.top/gtsupbiszn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.guowangkeji.top/gtobcllwkm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.shanyushiyangkeji.top/gtfrycmlee.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jqgufenzy.top/gtgvlvtpvc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.0kj1m.cn/gtpypwmien.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.feifeiyinyue.top/gtynfbkktt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yueranfly.top/gtyeakublm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.sysykeji.top/gtcztdzpne.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.guannengcc.top/gtebcxaqsu.html

[N05] 最大公约数
来源：http://hz.aibaodan.cn/gtpxwfchfu.html

Py:   math.gcd(a, b)
来源：http://hz.sufxvd.cn/gtncxyihpa.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.chenzaomai.com/gttemhvels.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.bjfxy.top/gttnvozmzp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hysaishi.cn/gtegahgmnq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yj20258.top/gtffbleaor.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yonumen.top/gtgjmibdrj.html

Ruby: a.gcd(b)
来源：http://hz.xuetiantiany.cn/gthvjjmtdz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.smart0.xyz/gtrmczbvri.html

[N06] 判断回文字符串
来源：http://hz.yongpay.top/gtwcldhupn.html

Py:   s == s[::-1]
来源：http://hz.9152youxi.cn/gtnibtltvn.html

PHP:  $s === strrev($s);
来源：http://hz.shuidangran.top/gtsortegqy.html

JS:   s === [...s].reverse().join("")
来源：http://hz.smart0.xyz/gtmqshbcye.html

TS:   s === [...s].reverse().join("")
来源：http://hz.vqdsnc.cn/gtvnfypwll.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhengqikj.top/gtgsldmnkd.html

Go:   // 双指针从两端比较
来源：http://hz.52xcode.cn/gtkyuizwtl.html

Ruby: s == s.reverse
来源：http://hz.daxiang520.top/gtnsgdlble.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yj20258888.top/gtsigakgcp.html

[N07] 两数之和（返回下标）
来源：http://hz.pengpengdd.cyou/gtvnbaklbn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.pengpengdd.cyou/gteopckbgr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.fengsongda.top/gtiejeljxx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.iojbl.cn/gtxusggddr.html

TS:   // 手写 Map<string, number>
来源：http://hz.jqgufenzy.top/gtvxigzsvl.html

Java: // 手写 HashMap
来源：http://hz.daxiang520.top/gtuzyfidif.html

Go:   // 手写 map[int]int
来源：http://hz.hysaishi.cn/gtkouwzslp.html

Ruby: // 手写 Hash
来源：http://hz.jinghuilouyu.cn/gtdasznhtb.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.aizwys.cn/gtionpkeoa.html

[N08] 生成全排列
来源：http://hz.cucudq.cn/gtsdlxjluy.html

Py:   itertools.permutations(arr)
来源：http://hz.feifeiyinyue.top/gttwdhzkjs.html

PHP:  // 手写递归交换
来源：http://hz.vqdsnc.cn/gtzzcmjtxv.html

JS:   // 手写回溯递归
来源：http://hz.jqgfzy.top/gtjfwdrkhd.html

TS:   // 手写回溯递归
来源：http://hz.chenzaomai.com/gtfrapfvbt.html

Java: // 手写回溯递归
来源：http://hz.shuidangran.top/gtwwqvcbea.html

Go:   // 手写回溯递归
来源：http://hz.andypj.xyz/gtoychcvcz.html

Ruby: arr.permutation.to_a
来源：http://hz.pycfn.com/gtjwmzwriu.html

C#:   // 手写回溯递归
来源：http://hz.nwbrower.top/gtxaggflql.html

[N09] 栈与队列
来源：http://hz.shanyushiyangtech.top/gtlpkhkray.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.fzhhl.top/gtchzkklhu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.meibo888.top/gttpiyzsga.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.haohaochexian.top/gtdynjodyn.html


<!-- 参考信息 -->