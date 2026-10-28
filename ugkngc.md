代发 wailian999

================================================================================
来源：http://hz.aizwys.cn/gtxflwkcuj.html

K. JSON 与序列化
来源：http://hz.jinqigufen.top/gtplzotixd.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtwafvirmg.html

[K01] 对象转 JSON 字符串
来源：http://hz.yangfankeji.com/gtyxwoough.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.xinyue.icu/gttrnxlehp.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.tian-w.cn/gtlocgzxue.html

JS:   JSON.stringify(obj)
来源：http://hz.vqdsnc.cn/gtjuawutjw.html

TS:   JSON.stringify(obj)
来源：http://hz.yvedp.cn/gtxsaiuzhs.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.andypj.xyz/gtbupiznoz.html

Go:   json.Marshal(obj)
来源：http://hz.yueranfly.top/gtknvxhank.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shanyushiyangtech.top/gtfjlsiddv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ehwqpu.com/gtnfnkuxqu.html

[K02] JSON 字符串转对象
来源：http://hz.yuxming.cn/gtlncwbthz.html

Py:   json.loads(s)
来源：http://hz.jianghu66.top/gtxwgdgqcx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.dianchejie.cn/gtzvhdwfdc.html

JS:   JSON.parse(s)
来源：http://hz.ydzc1.top/gtuklhrwmu.html

TS:   JSON.parse(s)
来源：http://hz.zhengqikj.top/gtisdsifie.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xingfuxueyuan.xyz/gtbbuxxzyx.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zycfv.cn/gturxaiokj.html

Ruby: JSON.parse(s)
来源：http://hz.xylfe.cn/gtlbyfcila.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.sweek.top/gttloupjvb.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yongpay.top/gtstjoiniv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yangfankeji.com/gtjsfeszqp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.gogol.net.cn/gtzbleoaoo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ywan-chungtsiang.top/gtqptbvoxn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yonumen.top/gtxlvvoich.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hnxiangtu.top/gtmwbrmmhn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jqgfzy.top/gtuikwgvur.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yj20258888.top/gtsjaaffrv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cheryme.top/gtmtbeltmd.html

[K04] 读取 JSON 文件
来源：http://hz.chenlongwang.top/gtfuxaigok.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.cdnleiting.top/gtdbwigdog.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.nanxuanxn.top/gtyhhzvuzj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shuidangran.top/gtielcmuyw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cashguo.top/gtxwmplatt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.sufxvd.cn/gtshmbcthv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hongshengwenyu.top/gtckxwqvzl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.0kj1m.cn/gtwzmldmgz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.redwolf501.top/gteeepfhbf.html

[K05] 深拷贝对象
来源：http://hz.andypj.xyz/gtejihqutt.html

Py:   copy.deepcopy(obj)
来源：http://hz.zycfv.cn/gtvcfdjxux.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jyoumei.cn/gtcrfsgrbr.html

JS:   structuredClone(obj)
来源：http://hz.chenjidiqi.icu/gtudzoawdf.html

TS:   structuredClone(obj)
来源：http://hz.zhaomingkeji.xyz/gtbpdugyea.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jiagoushi.top/gtzfawhjsr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yj202588.top/gtpktuvmuv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.pycfn.com/gtecmqnusu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.fzhhl.top/gtayzhknoe.html

[K06] 解析 URL 查询串
来源：http://hz.jinyuanbaomall.cn/gtiruzpvnx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.chenzaomai.com/gtnlwjiqyv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hfpthk.cn/gtgrhubybt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hfpthk.cn/gtxiytstvv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jqgufenzy.top/gtfynysulh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jqgfzy.top/gtomzzygjy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.ydzc1.top/gtunzgquzm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.feifeiyinyue.top/gtzkhtecpq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yj20258888.top/gteldtfufp.html

[K07] 进制转换
来源：http://hz.sufxvd.cn/gtnaipcfkl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.xuetiantiany.cn/gtlaxdvzap.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ppjwa.cn/gtoqmbbucz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shanyushiyangtech.top/gttqfnokbt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.shanyushiyangtech.top/gtqeoraxag.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jinqigfzy.top/gtmyqpvyzs.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xylfe.cn/gtlyxvjphc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.shuidangran.top/gttwtvamhu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yuxming.cn/gtgmugqwhm.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.redwolf501.top/gtxbpmyxiy.html

Py:   pickle.dumps(obj)
来源：http://hz.yvedp.cn/gtbidgoucv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.chenjidiqi.icu/gthzucmkgw.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hongshengwenyu.top/gtyhljzwne.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.52xcode.cn/gtnanjjnmx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.316326.xyz/gtnhddprei.html

Go:   encoding/gob
来源：http://hz.cucudq.cn/gtcfarbmfc.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhaomingkeji.xyz/gtbevugvsj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ybcxt.top/gtiwymfvcd.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtwonmtawa.html

L. 网络请求
来源：http://hz.ivvv.top/gtjbhilgtx.html

================================================================================
来源：http://hz.nanxinkj.top/gtkkqekdzp.html

[L01] 发送 GET 请求
来源：http://hz.ydzc1.top/gtsgjdgdsg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zhaomingkeji.xyz/gtdlvkijnv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.chenlongwang.top/gtuslszyyo.html

JS:   await fetch(url)
来源：http://hz.52xcode.cn/gtvftzvxlk.html

TS:   await fetch(url)
来源：http://hz.guannengcc.top/gtkjzrfqqq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.shuidangran.top/gtlmflywan.html

Go:   resp, err := http.Get(url)
来源：http://hz.dianchejie.cn/gtngklbyck.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jlsjyb.cn/gttuvrrfux.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.9152youxi.cn/gtbtgcurch.html

[L02] 发送 POST JSON
来源：http://hz.feifeiyinyue.top/gtffktfvlu.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jianghu66.top/gtnfkrcygo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.shanyushiyangtech.top/gthyswqhbv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.mhx1999.top/gtzhjdefad.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.0kj1m.cn/gtnsskbefv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jinghuilouyu.cn/gtyhyltqge.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.smart0.xyz/gtwveugots.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.c1oappe.top/gtewoiybxi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jiagoushi.top/gtzzjmlllq.html

[L03] 设置自定义请求头
来源：http://hz.sufxvd.cn/gtwziwqodk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhoulong.xyz/gtipvzgcwk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.chenlongwang.top/gtjvdogtbo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shzxlz.cn/gtgslgbvwq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jianghu66.top/gtdfkqgwwi.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.xuanzx.com/gtfwzkwkns.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jinghuilouyu.cn/gtpsxfxmxq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jinghuilouyu.cn/gtfjggryek.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.gzhubu.top/gttxysbgzt.html

[L04] 设置超时
来源：http://hz.vqdsnc.cn/gtsygtneoa.html

Py:   requests.get(url, timeout=5)
来源：http://hz.shanyushiyangkeji.top/gtlnyaehss.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.shangyingyoupin.top/gtpymyjxzm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.c1oappe.top/gtctovcfno.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.dashuyun.cn/gtbbwopibf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.cucudq.cn/gtssqiasas.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yj20258.top/gtsulslqui.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yongpay.top/gtjcpzigdo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.vqdsnc.cn/gtlmrswgym.html

[L05] 上传文件（multipart）
来源：http://hz.tianlin.xyz/gtowcumwoo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jlsjyb.cn/gtdeaeaykr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zdqjudy.top/gtklcntcfs.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.0kj1m.cn/gtmtvyzyss.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhixingplan.top/gtpphbuatv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.fengsongda.top/gttrpmkphz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.guannengcc.top/gtbzizyltc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.0kj1m.cn/gtpwupccfi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhoulong.xyz/gtvwmmwizg.html

[L06] 解析响应为 JSON
来源：http://hz.yonumen.top/gtkodusuax.html

Py:   resp.json()
来源：http://hz.ydjk.org.cn/gtzbhjoano.html

PHP:  json_decode($body, true);
来源：http://hz.jianghu66.top/gtdwrhcxeg.html

JS:   await resp.json()
来源：http://hz.chenjidiqi.icu/gtlamzldvq.html

TS:   await resp.json()
来源：http://hz.hnqzz.top/gtuiwfkgdg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.ppjwa.cn/gtjptwnrgu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hnqzz.top/gtdrwvkvgq.html

Ruby: JSON.parse(resp.body)
来源：http://hz.hysaishi.cn/gtvegaatov.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hywenlv.cn/gthcivtojn.html

[L07] 处理 HTTP 状态码
来源：http://hz.aizwys.cn/gtqblqspgy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhongyouzk.top/gtnpsmdbnq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hysaishi.cn/gtpesttefu.html

JS:   resp.ok;  resp.status
来源：http://hz.andypj.xyz/gtwbbqotkd.html

TS:   resp.ok;  resp.status
来源：http://hz.zhixingplan.top/gtzzsflqwr.html

Java: resp.statusCode()
来源：http://hz.dashuyun.cn/gtxhydgiej.html

Go:   resp.StatusCode
来源：http://hz.guannengcc.top/gteznjnnbh.html

Ruby: resp.code.to_i
来源：http://hz.snrcjt.cn/gtkpdsxghx.html

C#:   (int)resp.StatusCode
来源：http://hz.jianghu66.top/gtmbiacddz.html

[L08] 并发请求多个地址
来源：http://hz.hysaishi.cn/gtjzbatsgh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jianghu66.top/gtfvgukwum.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhoulong.xyz/gtudbgsjqg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.meibo888.top/gtftxkyqmt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhiwuduotai.top/gtgniwfnwj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ydjk.org.cn/gtygfrcesb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hongshengwenyu.top/gtnzmqpttc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ydzc1.top/gtrbwfbawg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.cucudq.cn/gtsmwcmnrc.html

================================================================================
来源：http://hz.sxryk.cn/gtgxxfqfao.html

M. 命令行 / 进程 / 环境
来源：http://hz.yvedp.cn/gtldfhwqdc.html

================================================================================
来源：http://hz.cdnleiting.top/gtzdabfvbz.html

[M01] 读取命令行参数
来源：http://hz.iojbl.cn/gtrzkxibxx.html

Py:   sys.argv[1:]
来源：http://hz.gotoacloud.top/gtuudbjqrw.html

PHP:  $argv;  $argc;
来源：http://hz.cucudq.cn/gtrsiuouek.html

JS:   process.argv.slice(2)
来源：http://hz.kuanghao11.cn/gtuvupqenb.html

TS:   process.argv.slice(2)
来源：http://hz.ydjk.org.cn/gtwfctbhud.html

Java: args 数组（main 方法参数）
来源：http://hz.kuanghao11.cn/gtidxbraio.html

Go:   os.Args[1:]
来源：http://hz.hfpthk.cn/gtggfwuasx.html

Ruby: ARGV
来源：http://hz.jinghuilouyu.cn/gtnmawlzkr.html

C#:   args 数组（Main 方法参数）
来源：http://hz.chenjidiqi.icu/gtxuzrxbaq.html

[M02] 读取环境变量
来源：http://hz.yueranfly.top/gtancdhibx.html

Py:   os.environ.get("HOME")
来源：http://hz.tianlin.xyz/gtdzmfokss.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.gogol.net.cn/gtrlnqkdzu.html

JS:   process.env.HOME
来源：http://hz.jianghu66.top/gtsgdwylli.html

TS:   process.env.HOME
来源：http://hz.feifeiyinyue.top/gttgzzfyip.html

Java: System.getenv("HOME")
来源：http://hz.bjfxy.top/gthnoakibt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.ppjwa.cn/gtnizbhyhm.html

Ruby: ENV["HOME"]
来源：http://hz.9152youxi.cn/gtkhxhmcfz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jinghuilouyu.cn/gtpszkgsqv.html

[M03] 执行外部命令
来源：http://hz.52xcode.cn/gtpskvnrsv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jqgufenzy.top/gtpmdqvhyj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.fengsongda.top/gtofcqtnmq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.chenlongwang.top/gtkajillrc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.snrcjt.cn/gtigwmqlxn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhongyouzk.top/gtceiuhhwy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hongshengwenyu.top/gtemnlzuzs.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.nanxinkj.top/gtrmcdhfxf.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yuanzhike.top/gtzaonozdz.html

[M04] 获取当前工作目录
来源：http://hz.svipenyu.cn/gtbcvwzeof.html

Py:   os.getcwd()
来源：http://hz.wangshuangyany.cn/gtfszpurxi.html

PHP:  getcwd();
来源：http://hz.wangdashe.top/gtsqlmcqke.html

JS:   process.cwd()
来源：http://hz.nwbrower.top/gtjycwecpv.html

TS:   process.cwd()
来源：http://hz.wangshuangyany.cn/gtlukrcoza.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.gzhubu.top/gtuvofilsh.html

Go:   os.Getwd()
来源：http://hz.nanxinkj.top/gtibozdnsu.html

Ruby: Dir.pwd
来源：http://hz.wangshuangyany.cn/gtjyzuiwfd.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.tian-w.cn/gtyhvmnqst.html

[M05] 设置退出码
来源：http://hz.ydzc1.top/gtgdpaiwkx.html

Py:   sys.exit(1)
来源：http://hz.snrcjt.cn/gtlpiuphyr.html

PHP:  exit(1);
来源：http://hz.zycfv.cn/gtysknijop.html

JS:   process.exit(1)
来源：http://hz.sufxvd.cn/gtfjaquqto.html

TS:   process.exit(1)
来源：http://hz.andypj.xyz/gtevpbinhg.html

Java: System.exit(1)
来源：http://hz.ydjk.org.cn/gtajiphlzs.html

Go:   os.Exit(1)
来源：http://hz.zhixingplan.top/gtfgjwnxue.html

Ruby: exit 1
来源：http://hz.svipenyu.cn/gtgqybebfo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.pycfn.com/gtqslivwua.html

[M06] 向标准错误输出
来源：http://hz.ppjwa.cn/gtmttzjzpx.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ydzc1.top/gtklzvrqgf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xingfuxueyuan.xyz/gtwxlrmzzn.html

JS:   console.error("err")
来源：http://hz.yuxming.cn/gtnsnpuepk.html

TS:   console.error("err")
来源：http://hz.jqgufenzy.top/gtniblzbuy.html

Java: System.err.println("err")
来源：http://hz.jianghu66.top/gtxkkxxqrh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ivvv.top/gtinpajcqn.html

Ruby: warn "err"
来源：http://hz.daria6918.cn/gthcbfwrqq.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jlsjyb.cn/gtkgeggaql.html

[M07] 判断是否为主入口
来源：http://hz.daria6918.cn/gtzwjfpaht.html

Py:   if __name__ == "__main__":
来源：http://hz.zdqjudy.top/gtctogyemg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.gzhubu.top/gtuikndeme.html

JS:   require.main === module
来源：http://hz.dashuyun.cn/gtzzkajirz.html

TS:   require.main === module
来源：http://hz.gzhubu.top/gtpkyopkug.html

Java: public static void main(String[] args)
来源：http://hz.shuidangran.top/gtnzyhcqhz.html

Go:   func main()
来源：http://hz.jiagoushi.top/gtyvqdritw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.shuidangran.top/gtekerpgvb.html

C#:   static void Main(string[] args)
来源：http://hz.yanxiufei.cn/gtbgxafhec.html

[M08] 获取系统与运行时信息
来源：http://hz.nanxuanxn.top/gtmbentfdq.html

Py:   platform.system();  platform.python_version()
来源：http://hz.cheryme.top/gtnchxpzve.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jianghu66.top/gtuekwysww.html

JS:   process.platform;  process.version
来源：http://hz.smart0.xyz/gtapoikufv.html

TS:   process.platform;  process.version
来源：http://hz.sxryk.cn/gtbzjqzlfw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.ydjk.org.cn/gtzseqsfxj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yj20258.top/gtxeydnlxr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ppjwa.cn/gtrdqmcafu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hfpthk.cn/gthlwqfaqh.html

================================================================================
来源：http://hz.cdnleiting.top/gtrohmktrw.html

N. 数据结构与算法
来源：http://hz.svipenyu.cn/gtlflalhnn.html

================================================================================
来源：http://hz.cashguo.top/gtgxwfrnec.html

[N01] 二分查找（有序数组）
来源：http://hz.tianlin.xyz/gtpwdkxgoh.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.52xcode.cn/gthuxzkgun.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ybcxt.top/gtszcpjjvm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.nanxuanxn.top/gtxvluzygu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shzxlz.cn/gtqfrjdoyh.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hywenlv.cn/gtttvmeaib.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cucudq.cn/gtyfmqbaiy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yj202588.top/gtrqrmtkpt.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.chenzaomai.com/gtxhpzhahw.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.chenzaomai.com/gtjgougkau.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ppjwa.cn/gtuxktvzgv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.fengsongda.top/gtvsroxezn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.dashuyun.cn/gteemvgtvn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yangfankeji.com/gtfeewwkju.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.nwbrower.top/gtftxmuaou.html

Go:   slices.Sort(arr)
来源：http://hz.52xcode.cn/gtzctikvjc.html

Ruby: arr.sort
来源：http://hz.zhengqikj.top/gtijsebemd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.haohaochexian.top/gtwgnlfutk.html

[N03] 快速排序（分治示例）
来源：http://hz.quarkkingdee.top/gtnkdpyfgj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.gotoacloud.top/gtscrbgppg.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yueranfly.top/gtggvzsmmb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.snrcjt.cn/gtrgtqyuqb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.quarkkingdee.top/gtxmglkdex.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.shanyushiyangtech.top/gtuscrfndi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.hammf.cn/gtxwkuwtxq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.vqdsnc.cn/gtqssbnwzf.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.cheryme.top/gtuxelyzph.html

[N04] 斐波那契数列
来源：http://hz.zycfv.cn/gtdrpbtdau.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.snrcjt.cn/gttbytrwxn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jinqigfzy.top/gttktkphtq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinyuanbaomall.cn/gtytoqfmrp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nanxinkj.top/gtpvkdfpcp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.feifeiyinyue.top/gtuhlpqxmn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jinghuilouyu.cn/gtwpalbguf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.gogol.net.cn/gtaesbtrmp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.ydzc1.top/gthohfrpvg.html

[N05] 最大公约数
来源：http://hz.fzhhl.top/gtgqidyrej.html

Py:   math.gcd(a, b)
来源：http://hz.aibaodan.cn/gtiobkmxwe.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yongpay.top/gtfhqfztus.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shuidangran.top/gtxbqioytm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.smart0.xyz/gturukxrox.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zhaomingkeji.xyz/gtbqhoefaq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hnxiangtu.top/gtzlzjolze.html

Ruby: a.gcd(b)
来源：http://hz.cqqwz.cn/gthkiixwiv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhongyouzk.top/gtfxukpblj.html

[N06] 判断回文字符串
来源：http://hz.snrcjt.cn/gtvimkryha.html

Py:   s == s[::-1]
来源：http://hz.dashuyun.cn/gtewivluze.html

PHP:  $s === strrev($s);
来源：http://hz.iojbl.cn/gtjwoqwpyp.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhengqikj.top/gtormspwny.html

TS:   s === [...s].reverse().join("")
来源：http://hz.daxiang520.top/gtiyilpuog.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.gzhubu.top/gtmikvcaoh.html

Go:   // 双指针从两端比较
来源：http://hz.chenlongwang.top/gtvnptkqmg.html

Ruby: s == s.reverse
来源：http://hz.tian-w.cn/gtomupukve.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.chenzaomai.com/gtvbrnqiye.html

[N07] 两数之和（返回下标）
来源：http://hz.snrcjt.cn/gtawggavnp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.52xcode.cn/gtvigtmdtj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.birdmap.top/gtxiuwhxns.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.gzhubu.top/gtimlrmbxu.html

TS:   // 手写 Map<string, number>
来源：http://hz.xuetiantiany.cn/gtxvhqsxht.html

Java: // 手写 HashMap
来源：http://hz.ivvv.top/gtjkwzcvcm.html

Go:   // 手写 map[int]int
来源：http://hz.ywan-chungtsiang.top/gtpappivyz.html

Ruby: // 手写 Hash
来源：http://hz.vqdsnc.cn/gtlhlpojne.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zycfv.cn/gtvhkvuboo.html

[N08] 生成全排列
来源：http://hz.bjfxy.top/gtezhvvxeh.html

Py:   itertools.permutations(arr)
来源：http://hz.zhoulong.xyz/gtbsxmhjik.html

PHP:  // 手写递归交换
来源：http://hz.cashguo.top/gtphlysaor.html

JS:   // 手写回溯递归
来源：http://hz.aizwys.cn/gtaciuzjqr.html

TS:   // 手写回溯递归
来源：http://hz.yonumen.top/gtwqvvpyoz.html

Java: // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gtpwaqjzmk.html

Go:   // 手写回溯递归
来源：http://hz.zhengqikj.top/gtsvwpcrhu.html

Ruby: arr.permutation.to_a
来源：http://hz.andypj.xyz/gtijnticij.html

C#:   // 手写回溯递归
来源：http://hz.zhoulong.xyz/gtiiqblrlx.html


<!-- 参考信息 -->