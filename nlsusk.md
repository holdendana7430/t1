代发 wailian999

================================================================================
来源：http://hz.cdnleiting.top/gtsealslip.html

K. JSON 与序列化
来源：http://hz.xinyue.icu/gtvsamtaoq.html

================================================================================
来源：http://hz.gzhubu.top/gtvmhrcbzp.html

[K01] 对象转 JSON 字符串
来源：http://hz.jlsjyb.cn/gtrihnhvnf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.birdmap.top/gthnaksoly.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.vqdsnc.cn/gtghhnchkp.html

JS:   JSON.stringify(obj)
来源：http://hz.redwolf501.top/gtxexcssjg.html

TS:   JSON.stringify(obj)
来源：http://hz.jqgfzy.top/gtiramjedq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.smart0.xyz/gtawrtjcoe.html

Go:   json.Marshal(obj)
来源：http://hz.gotoacloud.top/gtaelzdxab.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cheryme.top/gtvvtphrke.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.dashuyun.cn/gthdrlrcru.html

[K02] JSON 字符串转对象
来源：http://hz.bjfxy.top/gtahchbgqi.html

Py:   json.loads(s)
来源：http://hz.cdnleiting.top/gtocehxzso.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yj20258.top/gtzmkvxeqq.html

JS:   JSON.parse(s)
来源：http://hz.fengsongda.top/gtlfpnpmfr.html

TS:   JSON.parse(s)
来源：http://hz.pycfn.com/gtgzevsdzp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.cdnleiting.top/gthdwymfsc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xingfuxueyuan.xyz/gtbboeanhi.html

Ruby: JSON.parse(s)
来源：http://hz.quarkkingdee.top/gtdlbcbvbs.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hongshengwenyu.top/gtykcbiojj.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.xziqi.cn/gtkdfkzide.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jinyuanbaomall.cn/gtcnbvggjn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.wangshuangyany.cn/gtjfegteaa.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.snrcjt.cn/gtspjerhjm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.52xcode.cn/gthpbankfg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hysaishi.cn/gtzzbgdwkm.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jqgfzy.top/gtibpoelcg.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.shzxlz.cn/gtghrbojak.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zdqjudy.top/gthrpmvqft.html

[K04] 读取 JSON 文件
来源：http://hz.xziqi.cn/gtzwejydhu.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yj20258.top/gthrniyfxn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.daxiang520.top/gtwvpqhejw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jianghu66.top/gtwkifqpaa.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.guowangkeji.top/gthqpjorcq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jqgufenzy.top/gtlqqrelaa.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhiwuduotai.top/gtoofdmabu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.0kj1m.cn/gtfntwbbrp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.pycfn.com/gtgqgxegeu.html

[K05] 深拷贝对象
来源：http://hz.jqgfzy.top/gtxjlhyutx.html

Py:   copy.deepcopy(obj)
来源：http://hz.tanke756.top/gtttgueicx.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hywenlv.cn/gtmzqtgyam.html

JS:   structuredClone(obj)
来源：http://hz.zhiwuduotai.top/gtktfvnzlx.html

TS:   structuredClone(obj)
来源：http://hz.quarkkingdee.top/gtovjywjwv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jianghu66.top/gtanaooamo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.aibaodan.cn/gthrfexfmc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yj202588.top/gtvzjnzxwi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.guannengcc.top/gtybghugey.html

[K06] 解析 URL 查询串
来源：http://hz.tianlin.xyz/gtwcqjdjsu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yj20258888.top/gtwoonxhzs.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yj20258888.top/gtxiveznyr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jyoumei.cn/gtmuzwzepd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.guowangkeji.top/gtqupmcvly.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yuxming.cn/gtwvbifcqf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.52xcode.cn/gtgdpltrwz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.tanke756.top/gtdhxcwsbq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.shangyingyoupin.top/gtbxaeachm.html

[K07] 进制转换
来源：http://hz.chenjidiqi.icu/gtpkujkcsd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ydzc1.top/gtipfgjaxe.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.sufxvd.cn/gtblksdspo.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.316326.xyz/gtljihdonp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yangfankeji.com/gtmawfsrsl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.9152youxi.cn/gtasdoszel.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhixingplan.top/gtsckuzzkw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yj202588.top/gtvnmxwyjc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.smart0.xyz/gteqojjkab.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.9152youxi.cn/gtcpttjpii.html

Py:   pickle.dumps(obj)
来源：http://hz.zhaomingkeji.xyz/gtuutuszou.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yj20258888.top/gtdcweyyqv.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zdqjudy.top/gtwpciceky.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.316326.xyz/gtpjnfyoqw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhengqikj.top/gttwyyrlpv.html

Go:   encoding/gob
来源：http://hz.yangfankeji.com/gtisjeemdy.html

Ruby: Marshal.dump(obj)
来源：http://hz.xinyue.icu/gtrhrsghne.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zdqjudy.top/gtdpmonohp.html

================================================================================
来源：http://hz.hysaishi.cn/gtwiysypst.html

L. 网络请求
来源：http://hz.hfpthk.cn/gtndpxohvd.html

================================================================================
来源：http://hz.xinyue.icu/gtwaxreckm.html

[L01] 发送 GET 请求
来源：http://hz.haohaochexian.top/gtdinwzibh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jinghuilouyu.cn/gtptbugqrj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.sysykeji.top/gthifxqagd.html

JS:   await fetch(url)
来源：http://hz.zhoulong.xyz/gtlspgdhve.html

TS:   await fetch(url)
来源：http://hz.smart0.xyz/gtqfmphuwh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yongpay.top/gtfuzfbrjg.html

Go:   resp, err := http.Get(url)
来源：http://hz.cucudq.cn/gtbpqrvsny.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hfpthk.cn/gtuiaikmui.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.pycfn.com/gtjyqsmbjb.html

[L02] 发送 POST JSON
来源：http://hz.9152youxi.cn/gtyhgwkwql.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.cashguo.top/gthntyxjew.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ybcxt.top/gtzumixdin.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jqgufenzy.top/gtjmqknfyq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tian-w.cn/gtsquylwzj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.quarkkingdee.top/gtwqwhfrav.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.snrcjt.cn/gtdtkvlfxa.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhoulong.xyz/gtefwohwxd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xuanzx.com/gtuwgsqkre.html

[L03] 设置自定义请求头
来源：http://hz.ybcxt.top/gtdpdehhga.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ybcxt.top/gteqjhjckl.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jinqigfzy.top/gtdhfvfiqj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.andypj.xyz/gtdthkmama.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hnqzz.top/gtmrooxfsw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.vqdsnc.cn/gtpeikrery.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.xylfe.cn/gtipsvmbsu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.feifeiyinyue.top/gtzqimisle.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhaomingkeji.xyz/gtpthlwhrh.html

[L04] 设置超时
来源：http://hz.c1oappe.top/gttfypvucv.html

Py:   requests.get(url, timeout=5)
来源：http://hz.bjfxy.top/gthqitybao.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.xingfuxueyuan.xyz/gtjsyhbigo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ehwqpu.com/gtyxyocjqt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hammf.cn/gtnuxayapm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.nanxinkj.top/gtttbloknv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.sweek.top/gtvgyyvgvh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hongshengwenyu.top/gtnjdjfaot.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.iojbl.cn/gtfgzjboiw.html

[L05] 上传文件（multipart）
来源：http://hz.c1oappe.top/gthbubbjif.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.sufxvd.cn/gtlrhrazub.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xingfuxueyuan.xyz/gtvwhajbfz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.cqqwz.cn/gttzeydanp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.dianchejie.cn/gtrslffbsx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jinghuilouyu.cn/gtlxnrxyxd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jinyuanbaomall.cn/gtjkjmubxl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhongyouzk.top/gtvmwzllla.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.daria6918.cn/gtiuptmidc.html

[L06] 解析响应为 JSON
来源：http://hz.ybcxt.top/gtqwixhhhs.html

Py:   resp.json()
来源：http://hz.guowangkeji.top/gtzbhgxzdn.html

PHP:  json_decode($body, true);
来源：http://hz.dianchejie.cn/gtxpqhwnnz.html

JS:   await resp.json()
来源：http://hz.dianchejie.cn/gtaicfzkoa.html

TS:   await resp.json()
来源：http://hz.cdnleiting.top/gtyujmqjfx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.xingfuxueyuan.xyz/gtphheegqx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xuetiantiany.cn/gtjynbkhgg.html

Ruby: JSON.parse(resp.body)
来源：http://hz.sxryk.cn/gtfbxibqqv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yj20258888.top/gthlsolbvn.html

[L07] 处理 HTTP 状态码
来源：http://hz.chenzaomai.com/gtamscmrat.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hysaishi.cn/gtvibjarth.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jinyuanbaomall.cn/gtadehglpz.html

JS:   resp.ok;  resp.status
来源：http://hz.zdqjudy.top/gtveusskpx.html

TS:   resp.ok;  resp.status
来源：http://hz.sweek.top/gtrnakfxvk.html

Java: resp.statusCode()
来源：http://hz.daria6918.cn/gthypzzkjb.html

Go:   resp.StatusCode
来源：http://hz.shzxlz.cn/gtbmuaqpwg.html

Ruby: resp.code.to_i
来源：http://hz.yuanzhike.top/gteelfolba.html

C#:   (int)resp.StatusCode
来源：http://hz.hammf.cn/gtbgsvvjpu.html

[L08] 并发请求多个地址
来源：http://hz.birdmap.top/gtlzshbvlx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jlsjyb.cn/gtjglkxfbv.html

PHP:  curl_multi_init() 系列
来源：http://hz.ydjk.org.cn/gtbhxubkii.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nwbrower.top/gtsnwyageb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jianghu66.top/gtfnnwrvvi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.gzhubu.top/gtmxoypnmm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.cucudq.cn/gtsbfhngye.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.meibo888.top/gtzjuhzorp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.redwolf501.top/gthumpveut.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtwaugecuu.html

M. 命令行 / 进程 / 环境
来源：http://hz.ivvv.top/gtbgmygxxh.html

================================================================================
来源：http://hz.iojbl.cn/gthnkhltif.html

[M01] 读取命令行参数
来源：http://hz.guannengcc.top/gtoexmgkza.html

Py:   sys.argv[1:]
来源：http://hz.quarkkingdee.top/gthywmxozl.html

PHP:  $argv;  $argc;
来源：http://hz.svipenyu.cn/gtlnatganl.html

JS:   process.argv.slice(2)
来源：http://hz.jinqigfzy.top/gtmyrhkglz.html

TS:   process.argv.slice(2)
来源：http://hz.kuanghao11.cn/gtfozcrrsf.html

Java: args 数组（main 方法参数）
来源：http://hz.hywenlv.cn/gtfrivgxlp.html

Go:   os.Args[1:]
来源：http://hz.ehwqpu.com/gtvbbdjzyu.html

Ruby: ARGV
来源：http://hz.yangfankeji.com/gttxnmpygk.html

C#:   args 数组（Main 方法参数）
来源：http://hz.dashuyun.cn/gtfwnfiayq.html

[M02] 读取环境变量
来源：http://hz.zhoulong.xyz/gtqqrmibaq.html

Py:   os.environ.get("HOME")
来源：http://hz.quarkkingdee.top/gtlyaaimfn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.meibo888.top/gtexdyxrjk.html

JS:   process.env.HOME
来源：http://hz.sweek.top/gtkmcpgaqk.html

TS:   process.env.HOME
来源：http://hz.ybcxt.top/gtktuntprh.html

Java: System.getenv("HOME")
来源：http://hz.ehwqpu.com/gtfbbiswoz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.chenjidiqi.icu/gtbpxnesnt.html

Ruby: ENV["HOME"]
来源：http://hz.nanxinkj.top/gtvljqjrgu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.pengpengdd.cyou/gtyouqfkoo.html

[M03] 执行外部命令
来源：http://hz.zhengqikj.top/gtdvqbkpkb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.aizwys.cn/gtmxdxokya.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.tian-w.cn/gtlruukkfp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.nwbrower.top/gtpzcgymtw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.gaohongyu789.top/gtsvgsavng.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.cashguo.top/gthbkhckzv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.sweek.top/gtcgmwlcoj.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.cdnleiting.top/gtfrfxtqwn.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yvedp.cn/gtsikdfrux.html

[M04] 获取当前工作目录
来源：http://hz.gaohongyu789.top/gtcxrgftfv.html

Py:   os.getcwd()
来源：http://hz.cashguo.top/gtsilgxhvv.html

PHP:  getcwd();
来源：http://hz.nwbrower.top/gtncnlxyrn.html

JS:   process.cwd()
来源：http://hz.shanyushiyangtech.top/gttrpcktdx.html

TS:   process.cwd()
来源：http://hz.jyoumei.cn/gtoievxudg.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.feifeiyinyue.top/gttihipzax.html

Go:   os.Getwd()
来源：http://hz.yuxming.cn/gtshmiwfyx.html

Ruby: Dir.pwd
来源：http://hz.jlsjyb.cn/gtptscykba.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hysaishi.cn/gtzxcvvbqp.html

[M05] 设置退出码
来源：http://hz.sufxvd.cn/gtkskyvjtp.html

Py:   sys.exit(1)
来源：http://hz.ppjwa.cn/gtdgjqjhem.html

PHP:  exit(1);
来源：http://hz.nanxuanxn.top/gtkcinowoi.html

JS:   process.exit(1)
来源：http://hz.chenlongwang.top/gtrgsvpiqb.html

TS:   process.exit(1)
来源：http://hz.snrcjt.cn/gtojmdsnza.html

Java: System.exit(1)
来源：http://hz.yj202588.top/gtmtlokzgu.html

Go:   os.Exit(1)
来源：http://hz.shzxlz.cn/gtjbempgmy.html

Ruby: exit 1
来源：http://hz.yongpay.top/gtoizztbwf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.redwolf501.top/gtgwzdogiw.html

[M06] 向标准错误输出
来源：http://hz.bjfxy.top/gtbjiiukac.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yj20258.top/gtzsknouey.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.nanxinkj.top/gtrrvzasyq.html

JS:   console.error("err")
来源：http://hz.jianghu66.top/gtdifuqper.html

TS:   console.error("err")
来源：http://hz.smart0.xyz/gtpsxhtiqf.html

Java: System.err.println("err")
来源：http://hz.zhaomingkeji.xyz/gtllahwiav.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ybcxt.top/gtlmimvfea.html

Ruby: warn "err"
来源：http://hz.zhaomingkeji.xyz/gtjhmiywys.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhaomingkeji.xyz/gtqoycfqkv.html

[M07] 判断是否为主入口
来源：http://hz.bjfxy.top/gtrykitvho.html

Py:   if __name__ == "__main__":
来源：http://hz.tanke756.top/gtrvbouhvl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shzxlz.cn/gterjuqmcr.html

JS:   require.main === module
来源：http://hz.shangyingyoupin.top/gtpfjdaiqp.html

TS:   require.main === module
来源：http://hz.jyoumei.cn/gtjhnvkszl.html

Java: public static void main(String[] args)
来源：http://hz.yvedp.cn/gtccimxhwb.html

Go:   func main()
来源：http://hz.ivvv.top/gtedpddalx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jlsjyb.cn/gttfubkjpo.html

C#:   static void Main(string[] args)
来源：http://hz.ivvv.top/gtqktibqnq.html

[M08] 获取系统与运行时信息
来源：http://hz.cashguo.top/gtywtahzoc.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ivvv.top/gtppkknvai.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.gaohongyu789.top/gtpsaxdfly.html

JS:   process.platform;  process.version
来源：http://hz.smart0.xyz/gtfxtqtsdb.html

TS:   process.platform;  process.version
来源：http://hz.yj20258.top/gtcgqskvhx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.nanxinkj.top/gtfjyqpkpg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jqgfzy.top/gtrczwrptl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.chenlongwang.top/gtgcjwtfri.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.kuanghao11.cn/gtrfkobhbl.html

================================================================================
来源：http://hz.jinqigufen.top/gtdcweuolg.html

N. 数据结构与算法
来源：http://hz.wangdashe.top/gtqjzqcqqz.html

================================================================================
来源：http://hz.redwolf501.top/gtxhquzgai.html

[N01] 二分查找（有序数组）
来源：http://hz.zhongyouzk.top/gtntqqbbyk.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.gogol.net.cn/gtyqwxkcsl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.svipenyu.cn/gtonurqjsj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhengqikj.top/gticgycujg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.vqdsnc.cn/gtivasppxh.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.guowangkeji.top/gtxhrdtoph.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.nwbrower.top/gtdzezjhhn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.shanyushiyangtech.top/gtgeqzbema.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ehwqpu.com/gtkqbilfpx.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ywan-chungtsiang.top/gtgvlluqsv.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xingfuxueyuan.xyz/gtczxtqhiv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhaomingkeji.xyz/gthrhiamnu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nanxuanxn.top/gtacanwzud.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.vqdsnc.cn/gtcydvoafb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hnqzz.top/gttluimems.html

Go:   slices.Sort(arr)
来源：http://hz.jqgfzy.top/gttfqdgpfk.html

Ruby: arr.sort
来源：http://hz.aibaodan.cn/gthlpxiynl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jinghuilouyu.cn/gtwyndpzvd.html

[N03] 快速排序（分治示例）
来源：http://hz.shangyingyoupin.top/gtspimwryc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.mhx1999.top/gtdrcmutwr.html

PHP:  // 递归实现，或用 usort
来源：http://hz.guowangkeji.top/gtyktiakox.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cheryme.top/gtchbnbntb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ivvv.top/gtweuifdrc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinyuanbaomall.cn/gtaiszvoqc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.shanyushiyangkeji.top/gtqofbkswc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yuxming.cn/gtumwrgkzt.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhengqikj.top/gtifyobmbx.html

[N04] 斐波那契数列
来源：http://hz.meibo888.top/gtveeapsjo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.smart0.xyz/gtopbbowmt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yuanzhike.top/gtebezgsco.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.tian-w.cn/gttmbacywg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.bjfxy.top/gtfpshctau.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.cucudq.cn/gtmuhtjnok.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ppjwa.cn/gtdospeazj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.gzhubu.top/gtpvkqhsev.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.chenlongwang.top/gtcavcxobk.html

[N05] 最大公约数
来源：http://hz.sysykeji.top/gtgsekragd.html

Py:   math.gcd(a, b)
来源：http://hz.zhiwuduotai.top/gtqtmtxcup.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.sweek.top/gtdebkbcdx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sxryk.cn/gtdhexksnj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yj20258888.top/gtouhqclib.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.andypj.xyz/gtkpuvuwfj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.ydjk.org.cn/gthoxhmvmb.html

Ruby: a.gcd(b)
来源：http://hz.ybcxt.top/gtzckebyph.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.gzhubu.top/gtxylrzqey.html

[N06] 判断回文字符串
来源：http://hz.wangdashe.top/gtgdelgyfk.html

Py:   s == s[::-1]
来源：http://hz.ydjk.org.cn/gtfarxagsd.html

PHP:  $s === strrev($s);
来源：http://hz.zycfv.cn/gtjuurvile.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhongyouzk.top/gtvonzdbwd.html

TS:   s === [...s].reverse().join("")
来源：http://hz.cashguo.top/gttgzogyyl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yj20258888.top/gtyimybstt.html

Go:   // 双指针从两端比较
来源：http://hz.kuanghao11.cn/gtfutyxjzi.html

Ruby: s == s.reverse
来源：http://hz.pengpengdd.cyou/gtxredyjmo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.smart0.xyz/gtznkhxmih.html

[N07] 两数之和（返回下标）
来源：http://hz.vqdsnc.cn/gtusnpdrui.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hfpthk.cn/gtdjotnerz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.cheryme.top/gtcpvccncb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.shzxlz.cn/gtnccblmto.html

TS:   // 手写 Map<string, number>
来源：http://hz.quarkkingdee.top/gtxyhwxvhq.html

Java: // 手写 HashMap
来源：http://hz.9152youxi.cn/gtqneamygy.html

Go:   // 手写 map[int]int
来源：http://hz.xylfe.cn/gtqxceoifp.html

Ruby: // 手写 Hash
来源：http://hz.tanke756.top/gtwqawhody.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.cqqwz.cn/gtjwafczhz.html

[N08] 生成全排列
来源：http://hz.cucudq.cn/gtovralbcf.html

Py:   itertools.permutations(arr)
来源：http://hz.yueranfly.top/gtduyemboe.html

PHP:  // 手写递归交换
来源：http://hz.cheryme.top/gtgzqshplx.html

JS:   // 手写回溯递归
来源：http://hz.cheryme.top/gtwprdtcvw.html

TS:   // 手写回溯递归
来源：http://hz.tian-w.cn/gtzedtymnj.html

Java: // 手写回溯递归
来源：http://hz.0kj1m.cn/gtgqioxsqt.html

Go:   // 手写回溯递归
来源：http://hz.zhoulong.xyz/gtafwfutfr.html

Ruby: arr.permutation.to_a
来源：http://hz.vqdsnc.cn/gtsmimjboh.html

C#:   // 手写回溯递归
来源：http://hz.chenzaomai.com/gtnnxvxymg.html


<!-- 参考信息 -->