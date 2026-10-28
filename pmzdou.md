代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jinyuanbaomall.cn/gtzjwektwo.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ydjk.org.cn/gtrfpknkdk.html

JS:   JSON.stringify(obj)
来源：http://hz.zhiwuduotai.top/gtvfimimcp.html

TS:   JSON.stringify(obj)
来源：http://hz.bjfxy.top/gtnrhesfyu.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.fzhhl.top/gtdmhhszhu.html

Go:   json.Marshal(obj)
来源：http://hz.wangshuangyany.cn/gtvulclghj.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.316326.xyz/gteqfzemuo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hnxiangtu.top/gtogsbwqcn.html

[K02] JSON 字符串转对象
来源：http://hz.quarkkingdee.top/gtfwquftnk.html

Py:   json.loads(s)
来源：http://hz.chenzaomai.com/gtqvixffwx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.smart0.xyz/gtfbunbefv.html

JS:   JSON.parse(s)
来源：http://hz.sxryk.cn/gtasbhczgm.html

TS:   JSON.parse(s)
来源：http://hz.meibo888.top/gtwuqsxkxd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.cqqwz.cn/gtkbdpprxv.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.aibaodan.cn/gtjikycgsa.html

Ruby: JSON.parse(s)
来源：http://hz.fengsongda.top/gtsttkiwki.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.shanyushiyangkeji.top/gtyqvalaxu.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.nanxinkj.top/gtjygdxpfw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hfpthk.cn/gtbzbwzhcp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.chenjidiqi.icu/gtifnmnnim.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yvedp.cn/gtujzepprm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.sufxvd.cn/gthivcmlxu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.bjfxy.top/gtaadqysmu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.c1oappe.top/gtqczqczob.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ybcxt.top/gtmfndxzda.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hfpthk.cn/gthcdlaeox.html

[K04] 读取 JSON 文件
来源：http://hz.jlsjyb.cn/gtoayknqda.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.sufxvd.cn/gtpnysnvtc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ywan-chungtsiang.top/gtnrsafmna.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinqigufen.top/gtlagnxhro.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.pengpengdd.cyou/gtnugpdskr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hammf.cn/gtnyuckcay.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.shuidangran.top/gtzvkfxznc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.nanxinkj.top/gthnnpuwnf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ywan-chungtsiang.top/gtgguthkns.html

[K05] 深拷贝对象
来源：http://hz.shangyingyoupin.top/gtbszdpcfq.html

Py:   copy.deepcopy(obj)
来源：http://hz.xylfe.cn/gtgojzrsey.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhiwuduotai.top/gtewkiaowd.html

JS:   structuredClone(obj)
来源：http://hz.jlsjyb.cn/gtpgntjarn.html

TS:   structuredClone(obj)
来源：http://hz.aizwys.cn/gtmdzhgbzs.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.cashguo.top/gtylqtalgh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.vqdsnc.cn/gtqujmnvyn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.cashguo.top/gtbdocbiob.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.chenlongwang.top/gtnngcedkd.html

[K06] 解析 URL 查询串
来源：http://hz.quarkkingdee.top/gtejjluono.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jlsjyb.cn/gtxlrikecy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yonumen.top/gtowmqdxbs.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ydjk.org.cn/gtzcicewjh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj20258888.top/gtcffqhmeu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.daria6918.cn/gtbwpqebaf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.xylfe.cn/gtdjnuyxma.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jianghu66.top/gtfsdwbysz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yj202588.top/gtnifdesrn.html

[K07] 进制转换
来源：http://hz.kuanghao11.cn/gtiawetjvu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.nanxuanxn.top/gtuygujiql.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.mhx1999.top/gtvswlhnjv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.nanxuanxn.top/gtrhmiaxxw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.guowangkeji.top/gtydivafvr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhijiandao.cn/gtyaomlpwq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.ybcxt.top/gtsdykwgtz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zhaomingkeji.xyz/gtfrcpghjb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.daxiang520.top/gtxcdgsabj.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.52xcode.cn/gtpcoxumwr.html

Py:   pickle.dumps(obj)
来源：http://hz.guowangkeji.top/gtkrzaliwn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.fzhhl.top/gtoyzncgaa.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.tanke756.top/gtlqipazhv.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xylfe.cn/gtcyxzcdvb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yj202588.top/gthwawyoxv.html

Go:   encoding/gob
来源：http://hz.gogol.net.cn/gtzkbwkime.html

Ruby: Marshal.dump(obj)
来源：http://hz.gogol.net.cn/gtkwtrhfjc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.daxiang520.top/gtdfbkkqvb.html

================================================================================
来源：http://hz.nanxinkj.top/gthozrikld.html

L. 网络请求
来源：http://hz.ydzc1.top/gtgvxmidke.html

================================================================================
来源：http://hz.yonumen.top/gtqxkzxtdr.html

[L01] 发送 GET 请求
来源：http://hz.cheryme.top/gtstnpvvsc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yanxiufei.cn/gtfrfdgdno.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.chenzaomai.com/gtxdbntwdy.html

JS:   await fetch(url)
来源：http://hz.wangshuangyany.cn/gtlztlwiip.html

TS:   await fetch(url)
来源：http://hz.daxiang520.top/gtsdibhgcr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.pycfn.com/gtxguezoyw.html

Go:   resp, err := http.Get(url)
来源：http://hz.kuanghao11.cn/gtdxogjyzj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zycfv.cn/gtzxeavjkv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.xinyue.icu/gtulsmbsqn.html

[L02] 发送 POST JSON
来源：http://hz.jinqigufen.top/gtooqceasr.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ybcxt.top/gtkaljtdux.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.smart0.xyz/gtprhevirb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ppjwa.cn/gtitsosmqn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.wangshuangyany.cn/gtotgngoqu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.gotoacloud.top/gtobofvrsg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ehwqpu.com/gtiuxrxbkh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.fengsongda.top/gtrvgchxns.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yj202588.top/gtuanjitkn.html

[L03] 设置自定义请求头
来源：http://hz.xylfe.cn/gtoumhzbxn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.wangdashe.top/gtwmmcdzmj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.fzhhl.top/gtdgslqlwr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.daria6918.cn/gtrnngvmiu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj20258888.top/gtswxquzyg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jyoumei.cn/gtlzymqjld.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.gzhubu.top/gthwobsgsu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zycfv.cn/gtzncycbom.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.havefunace.top/gtbdyjpjvg.html

[L04] 设置超时
来源：http://hz.chenzaomai.com/gtbzddqqyq.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ywan-chungtsiang.top/gtdppkpyrc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yj20258888.top/gtoulaxifq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.svipenyu.cn/gtsdbruraa.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinyuanbaomall.cn/gtgxcssvlb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jinqigufen.top/gtlqeqrrnb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yj20258888.top/gthcpkfttt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.cashguo.top/gtgzejqatw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.cheryme.top/gttwsplylj.html

[L05] 上传文件（multipart）
来源：http://hz.xziqi.cn/gteoudgcvf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hnqzz.top/gtpoaydcfz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhaomingkeji.xyz/gtrwyejjnn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.sxryk.cn/gtjgdtzenf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.9152youxi.cn/gtnefbghdj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhiwuduotai.top/gtjaarqfyt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ydzc1.top/gtlayuaghh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ivvv.top/gtzwzjeeoy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.cdnleiting.top/gtjikcgalr.html

[L06] 解析响应为 JSON
来源：http://hz.gaohongyu789.top/gteqqjrtfu.html

Py:   resp.json()
来源：http://hz.xinyue.icu/gtljlbsqze.html

PHP:  json_decode($body, true);
来源：http://hz.hnxiangtu.top/gtjeibhbnh.html

JS:   await resp.json()
来源：http://hz.hfpthk.cn/gtmjpcevna.html

TS:   await resp.json()
来源：http://hz.xingfuxueyuan.xyz/gtskyuiyel.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yj202588.top/gtgykmuthu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.shzxlz.cn/gtejzggvzm.html

Ruby: JSON.parse(resp.body)
来源：http://hz.316326.xyz/gtndizqjvv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.cqqwz.cn/gtrbxvdgdv.html

[L07] 处理 HTTP 状态码
来源：http://hz.jinyuanbaomall.cn/gtqiwnxbsy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.havefunace.top/gthfkdhklz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yj20258888.top/gtwajcqxza.html

JS:   resp.ok;  resp.status
来源：http://hz.hysaishi.cn/gtdjudguwe.html

TS:   resp.ok;  resp.status
来源：http://hz.ywan-chungtsiang.top/gtsvmsvvbe.html

Java: resp.statusCode()
来源：http://hz.haohaochexian.top/gtvkkivrcd.html

Go:   resp.StatusCode
来源：http://hz.wangshuangyany.cn/gtombgmddn.html

Ruby: resp.code.to_i
来源：http://hz.yj20258888.top/gtapilpzqg.html

C#:   (int)resp.StatusCode
来源：http://hz.vqdsnc.cn/gtacogmefe.html

[L08] 并发请求多个地址
来源：http://hz.zdqjudy.top/gticwtinjz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.mhx1999.top/gtsutolhvy.html

PHP:  curl_multi_init() 系列
来源：http://hz.jiagoushi.top/gtxyqsczsn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yj20258888.top/gtmrisibjh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.haohaochexian.top/gtieorsdue.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yongpay.top/gttnpfadpe.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.dianchejie.cn/gtdzujshvn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jinqigfzy.top/gtvpgtdkdp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.kuanghao11.cn/gtnclhvjxn.html

================================================================================
来源：http://hz.fzhhl.top/gtswvdnpug.html

M. 命令行 / 进程 / 环境
来源：http://hz.guannengcc.top/gtbyezevtz.html

================================================================================
来源：http://hz.cdnleiting.top/gtwzyhyjgj.html

[M01] 读取命令行参数
来源：http://hz.cashguo.top/gtripgkqpo.html

Py:   sys.argv[1:]
来源：http://hz.kuanghao11.cn/gtemdyjwix.html

PHP:  $argv;  $argc;
来源：http://hz.zhijiandao.cn/gtykrzlcuj.html

JS:   process.argv.slice(2)
来源：http://hz.wangdashe.top/gtvkmbdvfq.html

TS:   process.argv.slice(2)
来源：http://hz.daxiang520.top/gtjpmjpluh.html

Java: args 数组（main 方法参数）
来源：http://hz.gotoacloud.top/gtaitqggdm.html

Go:   os.Args[1:]
来源：http://hz.shanyushiyangtech.top/gtqxgfltvm.html

Ruby: ARGV
来源：http://hz.chenjidiqi.icu/gtsyflnupq.html

C#:   args 数组（Main 方法参数）
来源：http://hz.nwbrower.top/gtaawzrpmt.html

[M02] 读取环境变量
来源：http://hz.shanyushiyangkeji.top/gtqnisyicb.html

Py:   os.environ.get("HOME")
来源：http://hz.yuanzhike.top/gtsyyxxnqf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hnxiangtu.top/gtogwqpfzv.html

JS:   process.env.HOME
来源：http://hz.zhiwuduotai.top/gttoxvuqek.html

TS:   process.env.HOME
来源：http://hz.yj20258888.top/gteojuqful.html

Java: System.getenv("HOME")
来源：http://hz.hammf.cn/gtocdsbcel.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yvedp.cn/gtqiytinbr.html

Ruby: ENV["HOME"]
来源：http://hz.ehwqpu.com/gtclxkrgoh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.vqdsnc.cn/gtxzriagng.html

[M03] 执行外部命令
来源：http://hz.hammf.cn/gthwgewkzz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yj20258888.top/gtwfopjwad.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.cdnleiting.top/gtdclrlxsg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ivvv.top/gtzugfhjfw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ydzc1.top/gthyfqviab.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.wangshuangyany.cn/gtutromunh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.nwbrower.top/gtidmsooih.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.0kj1m.cn/gtzmsbufse.html

C#:   Process.Start("ls", "-l");
来源：http://hz.fengsongda.top/gtvatkprxn.html

[M04] 获取当前工作目录
来源：http://hz.zhongyouzk.top/gtbgpsblpv.html

Py:   os.getcwd()
来源：http://hz.cucudq.cn/gtnqxemkbx.html

PHP:  getcwd();
来源：http://hz.ivvv.top/gtluojlviy.html

JS:   process.cwd()
来源：http://hz.jqgufenzy.top/gtdwjrmtvm.html

TS:   process.cwd()
来源：http://hz.vqdsnc.cn/gtzxlpgloa.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.sufxvd.cn/gtrgrwqxhz.html

Go:   os.Getwd()
来源：http://hz.hongshengwenyu.top/gtpwqsivqh.html

Ruby: Dir.pwd
来源：http://hz.gzhubu.top/gtfrrqehwa.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.havefunace.top/gtjzxdiedd.html

[M05] 设置退出码
来源：http://hz.chenjidiqi.icu/gtmkyannxo.html

Py:   sys.exit(1)
来源：http://hz.jqgufenzy.top/gtbqivvpoy.html

PHP:  exit(1);
来源：http://hz.ywan-chungtsiang.top/gtapwfpnkl.html

JS:   process.exit(1)
来源：http://hz.yanxiufei.cn/gtttyflpul.html

TS:   process.exit(1)
来源：http://hz.chenzaomai.com/gtkpceilur.html

Java: System.exit(1)
来源：http://hz.guowangkeji.top/gtfywnfnos.html

Go:   os.Exit(1)
来源：http://hz.cqqwz.cn/gttblirozp.html

Ruby: exit 1
来源：http://hz.shanyushiyangkeji.top/gtfoynrcge.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.hywenlv.cn/gtpdhuhcjo.html

[M06] 向标准错误输出
来源：http://hz.yanxiufei.cn/gtzdylbbxg.html

Py:   print("err", file=sys.stderr)
来源：http://hz.shanyushiyangkeji.top/gtipfstjjx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hfpthk.cn/gtuziujanf.html

JS:   console.error("err")
来源：http://hz.andypj.xyz/gthrlevrnw.html

TS:   console.error("err")
来源：http://hz.cdnleiting.top/gtfiejtynj.html

Java: System.err.println("err")
来源：http://hz.xuanzx.com/gtpwmteajt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xuetiantiany.cn/gtwgadwpoz.html

Ruby: warn "err"
来源：http://hz.xuetiantiany.cn/gtphozpbga.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.xingfuxueyuan.xyz/gtbonhsklx.html

[M07] 判断是否为主入口
来源：http://hz.yanxiufei.cn/gtasacribq.html

Py:   if __name__ == "__main__":
来源：http://hz.mhx1999.top/gtygphwyli.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ydzc1.top/gturbyopcr.html

JS:   require.main === module
来源：http://hz.guowangkeji.top/gtycorquwc.html

TS:   require.main === module
来源：http://hz.hnqzz.top/gtyfijmram.html

Java: public static void main(String[] args)
来源：http://hz.ehwqpu.com/gtpsucuweq.html

Go:   func main()
来源：http://hz.jqgfzy.top/gtlphojylw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cashguo.top/gtirflsfre.html

C#:   static void Main(string[] args)
来源：http://hz.aizwys.cn/gtmbzdeaim.html

[M08] 获取系统与运行时信息
来源：http://hz.yangfankeji.com/gtssazqrvs.html

Py:   platform.system();  platform.python_version()
来源：http://hz.xingfuxueyuan.xyz/gtxpdafvva.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jinqigfzy.top/gtkcplgcan.html

JS:   process.platform;  process.version
来源：http://hz.tanke756.top/gtotgxhmry.html

TS:   process.platform;  process.version
来源：http://hz.mhx1999.top/gtqukyyyts.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.gogol.net.cn/gtnrjcnvkb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yonumen.top/gtzzcveiqu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.xuetiantiany.cn/gttcweumze.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jinghuilouyu.cn/gttvrmuvnn.html

================================================================================
来源：http://hz.ybcxt.top/gtmtkamwyb.html

N. 数据结构与算法
来源：http://hz.dashuyun.cn/gtgcculpjw.html

================================================================================
来源：http://hz.zycfv.cn/gtemkneoib.html

[N01] 二分查找（有序数组）
来源：http://hz.nanxuanxn.top/gthsebddzh.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ydzc1.top/gteckoadnn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jiagoushi.top/gtqzzggavv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zycfv.cn/gtwhicolqq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sysykeji.top/gtfbamoldm.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jinqigfzy.top/gtrwouktwm.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.dianchejie.cn/gtnkfnfolx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.shuidangran.top/gtmxuiynnt.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zhoulong.xyz/gtsaejbeux.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.cheryme.top/gteaykrurb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ehwqpu.com/gtqpkhsyru.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jinghuilouyu.cn/gtqiphmlco.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shanyushiyangtech.top/gtvqifxyhi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.tanke756.top/gtuiuuyouu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.xziqi.cn/gtpgyjclpw.html

Go:   slices.Sort(arr)
来源：http://hz.yanxiufei.cn/gtumlkhodg.html

Ruby: arr.sort
来源：http://hz.aizwys.cn/gtkdjaxksg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhijiandao.cn/gtzcjdiohq.html

[N03] 快速排序（分治示例）
来源：http://hz.xziqi.cn/gtlwgujgaz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.9152youxi.cn/gtnomcszvs.html

PHP:  // 递归实现，或用 usort
来源：http://hz.feifeiyinyue.top/gtahacujyc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.havefunace.top/gtvtgpeqrx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ivvv.top/gtoxrdtvfs.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.sysykeji.top/gtqmjrrfto.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhiwuduotai.top/gtplvyovta.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ppjwa.cn/gteijcdkly.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.fzhhl.top/gtcnadkcnm.html

[N04] 斐波那契数列
来源：http://hz.tian-w.cn/gtlgzfopyd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhaomingkeji.xyz/gtbikptlai.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhoulong.xyz/gttmxvecvl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nwbrower.top/gtyxqjvpll.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jlsjyb.cn/gtxvkykspm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.sweek.top/gtzerdvmac.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jinyuanbaomall.cn/gtgumxzmpd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.shanyushiyangtech.top/gtsnoovkmt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.gogol.net.cn/gtxwznoghh.html

[N05] 最大公约数
来源：http://hz.tianlin.xyz/gtygxlanny.html

Py:   math.gcd(a, b)
来源：http://hz.hfpthk.cn/gtlxvtyffm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zdqjudy.top/gtuicenwbq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xziqi.cn/gtiuhpmkpt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.dashuyun.cn/gtevdsdyvc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.wangdashe.top/gtbeinwhpv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.guannengcc.top/gtwantscmm.html

Ruby: a.gcd(b)
来源：http://hz.gzhubu.top/gtaosgwndn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.aizwys.cn/gtlybcryoq.html

[N06] 判断回文字符串
来源：http://hz.gogol.net.cn/gtgzklyyya.html

Py:   s == s[::-1]
来源：http://hz.jinyuanbaomall.cn/gtxglwoiva.html

PHP:  $s === strrev($s);
来源：http://hz.gotoacloud.top/gtgcydizff.html

JS:   s === [...s].reverse().join("")
来源：http://hz.xziqi.cn/gtukricsvl.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hnxiangtu.top/gtfdhlprlc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.wangdashe.top/gtkmlocrmd.html

Go:   // 双指针从两端比较
来源：http://hz.feifeiyinyue.top/gtgbchhphs.html

Ruby: s == s.reverse
来源：http://hz.sysykeji.top/gttlatnycu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.redwolf501.top/gtxgwcscuh.html

[N07] 两数之和（返回下标）
来源：http://hz.havefunace.top/gtjorrcofx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.aibaodan.cn/gtjsrhqyxp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.gzhubu.top/gtyfofrwgt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xziqi.cn/gtkrafchqp.html

TS:   // 手写 Map<string, number>
来源：http://hz.0kj1m.cn/gtgfrpexjj.html

Java: // 手写 HashMap
来源：http://hz.yj20258888.top/gtrdqoachu.html

Go:   // 手写 map[int]int
来源：http://hz.birdmap.top/gturhokyky.html

Ruby: // 手写 Hash
来源：http://hz.ywan-chungtsiang.top/gthwuujnkj.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.pycfn.com/gtbnpjuajk.html

[N08] 生成全排列
来源：http://hz.ydjk.org.cn/gtrlypaqsm.html

Py:   itertools.permutations(arr)
来源：http://hz.daxiang520.top/gtesstqaqp.html

PHP:  // 手写递归交换
来源：http://hz.hongshengwenyu.top/gtincfgajm.html

JS:   // 手写回溯递归
来源：http://hz.yonumen.top/gtxyvnfjgi.html

TS:   // 手写回溯递归
来源：http://hz.shzxlz.cn/gturfsrrry.html

Java: // 手写回溯递归
来源：http://hz.meibo888.top/gtoidvmokz.html

Go:   // 手写回溯递归
来源：http://hz.nanxuanxn.top/gteqnekhlc.html

Ruby: arr.permutation.to_a
来源：http://hz.pycfn.com/gtaiuvmdry.html

C#:   // 手写回溯递归
来源：http://hz.xuanzx.com/gtlwcriqfo.html

[N09] 栈与队列
来源：http://hz.yonumen.top/gthkemmoyn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.shanyushiyangtech.top/gtgmkuhplp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.9152youxi.cn/gtrejdquha.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.snrcjt.cn/gtrmimmits.html


<!-- 参考信息 -->