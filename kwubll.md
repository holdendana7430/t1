代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jlsjyb.cn/gttkibntfk.html

Go:   json.Marshal(obj)
来源：http://hz.havefunace.top/gtpfpzdwmd.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yvedp.cn/gtlxmlvkgg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hfpthk.cn/gtrvyszmgz.html

[K02] JSON 字符串转对象
来源：http://hz.pycfn.com/gtgcbvshwy.html

Py:   json.loads(s)
来源：http://hz.iojbl.cn/gtgrauoehk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.dashuyun.cn/gtkneoolwz.html

JS:   JSON.parse(s)
来源：http://hz.daria6918.cn/gtiyombvvd.html

TS:   JSON.parse(s)
来源：http://hz.xuanzx.com/gtjccqaewp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhiwuduotai.top/gtegvurpnd.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.birdmap.top/gtxghbjfzj.html

Ruby: JSON.parse(s)
来源：http://hz.yj202588.top/gtayptmsau.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jianghu66.top/gtbtpphfoj.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.sweek.top/gttlhccqar.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.snrcjt.cn/gtncumroej.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.cqqwz.cn/gtgdfzgmnt.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.gotoacloud.top/gtbtiowdgz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.daria6918.cn/gtnbwmnlys.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.cdnleiting.top/gtplzpvsfh.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhoulong.xyz/gtjhifcdcr.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.52xcode.cn/gtakrubiea.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ywan-chungtsiang.top/gtavtlvgrl.html

[K04] 读取 JSON 文件
来源：http://hz.wangdashe.top/gtfwmcvzgf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hywenlv.cn/gthunsbdsg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yangfankeji.com/gtjhpotgjk.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sxryk.cn/gtnefoxjbz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hywenlv.cn/gtzkzsweow.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hywenlv.cn/gtplpctkuw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhiwuduotai.top/gtdedgxiav.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.chenzaomai.com/gtqgtpavky.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.tianlin.xyz/gtxsbkwzzi.html

[K05] 深拷贝对象
来源：http://hz.yvedp.cn/gttkjmerwe.html

Py:   copy.deepcopy(obj)
来源：http://hz.daxiang520.top/gtuzzwncdi.html

PHP:  unserialize(serialize($obj));
来源：http://hz.dianchejie.cn/gtcgbnbsnb.html

JS:   structuredClone(obj)
来源：http://hz.yongpay.top/gtmkschhce.html

TS:   structuredClone(obj)
来源：http://hz.jinqigufen.top/gtfdolelqm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.sweek.top/gtiatfcqeg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.aizwys.cn/gttnikrxiz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ydzc1.top/gtjawktxek.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ybcxt.top/gtkyaufgdx.html

[K06] 解析 URL 查询串
来源：http://hz.fzhhl.top/gtpbpztrul.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.pengpengdd.cyou/gtdpnaaucw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.feifeiyinyue.top/gtmhxndtgt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.birdmap.top/gtxrncyber.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.c1oappe.top/gtkourltfv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.gogol.net.cn/gtkpgzrlxa.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.bjfxy.top/gtzoxbzewl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.tian-w.cn/gtovfllfer.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhijiandao.cn/gttnzpyzjc.html

[K07] 进制转换
来源：http://hz.tian-w.cn/gtfjekxccx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.kuanghao11.cn/gtlgpoyhom.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.cheryme.top/gtavwcnywh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.iojbl.cn/gtzibaskgt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yanxiufei.cn/gtxtckqvcl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xinyue.icu/gtnjzhzswx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hammf.cn/gtejnpzkjq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xuetiantiany.cn/gthpzpnwvn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hnxiangtu.top/gtvxjjihef.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.hongshengwenyu.top/gtjephxgod.html

Py:   pickle.dumps(obj)
来源：http://hz.ppjwa.cn/gtrojekptp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jinqigufen.top/gtritqlmcr.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yonumen.top/gtczcrhbko.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.gogol.net.cn/gtvpajznvq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hysaishi.cn/gtoermpeay.html

Go:   encoding/gob
来源：http://hz.zhixingplan.top/gtgwqbolbj.html

Ruby: Marshal.dump(obj)
来源：http://hz.pengpengdd.cyou/gtxfsjfcgy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.c1oappe.top/gtcrtbroiu.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtslmfuztl.html

L. 网络请求
来源：http://hz.shanyushiyangtech.top/gtrnvipuwl.html

================================================================================
来源：http://hz.ybcxt.top/gticrxsqdr.html

[L01] 发送 GET 请求
来源：http://hz.zhoulong.xyz/gtxqsxemif.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.xinyue.icu/gtbprbhhdb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.cashguo.top/gtznfhcyjl.html

JS:   await fetch(url)
来源：http://hz.ppjwa.cn/gtcywzfjnb.html

TS:   await fetch(url)
来源：http://hz.gogol.net.cn/gtubtddflm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yuxming.cn/gtzcqaufrz.html

Go:   resp, err := http.Get(url)
来源：http://hz.nwbrower.top/gtgjxdbqyi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.guowangkeji.top/gthfyxreow.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hammf.cn/gtzyyjzsth.html

[L02] 发送 POST JSON
来源：http://hz.shanyushiyangtech.top/gtdgcqvppj.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zycfv.cn/gttfualsgt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ywan-chungtsiang.top/gtbyecexmy.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.pengpengdd.cyou/gtncyqbqhd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sufxvd.cn/gtoxfmnmce.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.iojbl.cn/gtgllhgxvc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xinyue.icu/gtozhdiuii.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yangfankeji.com/gtqfvlexgb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.nanxuanxn.top/gtiynnmgag.html

[L03] 设置自定义请求头
来源：http://hz.cdnleiting.top/gtybpbrhro.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhixingplan.top/gtewbffmik.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.shanyushiyangtech.top/gtmheklmed.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.redwolf501.top/gtwkmzdszv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gogol.net.cn/gtxewiatsa.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.shzxlz.cn/gtrtbornkx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.gogol.net.cn/gtyvrcnsxx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yongpay.top/gtewtblbxi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.dianchejie.cn/gtxuamflvc.html

[L04] 设置超时
来源：http://hz.yuanzhike.top/gtzedkybcy.html

Py:   requests.get(url, timeout=5)
来源：http://hz.fengsongda.top/gtsbcmdndr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.hfpthk.cn/gtqvqfcxvm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.fengsongda.top/gttarxhsnn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nwbrower.top/gtwecuizmz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ehwqpu.com/gtuivvineq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hywenlv.cn/gtdmojovgk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.wangshuangyany.cn/gtflpctvsn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hongshengwenyu.top/gtfgdpgeaf.html

[L05] 上传文件（multipart）
来源：http://hz.316326.xyz/gtymdskfjo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.chenlongwang.top/gthohlhzbf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jiagoushi.top/gtrpeqdbpt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yj202588.top/gtqrhundiu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.sysykeji.top/gtocfqjxqs.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hongshengwenyu.top/gtjxlhybzy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.9152youxi.cn/gtqmouwgkb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yuanzhike.top/gtccyhuncp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yuanzhike.top/gtnclxolbt.html

[L06] 解析响应为 JSON
来源：http://hz.hammf.cn/gtdasjyhvp.html

Py:   resp.json()
来源：http://hz.zhongyouzk.top/gtlljlzorj.html

PHP:  json_decode($body, true);
来源：http://hz.zhengqikj.top/gtdrklzuwc.html

JS:   await resp.json()
来源：http://hz.jyoumei.cn/gtpetsrgek.html

TS:   await resp.json()
来源：http://hz.zhijiandao.cn/gtmnevbktt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yonumen.top/gtrtnwjauj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.gotoacloud.top/gtrfvepzqt.html

Ruby: JSON.parse(resp.body)
来源：http://hz.shangyingyoupin.top/gtgiwxxcft.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.c1oappe.top/gtwstjihzu.html

[L07] 处理 HTTP 状态码
来源：http://hz.ywan-chungtsiang.top/gtvvywmemw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.chenjidiqi.icu/gtydzxxwgh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.sxryk.cn/gtfygaoocy.html

JS:   resp.ok;  resp.status
来源：http://hz.yuanzhike.top/gtenbzhuqn.html

TS:   resp.ok;  resp.status
来源：http://hz.hammf.cn/gtkjitrorw.html

Java: resp.statusCode()
来源：http://hz.pycfn.com/gtzofoxswj.html

Go:   resp.StatusCode
来源：http://hz.cucudq.cn/gtcximfjea.html

Ruby: resp.code.to_i
来源：http://hz.shanyushiyangtech.top/gtgyyvasth.html

C#:   (int)resp.StatusCode
来源：http://hz.dianchejie.cn/gttnywbyhg.html

[L08] 并发请求多个地址
来源：http://hz.snrcjt.cn/gthpjwamiv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.52xcode.cn/gtabxobrzg.html

PHP:  curl_multi_init() 系列
来源：http://hz.daxiang520.top/gtqewacrvo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yuanzhike.top/gtppejvoba.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinqigfzy.top/gtwpsylgyw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.dianchejie.cn/gtyfhwlzqm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.feifeiyinyue.top/gtqirhadco.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhijiandao.cn/gtmwzmmeet.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.aizwys.cn/gtgnskkcwq.html

================================================================================
来源：http://hz.sufxvd.cn/gtiabrljlx.html

M. 命令行 / 进程 / 环境
来源：http://hz.yanxiufei.cn/gtmfwmupnh.html

================================================================================
来源：http://hz.ehwqpu.com/gtqtuxhjvt.html

[M01] 读取命令行参数
来源：http://hz.zhengqikj.top/gtrdluivnu.html

Py:   sys.argv[1:]
来源：http://hz.aibaodan.cn/gtdvohpqdg.html

PHP:  $argv;  $argc;
来源：http://hz.daria6918.cn/gtfonzmtwd.html

JS:   process.argv.slice(2)
来源：http://hz.ivvv.top/gtavmponmj.html

TS:   process.argv.slice(2)
来源：http://hz.tanke756.top/gtcjgsaldh.html

Java: args 数组（main 方法参数）
来源：http://hz.xylfe.cn/gtsvzcmdsd.html

Go:   os.Args[1:]
来源：http://hz.nanxuanxn.top/gtigcdlhhp.html

Ruby: ARGV
来源：http://hz.tanke756.top/gtlayedujt.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhengqikj.top/gtnxinhiah.html

[M02] 读取环境变量
来源：http://hz.shangyingyoupin.top/gtkeropuur.html

Py:   os.environ.get("HOME")
来源：http://hz.cdnleiting.top/gtzioacfcc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jqgufenzy.top/gttbsjgcff.html

JS:   process.env.HOME
来源：http://hz.jqgfzy.top/gtonpabqpp.html

TS:   process.env.HOME
来源：http://hz.gotoacloud.top/gtwixatpgx.html

Java: System.getenv("HOME")
来源：http://hz.yongpay.top/gtavmqgtgp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.fzhhl.top/gtqdfmtwsl.html

Ruby: ENV["HOME"]
来源：http://hz.sxryk.cn/gtuuluqjos.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.quarkkingdee.top/gtoceqkfek.html

[M03] 执行外部命令
来源：http://hz.havefunace.top/gtxiwtqzlw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yuxming.cn/gtkdkhyrjn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.aibaodan.cn/gtnwtckbbh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xuetiantiany.cn/gtaayzmukg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.feifeiyinyue.top/gtmjcvlyhu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.bjfxy.top/gthuqnmzrl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jinyuanbaomall.cn/gtmjfxgmik.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.daxiang520.top/gtvbcpueqw.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yuanzhike.top/gtvtpiqnqu.html

[M04] 获取当前工作目录
来源：http://hz.sysykeji.top/gtcrdxgapm.html

Py:   os.getcwd()
来源：http://hz.zhongyouzk.top/gtehyeyryo.html

PHP:  getcwd();
来源：http://hz.redwolf501.top/gtuzrnexod.html

JS:   process.cwd()
来源：http://hz.dashuyun.cn/gthddauepb.html

TS:   process.cwd()
来源：http://hz.cashguo.top/gtudusgqff.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhijiandao.cn/gtrobndvdg.html

Go:   os.Getwd()
来源：http://hz.chenlongwang.top/gtdxbgjeuk.html

Ruby: Dir.pwd
来源：http://hz.snrcjt.cn/gtvddrwbwm.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.nanxinkj.top/gtifemasii.html

[M05] 设置退出码
来源：http://hz.yongpay.top/gtzgwktizl.html

Py:   sys.exit(1)
来源：http://hz.snrcjt.cn/gtpxjsqbvg.html

PHP:  exit(1);
来源：http://hz.dashuyun.cn/gtiyhmheuk.html

JS:   process.exit(1)
来源：http://hz.shanyushiyangtech.top/gtknwqipir.html

TS:   process.exit(1)
来源：http://hz.yueranfly.top/gtbhnhmaah.html

Java: System.exit(1)
来源：http://hz.gotoacloud.top/gtwhcmcpqi.html

Go:   os.Exit(1)
来源：http://hz.tanke756.top/gtnyjitggs.html

Ruby: exit 1
来源：http://hz.hysaishi.cn/gtmqcsgjmo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.xinyue.icu/gtfghicbsz.html

[M06] 向标准错误输出
来源：http://hz.jinqigufen.top/gtilfbjaba.html

Py:   print("err", file=sys.stderr)
来源：http://hz.daxiang520.top/gtcvxejios.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jlsjyb.cn/gtuyicdwro.html

JS:   console.error("err")
来源：http://hz.ydzc1.top/gtgjeaoksq.html

TS:   console.error("err")
来源：http://hz.xinyue.icu/gtuenjogea.html

Java: System.err.println("err")
来源：http://hz.ivvv.top/gtaaaeombe.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zdqjudy.top/gtnnkedbmh.html

Ruby: warn "err"
来源：http://hz.tanke756.top/gtbvoslfhc.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jlsjyb.cn/gtdpnllxzf.html

[M07] 判断是否为主入口
来源：http://hz.yj20258888.top/gtlabeqyas.html

Py:   if __name__ == "__main__":
来源：http://hz.jinyuanbaomall.cn/gtrszgwhhn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ydjk.org.cn/gtzscrznko.html

JS:   require.main === module
来源：http://hz.dashuyun.cn/gtjoecvvej.html

TS:   require.main === module
来源：http://hz.aibaodan.cn/gtanptsqac.html

Java: public static void main(String[] args)
来源：http://hz.zycfv.cn/gtzuwjbmqf.html

Go:   func main()
来源：http://hz.xingfuxueyuan.xyz/gtgyhjjter.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.xinyue.icu/gtdrvtjsfi.html

C#:   static void Main(string[] args)
来源：http://hz.yj20258888.top/gthtisupgj.html

[M08] 获取系统与运行时信息
来源：http://hz.nwbrower.top/gtakdcarwa.html

Py:   platform.system();  platform.python_version()
来源：http://hz.mhx1999.top/gtuxappabb.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.birdmap.top/gtejsscmzv.html

JS:   process.platform;  process.version
来源：http://hz.shuidangran.top/gtldlpujqt.html

TS:   process.platform;  process.version
来源：http://hz.ydjk.org.cn/gtwnjzgwmy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.wangshuangyany.cn/gtpevnycqw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.birdmap.top/gtqpmanors.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ivvv.top/gtzavjzoyj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.tanke756.top/gtnaxdbtaq.html

================================================================================
来源：http://hz.yangfankeji.com/gtwkvclnkf.html

N. 数据结构与算法
来源：http://hz.snrcjt.cn/gtjjbrklcq.html

================================================================================
来源：http://hz.fzhhl.top/gtogtlykwc.html

[N01] 二分查找（有序数组）
来源：http://hz.yonumen.top/gtflbjcjre.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yj20258.top/gtpybpiwge.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.gaohongyu789.top/gtpifvkhfl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.fengsongda.top/gtcwznmocp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shuidangran.top/gtlznobeui.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.shangyingyoupin.top/gtepannytp.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.316326.xyz/gttsaipeih.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yuanzhike.top/gtmraiajiw.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xuanzx.com/gthehcoxtr.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yj20258888.top/gthskjqqhg.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gzhubu.top/gtwzwawzyz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.dashuyun.cn/gtflykavsv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jiagoushi.top/gtuitjnxui.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhijiandao.cn/gtpnyepfvq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.sysykeji.top/gtppflnnti.html

Go:   slices.Sort(arr)
来源：http://hz.andypj.xyz/gtdzwucaun.html

Ruby: arr.sort
来源：http://hz.mhx1999.top/gtgekaglkh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ybcxt.top/gtjdswcnyt.html

[N03] 快速排序（分治示例）
来源：http://hz.316326.xyz/gtuizjyizr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.fzhhl.top/gtythbdatz.html

PHP:  // 递归实现，或用 usort
来源：http://hz.sysykeji.top/gtwwfhpdcn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jiagoushi.top/gttmsstjee.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.pengpengdd.cyou/gtmyqlogas.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.52xcode.cn/gtupyfmgae.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.cdnleiting.top/gtkwjunuta.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yj20258.top/gtugbmsald.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.dashuyun.cn/gtugjptief.html

[N04] 斐波那契数列
来源：http://hz.nanxinkj.top/gtlzhlgtgl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yueranfly.top/gtitkqiwjw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.iojbl.cn/gtvfbxnyom.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jlsjyb.cn/gtglktwsqd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shanyushiyangkeji.top/gtzbziblef.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.c1oappe.top/gtrlnhnjly.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.mhx1999.top/gtohbpskze.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yj20258.top/gtljnzwzvl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.meibo888.top/gtslnxhfqw.html

[N05] 最大公约数
来源：http://hz.wangshuangyany.cn/gtuumcgnpb.html

Py:   math.gcd(a, b)
来源：http://hz.cdnleiting.top/gtxeznintp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hywenlv.cn/gttvbaxenz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.pengpengdd.cyou/gtkifxviri.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.aibaodan.cn/gtqsserkns.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jinqigfzy.top/gtmltsrvkb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.ydjk.org.cn/gtfihkwbay.html

Ruby: a.gcd(b)
来源：http://hz.pengpengdd.cyou/gttllopmga.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.smart0.xyz/gttvmbvktu.html

[N06] 判断回文字符串
来源：http://hz.gogol.net.cn/gthlewdcrl.html

Py:   s == s[::-1]
来源：http://hz.cheryme.top/gtuoxivckl.html

PHP:  $s === strrev($s);
来源：http://hz.fzhhl.top/gtcolmrxds.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yj20258888.top/gtnjxmmvoe.html

TS:   s === [...s].reverse().join("")
来源：http://hz.tanke756.top/gtjcswhvfp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.sweek.top/gtzezobfcy.html

Go:   // 双指针从两端比较
来源：http://hz.fengsongda.top/gtzftxpnra.html

Ruby: s == s.reverse
来源：http://hz.zhongyouzk.top/gtwbhuwovi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hammf.cn/gtbrkaqsuc.html

[N07] 两数之和（返回下标）
来源：http://hz.tian-w.cn/gtpdtyndzt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhaomingkeji.xyz/gtjapldiji.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.shanyushiyangkeji.top/gtqkuvraxg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.wangdashe.top/gticdqpmqm.html

TS:   // 手写 Map<string, number>
来源：http://hz.andypj.xyz/gtsdizxzvn.html

Java: // 手写 HashMap
来源：http://hz.zhongyouzk.top/gtwtpwbcle.html

Go:   // 手写 map[int]int
来源：http://hz.zycfv.cn/gtwhcwwyvd.html

Ruby: // 手写 Hash
来源：http://hz.yj20258888.top/gtoukjxqbb.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zhixingplan.top/gtyhytdihc.html

[N08] 生成全排列
来源：http://hz.svipenyu.cn/gtzjheflts.html

Py:   itertools.permutations(arr)
来源：http://hz.hfpthk.cn/gtkbmliydb.html

PHP:  // 手写递归交换
来源：http://hz.shzxlz.cn/gthibopxmt.html

JS:   // 手写回溯递归
来源：http://hz.xylfe.cn/gtaiienjab.html

TS:   // 手写回溯递归
来源：http://hz.zhixingplan.top/gtrzgcxjyh.html

Java: // 手写回溯递归
来源：http://hz.hfpthk.cn/gtsjwbjdrt.html

Go:   // 手写回溯递归
来源：http://hz.haohaochexian.top/gtlvoabnpz.html

Ruby: arr.permutation.to_a
来源：http://hz.jinghuilouyu.cn/gtnzltehgq.html

C#:   // 手写回溯递归
来源：http://hz.sxryk.cn/gteaettzre.html

[N09] 栈与队列
来源：http://hz.yonumen.top/gtsjvcrxxm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.xylfe.cn/gtcdkvbibp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.smart0.xyz/gtwaouodoa.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.guannengcc.top/gtbifytrzu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhijiandao.cn/gtkivvmadi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ybcxt.top/gtdabpbwxm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ydjk.org.cn/gtpzurhqkv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.cdnleiting.top/gtgeanztzo.html


<!-- 参考信息 -->