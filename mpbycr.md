代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.gotoacloud.top/gtsulgwwsc.html

Go:   json.Marshal(obj)
来源：http://hz.tianlin.xyz/gtygkqxzlx.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shuidangran.top/gtowtwlfja.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.sysykeji.top/gttchpoges.html

[K02] JSON 字符串转对象
来源：http://hz.snrcjt.cn/gtqravkmay.html

Py:   json.loads(s)
来源：http://hz.jinqigufen.top/gtuxondsnm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yj20258.top/gtxyezrcon.html

JS:   JSON.parse(s)
来源：http://hz.ywan-chungtsiang.top/gtuhlsyorb.html

TS:   JSON.parse(s)
来源：http://hz.hnqzz.top/gtekpcyiph.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.iojbl.cn/gtpwetvvfl.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ydjk.org.cn/gtmpnniwlb.html

Ruby: JSON.parse(s)
来源：http://hz.jqgufenzy.top/gtfxnmacoc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.gzhubu.top/gtaqeufhft.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jqgufenzy.top/gtrreupsaj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yvedp.cn/gtbycitomm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.mhx1999.top/gtssotubtr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.cqqwz.cn/gtmcqegehx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.quarkkingdee.top/gtwhkxebxx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jlsjyb.cn/gtshbhndua.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.tianlin.xyz/gtsaclpmuc.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.daria6918.cn/gtijvggetb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.chenjidiqi.icu/gtetkifgqo.html

[K04] 读取 JSON 文件
来源：http://hz.ehwqpu.com/gtwgwrysar.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yanxiufei.cn/gtawjcmewr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yj20258.top/gtxsoxamqs.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.guannengcc.top/gtycyhxayg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.dianchejie.cn/gtfipmedlx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.quarkkingdee.top/gtvaktkzsi.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhiwuduotai.top/gthkmqkdso.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zdqjudy.top/gtxmisfulu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hywenlv.cn/gtqlsunpbz.html

[K05] 深拷贝对象
来源：http://hz.aibaodan.cn/gtyksskgez.html

Py:   copy.deepcopy(obj)
来源：http://hz.xinyue.icu/gtcrytbvgr.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cheryme.top/gtzotdhret.html

JS:   structuredClone(obj)
来源：http://hz.ywan-chungtsiang.top/gtkolkrbis.html

TS:   structuredClone(obj)
来源：http://hz.zhongyouzk.top/gtdngmccjd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.guannengcc.top/gtpvfokmve.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.birdmap.top/gtsbeodzjo.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.guowangkeji.top/gtyyeujtnz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.316326.xyz/gtcnhcdtws.html

[K06] 解析 URL 查询串
来源：http://hz.yanxiufei.cn/gtniorgurx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.smart0.xyz/gtgpdoueei.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.gaohongyu789.top/gtedesslek.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.pengpengdd.cyou/gtwwrdvaoj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jiagoushi.top/gtoiblbbvh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.fzhhl.top/gtsdydbvkr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhengqikj.top/gtscmygnvv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hnqzz.top/gtkddtlhis.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.gzhubu.top/gtnqscwwdz.html

[K07] 进制转换
来源：http://hz.sweek.top/gtyziaxixk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.nanxinkj.top/gtbsxpsjyo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xingfuxueyuan.xyz/gtxnzdyvqd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.gogol.net.cn/gtzwjmvtgu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yuxming.cn/gtmgufzlqc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.vqdsnc.cn/gtdipyqllh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xylfe.cn/gtcymblnoo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yvedp.cn/gtmoaoezcn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yueranfly.top/gtyqfeywyc.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.pycfn.com/gtgeumwlgh.html

Py:   pickle.dumps(obj)
来源：http://hz.redwolf501.top/gtrkckyzxg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.shanyushiyangkeji.top/gtakrllmpf.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.sysykeji.top/gtscybkgsx.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.dashuyun.cn/gtigyinyqa.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.quarkkingdee.top/gtrnrldbhq.html

Go:   encoding/gob
来源：http://hz.andypj.xyz/gtempfeagp.html

Ruby: Marshal.dump(obj)
来源：http://hz.dianchejie.cn/gthhrbdhky.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yj20258.top/gtzcsnxkdu.html

================================================================================
来源：http://hz.zhoulong.xyz/gtujrchzdq.html

L. 网络请求
来源：http://hz.jiagoushi.top/gtmpkkoseq.html

================================================================================
来源：http://hz.sweek.top/gtpezoghmh.html

[L01] 发送 GET 请求
来源：http://hz.hnqzz.top/gthclesooq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.mhx1999.top/gtxvwcpsvu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yonumen.top/gtthjzjcvz.html

JS:   await fetch(url)
来源：http://hz.fengsongda.top/gtdjmkiubo.html

TS:   await fetch(url)
来源：http://hz.cashguo.top/gtzaeqlbma.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hnqzz.top/gtxffblnai.html

Go:   resp, err := http.Get(url)
来源：http://hz.jinqigufen.top/gtthdjstpa.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yongpay.top/gtfinldddl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.xziqi.cn/gtfcivqnno.html

[L02] 发送 POST JSON
来源：http://hz.wangdashe.top/gtmnigxikl.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.tanke756.top/gttqmzrdgs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yueranfly.top/gtckebzhgs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.wangshuangyany.cn/gttmfmreqw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ydjk.org.cn/gtyqzmtcpc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yanxiufei.cn/gtsdptfkou.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ivvv.top/gttqxzzwxg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.sysykeji.top/gtgreqsbzm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.feifeiyinyue.top/gtvdtrnguz.html

[L03] 设置自定义请求头
来源：http://hz.daria6918.cn/gtbffznzil.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.sxryk.cn/gtdeazabye.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jianghu66.top/gthjwrcoos.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ivvv.top/gtfpabgots.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.c1oappe.top/gtzshqurza.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ehwqpu.com/gtvoegcock.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhixingplan.top/gtfhbibeml.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.gzhubu.top/gtwwktudip.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.feifeiyinyue.top/gtferzsdio.html

[L04] 设置超时
来源：http://hz.yanxiufei.cn/gtdujsxmjk.html

Py:   requests.get(url, timeout=5)
来源：http://hz.haohaochexian.top/gtdmqqdgne.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yueranfly.top/gtsgoebvqf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shanyushiyangtech.top/gtjkwlxsac.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.svipenyu.cn/gtzcgyqczf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.cashguo.top/gtveaioomj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yueranfly.top/gtnytrwsyp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zdqjudy.top/gtolucprtl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.andypj.xyz/gtdpitzsee.html

[L05] 上传文件（multipart）
来源：http://hz.zhengqikj.top/gtknrhnkng.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.xylfe.cn/gtoxobvoaf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.nanxuanxn.top/gtuqxpdrws.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.quarkkingdee.top/gtjewqnjtq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.mhx1999.top/gtwnirqwiz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ydjk.org.cn/gtgxtfxywb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yj20258888.top/gtrponenxl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.vqdsnc.cn/gtjuywjhgn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.xylfe.cn/gtqwxzljtt.html

[L06] 解析响应为 JSON
来源：http://hz.gotoacloud.top/gtdehwsndg.html

Py:   resp.json()
来源：http://hz.snrcjt.cn/gtttyierpf.html

PHP:  json_decode($body, true);
来源：http://hz.hnqzz.top/gtregdiaem.html

JS:   await resp.json()
来源：http://hz.tian-w.cn/gtoilrmdzd.html

TS:   await resp.json()
来源：http://hz.jinqigufen.top/gtzkxmaoib.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.gotoacloud.top/gttefjkikb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.ywan-chungtsiang.top/gtgfhswoeb.html

Ruby: JSON.parse(resp.body)
来源：http://hz.svipenyu.cn/gtxwpkbrfr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.gotoacloud.top/gtcxcnqwru.html

[L07] 处理 HTTP 状态码
来源：http://hz.shangyingyoupin.top/gtmfgigmcm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hfpthk.cn/gtnfatenrf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.gzhubu.top/gtwxjytqxq.html

JS:   resp.ok;  resp.status
来源：http://hz.tanke756.top/gthtfmwqal.html

TS:   resp.ok;  resp.status
来源：http://hz.xinyue.icu/gtzlsmeddg.html

Java: resp.statusCode()
来源：http://hz.snrcjt.cn/gtxafcfwvn.html

Go:   resp.StatusCode
来源：http://hz.tianlin.xyz/gtusszhrwr.html

Ruby: resp.code.to_i
来源：http://hz.yvedp.cn/gtrvnoopsh.html

C#:   (int)resp.StatusCode
来源：http://hz.jinghuilouyu.cn/gtwpydtdbf.html

[L08] 并发请求多个地址
来源：http://hz.sysykeji.top/gtrechjyla.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yvedp.cn/gtwuppuljh.html

PHP:  curl_multi_init() 系列
来源：http://hz.jinqigfzy.top/gtxrheelmc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hywenlv.cn/gtclsfchri.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ppjwa.cn/gtmukxlzjl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.cdnleiting.top/gtqswejykl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.fengsongda.top/gtcvpmhgpv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jqgfzy.top/gtwluowvbg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.9152youxi.cn/gtpypnltzb.html

================================================================================
来源：http://hz.birdmap.top/gtyehqddxw.html

M. 命令行 / 进程 / 环境
来源：http://hz.316326.xyz/gtpvenctsf.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtatwdkdpz.html

[M01] 读取命令行参数
来源：http://hz.cashguo.top/gtbetsqeni.html

Py:   sys.argv[1:]
来源：http://hz.sweek.top/gtofgcmjpj.html

PHP:  $argv;  $argc;
来源：http://hz.hywenlv.cn/gtflepljvm.html

JS:   process.argv.slice(2)
来源：http://hz.pengpengdd.cyou/gtztqgmrfl.html

TS:   process.argv.slice(2)
来源：http://hz.shzxlz.cn/gtladopcga.html

Java: args 数组（main 方法参数）
来源：http://hz.cdnleiting.top/gtxdsuqspe.html

Go:   os.Args[1:]
来源：http://hz.tian-w.cn/gtuwuuhzyt.html

Ruby: ARGV
来源：http://hz.xinyue.icu/gtrmhajcwu.html

C#:   args 数组（Main 方法参数）
来源：http://hz.pycfn.com/gtlhoofmuh.html

[M02] 读取环境变量
来源：http://hz.nwbrower.top/gtnszqitzx.html

Py:   os.environ.get("HOME")
来源：http://hz.9152youxi.cn/gtbsifdazc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.nanxuanxn.top/gthfkghbcj.html

JS:   process.env.HOME
来源：http://hz.fengsongda.top/gtndgljbyr.html

TS:   process.env.HOME
来源：http://hz.zdqjudy.top/gtntuxqgms.html

Java: System.getenv("HOME")
来源：http://hz.jinghuilouyu.cn/gtxgvzkzon.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.sweek.top/gtnnrfnqkq.html

Ruby: ENV["HOME"]
来源：http://hz.kuanghao11.cn/gtxqslqdwm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.0kj1m.cn/gtdivcnodz.html

[M03] 执行外部命令
来源：http://hz.zhongyouzk.top/gtzpnnzlei.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.aibaodan.cn/gtrlosshrz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hnxiangtu.top/gtyuohatsk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ehwqpu.com/gtbdzxpwpc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ydzc1.top/gtfanprrch.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.bjfxy.top/gthbkelflp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.xuetiantiany.cn/gtlafzkrfy.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.pycfn.com/gtlvjthuga.html

C#:   Process.Start("ls", "-l");
来源：http://hz.cucudq.cn/gtyzgpumpy.html

[M04] 获取当前工作目录
来源：http://hz.havefunace.top/gtylgvzxob.html

Py:   os.getcwd()
来源：http://hz.havefunace.top/gtsbjgkyxr.html

PHP:  getcwd();
来源：http://hz.chenlongwang.top/gtnexstonm.html

JS:   process.cwd()
来源：http://hz.cheryme.top/gtyyaefbdm.html

TS:   process.cwd()
来源：http://hz.iojbl.cn/gtcqcaufvi.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhaomingkeji.xyz/gtyqxbmwpc.html

Go:   os.Getwd()
来源：http://hz.aizwys.cn/gtslqoygze.html

Ruby: Dir.pwd
来源：http://hz.zhongyouzk.top/gtvpxxncpg.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ybcxt.top/gtfnswfsyn.html

[M05] 设置退出码
来源：http://hz.meibo888.top/gtaqiiwwis.html

Py:   sys.exit(1)
来源：http://hz.ydzc1.top/gtunqaikqp.html

PHP:  exit(1);
来源：http://hz.guowangkeji.top/gtlcuycihj.html

JS:   process.exit(1)
来源：http://hz.feifeiyinyue.top/gtehivetcj.html

TS:   process.exit(1)
来源：http://hz.gogol.net.cn/gtrfnbqzxg.html

Java: System.exit(1)
来源：http://hz.jiagoushi.top/gtejyfyhka.html

Go:   os.Exit(1)
来源：http://hz.yuanzhike.top/gtbcbavizy.html

Ruby: exit 1
来源：http://hz.xinyue.icu/gtqfcduylq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jianghu66.top/gtjclseydg.html

[M06] 向标准错误输出
来源：http://hz.hongshengwenyu.top/gtgletramh.html

Py:   print("err", file=sys.stderr)
来源：http://hz.gotoacloud.top/gtsgynqbuk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.guowangkeji.top/gtcrpsalrc.html

JS:   console.error("err")
来源：http://hz.sysykeji.top/gtcmjlqeiu.html

TS:   console.error("err")
来源：http://hz.ybcxt.top/gtiigvuowv.html

Java: System.err.println("err")
来源：http://hz.haohaochexian.top/gtwuepxawd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.hongshengwenyu.top/gtrxuypcor.html

Ruby: warn "err"
来源：http://hz.hammf.cn/gtozmbhhoz.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.wangshuangyany.cn/gtljmrvbfi.html

[M07] 判断是否为主入口
来源：http://hz.fzhhl.top/gttrhqqseg.html

Py:   if __name__ == "__main__":
来源：http://hz.haohaochexian.top/gtphppcqkp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.dashuyun.cn/gtpzgayuaa.html

JS:   require.main === module
来源：http://hz.zhiwuduotai.top/gtztvflfxa.html

TS:   require.main === module
来源：http://hz.hammf.cn/gtivlnjvay.html

Java: public static void main(String[] args)
来源：http://hz.jiagoushi.top/gtydlzuwdd.html

Go:   func main()
来源：http://hz.birdmap.top/gtbtqljrxb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.xylfe.cn/gtfooaskcu.html

C#:   static void Main(string[] args)
来源：http://hz.meibo888.top/gtuqacodku.html

[M08] 获取系统与运行时信息
来源：http://hz.zhijiandao.cn/gtmpxyswlq.html

Py:   platform.system();  platform.python_version()
来源：http://hz.feifeiyinyue.top/gtthsnekre.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.tanke756.top/gtggdxwgga.html

JS:   process.platform;  process.version
来源：http://hz.jianghu66.top/gtjskyzgzx.html

TS:   process.platform;  process.version
来源：http://hz.gogol.net.cn/gtqfqxfdxl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yuanzhike.top/gtcjvffnmb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.sxryk.cn/gtwfrchqpc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yvedp.cn/gtvizfcqyn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.nwbrower.top/gtgycqseci.html

================================================================================
来源：http://hz.jqgufenzy.top/gtugqwfogx.html

N. 数据结构与算法
来源：http://hz.vqdsnc.cn/gthswmbipo.html

================================================================================
来源：http://hz.yongpay.top/gtixkwbycz.html

[N01] 二分查找（有序数组）
来源：http://hz.dianchejie.cn/gtdcfroqpo.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.316326.xyz/gtnkvlnmag.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.feifeiyinyue.top/gtnwapsdrr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.haohaochexian.top/gtnzsavnpz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.pycfn.com/gtcebmgabw.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.quarkkingdee.top/gttqzcgxpg.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.smart0.xyz/gtcxsdmqvq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jinqigufen.top/gtioetyspb.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.sufxvd.cn/gthbowkxjq.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.xingfuxueyuan.xyz/gtxvfkqfji.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hammf.cn/gtpvjobifs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.redwolf501.top/gtzcbigrdi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.daria6918.cn/gtrnpdshzp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jqgufenzy.top/gteobgchqq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yonumen.top/gtdbtumltq.html

Go:   slices.Sort(arr)
来源：http://hz.quarkkingdee.top/gtrzyqkqdm.html

Ruby: arr.sort
来源：http://hz.jiagoushi.top/gtkmrkthhk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jqgufenzy.top/gtgkxjbxks.html

[N03] 快速排序（分治示例）
来源：http://hz.zhongyouzk.top/gtdzqritid.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.aizwys.cn/gtjznxrqpw.html

PHP:  // 递归实现，或用 usort
来源：http://hz.tian-w.cn/gtrwttfnpk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jlsjyb.cn/gtwdkdlgmo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.chenlongwang.top/gthagmxlno.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.chenzaomai.com/gtmtppbbhj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.svipenyu.cn/gtwnviqcdd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jinqigfzy.top/gtceybdzqd.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yvedp.cn/gtrishqwfo.html

[N04] 斐波那契数列
来源：http://hz.bjfxy.top/gtsbvswsyz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.guowangkeji.top/gtwdhuwilb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.xuetiantiany.cn/gtevanxtze.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.chenzaomai.com/gttebwcrmt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinghuilouyu.cn/gttzzbvnyd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zycfv.cn/gtynucxure.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.xuetiantiany.cn/gteplumwgy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.mhx1999.top/gtmwuufzjf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xuanzx.com/gtvltikpqr.html

[N05] 最大公约数
来源：http://hz.xziqi.cn/gtbouzrecx.html

Py:   math.gcd(a, b)
来源：http://hz.feifeiyinyue.top/gtguqcbhdy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.fzhhl.top/gtgtlfecxd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xylfe.cn/gticbavmaa.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cashguo.top/gtpaeatami.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.vqdsnc.cn/gtgpejbpkm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.wangdashe.top/gteukanwmf.html

Ruby: a.gcd(b)
来源：http://hz.sufxvd.cn/gtmtyvpiyj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.gotoacloud.top/gtabnowapy.html

[N06] 判断回文字符串
来源：http://hz.hnxiangtu.top/gtkjgxocdf.html

Py:   s == s[::-1]
来源：http://hz.fengsongda.top/gtmczishki.html

PHP:  $s === strrev($s);
来源：http://hz.yanxiufei.cn/gtxjwbbulx.html

JS:   s === [...s].reverse().join("")
来源：http://hz.iojbl.cn/gtgregwkof.html

TS:   s === [...s].reverse().join("")
来源：http://hz.316326.xyz/gtmmbsbctq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jinyuanbaomall.cn/gtqqoknniq.html

Go:   // 双指针从两端比较
来源：http://hz.sweek.top/gtbvdxxozk.html

Ruby: s == s.reverse
来源：http://hz.xziqi.cn/gtjmgntxlq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.tanke756.top/gtdujlvxvs.html

[N07] 两数之和（返回下标）
来源：http://hz.dashuyun.cn/gtakpfnasf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.vqdsnc.cn/gtrzliltsm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yj20258888.top/gtxlwnybuk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhaomingkeji.xyz/gtuivsbznc.html

TS:   // 手写 Map<string, number>
来源：http://hz.cqqwz.cn/gtslbgnpvl.html

Java: // 手写 HashMap
来源：http://hz.yvedp.cn/gtoazzntuk.html

Go:   // 手写 map[int]int
来源：http://hz.iojbl.cn/gtdibsxbcu.html

Ruby: // 手写 Hash
来源：http://hz.daria6918.cn/gtzcjipyhd.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.xziqi.cn/gtnmzrzoap.html

[N08] 生成全排列
来源：http://hz.gaohongyu789.top/gtfsuzrnpk.html

Py:   itertools.permutations(arr)
来源：http://hz.dianchejie.cn/gtwruyskhw.html

PHP:  // 手写递归交换
来源：http://hz.0kj1m.cn/gtxetnwahi.html

JS:   // 手写回溯递归
来源：http://hz.daxiang520.top/gtwdclazsh.html

TS:   // 手写回溯递归
来源：http://hz.hysaishi.cn/gtizxbtcrc.html

Java: // 手写回溯递归
来源：http://hz.xziqi.cn/gtjehsxata.html

Go:   // 手写回溯递归
来源：http://hz.9152youxi.cn/gtrvilessd.html

Ruby: arr.permutation.to_a
来源：http://hz.ydzc1.top/gtiskyokkh.html

C#:   // 手写回溯递归
来源：http://hz.gotoacloud.top/gtjruhnfnl.html

[N09] 栈与队列
来源：http://hz.wangshuangyany.cn/gtmblqzltm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.birdmap.top/gtiqhufhku.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.svipenyu.cn/gterxfytmf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhaomingkeji.xyz/gtnxulnrsc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.shanyushiyangkeji.top/gtuecwihij.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.52xcode.cn/gtuqbthdpz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.dianchejie.cn/gtzzmxgfqx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.sweek.top/gtmpyrblvj.html


<!-- 参考信息 -->