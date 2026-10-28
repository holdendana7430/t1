代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yuanzhike.top/gtopdrdvqi.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.gogol.net.cn/gtuiclbpcj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.pengpengdd.cyou/gtnexhcduu.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.sysykeji.top/gtlffowiel.html

================================================================================
来源：http://hz.hywenlv.cn/gthyubtljy.html

K. JSON 与序列化
来源：http://hz.jinghuilouyu.cn/gtyhdcrikz.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtcthvraea.html

[K01] 对象转 JSON 字符串
来源：http://hz.vqdsnc.cn/gtgvxcudnq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.aizwys.cn/gtttkkikhq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yangfankeji.com/gtgkubqtfx.html

JS:   JSON.stringify(obj)
来源：http://hz.zhixingplan.top/gtakrvwuzg.html

TS:   JSON.stringify(obj)
来源：http://hz.0kj1m.cn/gtxoszqpdk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.gotoacloud.top/gtieoocved.html

Go:   json.Marshal(obj)
来源：http://hz.iojbl.cn/gtlezxmsow.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yj202588.top/gtuidqrpur.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.dianchejie.cn/gtkyvbtdac.html

[K02] JSON 字符串转对象
来源：http://hz.ppjwa.cn/gtgtbmcoee.html

Py:   json.loads(s)
来源：http://hz.guowangkeji.top/gtqgilwefl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.dashuyun.cn/gtjguedhmf.html

JS:   JSON.parse(s)
来源：http://hz.ybcxt.top/gtudgeojmv.html

TS:   JSON.parse(s)
来源：http://hz.tanke756.top/gtaiahrxah.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jinyuanbaomall.cn/gthjtmjcby.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhixingplan.top/gtjbmpxpsw.html

Ruby: JSON.parse(s)
来源：http://hz.chenjidiqi.icu/gttshwfenl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zdqjudy.top/gtdivuuetd.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zycfv.cn/gtmzgmszbd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.gaohongyu789.top/gtqmgrtomc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.guannengcc.top/gtceuvrxvd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xinyue.icu/gtdoprhtwp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj20258.top/gttbtevdig.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.0kj1m.cn/gtijgymqrp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.dianchejie.cn/gtvezxighs.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.tian-w.cn/gtmxeyilry.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hongshengwenyu.top/gtskxcfzhr.html

[K04] 读取 JSON 文件
来源：http://hz.ybcxt.top/gtdkmeoedw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xingfuxueyuan.xyz/gtfytengna.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.chenlongwang.top/gtfvjttnfv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ydjk.org.cn/gtrigqeamy.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cheryme.top/gtsivpbtqt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.fzhhl.top/gtkzaunojq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.tian-w.cn/gtmnbiuxsy.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yongpay.top/gtzutdxidv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.nwbrower.top/gtdldhkrqz.html

[K05] 深拷贝对象
来源：http://hz.cucudq.cn/gtlousnodl.html

Py:   copy.deepcopy(obj)
来源：http://hz.xingfuxueyuan.xyz/gtrvflpkbf.html

PHP:  unserialize(serialize($obj));
来源：http://hz.haohaochexian.top/gtqpwsdbjk.html

JS:   structuredClone(obj)
来源：http://hz.snrcjt.cn/gthfseuwzc.html

TS:   structuredClone(obj)
来源：http://hz.jqgfzy.top/gtahlsffbd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.vqdsnc.cn/gtyvyvpfrx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.sysykeji.top/gtmwegzwxv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.iojbl.cn/gtifbxniko.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhaomingkeji.xyz/gtktkeloje.html

[K06] 解析 URL 查询串
来源：http://hz.smart0.xyz/gtqsllcnpl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.iojbl.cn/gtopnjsjsn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.haohaochexian.top/gtrdbejxnw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yonumen.top/gtulfxwpmb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yvedp.cn/gtzdsywqcv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yj20258.top/gtselibaiv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.ydjk.org.cn/gtvdzwrjqy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yj20258.top/gthkqgpktr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhengqikj.top/gtbhrgtuej.html

[K07] 进制转换
来源：http://hz.gogol.net.cn/gtrhqjpsfh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hfpthk.cn/gttsgkfzln.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jqgfzy.top/gtizpkhjcy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.aizwys.cn/gtphyhncpr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhixingplan.top/gtibbpkoqh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jinghuilouyu.cn/gtqzgsccrq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hysaishi.cn/gtqlrycfqm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zycfv.cn/gtyvbbtakt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yueranfly.top/gtmfmqqjap.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.316326.xyz/gtterqqelw.html

Py:   pickle.dumps(obj)
来源：http://hz.chenzaomai.com/gtnupfwoyz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hywenlv.cn/gttstjhtlu.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shanyushiyangkeji.top/gtvipspauw.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.feifeiyinyue.top/gtmaorogis.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.tian-w.cn/gtfcjabsvj.html

Go:   encoding/gob
来源：http://hz.jlsjyb.cn/gtlqcummvj.html

Ruby: Marshal.dump(obj)
来源：http://hz.chenlongwang.top/gtutwejmfj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.sweek.top/gtlrzndqkg.html

================================================================================
来源：http://hz.yonumen.top/gtktbjrioo.html

L. 网络请求
来源：http://hz.pycfn.com/gtstnplbvh.html

================================================================================
来源：http://hz.bjfxy.top/gtdzefkvpz.html

[L01] 发送 GET 请求
来源：http://hz.yueranfly.top/gtzmzhlqel.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.xinyue.icu/gtoghfijvs.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.fengsongda.top/gteeztcsug.html

JS:   await fetch(url)
来源：http://hz.dianchejie.cn/gtwipmmkpy.html

TS:   await fetch(url)
来源：http://hz.wangdashe.top/gtrpnisepw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.cdnleiting.top/gtouwpblus.html

Go:   resp, err := http.Get(url)
来源：http://hz.snrcjt.cn/gtixoozdkr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cucudq.cn/gtgoheguob.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.tian-w.cn/gtonhtjjiq.html

[L02] 发送 POST JSON
来源：http://hz.yanxiufei.cn/gtejzbbolf.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.cheryme.top/gtijaleuna.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xuanzx.com/gtjfmkrgqm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.haohaochexian.top/gtstfybhtt.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ywan-chungtsiang.top/gtefubtgqg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.quarkkingdee.top/gtaaaxbgqn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.tianlin.xyz/gtuoreumem.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yvedp.cn/gtbjdromfp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zycfv.cn/gtazfaihlh.html

[L03] 设置自定义请求头
来源：http://hz.yj20258888.top/gtxrzxraps.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jianghu66.top/gtqltmfmml.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.haohaochexian.top/gtjdjaxisn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.daria6918.cn/gtxhjdswcr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.wangshuangyany.cn/gtawwdorwf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.shuidangran.top/gtrrhgorcl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yanxiufei.cn/gtfepnbiwz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhijiandao.cn/gtrzxsjeeb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.tianlin.xyz/gtpqtaaztj.html

[L04] 设置超时
来源：http://hz.316326.xyz/gtdpnegtka.html

Py:   requests.get(url, timeout=5)
来源：http://hz.havefunace.top/gtbiobxhnb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yueranfly.top/gtswhzvyuw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.svipenyu.cn/gtfiuviteu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jqgfzy.top/gteakuxhvw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhijiandao.cn/gtlidjcmsn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.cucudq.cn/gtqqvavluo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.fzhhl.top/gtleocfbwl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.guannengcc.top/gthjfwsszb.html

[L05] 上传文件（multipart）
来源：http://hz.vqdsnc.cn/gtxqzrlrqc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yj20258888.top/gtektquwrz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yj202588.top/gtjqczizdt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.havefunace.top/gtrjtiyrxy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.xuetiantiany.cn/gttgzkweks.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.gaohongyu789.top/gtxoslfcgp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.sweek.top/gtpznxmpug.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.gaohongyu789.top/gtmwagcqst.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.snrcjt.cn/gtdsrscqci.html

[L06] 解析响应为 JSON
来源：http://hz.zhoulong.xyz/gtzuldplbr.html

Py:   resp.json()
来源：http://hz.nanxuanxn.top/gtbtyhdfqp.html

PHP:  json_decode($body, true);
来源：http://hz.xinyue.icu/gtcwufoqkr.html

JS:   await resp.json()
来源：http://hz.andypj.xyz/gtqaevqgtt.html

TS:   await resp.json()
来源：http://hz.zdqjudy.top/gtwcjpcawc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.wangdashe.top/gtcixhzlix.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.tanke756.top/gtgpewhyvm.html

Ruby: JSON.parse(resp.body)
来源：http://hz.redwolf501.top/gtvecddgpa.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.chenzaomai.com/gtwypayuio.html

[L07] 处理 HTTP 状态码
来源：http://hz.yueranfly.top/gtaonobdzw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.ivvv.top/gtxctejejs.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yanxiufei.cn/gtjlewbumw.html

JS:   resp.ok;  resp.status
来源：http://hz.aibaodan.cn/gtnvabegic.html

TS:   resp.ok;  resp.status
来源：http://hz.cashguo.top/gtwjuleoab.html

Java: resp.statusCode()
来源：http://hz.hfpthk.cn/gtiyideuzf.html

Go:   resp.StatusCode
来源：http://hz.sysykeji.top/gtrytfsqyk.html

Ruby: resp.code.to_i
来源：http://hz.xingfuxueyuan.xyz/gtsvjdwiwr.html

C#:   (int)resp.StatusCode
来源：http://hz.feifeiyinyue.top/gtadvajspm.html

[L08] 并发请求多个地址
来源：http://hz.yangfankeji.com/gtwowzuymd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.guannengcc.top/gtesodwell.html

PHP:  curl_multi_init() 系列
来源：http://hz.pycfn.com/gtreeuantp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shangyingyoupin.top/gtcpdkooog.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.havefunace.top/gtaunjmbns.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hnxiangtu.top/gtwzcgkwes.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.gotoacloud.top/gtflpqiqlw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ivvv.top/gtiemyhpqf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.svipenyu.cn/gtqlcpldqx.html

================================================================================
来源：http://hz.ydjk.org.cn/gtfdsiirwe.html

M. 命令行 / 进程 / 环境
来源：http://hz.jinqigfzy.top/gtfcopwvbd.html

================================================================================
来源：http://hz.xuanzx.com/gtusafiklx.html

[M01] 读取命令行参数
来源：http://hz.jlsjyb.cn/gtmnvxzsou.html

Py:   sys.argv[1:]
来源：http://hz.jlsjyb.cn/gtcmmpwmvq.html

PHP:  $argv;  $argc;
来源：http://hz.wangdashe.top/gteprgmhfg.html

JS:   process.argv.slice(2)
来源：http://hz.shangyingyoupin.top/gtrxacydiv.html

TS:   process.argv.slice(2)
来源：http://hz.chenzaomai.com/gtfjfijpvi.html

Java: args 数组（main 方法参数）
来源：http://hz.meibo888.top/gtrcjxvoeb.html

Go:   os.Args[1:]
来源：http://hz.chenjidiqi.icu/gttigoyhvp.html

Ruby: ARGV
来源：http://hz.jqgufenzy.top/gtjhbdmlvn.html

C#:   args 数组（Main 方法参数）
来源：http://hz.wangshuangyany.cn/gtjtwrefdl.html

[M02] 读取环境变量
来源：http://hz.shanyushiyangkeji.top/gtixlggvgt.html

Py:   os.environ.get("HOME")
来源：http://hz.yj20258888.top/gteskpvojv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.svipenyu.cn/gtkitqbizf.html

JS:   process.env.HOME
来源：http://hz.ydjk.org.cn/gtjvnvygrs.html

TS:   process.env.HOME
来源：http://hz.fengsongda.top/gtqbvghjkh.html

Java: System.getenv("HOME")
来源：http://hz.nanxuanxn.top/gtusfzzvtv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.svipenyu.cn/gtpbcisunf.html

Ruby: ENV["HOME"]
来源：http://hz.sufxvd.cn/gtovgbaesa.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shuidangran.top/gtnmoxhrbi.html

[M03] 执行外部命令
来源：http://hz.kuanghao11.cn/gtpiphqqzt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.sufxvd.cn/gtykwfzsoz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hammf.cn/gtbgeiomej.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.sxryk.cn/gtdhungwkm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yj202588.top/gtgffoeeeo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.chenzaomai.com/gtemxitapr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.nanxuanxn.top/gtivueoyjq.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.gzhubu.top/gttcksalki.html

C#:   Process.Start("ls", "-l");
来源：http://hz.gotoacloud.top/gtbfebqspu.html

[M04] 获取当前工作目录
来源：http://hz.316326.xyz/gtxsgjegft.html

Py:   os.getcwd()
来源：http://hz.meibo888.top/gtldxdrzee.html

PHP:  getcwd();
来源：http://hz.snrcjt.cn/gtdtbtduzx.html

JS:   process.cwd()
来源：http://hz.xuanzx.com/gtavbppcgy.html

TS:   process.cwd()
来源：http://hz.yonumen.top/gtpnbuechp.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.tian-w.cn/gtyydfybzq.html

Go:   os.Getwd()
来源：http://hz.zycfv.cn/gthmadlsbv.html

Ruby: Dir.pwd
来源：http://hz.yangfankeji.com/gtsiksbyii.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhongyouzk.top/gttudybrjo.html

[M05] 设置退出码
来源：http://hz.cashguo.top/gtgpkbsabv.html

Py:   sys.exit(1)
来源：http://hz.chenjidiqi.icu/gtqhewddsi.html

PHP:  exit(1);
来源：http://hz.hywenlv.cn/gtqzbwkhxq.html

JS:   process.exit(1)
来源：http://hz.yongpay.top/gtrfhxziyo.html

TS:   process.exit(1)
来源：http://hz.shanyushiyangkeji.top/gtjbkjmvuo.html

Java: System.exit(1)
来源：http://hz.jinyuanbaomall.cn/gtlthdyrdn.html

Go:   os.Exit(1)
来源：http://hz.cheryme.top/gtyqsppjrd.html

Ruby: exit 1
来源：http://hz.yangfankeji.com/gtjalrgwtv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.pengpengdd.cyou/gtswywizmk.html

[M06] 向标准错误输出
来源：http://hz.snrcjt.cn/gtlwicuspt.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhijiandao.cn/gtogvqgqgb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.shangyingyoupin.top/gtnypnrowo.html

JS:   console.error("err")
来源：http://hz.zhixingplan.top/gtnajlumpg.html

TS:   console.error("err")
来源：http://hz.yj20258888.top/gtkrquwalb.html

Java: System.err.println("err")
来源：http://hz.ybcxt.top/gtumqdzklf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.meibo888.top/gtlvwaluvd.html

Ruby: warn "err"
来源：http://hz.gogol.net.cn/gtwhmmjbwo.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yuxming.cn/gtwlfvvbja.html

[M07] 判断是否为主入口
来源：http://hz.zhiwuduotai.top/gtgyvbytgc.html

Py:   if __name__ == "__main__":
来源：http://hz.xinyue.icu/gtyvqvlbkf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.nanxinkj.top/gtiujqxztu.html

JS:   require.main === module
来源：http://hz.sxryk.cn/gthhaarpwx.html

TS:   require.main === module
来源：http://hz.andypj.xyz/gtyuspvhka.html

Java: public static void main(String[] args)
来源：http://hz.xziqi.cn/gtkgsxvwzl.html

Go:   func main()
来源：http://hz.aizwys.cn/gtdedvunry.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.smart0.xyz/gtwhaezlmc.html

C#:   static void Main(string[] args)
来源：http://hz.shanyushiyangtech.top/gtyepxzhgg.html

[M08] 获取系统与运行时信息
来源：http://hz.tianlin.xyz/gtvxzaxfxc.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yongpay.top/gtojculsvc.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.guowangkeji.top/gtotbkvvqa.html

JS:   process.platform;  process.version
来源：http://hz.shanyushiyangtech.top/gtazxuhkga.html

TS:   process.platform;  process.version
来源：http://hz.jinghuilouyu.cn/gtkmayefgk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.aizwys.cn/gtmcoukbub.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yuxming.cn/gtfopetuik.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.sysykeji.top/gtctkdskzi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ppjwa.cn/gtpibncdnt.html

================================================================================
来源：http://hz.tanke756.top/gtaunwixbz.html

N. 数据结构与算法
来源：http://hz.gzhubu.top/gtgggbvgho.html

================================================================================
来源：http://hz.jiagoushi.top/gtfmpahazb.html

[N01] 二分查找（有序数组）
来源：http://hz.xuetiantiany.cn/gtyinungrn.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hfpthk.cn/gtwgqxtzaj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.sufxvd.cn/gtujkrqfae.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhoulong.xyz/gtsscrkxnn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xuetiantiany.cn/gtzhworizb.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yueranfly.top/gttuikinbp.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.xuanzx.com/gtbopcbzco.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xuetiantiany.cn/gtjlovyjfw.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.gogol.net.cn/gtbgbzovlm.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.hnqzz.top/gtfiaycrqx.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cheryme.top/gtpnunhqrg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhijiandao.cn/gtybspjndb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhoulong.xyz/gtbhtpafvq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.wangdashe.top/gtqmviajsn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.snrcjt.cn/gtvcckgymk.html

Go:   slices.Sort(arr)
来源：http://hz.sufxvd.cn/gtahhufxxr.html

Ruby: arr.sort
来源：http://hz.dianchejie.cn/gtmpnttcsl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhongyouzk.top/gtktqnbuag.html

[N03] 快速排序（分治示例）
来源：http://hz.gzhubu.top/gtureqycch.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.gotoacloud.top/gtjvxtihhf.html

PHP:  // 递归实现，或用 usort
来源：http://hz.sysykeji.top/gtcdgwoxiy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gogol.net.cn/gtvqscfgxj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hnxiangtu.top/gtokgrtwuq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinqigfzy.top/gtuhtptrym.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.aibaodan.cn/gthgiqnfgl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.dashuyun.cn/gttclqhqie.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhixingplan.top/gtkaahdcwd.html

[N04] 斐波那契数列
来源：http://hz.ydjk.org.cn/gtkoewsqgl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.meibo888.top/gtwhnzaovc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.nwbrower.top/gtfnxjlykt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.guannengcc.top/gthmltyecz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj20258888.top/gtjoqfkcnf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.ivvv.top/gtawqwjmtp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hysaishi.cn/gtorpystqu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.xuanzx.com/gtyhllfqwg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.shanyushiyangtech.top/gtpqsyprnw.html

[N05] 最大公约数
来源：http://hz.xinyue.icu/gtrxbaadlb.html

Py:   math.gcd(a, b)
来源：http://hz.hfpthk.cn/gthgxaurau.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.c1oappe.top/gtxrchuggv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shanyushiyangkeji.top/gtzsgwhoul.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ppjwa.cn/gtivzulrve.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zhongyouzk.top/gttfbcjgrm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.sysykeji.top/gtlgktzcac.html

Ruby: a.gcd(b)
来源：http://hz.redwolf501.top/gtjocppbvk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ivvv.top/gtwmmseruc.html

[N06] 判断回文字符串
来源：http://hz.jinyuanbaomall.cn/gtvwldlqvw.html

Py:   s == s[::-1]
来源：http://hz.nanxuanxn.top/gtdzxutpqv.html

PHP:  $s === strrev($s);
来源：http://hz.vqdsnc.cn/gttesrnvbg.html

JS:   s === [...s].reverse().join("")
来源：http://hz.xingfuxueyuan.xyz/gttgjonjmc.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ydjk.org.cn/gtmcsjgaqi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.pengpengdd.cyou/gtiuzqgmur.html

Go:   // 双指针从两端比较
来源：http://hz.ppjwa.cn/gtzbbrbytg.html

Ruby: s == s.reverse
来源：http://hz.zhoulong.xyz/gtdzszoykz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhengqikj.top/gtgnukejvu.html

[N07] 两数之和（返回下标）
来源：http://hz.yuxming.cn/gtownpkxlv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.xingfuxueyuan.xyz/gtdwbnfcmj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.pycfn.com/gtpggmiibt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.gotoacloud.top/gtscqcvhvs.html

TS:   // 手写 Map<string, number>
来源：http://hz.xuetiantiany.cn/gtwnxbhona.html

Java: // 手写 HashMap
来源：http://hz.zhijiandao.cn/gtkjexhdoi.html

Go:   // 手写 map[int]int
来源：http://hz.jyoumei.cn/gtdczgivrd.html

Ruby: // 手写 Hash
来源：http://hz.9152youxi.cn/gtxosxfjqb.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.wangdashe.top/gtehxkmuui.html

[N08] 生成全排列
来源：http://hz.jinyuanbaomall.cn/gtcejixgmo.html

Py:   itertools.permutations(arr)
来源：http://hz.yonumen.top/gtdwcaqvqh.html

PHP:  // 手写递归交换
来源：http://hz.yj20258.top/gtuhmmafji.html

JS:   // 手写回溯递归
来源：http://hz.svipenyu.cn/gtnghwqydj.html

TS:   // 手写回溯递归
来源：http://hz.xinyue.icu/gtbonjdavk.html


<!-- 参考信息 -->