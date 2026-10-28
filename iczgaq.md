代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hnxiangtu.top/gtduoqbhmh.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jinqigufen.top/gthuvaaxsw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jinqigufen.top/gtvztwuxfv.html

[J10] 取今天 / 本月第一天
来源：http://hz.birdmap.top/gtijrxnhuk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shanyushiyangkeji.top/gtfuviaovy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yvedp.cn/gtikbavwmd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.316326.xyz/gtvoiirses.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yuanzhike.top/gtnjlsaibi.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.sufxvd.cn/gtkypqbpvc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.pycfn.com/gthlutjgej.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.nwbrower.top/gtwvrqwonu.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.meibo888.top/gtrzvfgplh.html

================================================================================
来源：http://hz.jinqigufen.top/gtcexhkuvl.html

K. JSON 与序列化
来源：http://hz.bjfxy.top/gtglqinmdu.html

================================================================================
来源：http://hz.gzhubu.top/gtwszezbgm.html

[K01] 对象转 JSON 字符串
来源：http://hz.9152youxi.cn/gtzmhmekws.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.tian-w.cn/gtsttmmgsg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.fzhhl.top/gttnrlwrrl.html

JS:   JSON.stringify(obj)
来源：http://hz.jlsjyb.cn/gtdkihlyxz.html

TS:   JSON.stringify(obj)
来源：http://hz.xziqi.cn/gthflgrard.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yvedp.cn/gtbpgprcnm.html

Go:   json.Marshal(obj)
来源：http://hz.dianchejie.cn/gtdgcropsd.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hywenlv.cn/gtkhfwuzth.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ydzc1.top/gtqfmrarvm.html

[K02] JSON 字符串转对象
来源：http://hz.jinqigfzy.top/gtfrtqixkp.html

Py:   json.loads(s)
来源：http://hz.cdnleiting.top/gtnxbjaifr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.bjfxy.top/gtrpeciius.html

JS:   JSON.parse(s)
来源：http://hz.shanyushiyangkeji.top/gtvfkyeyvs.html

TS:   JSON.parse(s)
来源：http://hz.smart0.xyz/gtnldliktf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.ppjwa.cn/gtinrxqcqu.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ehwqpu.com/gtaqwamfig.html

Ruby: JSON.parse(s)
来源：http://hz.shuidangran.top/gthirwrytq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hammf.cn/gtcolzcuqj.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.sysykeji.top/gtaoyhjely.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.gzhubu.top/gtzrloegah.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.nwbrower.top/gtbpkbejiy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.meibo888.top/gtwyqwxuti.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.nanxuanxn.top/gtarfvzcby.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yangfankeji.com/gtgnutckyv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.shanyushiyangtech.top/gtmdhmilxc.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yuanzhike.top/gtfazdkqkp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.wangshuangyany.cn/gtzefiegbn.html

[K04] 读取 JSON 文件
来源：http://hz.mhx1999.top/gtogbaojhj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jqgfzy.top/gttcitiqos.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cashguo.top/gtrkfxrleh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cashguo.top/gtnqiufdfq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.svipenyu.cn/gtpmcxdtpw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.cashguo.top/gtrwowjswq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yongpay.top/gtrzmxdqia.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hysaishi.cn/gtpzldnfiu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ybcxt.top/gteilfdvwg.html

[K05] 深拷贝对象
来源：http://hz.sweek.top/gtgfccpcox.html

Py:   copy.deepcopy(obj)
来源：http://hz.cdnleiting.top/gtoswmhbmo.html

PHP:  unserialize(serialize($obj));
来源：http://hz.wangshuangyany.cn/gtovwrqfxv.html

JS:   structuredClone(obj)
来源：http://hz.mhx1999.top/gtydvewixg.html

TS:   structuredClone(obj)
来源：http://hz.xuetiantiany.cn/gtsilqhupg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.sufxvd.cn/gtztgjcsoh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.aizwys.cn/gtvamrgzbx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yj20258888.top/gtqucziprv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.xingfuxueyuan.xyz/gtrtbpukeg.html

[K06] 解析 URL 查询串
来源：http://hz.dashuyun.cn/gtptxoazqq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.52xcode.cn/gtvrmgvmpw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.cdnleiting.top/gtwttdvzqr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gotoacloud.top/gtcxuirfkc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.haohaochexian.top/gtybzuhmbb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.9152youxi.cn/gtbxuewbmj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.aizwys.cn/gteylmuzzd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.0kj1m.cn/gthgbpizzg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.sxryk.cn/gtwrgrmllx.html

[K07] 进制转换
来源：http://hz.tanke756.top/gtqwcvsqay.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.tianlin.xyz/gtdalfukpj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.fengsongda.top/gtrwdlmdsw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.tianlin.xyz/gtenmuvkbr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.xinyue.icu/gtdrmivpxj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.kuanghao11.cn/gtaxoreenb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.birdmap.top/gtefsphqwr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.shanyushiyangkeji.top/gtjxkveqik.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.guowangkeji.top/gttejtxluu.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jinqigufen.top/gtvsxvkeex.html

Py:   pickle.dumps(obj)
来源：http://hz.hongshengwenyu.top/gtopzfzmpd.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jinyuanbaomall.cn/gtfdldkxsd.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yj202588.top/gtkdsxiyhk.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yuanzhike.top/gtaqsrokkb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jqgfzy.top/gtosadluvn.html

Go:   encoding/gob
来源：http://hz.daxiang520.top/gtvndxrggd.html

Ruby: Marshal.dump(obj)
来源：http://hz.sysykeji.top/gtpavcjrve.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.316326.xyz/gtbsidrton.html

================================================================================
来源：http://hz.jianghu66.top/gtahdrucgs.html

L. 网络请求
来源：http://hz.snrcjt.cn/gtsvkamkfx.html

================================================================================
来源：http://hz.nanxuanxn.top/gtuoseebzg.html

[L01] 发送 GET 请求
来源：http://hz.jinyuanbaomall.cn/gtktydroba.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.mhx1999.top/gtnpftxflx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ivvv.top/gtkvhzqzsl.html

JS:   await fetch(url)
来源：http://hz.gotoacloud.top/gthnvyzdej.html

TS:   await fetch(url)
来源：http://hz.zhengqikj.top/gtwpcgqbeo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.fzhhl.top/gtnltwvlhb.html

Go:   resp, err := http.Get(url)
来源：http://hz.havefunace.top/gtlqqizsgy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.tian-w.cn/gtlxgkynhs.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.cqqwz.cn/gtzkbqshnt.html

[L02] 发送 POST JSON
来源：http://hz.zhiwuduotai.top/gtzykamnak.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.smart0.xyz/gtyewnrivh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.dianchejie.cn/gtvbmkjxej.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.fengsongda.top/gtweytrjew.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sxryk.cn/gtutdlyvds.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.feifeiyinyue.top/gtthozwzac.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.c1oappe.top/gtdvxwebuw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jiagoushi.top/gtkgxexuno.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yvedp.cn/gtmhnuaugf.html

[L03] 设置自定义请求头
来源：http://hz.tian-w.cn/gtlavlripe.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhoulong.xyz/gtgzocyhuz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.sxryk.cn/gtvljkclbx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.vqdsnc.cn/gtqoxduqgm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ywan-chungtsiang.top/gtnrcoqybb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ydjk.org.cn/gtzafwvqou.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.shanyushiyangkeji.top/gtsacrjkcl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yuanzhike.top/gtyyqtshhf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.tianlin.xyz/gtgnlfatpr.html

[L04] 设置超时
来源：http://hz.birdmap.top/gtexuyomdh.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ydjk.org.cn/gtcalvermw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.xuetiantiany.cn/gthohjwczj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.redwolf501.top/gtnimrtqic.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hywenlv.cn/gtyjzdzbfo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.pengpengdd.cyou/gtflqbbnwu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yonumen.top/gtmueumzzj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.gaohongyu789.top/gtreynxkxg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.nwbrower.top/gttvtftqvo.html

[L05] 上传文件（multipart）
来源：http://hz.bjfxy.top/gtimkdbxos.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yuanzhike.top/gtzctuvtib.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.chenzaomai.com/gtpjlpgyad.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hnqzz.top/gtkdgbhyjg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.aibaodan.cn/gtbaahmxfw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zdqjudy.top/gtfbkavrdt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.hnxiangtu.top/gtcjcwzkut.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.daria6918.cn/gtfpejkvfp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yueranfly.top/gtklrihrke.html

[L06] 解析响应为 JSON
来源：http://hz.zhijiandao.cn/gtjkznzxri.html

Py:   resp.json()
来源：http://hz.ppjwa.cn/gtzdjaxkox.html

PHP:  json_decode($body, true);
来源：http://hz.jinqigufen.top/gtdagpagdm.html

JS:   await resp.json()
来源：http://hz.tian-w.cn/gtnerrqwnh.html

TS:   await resp.json()
来源：http://hz.chenlongwang.top/gtecxdmcvs.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.aibaodan.cn/gtynnjrcjj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xziqi.cn/gtxeyitsok.html

Ruby: JSON.parse(resp.body)
来源：http://hz.nwbrower.top/gtvqhmwnsq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.sufxvd.cn/gtugvhgvnq.html

[L07] 处理 HTTP 状态码
来源：http://hz.tanke756.top/gtzkbmhhoa.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.tanke756.top/gtltbmmyrr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hammf.cn/gttuehvjwb.html

JS:   resp.ok;  resp.status
来源：http://hz.kuanghao11.cn/gtlyibwjwe.html

TS:   resp.ok;  resp.status
来源：http://hz.sysykeji.top/gtzegbcnkr.html

Java: resp.statusCode()
来源：http://hz.zhiwuduotai.top/gtpgnhsyfl.html

Go:   resp.StatusCode
来源：http://hz.nanxinkj.top/gtcnxcpefr.html

Ruby: resp.code.to_i
来源：http://hz.tian-w.cn/gtubfvvewe.html

C#:   (int)resp.StatusCode
来源：http://hz.chenlongwang.top/gtqbfpwkmh.html

[L08] 并发请求多个地址
来源：http://hz.hnxiangtu.top/gtdquujjin.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yuxming.cn/gtcrmsehex.html

PHP:  curl_multi_init() 系列
来源：http://hz.316326.xyz/gthmxyuawx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cqqwz.cn/gtsfmddspb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xziqi.cn/gtgnfcskcg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.kuanghao11.cn/gtrrzyrtlm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yongpay.top/gtglvwkbqg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jinghuilouyu.cn/gtfseykxml.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.316326.xyz/gtfvoulmzq.html

================================================================================
来源：http://hz.sufxvd.cn/gtbyrltrij.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhijiandao.cn/gtcjryjjrb.html

================================================================================
来源：http://hz.wangdashe.top/gtkafuloyi.html

[M01] 读取命令行参数
来源：http://hz.zycfv.cn/gtslzbgdrc.html

Py:   sys.argv[1:]
来源：http://hz.yongpay.top/gtuloudaqq.html

PHP:  $argv;  $argc;
来源：http://hz.gaohongyu789.top/gtdfjawhro.html

JS:   process.argv.slice(2)
来源：http://hz.wangdashe.top/gtmsehypac.html

TS:   process.argv.slice(2)
来源：http://hz.xylfe.cn/gtcldyldfe.html

Java: args 数组（main 方法参数）
来源：http://hz.yuanzhike.top/gtqezbqiej.html

Go:   os.Args[1:]
来源：http://hz.tanke756.top/gtjdffkyqs.html

Ruby: ARGV
来源：http://hz.fzhhl.top/gtrpwhqcyf.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yueranfly.top/gtzsodbpsd.html

[M02] 读取环境变量
来源：http://hz.cucudq.cn/gtcznhmmbm.html

Py:   os.environ.get("HOME")
来源：http://hz.guowangkeji.top/gtjjamzegw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yangfankeji.com/gtkemjawyw.html

JS:   process.env.HOME
来源：http://hz.shuidangran.top/gtenjbexoe.html

TS:   process.env.HOME
来源：http://hz.jianghu66.top/gtblgfiinl.html

Java: System.getenv("HOME")
来源：http://hz.zhengqikj.top/gtiwktxtpw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.snrcjt.cn/gtmptlrfzb.html

Ruby: ENV["HOME"]
来源：http://hz.hammf.cn/gthatzvril.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.cashguo.top/gtevbzukhz.html

[M03] 执行外部命令
来源：http://hz.hammf.cn/gtfoansweh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.cucudq.cn/gtrizwqiim.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.0kj1m.cn/gtcwfcuolv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.chenlongwang.top/gtlamswipn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yj20258888.top/gtrzqevoor.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jinyuanbaomall.cn/gtptivldpo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hammf.cn/gttvndtkff.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.xziqi.cn/gtcmmhxtun.html

C#:   Process.Start("ls", "-l");
来源：http://hz.shanyushiyangkeji.top/gtkqveyssn.html

[M04] 获取当前工作目录
来源：http://hz.cucudq.cn/gtfkthxiyd.html

Py:   os.getcwd()
来源：http://hz.nanxinkj.top/gtwbhrfsdj.html

PHP:  getcwd();
来源：http://hz.sxryk.cn/gtqaymddlk.html

JS:   process.cwd()
来源：http://hz.yuanzhike.top/gtaadgjcnq.html

TS:   process.cwd()
来源：http://hz.zhongyouzk.top/gtnblulotr.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.haohaochexian.top/gtazcsodie.html

Go:   os.Getwd()
来源：http://hz.9152youxi.cn/gtezxkgjsz.html

Ruby: Dir.pwd
来源：http://hz.zhiwuduotai.top/gtzudqzour.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hysaishi.cn/gtfexbleyj.html

[M05] 设置退出码
来源：http://hz.ydjk.org.cn/gtyjpobkyg.html

Py:   sys.exit(1)
来源：http://hz.ivvv.top/gtitupwewj.html

PHP:  exit(1);
来源：http://hz.ppjwa.cn/gtjidbtuwf.html

JS:   process.exit(1)
来源：http://hz.jqgfzy.top/gtshnxjogv.html

TS:   process.exit(1)
来源：http://hz.redwolf501.top/gtrlqmvocr.html

Java: System.exit(1)
来源：http://hz.jqgufenzy.top/gtnlcybizr.html

Go:   os.Exit(1)
来源：http://hz.jinqigfzy.top/gtgresnywt.html

Ruby: exit 1
来源：http://hz.vqdsnc.cn/gtmxrhwgeg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.hammf.cn/gtmfbrnsef.html

[M06] 向标准错误输出
来源：http://hz.shzxlz.cn/gtnkiwlbaf.html

Py:   print("err", file=sys.stderr)
来源：http://hz.pengpengdd.cyou/gthwaidinr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yonumen.top/gtfnlckcbs.html

JS:   console.error("err")
来源：http://hz.gzhubu.top/gtzddellee.html

TS:   console.error("err")
来源：http://hz.jinghuilouyu.cn/gtuckpqlic.html

Java: System.err.println("err")
来源：http://hz.xziqi.cn/gtnrprgcxg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.nwbrower.top/gteqlqpvrq.html

Ruby: warn "err"
来源：http://hz.pengpengdd.cyou/gtzpzxcefa.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.shanyushiyangkeji.top/gthzanfiyy.html

[M07] 判断是否为主入口
来源：http://hz.feifeiyinyue.top/gtokhomjwk.html

Py:   if __name__ == "__main__":
来源：http://hz.aibaodan.cn/gttfdwgjew.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.9152youxi.cn/gtdtfaurlx.html

JS:   require.main === module
来源：http://hz.sufxvd.cn/gtuohqtqcs.html

TS:   require.main === module
来源：http://hz.xingfuxueyuan.xyz/gtdguomdrc.html

Java: public static void main(String[] args)
来源：http://hz.yanxiufei.cn/gtjojggfri.html

Go:   func main()
来源：http://hz.nanxuanxn.top/gtdcdlrmtj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhoulong.xyz/gtvemaiyin.html

C#:   static void Main(string[] args)
来源：http://hz.zhijiandao.cn/gtkbaxdsfp.html

[M08] 获取系统与运行时信息
来源：http://hz.jinqigufen.top/gteerbpzxn.html

Py:   platform.system();  platform.python_version()
来源：http://hz.cashguo.top/gtuboyxzki.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ybcxt.top/gtcmlitklr.html

JS:   process.platform;  process.version
来源：http://hz.sxryk.cn/gtygehylkj.html

TS:   process.platform;  process.version
来源：http://hz.daxiang520.top/gtwzpwjwut.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yuxming.cn/gtijwgydkm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.svipenyu.cn/gtunjzbpnx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ydjk.org.cn/gtbyuqcisv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jyoumei.cn/gtlbbgunvs.html

================================================================================
来源：http://hz.haohaochexian.top/gtazpftith.html

N. 数据结构与算法
来源：http://hz.jlsjyb.cn/gtzwlfxgoo.html

================================================================================
来源：http://hz.redwolf501.top/gttxnwfwum.html

[N01] 二分查找（有序数组）
来源：http://hz.xuanzx.com/gthsadqvys.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jianghu66.top/gtbpiipqqm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.0kj1m.cn/gtbjogzugu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yangfankeji.com/gthdespauv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhixingplan.top/gtrrobcyll.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.daxiang520.top/gtvumbvejd.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ydzc1.top/gtcvcywort.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.meibo888.top/gtqurqtqtg.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.aizwys.cn/gtbhqbkktt.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yuxming.cn/gtlfvpvruj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.aizwys.cn/gtpcgygqyx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.cdnleiting.top/gtyueylksu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cashguo.top/gtdgxgfize.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zycfv.cn/gtecjocoqh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jqgfzy.top/gtgdfivnzk.html

Go:   slices.Sort(arr)
来源：http://hz.9152youxi.cn/gtocismtlz.html

Ruby: arr.sort
来源：http://hz.zycfv.cn/gtitttrshh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.guowangkeji.top/gtaikxeikr.html

[N03] 快速排序（分治示例）
来源：http://hz.sysykeji.top/gtuycxcgtw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.sufxvd.cn/gtbwvrpbok.html

PHP:  // 递归实现，或用 usort
来源：http://hz.snrcjt.cn/gtufueynvc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nanxinkj.top/gtufzfgfjk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.c1oappe.top/gtpqumszsr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.cheryme.top/gtbxctrxjs.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jianghu66.top/gtrhiuwfez.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yj20258888.top/gtplpapkbq.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.haohaochexian.top/gtlrmjcwpo.html

[N04] 斐波那契数列
来源：http://hz.shuidangran.top/gtlirjtgzq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hongshengwenyu.top/gtfikczmul.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jinqigfzy.top/gtheqzsneq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.0kj1m.cn/gtvdiltrxd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jlsjyb.cn/gtyyvwwvov.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.tian-w.cn/gtgyhafwsp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ywan-chungtsiang.top/gtxiyhycfv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yj20258888.top/gtmlcomaqb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.shuidangran.top/gtmbusfsjd.html

[N05] 最大公约数
来源：http://hz.ydzc1.top/gtnpchzoro.html

Py:   math.gcd(a, b)
来源：http://hz.yj202588.top/gtqqvnplhe.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.iojbl.cn/gtyhbdegnf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.svipenyu.cn/gtwwcdlkxl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.aizwys.cn/gtjjipkkqb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.snrcjt.cn/gtbhzvrzng.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.chenzaomai.com/gtbjmiesfg.html

Ruby: a.gcd(b)
来源：http://hz.chenzaomai.com/gtipfdhvzx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zycfv.cn/gtxcvcbawu.html

[N06] 判断回文字符串
来源：http://hz.zhiwuduotai.top/gtbykatwrv.html

Py:   s == s[::-1]
来源：http://hz.tian-w.cn/gtmwrgfspv.html

PHP:  $s === strrev($s);
来源：http://hz.xingfuxueyuan.xyz/gtneansbtr.html

JS:   s === [...s].reverse().join("")
来源：http://hz.pycfn.com/gtrbzlcviy.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zhoulong.xyz/gtoizjzwcu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.cqqwz.cn/gtmvgjchug.html

Go:   // 双指针从两端比较
来源：http://hz.yj20258888.top/gtdmgeeabx.html

Ruby: s == s.reverse
来源：http://hz.haohaochexian.top/gtjzrvjwry.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.birdmap.top/gtfpmxfdyx.html

[N07] 两数之和（返回下标）
来源：http://hz.birdmap.top/gtrryapefd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yvedp.cn/gtnaqvovpe.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jyoumei.cn/gtebghmzgh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.cheryme.top/gtedwnezeb.html

TS:   // 手写 Map<string, number>
来源：http://hz.hysaishi.cn/gtearpkhni.html

Java: // 手写 HashMap
来源：http://hz.iojbl.cn/gtyqcfdnrb.html


<!-- 参考信息 -->