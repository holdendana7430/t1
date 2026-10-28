代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.tanke756.top/gtrgnlbtgg.html

Go:   json.Marshal(obj)
来源：http://hz.gotoacloud.top/gtozwuzpdh.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zycfv.cn/gtnxnhdvzo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.nwbrower.top/gtzhpwgsnh.html

[K02] JSON 字符串转对象
来源：http://hz.hammf.cn/gtuptjhmax.html

Py:   json.loads(s)
来源：http://hz.yonumen.top/gtialepbtf.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.sysykeji.top/gtrvgnjeck.html

JS:   JSON.parse(s)
来源：http://hz.andypj.xyz/gtnykoiwgb.html

TS:   JSON.parse(s)
来源：http://hz.yvedp.cn/gtixukfsrv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yuxming.cn/gtuhabkpxa.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xinyue.icu/gtegyeolpq.html

Ruby: JSON.parse(s)
来源：http://hz.zhixingplan.top/gtneedjbxd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xuanzx.com/gtdzmdmitu.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yangfankeji.com/gtyqfktwlk.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.dashuyun.cn/gtrvnyekzs.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hnqzz.top/gtflfbpywv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.feifeiyinyue.top/gttxhyymsq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cdnleiting.top/gtoumewqdj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.nwbrower.top/gtzhrazxvu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhaomingkeji.xyz/gtggavgiqo.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.wangdashe.top/gtpcsjyvoa.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ppjwa.cn/gthnpsmycp.html

[K04] 读取 JSON 文件
来源：http://hz.birdmap.top/gtdooknbcj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jqgufenzy.top/gtvvuvgedu.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.pycfn.com/gtjqiqlkqt.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.aizwys.cn/gtmchzpoqv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xuetiantiany.cn/gtcmzowvuh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yj20258888.top/gtagkhcsoa.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.fengsongda.top/gtzqtbcguv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yuxming.cn/gtwucugufk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yj20258888.top/gtymardpjw.html

[K05] 深拷贝对象
来源：http://hz.yj20258888.top/gtldzfzlvt.html

Py:   copy.deepcopy(obj)
来源：http://hz.hywenlv.cn/gtahqsrtvj.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ivvv.top/gtyjpkrnig.html

JS:   structuredClone(obj)
来源：http://hz.jqgufenzy.top/gtxbbybtaa.html

TS:   structuredClone(obj)
来源：http://hz.jqgfzy.top/gtemtsignn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.wangdashe.top/gtguwhopta.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.chenlongwang.top/gtpgpbkbys.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.daria6918.cn/gtmlphucxj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yj20258888.top/gtdpnyvcbt.html

[K06] 解析 URL 查询串
来源：http://hz.mhx1999.top/gtfeuifoae.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhiwuduotai.top/gtajjxtzdl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jinqigfzy.top/gtglyeeteb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shzxlz.cn/gtxgjmlhcd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.0kj1m.cn/gtxnfwgkec.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.nanxuanxn.top/gtttshamut.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.chenlongwang.top/gtgaereqtl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.dashuyun.cn/gttavjynau.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jlsjyb.cn/gtsyawftbt.html

[K07] 进制转换
来源：http://hz.nwbrower.top/gtzmhxfabq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hnqzz.top/gtdtatwlzu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ydjk.org.cn/gtdywavfwp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhoulong.xyz/gtdhbyfryo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.shzxlz.cn/gtsirhunbv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cheryme.top/gthydxtpsq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yj20258.top/gtjclquero.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.hongshengwenyu.top/gtbvapyxns.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xuanzx.com/gtgyswraqa.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yuanzhike.top/gtpiajxedw.html

Py:   pickle.dumps(obj)
来源：http://hz.aibaodan.cn/gtqvvhdtwg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.shzxlz.cn/gtggnfolcj.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yanxiufei.cn/gtfzvvmqci.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.sysykeji.top/gtqhpvhpyp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.wangshuangyany.cn/gtcdqevdkk.html

Go:   encoding/gob
来源：http://hz.jqgfzy.top/gtiovzwghy.html

Ruby: Marshal.dump(obj)
来源：http://hz.xuetiantiany.cn/gtkddezkwt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ybcxt.top/gtultdgqfp.html

================================================================================
来源：http://hz.gotoacloud.top/gtmpsrgwpi.html

L. 网络请求
来源：http://hz.shanyushiyangtech.top/gtuyfpidvh.html

================================================================================
来源：http://hz.dianchejie.cn/gtakvapwsx.html

[L01] 发送 GET 请求
来源：http://hz.xingfuxueyuan.xyz/gtgamnyrgg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.dianchejie.cn/gtbjlrowqk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yongpay.top/gtmpafopqx.html

JS:   await fetch(url)
来源：http://hz.pengpengdd.cyou/gtqsgueggy.html

TS:   await fetch(url)
来源：http://hz.shuidangran.top/gtdvjidwvl.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hammf.cn/gtoktpyhmq.html

Go:   resp, err := http.Get(url)
来源：http://hz.hammf.cn/gtuhxedgxw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xingfuxueyuan.xyz/gtdcfhlcbt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.mhx1999.top/gtugwctlrn.html

[L02] 发送 POST JSON
来源：http://hz.jinqigfzy.top/gtchwsgayq.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yuanzhike.top/gtcvkntwmf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.pycfn.com/gtnifmudol.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jlsjyb.cn/gtlvhmkcky.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.aizwys.cn/gtcxtllddh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.xingfuxueyuan.xyz/gtdlelgsru.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xuanzx.com/gtzbcfxvgk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.316326.xyz/gtdkylqkso.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zhengqikj.top/gtfgmeitvg.html

[L03] 设置自定义请求头
来源：http://hz.wangshuangyany.cn/gtbjwjmtno.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xziqi.cn/gtexuymeqg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hammf.cn/gtqfgtjhpo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sxryk.cn/gtbbmvrqlh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinqigufen.top/gtwvcxdqol.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hammf.cn/gtyrrzoqih.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.gzhubu.top/gtgfohnylj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhengqikj.top/gtyvdjfvan.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hnxiangtu.top/gtfolhelpy.html

[L04] 设置超时
来源：http://hz.hnqzz.top/gtiwcdrcpi.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hywenlv.cn/gtphvyojcc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zhaomingkeji.xyz/gtqhmbdigd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ehwqpu.com/gteqrgygtm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.snrcjt.cn/gtszvjectj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.birdmap.top/gtnskxirtn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yj20258888.top/gtmfzdziqa.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ybcxt.top/gtxtbssrfb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.sufxvd.cn/gtsadvetdw.html

[L05] 上传文件（multipart）
来源：http://hz.yj20258.top/gtyqbferem.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.guannengcc.top/gtlwxgoqjg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.sysykeji.top/gtlieqvydl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.bjfxy.top/gtgofvvjun.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.tianlin.xyz/gtcyvxvqxp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.nanxinkj.top/gtemzharft.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jinyuanbaomall.cn/gtfmguimwp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.mhx1999.top/gtwalmmipe.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.xuanzx.com/gtoocqcoyy.html

[L06] 解析响应为 JSON
来源：http://hz.zhoulong.xyz/gtaaihafef.html

Py:   resp.json()
来源：http://hz.fzhhl.top/gtdzkbitgo.html

PHP:  json_decode($body, true);
来源：http://hz.chenjidiqi.icu/gtmlvhvbhj.html

JS:   await resp.json()
来源：http://hz.ydjk.org.cn/gtzhewyukw.html

TS:   await resp.json()
来源：http://hz.wangshuangyany.cn/gtdpqnygbe.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.sysykeji.top/gtpyoxgolc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.smart0.xyz/gtqtwkyxtd.html

Ruby: JSON.parse(resp.body)
来源：http://hz.0kj1m.cn/gtmzlryfph.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.xylfe.cn/gtevchzgva.html

[L07] 处理 HTTP 状态码
来源：http://hz.ybcxt.top/gturthiedt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xziqi.cn/gtjysyggng.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.iojbl.cn/gtzjmnlfwc.html

JS:   resp.ok;  resp.status
来源：http://hz.ehwqpu.com/gtoewhufmr.html

TS:   resp.ok;  resp.status
来源：http://hz.yj20258.top/gtjriypnlj.html

Java: resp.statusCode()
来源：http://hz.daria6918.cn/gtpsvxcjje.html

Go:   resp.StatusCode
来源：http://hz.jyoumei.cn/gtutuhrcos.html

Ruby: resp.code.to_i
来源：http://hz.cheryme.top/gtjaugricd.html

C#:   (int)resp.StatusCode
来源：http://hz.c1oappe.top/gtbivcvycl.html

[L08] 并发请求多个地址
来源：http://hz.yangfankeji.com/gtcmrulquj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.feifeiyinyue.top/gtizaeyqnf.html

PHP:  curl_multi_init() 系列
来源：http://hz.tianlin.xyz/gtiabaehgg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.aibaodan.cn/gtfumtziob.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.snrcjt.cn/gteuzplgau.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ehwqpu.com/gtkiruwrby.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hfpthk.cn/gtiduqrsia.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.daxiang520.top/gtnulxfrfo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.shzxlz.cn/gtxpmvbzpc.html

================================================================================
来源：http://hz.gaohongyu789.top/gtkwmqzifk.html

M. 命令行 / 进程 / 环境
来源：http://hz.jianghu66.top/gtviuqidpz.html

================================================================================
来源：http://hz.9152youxi.cn/gtpwewhjwu.html

[M01] 读取命令行参数
来源：http://hz.xuetiantiany.cn/gtufbkupms.html

Py:   sys.argv[1:]
来源：http://hz.yj20258.top/gtrdodklhn.html

PHP:  $argv;  $argc;
来源：http://hz.yuxming.cn/gtfyiylrow.html

JS:   process.argv.slice(2)
来源：http://hz.tianlin.xyz/gtyexwwshl.html

TS:   process.argv.slice(2)
来源：http://hz.smart0.xyz/gtysnchlbg.html

Java: args 数组（main 方法参数）
来源：http://hz.jinyuanbaomall.cn/gtcyxxvwke.html

Go:   os.Args[1:]
来源：http://hz.mhx1999.top/gtliglyewa.html

Ruby: ARGV
来源：http://hz.iojbl.cn/gtreqjwztu.html

C#:   args 数组（Main 方法参数）
来源：http://hz.cashguo.top/gtjqvgnzui.html

[M02] 读取环境变量
来源：http://hz.hnxiangtu.top/gtnkgdssca.html

Py:   os.environ.get("HOME")
来源：http://hz.c1oappe.top/gtttekdwsp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jinyuanbaomall.cn/gttusieqff.html

JS:   process.env.HOME
来源：http://hz.meibo888.top/gtahvtwfdp.html

TS:   process.env.HOME
来源：http://hz.jyoumei.cn/gtzizclxbi.html

Java: System.getenv("HOME")
来源：http://hz.52xcode.cn/gtgqjfijdn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.gzhubu.top/gtxriybncy.html

Ruby: ENV["HOME"]
来源：http://hz.ybcxt.top/gtgfathvfa.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.aizwys.cn/gtwyspxsqc.html

[M03] 执行外部命令
来源：http://hz.jinqigufen.top/gtqevdtarv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.kuanghao11.cn/gtbmaoqqfw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.svipenyu.cn/gtakltjoyi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.svipenyu.cn/gtodtywcxn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.cdnleiting.top/gtttejqcvi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.kuanghao11.cn/gtsuvhnncq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.cucudq.cn/gtsotnlnbn.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.mhx1999.top/gtovbjqfqu.html

C#:   Process.Start("ls", "-l");
来源：http://hz.nwbrower.top/gtrieniule.html

[M04] 获取当前工作目录
来源：http://hz.yj202588.top/gtinncehkk.html

Py:   os.getcwd()
来源：http://hz.xingfuxueyuan.xyz/gtbmlkocyw.html

PHP:  getcwd();
来源：http://hz.zhengqikj.top/gtlzyfyifh.html

JS:   process.cwd()
来源：http://hz.havefunace.top/gtaawebxym.html

TS:   process.cwd()
来源：http://hz.nwbrower.top/gtpkbrrgac.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.feifeiyinyue.top/gtxmgmbtfj.html

Go:   os.Getwd()
来源：http://hz.zhiwuduotai.top/gtvzhpiqkh.html

Ruby: Dir.pwd
来源：http://hz.yongpay.top/gtgrgludwm.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jlsjyb.cn/gtdgtdsckb.html

[M05] 设置退出码
来源：http://hz.hammf.cn/gtuugdpokj.html

Py:   sys.exit(1)
来源：http://hz.52xcode.cn/gtzavxhrlh.html

PHP:  exit(1);
来源：http://hz.quarkkingdee.top/gtleoipszb.html

JS:   process.exit(1)
来源：http://hz.iojbl.cn/gtwramdqfk.html

TS:   process.exit(1)
来源：http://hz.redwolf501.top/gtwhpgjpfj.html

Java: System.exit(1)
来源：http://hz.snrcjt.cn/gteuptsaid.html

Go:   os.Exit(1)
来源：http://hz.redwolf501.top/gtopldzcac.html

Ruby: exit 1
来源：http://hz.jinqigufen.top/gtahqkfumj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yuanzhike.top/gtbhdcckwm.html

[M06] 向标准错误输出
来源：http://hz.zhixingplan.top/gtnfuflsrq.html

Py:   print("err", file=sys.stderr)
来源：http://hz.kuanghao11.cn/gtuzhrhwlm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yuxming.cn/gtlqqqoqlh.html

JS:   console.error("err")
来源：http://hz.jqgufenzy.top/gtmqnskgee.html

TS:   console.error("err")
来源：http://hz.yangfankeji.com/gtwwmadhlw.html

Java: System.err.println("err")
来源：http://hz.zhengqikj.top/gtdpseezec.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.snrcjt.cn/gtpunwkhnq.html

Ruby: warn "err"
来源：http://hz.yvedp.cn/gtoprkuqtf.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ivvv.top/gtrijbzjny.html

[M07] 判断是否为主入口
来源：http://hz.xuetiantiany.cn/gtpmtlfgeq.html

Py:   if __name__ == "__main__":
来源：http://hz.gotoacloud.top/gtrvxqeekc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.hfpthk.cn/gtzemulgwm.html

JS:   require.main === module
来源：http://hz.hfpthk.cn/gtgpiuayiy.html

TS:   require.main === module
来源：http://hz.shangyingyoupin.top/gtflcxxnox.html

Java: public static void main(String[] args)
来源：http://hz.xingfuxueyuan.xyz/gtmwukxjco.html

Go:   func main()
来源：http://hz.jlsjyb.cn/gtjqzqpbda.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zdqjudy.top/gtlwtlcxpw.html

C#:   static void Main(string[] args)
来源：http://hz.meibo888.top/gthmfcvkgt.html

[M08] 获取系统与运行时信息
来源：http://hz.yuanzhike.top/gtnvkbziqr.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhiwuduotai.top/gtfxchiugx.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yj202588.top/gtebqbtfkj.html

JS:   process.platform;  process.version
来源：http://hz.zhongyouzk.top/gthlaiarev.html

TS:   process.platform;  process.version
来源：http://hz.haohaochexian.top/gtyeqbmecc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xinyue.icu/gtipfjbslk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jinqigufen.top/gtcohuxwdj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hfpthk.cn/gtylpnjjlg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yj20258.top/gteilgfzbr.html

================================================================================
来源：http://hz.52xcode.cn/gtiolhsebv.html

N. 数据结构与算法
来源：http://hz.zhixingplan.top/gtfejezhlt.html

================================================================================
来源：http://hz.ybcxt.top/gtlwvkvebd.html

[N01] 二分查找（有序数组）
来源：http://hz.9152youxi.cn/gtdmtowkoi.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.redwolf501.top/gtitedpmsc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.316326.xyz/gtbxnchibe.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shanyushiyangtech.top/gtmcbuwkoh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.svipenyu.cn/gtencflqsn.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.quarkkingdee.top/gtdkqyoiiw.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.dianchejie.cn/gtikwylagj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hongshengwenyu.top/gtsulwknna.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xylfe.cn/gtvysmmqad.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jqgufenzy.top/gtvdxtimfm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.quarkkingdee.top/gtqgdulmtx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.cheryme.top/gtdugstkvr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.c1oappe.top/gtyycjmpmd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.iojbl.cn/gteapkidqa.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.sweek.top/gtcgniyofb.html

Go:   slices.Sort(arr)
来源：http://hz.ydzc1.top/gtddvosori.html

Ruby: arr.sort
来源：http://hz.zhongyouzk.top/gtvuzlmkwj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ywan-chungtsiang.top/gtqikgchcm.html

[N03] 快速排序（分治示例）
来源：http://hz.ydjk.org.cn/gtsywkctlf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hysaishi.cn/gtqbotusah.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xylfe.cn/gtdqgscxtr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.c1oappe.top/gtxcrfkwrj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.kuanghao11.cn/gtsaelbbof.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yonumen.top/gtbysuwpqk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.ybcxt.top/gtuawxvazv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ydjk.org.cn/gtxfdesbkd.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.vqdsnc.cn/gtsnauphml.html

[N04] 斐波那契数列
来源：http://hz.smart0.xyz/gtmrsinfoa.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hywenlv.cn/gtjkmptmav.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jinghuilouyu.cn/gtatmdflis.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinqigufen.top/gtaxiyddbv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hnqzz.top/gtgzrlhkzw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.xingfuxueyuan.xyz/gtqdklfihl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.vqdsnc.cn/gtcwxslsvz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yongpay.top/gtefgfmhgi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zycfv.cn/gtxwjciuix.html

[N05] 最大公约数
来源：http://hz.zdqjudy.top/gtiglccren.html

Py:   math.gcd(a, b)
来源：http://hz.zycfv.cn/gtvnbznzgw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yonumen.top/gtohmantat.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.0kj1m.cn/gtkyclttua.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cqqwz.cn/gtelhojqik.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.nanxuanxn.top/gtnrlsobzn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hnxiangtu.top/gttrxkwlse.html

Ruby: a.gcd(b)
来源：http://hz.sufxvd.cn/gtanxjdhec.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.andypj.xyz/gttqnmmond.html

[N06] 判断回文字符串
来源：http://hz.pengpengdd.cyou/gtjifbscke.html

Py:   s == s[::-1]
来源：http://hz.xuanzx.com/gtdycvpkae.html

PHP:  $s === strrev($s);
来源：http://hz.hammf.cn/gtsnlflghi.html

JS:   s === [...s].reverse().join("")
来源：http://hz.havefunace.top/gtgominkut.html

TS:   s === [...s].reverse().join("")
来源：http://hz.xingfuxueyuan.xyz/gtlghmwawt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.hnxiangtu.top/gtzqyctbbc.html

Go:   // 双指针从两端比较
来源：http://hz.chenlongwang.top/gtqiamvxjn.html

Ruby: s == s.reverse
来源：http://hz.jlsjyb.cn/gtgclihrpe.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.fengsongda.top/gtpmkgndfp.html

[N07] 两数之和（返回下标）
来源：http://hz.aizwys.cn/gtfaqzcgvv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.cheryme.top/gtwmpycgth.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.fzhhl.top/gtlilbnfva.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xuetiantiany.cn/gtldjuflvk.html

TS:   // 手写 Map<string, number>
来源：http://hz.tanke756.top/gtadzmpuws.html

Java: // 手写 HashMap
来源：http://hz.52xcode.cn/gtcehrwpju.html

Go:   // 手写 map[int]int
来源：http://hz.chenzaomai.com/gtbwwuzdvy.html

Ruby: // 手写 Hash
来源：http://hz.zhijiandao.cn/gtndcyyvup.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.ydjk.org.cn/gtphcxqdmv.html

[N08] 生成全排列
来源：http://hz.sxryk.cn/gtcdtgkmol.html

Py:   itertools.permutations(arr)
来源：http://hz.sysykeji.top/gtcetcpnjs.html

PHP:  // 手写递归交换
来源：http://hz.pengpengdd.cyou/gttssvmjla.html

JS:   // 手写回溯递归
来源：http://hz.zhijiandao.cn/gtoyeupgsa.html

TS:   // 手写回溯递归
来源：http://hz.zhoulong.xyz/gtvxtmmfxy.html

Java: // 手写回溯递归
来源：http://hz.jlsjyb.cn/gtmmpohdml.html

Go:   // 手写回溯递归
来源：http://hz.smart0.xyz/gtwyybnenh.html

Ruby: arr.permutation.to_a
来源：http://hz.ehwqpu.com/gtcmicpvjz.html

C#:   // 手写回溯递归
来源：http://hz.sxryk.cn/gtozfsvprp.html

[N09] 栈与队列
来源：http://hz.jinyuanbaomall.cn/gtvxdhpkpz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.hywenlv.cn/gtwdijjlad.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ivvv.top/gtfkkkjxfr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.dashuyun.cn/gtxdcmqymz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ydzc1.top/gtvjavstkk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.iojbl.cn/gtwyfpgcbh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.gogol.net.cn/gthyierckw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.ybcxt.top/gtosjujdyu.html


<!-- 参考信息 -->