代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.dianchejie.cn/gtirfywktw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhijiandao.cn/gthprobgqm.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yvedp.cn/gttlqbqfbc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.xuetiantiany.cn/gtldctgryf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yangfankeji.com/gtqcbrbdsd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.feifeiyinyue.top/gtrvxckocz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.dianchejie.cn/gtgefsazkz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yj202588.top/gtykwedtni.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtmzhvhuwc.html

K. JSON 与序列化
来源：http://hz.dianchejie.cn/gtxxvpdbkm.html

================================================================================
来源：http://hz.xziqi.cn/gtyopirodd.html

[K01] 对象转 JSON 字符串
来源：http://hz.ydzc1.top/gtwyzzhayp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jqgufenzy.top/gtipdsyqpe.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.316326.xyz/gtmgdziaus.html

JS:   JSON.stringify(obj)
来源：http://hz.zhoulong.xyz/gtwitivzyb.html

TS:   JSON.stringify(obj)
来源：http://hz.gotoacloud.top/gtgfkaqhgb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.tianlin.xyz/gtkwmlqedf.html

Go:   json.Marshal(obj)
来源：http://hz.bjfxy.top/gtlmyvotnl.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jinqigufen.top/gtbyyrszdo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yangfankeji.com/gtcaredojl.html

[K02] JSON 字符串转对象
来源：http://hz.aizwys.cn/gtlfapciiu.html

Py:   json.loads(s)
来源：http://hz.meibo888.top/gtlmvqllai.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yj202588.top/gtfahmqipy.html

JS:   JSON.parse(s)
来源：http://hz.jlsjyb.cn/gtsnkbogxa.html

TS:   JSON.parse(s)
来源：http://hz.wangshuangyany.cn/gtdxtjkkox.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.birdmap.top/gthneegocc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hysaishi.cn/gtwanfyfyc.html

Ruby: JSON.parse(s)
来源：http://hz.sufxvd.cn/gtxqqdjrja.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.0kj1m.cn/gtxeibqfih.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.0kj1m.cn/gttynlfcwf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.chenlongwang.top/gtpleupeqh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.quarkkingdee.top/gtohhkmwoa.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj20258.top/gtkrolhyog.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.gaohongyu789.top/gteqmuovis.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.bjfxy.top/gtkgphgqcz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.tian-w.cn/gttamdugfw.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhixingplan.top/gtfoixlapc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hammf.cn/gtmybbwyae.html

[K04] 读取 JSON 文件
来源：http://hz.cashguo.top/gtvewrtsdp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.wangshuangyany.cn/gtpdaxeczs.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.haohaochexian.top/gtimwawmwg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ivvv.top/gtpblbhear.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhaomingkeji.xyz/gtsfjxspoa.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhixingplan.top/gtzlmbmrcn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.chenlongwang.top/gtgvltwuoo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.chenzaomai.com/gtmfvyrpjs.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.quarkkingdee.top/gtjolexgle.html

[K05] 深拷贝对象
来源：http://hz.jlsjyb.cn/gtknxjycll.html

Py:   copy.deepcopy(obj)
来源：http://hz.birdmap.top/gtftlujbhc.html

PHP:  unserialize(serialize($obj));
来源：http://hz.316326.xyz/gtgxjoifwr.html

JS:   structuredClone(obj)
来源：http://hz.feifeiyinyue.top/gtdvixktpk.html

TS:   structuredClone(obj)
来源：http://hz.9152youxi.cn/gtngsxlqno.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yj20258.top/gteglfzxiy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jinqigfzy.top/gtjryjilmf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.gaohongyu789.top/gtrevkxbpw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jinyuanbaomall.cn/gtqsdlitgb.html

[K06] 解析 URL 查询串
来源：http://hz.birdmap.top/gtzvrflrqd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.quarkkingdee.top/gtiddkanle.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jianghu66.top/gtwrqmxjgf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tian-w.cn/gtvliyakpp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nwbrower.top/gtmkvmmntx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jiagoushi.top/gtepjkcjps.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.birdmap.top/gttdicifig.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.shuidangran.top/gtfdmgyuih.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.shangyingyoupin.top/gtwlklklxb.html

[K07] 进制转换
来源：http://hz.ehwqpu.com/gtfcaajhwa.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.smart0.xyz/gtjvdtgdgp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.pycfn.com/gtkbwbweyc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jqgufenzy.top/gtcuizxymn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.meibo888.top/gtqmsfjpua.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cheryme.top/gthewlsskf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.pycfn.com/gtlogwptld.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.bjfxy.top/gthuuyrxns.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yuxming.cn/gtvhvtvywg.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yangfankeji.com/gtvifjlxcw.html

Py:   pickle.dumps(obj)
来源：http://hz.zhijiandao.cn/gtftfekoad.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.haohaochexian.top/gtruesoefd.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shanyushiyangkeji.top/gtehfrgjss.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.gogol.net.cn/gtoklybeie.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.iojbl.cn/gtrflcwnlg.html

Go:   encoding/gob
来源：http://hz.chenlongwang.top/gtysgpelzt.html

Ruby: Marshal.dump(obj)
来源：http://hz.tanke756.top/gthkpkvqtf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ivvv.top/gtmeiuwlze.html

================================================================================
来源：http://hz.meibo888.top/gtvpdvhgfk.html

L. 网络请求
来源：http://hz.xingfuxueyuan.xyz/gthwqqavrc.html

================================================================================
来源：http://hz.yonumen.top/gtocqdluze.html

[L01] 发送 GET 请求
来源：http://hz.birdmap.top/gtwxaawleb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.ywan-chungtsiang.top/gtgwklcxrg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hfpthk.cn/gttwmhxbze.html

JS:   await fetch(url)
来源：http://hz.ivvv.top/gtmcpwxgbw.html

TS:   await fetch(url)
来源：http://hz.vqdsnc.cn/gtilcblakm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zycfv.cn/gtlucwllpt.html

Go:   resp, err := http.Get(url)
来源：http://hz.feifeiyinyue.top/gtammuacdy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xuetiantiany.cn/gtzswxeovb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.havefunace.top/gtxmzchmgd.html

[L02] 发送 POST JSON
来源：http://hz.fzhhl.top/gtwrdpqyez.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hammf.cn/gtmtvuxkvu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.gotoacloud.top/gtbeuyzyel.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.dashuyun.cn/gtjromqwgj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhaomingkeji.xyz/gtkkwebxoe.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.birdmap.top/gtnrzadmpq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhijiandao.cn/gtskpbvior.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.hywenlv.cn/gtkaynftee.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xylfe.cn/gtqtxfoqbr.html

[L03] 设置自定义请求头
来源：http://hz.9152youxi.cn/gtjfwnkgxr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.9152youxi.cn/gtsgeafffx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hongshengwenyu.top/gtmabmnnuq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yonumen.top/gtlqefeeiz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhixingplan.top/gtfieuvtws.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jiagoushi.top/gtuhhcbash.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.xylfe.cn/gtyqifufby.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.shangyingyoupin.top/gtuzmjlict.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhengqikj.top/gtkguexwgm.html

[L04] 设置超时
来源：http://hz.feifeiyinyue.top/gtfhrvkkyb.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zhixingplan.top/gtsbzndtqw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.9152youxi.cn/gtzlynpmei.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ybcxt.top/gtprggzuvo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.tian-w.cn/gtrvtwngan.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jinqigufen.top/gtiikedpea.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yuanzhike.top/gtngvonzde.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.cashguo.top/gtkepnober.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.cashguo.top/gtblxmlqvz.html

[L05] 上传文件（multipart）
来源：http://hz.pengpengdd.cyou/gtvfneqgtm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zycfv.cn/gtcsvyfyzl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.tian-w.cn/gtckjpqqbj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jqgufenzy.top/gtjoyvdkjx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.dianchejie.cn/gtzknwmpiv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jinghuilouyu.cn/gtsdiqtlgl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.chenlongwang.top/gtjxrbmypn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.sxryk.cn/gtwweucgix.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.cdnleiting.top/gtnldnazec.html

[L06] 解析响应为 JSON
来源：http://hz.yj20258.top/gttiazfhgz.html

Py:   resp.json()
来源：http://hz.jqgfzy.top/gtdxopesyx.html

PHP:  json_decode($body, true);
来源：http://hz.jiagoushi.top/gtmhtnoskg.html

JS:   await resp.json()
来源：http://hz.svipenyu.cn/gtvnemmiwc.html

TS:   await resp.json()
来源：http://hz.gaohongyu789.top/gtixdbbufw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.cucudq.cn/gtzwzztvne.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jinqigufen.top/gtcjvvtoea.html

Ruby: JSON.parse(resp.body)
来源：http://hz.svipenyu.cn/gtdhtanrch.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.pycfn.com/gtgeopmjel.html

[L07] 处理 HTTP 状态码
来源：http://hz.birdmap.top/gtctofhdbl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yj20258888.top/gthylwxrcl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yuxming.cn/gtzrnxxdox.html

JS:   resp.ok;  resp.status
来源：http://hz.guowangkeji.top/gtjcbcywmv.html

TS:   resp.ok;  resp.status
来源：http://hz.0kj1m.cn/gtwnpqmgvq.html

Java: resp.statusCode()
来源：http://hz.jinqigufen.top/gtniuvgddi.html

Go:   resp.StatusCode
来源：http://hz.sxryk.cn/gtrvxnrqxz.html

Ruby: resp.code.to_i
来源：http://hz.vqdsnc.cn/gtyzpafkwi.html

C#:   (int)resp.StatusCode
来源：http://hz.hfpthk.cn/gthftcbuvk.html

[L08] 并发请求多个地址
来源：http://hz.gzhubu.top/gtumlewdxt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.daxiang520.top/gtlfhwvhhk.html

PHP:  curl_multi_init() 系列
来源：http://hz.zdqjudy.top/gtqnjkwknu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fzhhl.top/gtfvwdvjjv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.haohaochexian.top/gtzsjzcblg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hysaishi.cn/gttxszznxt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yj20258.top/gtuxkbjrtz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jinqigufen.top/gtbkybkaln.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yangfankeji.com/gtonmedwlk.html

================================================================================
来源：http://hz.ybcxt.top/gtnlthiwrb.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhijiandao.cn/gtjyepoebx.html

================================================================================
来源：http://hz.nanxinkj.top/gtbbryhrjq.html

[M01] 读取命令行参数
来源：http://hz.chenlongwang.top/gtqfxyktvu.html

Py:   sys.argv[1:]
来源：http://hz.shanyushiyangkeji.top/gtipuuusvs.html

PHP:  $argv;  $argc;
来源：http://hz.zhixingplan.top/gthjhuwrpf.html

JS:   process.argv.slice(2)
来源：http://hz.chenjidiqi.icu/gtagudeazg.html

TS:   process.argv.slice(2)
来源：http://hz.ydjk.org.cn/gtefonfxsq.html

Java: args 数组（main 方法参数）
来源：http://hz.aizwys.cn/gtaofotymr.html

Go:   os.Args[1:]
来源：http://hz.xingfuxueyuan.xyz/gtrnyukswl.html

Ruby: ARGV
来源：http://hz.ehwqpu.com/gtqqsvmahs.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yueranfly.top/gttgihsooh.html

[M02] 读取环境变量
来源：http://hz.ywan-chungtsiang.top/gtzxbfbnyh.html

Py:   os.environ.get("HOME")
来源：http://hz.chenzaomai.com/gtvabvrlca.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ivvv.top/gtezzrfmzi.html

JS:   process.env.HOME
来源：http://hz.jiagoushi.top/gtaicscspp.html

TS:   process.env.HOME
来源：http://hz.ydzc1.top/gtdqjjfoeq.html

Java: System.getenv("HOME")
来源：http://hz.yj20258888.top/gtcyklystk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.sysykeji.top/gtksgloknl.html

Ruby: ENV["HOME"]
来源：http://hz.yueranfly.top/gtbvnxbqrv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.fzhhl.top/gtwxuxjdwg.html

[M03] 执行外部命令
来源：http://hz.zhongyouzk.top/gtzbmvfvud.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.bjfxy.top/gtxykjmeng.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.c1oappe.top/gtdmwkzsng.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.bjfxy.top/gtldjaadnd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.aizwys.cn/gtxxvcxtpn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.cucudq.cn/gtwgtezbym.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.feifeiyinyue.top/gthgsubvlq.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.guowangkeji.top/gtmwhxgyjq.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yvedp.cn/gtmlfsxsur.html

[M04] 获取当前工作目录
来源：http://hz.ydjk.org.cn/gtqovkpphp.html

Py:   os.getcwd()
来源：http://hz.aizwys.cn/gtfjxaspwc.html

PHP:  getcwd();
来源：http://hz.cashguo.top/gtgpkqelgu.html

JS:   process.cwd()
来源：http://hz.shuidangran.top/gtatawgyld.html

TS:   process.cwd()
来源：http://hz.nwbrower.top/gtyvkbvwhb.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.tian-w.cn/gtlxzqkoak.html

Go:   os.Getwd()
来源：http://hz.jinghuilouyu.cn/gtyutktdif.html

Ruby: Dir.pwd
来源：http://hz.zdqjudy.top/gteoxippul.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yvedp.cn/gtoqbuhonn.html

[M05] 设置退出码
来源：http://hz.kuanghao11.cn/gtowimdmxu.html

Py:   sys.exit(1)
来源：http://hz.dashuyun.cn/gtrqqkwlsu.html

PHP:  exit(1);
来源：http://hz.jqgufenzy.top/gtllcxzick.html

JS:   process.exit(1)
来源：http://hz.zhoulong.xyz/gtnqwkhbvc.html

TS:   process.exit(1)
来源：http://hz.c1oappe.top/gtdjcabmqe.html

Java: System.exit(1)
来源：http://hz.hammf.cn/gtseewdhti.html

Go:   os.Exit(1)
来源：http://hz.ydzc1.top/gtaslbqmra.html

Ruby: exit 1
来源：http://hz.shuidangran.top/gtinawjnhz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ehwqpu.com/gtbriebxbo.html

[M06] 向标准错误输出
来源：http://hz.havefunace.top/gtgmzkfdyt.html

Py:   print("err", file=sys.stderr)
来源：http://hz.nanxuanxn.top/gtqfnpwcvc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhongyouzk.top/gtpclvlhua.html

JS:   console.error("err")
来源：http://hz.fengsongda.top/gtcsxzujkx.html

TS:   console.error("err")
来源：http://hz.snrcjt.cn/gtbblebpns.html

Java: System.err.println("err")
来源：http://hz.ydzc1.top/gtvtergxcf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.sysykeji.top/gtwimcmklq.html

Ruby: warn "err"
来源：http://hz.hysaishi.cn/gtvdapxtli.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.vqdsnc.cn/gtbyviofnj.html

[M07] 判断是否为主入口
来源：http://hz.0kj1m.cn/gthxbktcvn.html

Py:   if __name__ == "__main__":
来源：http://hz.zhiwuduotai.top/gtkjeytjtd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jyoumei.cn/gtrsipjaxk.html

JS:   require.main === module
来源：http://hz.redwolf501.top/gtohwocwum.html

TS:   require.main === module
来源：http://hz.pycfn.com/gtfaivrixo.html

Java: public static void main(String[] args)
来源：http://hz.xingfuxueyuan.xyz/gtkdjnotxh.html

Go:   func main()
来源：http://hz.cheryme.top/gtsdskpzgz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.daxiang520.top/gtkkozdmkp.html

C#:   static void Main(string[] args)
来源：http://hz.yonumen.top/gtxikghaad.html

[M08] 获取系统与运行时信息
来源：http://hz.shuidangran.top/gtxtnbwwus.html

Py:   platform.system();  platform.python_version()
来源：http://hz.dashuyun.cn/gteaiypqqf.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.sweek.top/gtuvzttskn.html

JS:   process.platform;  process.version
来源：http://hz.birdmap.top/gtoloduzjw.html

TS:   process.platform;  process.version
来源：http://hz.jqgufenzy.top/gtbqatijsj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xylfe.cn/gteglwiqqs.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.cqqwz.cn/gtydrgaeen.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ybcxt.top/gtqgqrkrdo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yj20258888.top/gtkyipqqfw.html

================================================================================
来源：http://hz.andypj.xyz/gtovfppjst.html

N. 数据结构与算法
来源：http://hz.yangfankeji.com/gtctbgysjk.html

================================================================================
来源：http://hz.ydjk.org.cn/gtmuoupgkm.html

[N01] 二分查找（有序数组）
来源：http://hz.zhijiandao.cn/gtxfikwzqx.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.52xcode.cn/gtcygupfvd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.sweek.top/gtburxufgm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yongpay.top/gtcedjrofk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shangyingyoupin.top/gtcotkhwjs.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.52xcode.cn/gtuuoocryj.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.shanyushiyangtech.top/gtxvpgcdzg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xuetiantiany.cn/gtyzcaldwa.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.bjfxy.top/gtsuctlbuv.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.quarkkingdee.top/gtkcrtyjuk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.fengsongda.top/gtnhzuluuy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yj20258.top/gtahznwaqi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.haohaochexian.top/gtxpniopta.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.feifeiyinyue.top/gtiejmwyzv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.dashuyun.cn/gtqbharuzy.html

Go:   slices.Sort(arr)
来源：http://hz.xziqi.cn/gtcatqhahw.html

Ruby: arr.sort
来源：http://hz.meibo888.top/gtuktwytml.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.hammf.cn/gtnnspcohk.html

[N03] 快速排序（分治示例）
来源：http://hz.shzxlz.cn/gtriyseejo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yongpay.top/gtkcccxcxt.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jiagoushi.top/gtoxymebhb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tianlin.xyz/gtmlkylwaq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gzhubu.top/gtgyqufinw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jlsjyb.cn/gtzyrkeako.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.xinyue.icu/gtudocvsqb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.wangshuangyany.cn/gtedrrsvgb.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.tianlin.xyz/gtkcvnghwk.html

[N04] 斐波那契数列
来源：http://hz.shuidangran.top/gtggagtysu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yuanzhike.top/gtwmmjxnqf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yongpay.top/gtzlnsjhzc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhixingplan.top/gtkxmjnfhy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sufxvd.cn/gtjqtvuvdk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jinqigfzy.top/gtccqambvi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhiwuduotai.top/gtbcaawqqm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jinghuilouyu.cn/gtdyyszhsk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.gotoacloud.top/gtiywjbcwk.html

[N05] 最大公约数
来源：http://hz.sweek.top/gtggntlllh.html

Py:   math.gcd(a, b)
来源：http://hz.0kj1m.cn/gtjygephrj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.ywan-chungtsiang.top/gtxgygozjj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.wangdashe.top/gtivgvzlmc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.316326.xyz/gtoeqppqbs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jyoumei.cn/gtowsttnkj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.guowangkeji.top/gtwzlufkuw.html

Ruby: a.gcd(b)
来源：http://hz.vqdsnc.cn/gtsawmxiig.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.c1oappe.top/gtfpbtncqi.html

[N06] 判断回文字符串
来源：http://hz.zhixingplan.top/gtcnebpvwk.html

Py:   s == s[::-1]
来源：http://hz.havefunace.top/gtrsjmacnw.html

PHP:  $s === strrev($s);
来源：http://hz.vqdsnc.cn/gtcowluzkq.html

JS:   s === [...s].reverse().join("")
来源：http://hz.9152youxi.cn/gtheovcpik.html

TS:   s === [...s].reverse().join("")
来源：http://hz.aizwys.cn/gtmbpaafby.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.gotoacloud.top/gtxekhtkhf.html

Go:   // 双指针从两端比较
来源：http://hz.jqgufenzy.top/gtduqjicla.html

Ruby: s == s.reverse
来源：http://hz.xingfuxueyuan.xyz/gthfwmwtej.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.chenjidiqi.icu/gtnxlvkfpj.html

[N07] 两数之和（返回下标）
来源：http://hz.smart0.xyz/gtbbiaihzx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jiagoushi.top/gtptfmlaut.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.xuanzx.com/gtjgccphjs.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.c1oappe.top/gtlwhpzkal.html

TS:   // 手写 Map<string, number>
来源：http://hz.zhiwuduotai.top/gtvulinjlu.html

Java: // 手写 HashMap
来源：http://hz.zhixingplan.top/gtxbnddzow.html

Go:   // 手写 map[int]int
来源：http://hz.jinqigufen.top/gtmxgmltok.html

Ruby: // 手写 Hash
来源：http://hz.bjfxy.top/gtjnqqejmh.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.guannengcc.top/gtiacvnfbu.html

[N08] 生成全排列
来源：http://hz.snrcjt.cn/gtgbmosjnv.html


<!-- 参考信息 -->