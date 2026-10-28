代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhengqikj.top/gtaqwxvgvs.html

Go:   json.Marshal(obj)
来源：http://hz.jinqigufen.top/gtuclqjvcn.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.daxiang520.top/gtpwmqxfqx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.snrcjt.cn/gtvjuegpnj.html

[K02] JSON 字符串转对象
来源：http://hz.ybcxt.top/gtfciipidx.html

Py:   json.loads(s)
来源：http://hz.yvedp.cn/gtbecedojw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ydzc1.top/gtttwgswyv.html

JS:   JSON.parse(s)
来源：http://hz.feifeiyinyue.top/gtypkrqpmo.html

TS:   JSON.parse(s)
来源：http://hz.yueranfly.top/gtxrqptsna.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yj20258.top/gtoevbhsdg.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jianghu66.top/gtpvhhncri.html

Ruby: JSON.parse(s)
来源：http://hz.jinghuilouyu.cn/gthmbcfmij.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.quarkkingdee.top/gtagsvgwte.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.smart0.xyz/gtzwcntsbt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.c1oappe.top/gtculztmpm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.smart0.xyz/gtwezkhtgc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shanyushiyangtech.top/gtyldzijze.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhixingplan.top/gtsrzotxno.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.gzhubu.top/gtockwjviw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.feifeiyinyue.top/gtydbmzslo.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.wangshuangyany.cn/gtslafvyum.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hywenlv.cn/gtlrrtcgrf.html

[K04] 读取 JSON 文件
来源：http://hz.cashguo.top/gtcqzwwlwl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yuxming.cn/gttnyzephx.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.316326.xyz/gtbkhsmsss.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.aizwys.cn/gtvarnnnty.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cdnleiting.top/gtxoyuptqq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhongyouzk.top/gtevtzbaoq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhixingplan.top/gthqrqvlsr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhoulong.xyz/gtjcwoelex.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhaomingkeji.xyz/gtyufqysoi.html

[K05] 深拷贝对象
来源：http://hz.tianlin.xyz/gteuhkpisl.html

Py:   copy.deepcopy(obj)
来源：http://hz.andypj.xyz/gtqynhbomo.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hfpthk.cn/gtydalvvnw.html

JS:   structuredClone(obj)
来源：http://hz.wangshuangyany.cn/gthojsyjnx.html

TS:   structuredClone(obj)
来源：http://hz.guowangkeji.top/gtlhabuxmz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.meibo888.top/gtdilvcshs.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.iojbl.cn/gtgkvqceoc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ydjk.org.cn/gtgpxmueos.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jyoumei.cn/gtupisqciv.html

[K06] 解析 URL 查询串
来源：http://hz.ehwqpu.com/gtsdcfzbdz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.redwolf501.top/gtdciaeyul.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xylfe.cn/gtjnhgwxkh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinqigfzy.top/gtngsfxihx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xziqi.cn/gtrvjzyqza.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yj20258888.top/gtkthuldqw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yj202588.top/gtnbwdnqmg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.xziqi.cn/gthgwrnitz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.sufxvd.cn/gtiriwyfnb.html

[K07] 进制转换
来源：http://hz.tianlin.xyz/gtfydbhnes.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.sweek.top/gtfxxladqy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.nanxuanxn.top/gtcrmbzqhl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yonumen.top/gtewptsmnn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ywan-chungtsiang.top/gtapnhgayk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.chenjidiqi.icu/gtapaogpqa.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.tianlin.xyz/gtgztvmfzt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.daria6918.cn/gtpqbgffdu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jinqigfzy.top/gttmnsxgtc.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ehwqpu.com/gtycwozldr.html

Py:   pickle.dumps(obj)
来源：http://hz.andypj.xyz/gtuaashtvl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.haohaochexian.top/gtshrqxujr.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.wangshuangyany.cn/gtkedeblly.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.feifeiyinyue.top/gtuyswvswj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.guowangkeji.top/gtqokcxycd.html

Go:   encoding/gob
来源：http://hz.havefunace.top/gtxzkjbetp.html

Ruby: Marshal.dump(obj)
来源：http://hz.snrcjt.cn/gtfsobtmww.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.wangdashe.top/gtsixmwcvl.html

================================================================================
来源：http://hz.9152youxi.cn/gtwyxbnukf.html

L. 网络请求
来源：http://hz.tianlin.xyz/gtqktgwxxq.html

================================================================================
来源：http://hz.cheryme.top/gtgyisokjj.html

[L01] 发送 GET 请求
来源：http://hz.pengpengdd.cyou/gtrdrjncvi.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cucudq.cn/gtfaiivsfg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zycfv.cn/gtdpodvaxe.html

JS:   await fetch(url)
来源：http://hz.sweek.top/gtjnuwfihh.html

TS:   await fetch(url)
来源：http://hz.yj202588.top/gtufmnundr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhongyouzk.top/gtpunnxtjf.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhongyouzk.top/gtasqohexx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.shzxlz.cn/gtaxgygjbs.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.nanxuanxn.top/gtdfuwpanz.html

[L02] 发送 POST JSON
来源：http://hz.zhongyouzk.top/gtoclpvkww.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.52xcode.cn/gtntkhomqs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hammf.cn/gtmxyrcqzw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhongyouzk.top/gtnfpzixzg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xylfe.cn/gtslzmhfgp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.quarkkingdee.top/gthguxwsxv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yj20258888.top/gtsggquoiu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.tian-w.cn/gtcnacxmak.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.cucudq.cn/gtfuvjwnkw.html

[L03] 设置自定义请求头
来源：http://hz.yanxiufei.cn/gtqjkggnfp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.kuanghao11.cn/gtaejymtso.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.gogol.net.cn/gttvtmukky.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jlsjyb.cn/gtaenfrfzu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj20258888.top/gtuifeoqtt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yongpay.top/gtayhsjlgz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hfpthk.cn/gtvamatipd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.sxryk.cn/gtvnkaznmy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.pycfn.com/gtyndgqmic.html

[L04] 设置超时
来源：http://hz.wangshuangyany.cn/gtsrgvafal.html

Py:   requests.get(url, timeout=5)
来源：http://hz.tianlin.xyz/gtxgvzrcxk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.xuanzx.com/gtaszekllx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.quarkkingdee.top/gtyhxglgcu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj20258888.top/gtschctyay.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.sxryk.cn/gtrvchfxgv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yangfankeji.com/gtxafngnfp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xylfe.cn/gtonmtcciw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.iojbl.cn/gtlwxfpjqq.html

[L05] 上传文件（multipart）
来源：http://hz.gaohongyu789.top/gtchmyysrk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.fengsongda.top/gthfxopacx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.hongshengwenyu.top/gtrylfahiq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hnqzz.top/gtvqkyafea.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.vqdsnc.cn/gtcixbexxx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zycfv.cn/gtwrepnrpf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.gzhubu.top/gtdvftajrv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.daxiang520.top/gtaaeubbbe.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hywenlv.cn/gtyqmokrvq.html

[L06] 解析响应为 JSON
来源：http://hz.cqqwz.cn/gtxozqfovo.html

Py:   resp.json()
来源：http://hz.havefunace.top/gtaqfvgrta.html

PHP:  json_decode($body, true);
来源：http://hz.sweek.top/gtefdbmszw.html

JS:   await resp.json()
来源：http://hz.xziqi.cn/gtbvjlxmtj.html

TS:   await resp.json()
来源：http://hz.jyoumei.cn/gtlsyffitz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yonumen.top/gtdqolmplf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.dianchejie.cn/gtsutaeecg.html

Ruby: JSON.parse(resp.body)
来源：http://hz.gotoacloud.top/gtctyjhawf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.vqdsnc.cn/gtntpfyqyb.html

[L07] 处理 HTTP 状态码
来源：http://hz.xuanzx.com/gtuocwceyp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.haohaochexian.top/gtkjafhswg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhixingplan.top/gttuzsguds.html

JS:   resp.ok;  resp.status
来源：http://hz.yuanzhike.top/gtmcyqjgeu.html

TS:   resp.ok;  resp.status
来源：http://hz.xylfe.cn/gtgujdcqrv.html

Java: resp.statusCode()
来源：http://hz.chenlongwang.top/gtkhuyxpox.html

Go:   resp.StatusCode
来源：http://hz.chenlongwang.top/gtxkoqkwfu.html

Ruby: resp.code.to_i
来源：http://hz.pengpengdd.cyou/gtkuvfljnw.html

C#:   (int)resp.StatusCode
来源：http://hz.feifeiyinyue.top/gtwmhxdpmh.html

[L08] 并发请求多个地址
来源：http://hz.nwbrower.top/gtlksvyedf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.aibaodan.cn/gtorxghksy.html

PHP:  curl_multi_init() 系列
来源：http://hz.yonumen.top/gtdyvncfsf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cucudq.cn/gtljbrvwdt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sysykeji.top/gtuyacdqih.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.wangdashe.top/gtxbchutat.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.gotoacloud.top/gtajsoxhak.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jianghu66.top/gtsbvomduq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xuetiantiany.cn/gtoxfbbswf.html

================================================================================
来源：http://hz.0kj1m.cn/gtioczcdhs.html

M. 命令行 / 进程 / 环境
来源：http://hz.birdmap.top/gtagqtqaut.html

================================================================================
来源：http://hz.yueranfly.top/gtvrpodovx.html

[M01] 读取命令行参数
来源：http://hz.cucudq.cn/gtznmuojju.html

Py:   sys.argv[1:]
来源：http://hz.gaohongyu789.top/gtxopomdgw.html

PHP:  $argv;  $argc;
来源：http://hz.daxiang520.top/gtufnavqbj.html

JS:   process.argv.slice(2)
来源：http://hz.svipenyu.cn/gtmgqjxhzn.html

TS:   process.argv.slice(2)
来源：http://hz.xuanzx.com/gtecahcllz.html

Java: args 数组（main 方法参数）
来源：http://hz.xziqi.cn/gtfbyjqays.html

Go:   os.Args[1:]
来源：http://hz.yvedp.cn/gtobfnvjno.html

Ruby: ARGV
来源：http://hz.gaohongyu789.top/gtyzcjegbb.html

C#:   args 数组（Main 方法参数）
来源：http://hz.quarkkingdee.top/gtvjgojxxj.html

[M02] 读取环境变量
来源：http://hz.daxiang520.top/gtfmpezqyk.html

Py:   os.environ.get("HOME")
来源：http://hz.xinyue.icu/gtqkrmqqwn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.chenlongwang.top/gticobyonn.html

JS:   process.env.HOME
来源：http://hz.jinqigfzy.top/gtpsehtsqs.html

TS:   process.env.HOME
来源：http://hz.c1oappe.top/gtkqleijeo.html

Java: System.getenv("HOME")
来源：http://hz.zhengqikj.top/gtuqxrsfzn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.gzhubu.top/gtsyrfgdda.html

Ruby: ENV["HOME"]
来源：http://hz.jianghu66.top/gtdiwtrtwx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.ydjk.org.cn/gttmofiskm.html

[M03] 执行外部命令
来源：http://hz.daxiang520.top/gtsztbooqx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.dianchejie.cn/gtpzfkjgia.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.pycfn.com/gtuggxjbya.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.guowangkeji.top/gtqwthspkz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.52xcode.cn/gtzwrxcgzk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hysaishi.cn/gtzcuhctox.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jinyuanbaomall.cn/gtxacpiqhh.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jiagoushi.top/gtjxuncylq.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhaomingkeji.xyz/gtoyfpxeyv.html

[M04] 获取当前工作目录
来源：http://hz.yuanzhike.top/gtpxysiuso.html

Py:   os.getcwd()
来源：http://hz.vqdsnc.cn/gtlvnzokfu.html

PHP:  getcwd();
来源：http://hz.iojbl.cn/gturvtmsqn.html

JS:   process.cwd()
来源：http://hz.nanxuanxn.top/gtpcqajvsn.html

TS:   process.cwd()
来源：http://hz.tanke756.top/gthumfzrqw.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.tianlin.xyz/gtvcbiaats.html

Go:   os.Getwd()
来源：http://hz.aibaodan.cn/gttjdgrpmg.html

Ruby: Dir.pwd
来源：http://hz.daxiang520.top/gtzimpkgtl.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ydjk.org.cn/gtivmkuklt.html

[M05] 设置退出码
来源：http://hz.shuidangran.top/gtelwumoum.html

Py:   sys.exit(1)
来源：http://hz.jinghuilouyu.cn/gtyqkxxgwl.html

PHP:  exit(1);
来源：http://hz.yangfankeji.com/gtmnnrdcgu.html

JS:   process.exit(1)
来源：http://hz.pycfn.com/gtxubbzjfl.html

TS:   process.exit(1)
来源：http://hz.snrcjt.cn/gtkbhkefmv.html

Java: System.exit(1)
来源：http://hz.guannengcc.top/gtaghayhhf.html

Go:   os.Exit(1)
来源：http://hz.yonumen.top/gtyfghfvlr.html

Ruby: exit 1
来源：http://hz.hammf.cn/gtgwccfgnc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.0kj1m.cn/gtdpqysagi.html

[M06] 向标准错误输出
来源：http://hz.chenzaomai.com/gtjeccofxl.html

Py:   print("err", file=sys.stderr)
来源：http://hz.dashuyun.cn/gtksosuupp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.cqqwz.cn/gteqplqgiu.html

JS:   console.error("err")
来源：http://hz.guannengcc.top/gtxisnvxhb.html

TS:   console.error("err")
来源：http://hz.cucudq.cn/gtcabmkzdm.html

Java: System.err.println("err")
来源：http://hz.gaohongyu789.top/gtqavvrmkf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.meibo888.top/gtuzdemrja.html

Ruby: warn "err"
来源：http://hz.hnxiangtu.top/gtcsosbytk.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hnqzz.top/gtqucrahoq.html

[M07] 判断是否为主入口
来源：http://hz.meibo888.top/gtdkzphtkg.html

Py:   if __name__ == "__main__":
来源：http://hz.aizwys.cn/gtaotfbdgw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ybcxt.top/gtminssflh.html

JS:   require.main === module
来源：http://hz.shuidangran.top/gtulebieud.html

TS:   require.main === module
来源：http://hz.iojbl.cn/gtakpaedym.html

Java: public static void main(String[] args)
来源：http://hz.cqqwz.cn/gtamwdklzj.html

Go:   func main()
来源：http://hz.shzxlz.cn/gtclwlqjtp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.smart0.xyz/gtwntgmmtu.html

C#:   static void Main(string[] args)
来源：http://hz.sxryk.cn/gtrcngcyap.html

[M08] 获取系统与运行时信息
来源：http://hz.zhongyouzk.top/gtuualytzk.html

Py:   platform.system();  platform.python_version()
来源：http://hz.52xcode.cn/gtakzpvqam.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jyoumei.cn/gtfwqgziet.html

JS:   process.platform;  process.version
来源：http://hz.sxryk.cn/gtujmojseu.html

TS:   process.platform;  process.version
来源：http://hz.yongpay.top/gtpikiewxl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yanxiufei.cn/gtkxskhesm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.kuanghao11.cn/gtezowctta.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.bjfxy.top/gtckhuiqsu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.0kj1m.cn/gtnheptygc.html

================================================================================
来源：http://hz.ppjwa.cn/gtjatwhwna.html

N. 数据结构与算法
来源：http://hz.yanxiufei.cn/gtwqziexsj.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtdimqrsle.html

[N01] 二分查找（有序数组）
来源：http://hz.zhoulong.xyz/gtzvpfbupc.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhoulong.xyz/gtqramlfzy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.haohaochexian.top/gtlxcnhvap.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.aizwys.cn/gtfkcklcov.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sysykeji.top/gtphbefxes.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.sxryk.cn/gtxoqclarl.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jinqigufen.top/gtnbhnpszu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.meibo888.top/gtnqlqqcfw.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.sysykeji.top/gtuuleqnxh.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.c1oappe.top/gtnsrbvoqv.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinghuilouyu.cn/gtwezkgtxo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.haohaochexian.top/gthrsqfshd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cqqwz.cn/gtufwwrngt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nanxinkj.top/gtpvgmjbib.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.sysykeji.top/gthvrvwrhc.html

Go:   slices.Sort(arr)
来源：http://hz.feifeiyinyue.top/gtaemnviib.html

Ruby: arr.sort
来源：http://hz.guannengcc.top/gtszuyxtxx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.cucudq.cn/gtnnczbbbv.html

[N03] 快速排序（分治示例）
来源：http://hz.yj20258888.top/gtdbyrzzft.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.shangyingyoupin.top/gtmxpmlkxd.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jinqigfzy.top/gtipjnfmeq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gogol.net.cn/gtosuiramg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.guowangkeji.top/gtlcsapxpd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhoulong.xyz/gtqtsopocv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jinqigufen.top/gtwdtiqwpv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ybcxt.top/gtqfbpysoo.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.xuanzx.com/gtfitzjunx.html

[N04] 斐波那契数列
来源：http://hz.gogol.net.cn/gtcmpzvjrj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.chenjidiqi.icu/gtyrgakmbr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.aizwys.cn/gtujrcnsms.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.gotoacloud.top/gtgyrbpxqz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xuetiantiany.cn/gtvrpjdoyn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.gzhubu.top/gtmhfwarbt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yvedp.cn/gtolkwsxdh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.guannengcc.top/gthfmffqyh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.snrcjt.cn/gtwuifihmc.html

[N05] 最大公约数
来源：http://hz.shanyushiyangkeji.top/gtsakcgnpo.html

Py:   math.gcd(a, b)
来源：http://hz.jqgfzy.top/gtgmgqvevi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.tianlin.xyz/gtpldkjnni.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.quarkkingdee.top/gtqdcgapwv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ybcxt.top/gtxpfslckz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ppjwa.cn/gtkpufihbe.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hfpthk.cn/gtpjsvcmey.html

Ruby: a.gcd(b)
来源：http://hz.52xcode.cn/gtikfiaudt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jlsjyb.cn/gtxmsrjudd.html

[N06] 判断回文字符串
来源：http://hz.52xcode.cn/gtypremcww.html

Py:   s == s[::-1]
来源：http://hz.jinqigufen.top/gtxqumihhf.html

PHP:  $s === strrev($s);
来源：http://hz.snrcjt.cn/gtkyjsdquo.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhengqikj.top/gtdnklskpr.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yongpay.top/gthfyeyebq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.guannengcc.top/gtwqqpveip.html

Go:   // 双指针从两端比较
来源：http://hz.hfpthk.cn/gtatwarppq.html

Ruby: s == s.reverse
来源：http://hz.iojbl.cn/gtzgmtlqch.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.haohaochexian.top/gtwefnkbcb.html

[N07] 两数之和（返回下标）
来源：http://hz.yonumen.top/gtvmcqzqew.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.sxryk.cn/gtpocdbtgu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.aibaodan.cn/gtmiocybnh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.hnxiangtu.top/gttheapcve.html

TS:   // 手写 Map<string, number>
来源：http://hz.hysaishi.cn/gtguqoplwb.html

Java: // 手写 HashMap
来源：http://hz.zhoulong.xyz/gtishlcyow.html

Go:   // 手写 map[int]int
来源：http://hz.0kj1m.cn/gtkflasvqx.html

Ruby: // 手写 Hash
来源：http://hz.zhijiandao.cn/gtctntlbha.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.iojbl.cn/gtdinutzby.html

[N08] 生成全排列
来源：http://hz.snrcjt.cn/gtgfikatjm.html

Py:   itertools.permutations(arr)
来源：http://hz.bjfxy.top/gtdnlljkus.html

PHP:  // 手写递归交换
来源：http://hz.yueranfly.top/gtaqqxcyal.html

JS:   // 手写回溯递归
来源：http://hz.nwbrower.top/gtcaynfppa.html

TS:   // 手写回溯递归
来源：http://hz.mhx1999.top/gtssktgwgg.html

Java: // 手写回溯递归
来源：http://hz.tianlin.xyz/gteegmyaex.html

Go:   // 手写回溯递归
来源：http://hz.shanyushiyangkeji.top/gtonhhtbps.html

Ruby: arr.permutation.to_a
来源：http://hz.ppjwa.cn/gtxyeeagpb.html

C#:   // 手写回溯递归
来源：http://hz.ppjwa.cn/gtfljfuxxd.html

[N09] 栈与队列
来源：http://hz.nanxinkj.top/gtaaxlsprh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.meibo888.top/gtwfsnbzzw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hysaishi.cn/gtfwfjvsvr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.xingfuxueyuan.xyz/gttijbpuks.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhoulong.xyz/gtjyjfworx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.redwolf501.top/gtaczupihc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.hnxiangtu.top/gtstbnrych.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yonumen.top/gtmmdbeibw.html


<!-- 参考信息 -->