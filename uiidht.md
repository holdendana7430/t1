代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.feifeiyinyue.top/gtnmgzarkr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.cucudq.cn/gtdpjyeokc.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.nwbrower.top/gtqkpbzyik.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yongpay.top/gtayxvazot.html

================================================================================
来源：http://hz.cdnleiting.top/gtaqfgoadf.html

K. JSON 与序列化
来源：http://hz.jqgfzy.top/gtioyihvig.html

================================================================================
来源：http://hz.0kj1m.cn/gtlotkoeby.html

[K01] 对象转 JSON 字符串
来源：http://hz.yuanzhike.top/gtjqhlnzya.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jqgfzy.top/gtbqrgezrs.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.guowangkeji.top/gttwlfpfcc.html

JS:   JSON.stringify(obj)
来源：http://hz.chenjidiqi.icu/gtsbtpcqmp.html

TS:   JSON.stringify(obj)
来源：http://hz.ybcxt.top/gtinxvfulu.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.aizwys.cn/gtsvrjyjxn.html

Go:   json.Marshal(obj)
来源：http://hz.cheryme.top/gttnspusjx.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.havefunace.top/gtirhtbsbl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.shanyushiyangkeji.top/gtogvcbjqg.html

[K02] JSON 字符串转对象
来源：http://hz.havefunace.top/gtknmrrpbg.html

Py:   json.loads(s)
来源：http://hz.cashguo.top/gtqlitctra.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.guowangkeji.top/gtbavlcfun.html

JS:   JSON.parse(s)
来源：http://hz.yonumen.top/gtbkvcjdjs.html

TS:   JSON.parse(s)
来源：http://hz.hammf.cn/gtffdkocoh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jqgufenzy.top/gtdaxdpdim.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.bjfxy.top/gtsxasonpd.html

Ruby: JSON.parse(s)
来源：http://hz.xuanzx.com/gtmitjrgra.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.smart0.xyz/gtemqioaxq.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.shzxlz.cn/gtmgqkgavh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xuetiantiany.cn/gtczhrprtc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.haohaochexian.top/gteufsklbk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shanyushiyangkeji.top/gtvvezvufx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jqgfzy.top/gtchanywaw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ydzc1.top/gtoyzwnqyl.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ehwqpu.com/gttyxjgsuk.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zycfv.cn/gtbbbyqyag.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.0kj1m.cn/gtjrcgpzrb.html

[K04] 读取 JSON 文件
来源：http://hz.xziqi.cn/gtxcqbmded.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yanxiufei.cn/gtdezarrtt.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.bjfxy.top/gthvcqovdm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.9152youxi.cn/gtpkdkulpd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hnqzz.top/gtmhgvqzjd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.birdmap.top/gtsoivuhxl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.aizwys.cn/gtkxfvvdix.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.chenjidiqi.icu/gtgicnlsqs.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.sweek.top/gtdcsqigat.html

[K05] 深拷贝对象
来源：http://hz.hysaishi.cn/gttffvsjcb.html

Py:   copy.deepcopy(obj)
来源：http://hz.shanyushiyangkeji.top/gttjwbmhkp.html

PHP:  unserialize(serialize($obj));
来源：http://hz.shangyingyoupin.top/gtecxiigio.html

JS:   structuredClone(obj)
来源：http://hz.xylfe.cn/gtgdoveoki.html

TS:   structuredClone(obj)
来源：http://hz.yvedp.cn/gtmjijwowu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.gogol.net.cn/gtjwpnnjsv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.52xcode.cn/gtjszpcwps.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xinyue.icu/gtynhffdvr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.mhx1999.top/gtztihrkup.html

[K06] 解析 URL 查询串
来源：http://hz.shzxlz.cn/gttcrgynmo.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.nanxuanxn.top/gtfcifjxoj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jianghu66.top/gtyrbdbgtv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.aibaodan.cn/gtyuqtawyn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.chenzaomai.com/gtcmgglclu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.nanxinkj.top/gtbopsemoa.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jianghu66.top/gtzqytouyh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ivvv.top/gtzvxdfwdx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cheryme.top/gtpvvjwjox.html

[K07] 进制转换
来源：http://hz.jianghu66.top/gtripjvfqu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhijiandao.cn/gtzgcuxpgx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.bjfxy.top/gtotqhkisi.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hongshengwenyu.top/gtyzfwwatk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jinqigufen.top/gtwwybooej.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.meibo888.top/gtgtqrzazk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.smart0.xyz/gtugwinoed.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.meibo888.top/gtadsopxqh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yuanzhike.top/gtuocomzdc.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jlsjyb.cn/gthqlhxorx.html

Py:   pickle.dumps(obj)
来源：http://hz.hfpthk.cn/gtwseoegph.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.gaohongyu789.top/gtdomtergs.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jiagoushi.top/gtpnwxmssq.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jianghu66.top/gtdrtjkhor.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.wangshuangyany.cn/gtfzrtnpba.html

Go:   encoding/gob
来源：http://hz.hysaishi.cn/gtoadbjaux.html

Ruby: Marshal.dump(obj)
来源：http://hz.guannengcc.top/gtfrqdtuhy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhoulong.xyz/gtejgrgkma.html

================================================================================
来源：http://hz.daxiang520.top/gtzozrhmuc.html

L. 网络请求
来源：http://hz.sxryk.cn/gtrorkvwzi.html

================================================================================
来源：http://hz.chenzaomai.com/gtcdfyonjw.html

[L01] 发送 GET 请求
来源：http://hz.nanxuanxn.top/gtrgfjugbi.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.guannengcc.top/gtmrzqcpvq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hammf.cn/gtfqcizirv.html

JS:   await fetch(url)
来源：http://hz.svipenyu.cn/gtobfyrmuh.html

TS:   await fetch(url)
来源：http://hz.ydzc1.top/gtzzkfgfow.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.iojbl.cn/gtblqplmis.html

Go:   resp, err := http.Get(url)
来源：http://hz.fzhhl.top/gtkxeeywdl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.shanyushiyangkeji.top/gtmkbflmcv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.nanxinkj.top/gtdlcddica.html

[L02] 发送 POST JSON
来源：http://hz.hnxiangtu.top/gtgvlvmcwf.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.gzhubu.top/gtvfdvwwzc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.andypj.xyz/gtpglqxlfk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhixingplan.top/gtfkpsevnw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yuxming.cn/gtpgqeiwac.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yangfankeji.com/gtfthkmkug.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yonumen.top/gtosmhbaac.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.c1oappe.top/gtqfmvsank.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jianghu66.top/gtvihvorei.html

[L03] 设置自定义请求头
来源：http://hz.hnxiangtu.top/gtsopvpmjc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.sufxvd.cn/gtjbzmxbln.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.xingfuxueyuan.xyz/gtirkqzidd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sxryk.cn/gtqnoqmvge.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ywan-chungtsiang.top/gtpnovrvpu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ppjwa.cn/gthsuicnkj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.xinyue.icu/gtpgarvtjo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.tanke756.top/gtvtmmsgfv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.daxiang520.top/gthcpcyoyp.html

[L04] 设置超时
来源：http://hz.snrcjt.cn/gtquxcljdu.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yonumen.top/gtfjqszdsz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jqgufenzy.top/gttuxobrrz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.9152youxi.cn/gtwuqofoaz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.redwolf501.top/gtvypudnyw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.9152youxi.cn/gtowhlvzxj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.birdmap.top/gtnattejzp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xuetiantiany.cn/gtnktjhifx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.svipenyu.cn/gteleivrki.html

[L05] 上传文件（multipart）
来源：http://hz.kuanghao11.cn/gtqnuswbze.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.tanke756.top/gtvihmbwyn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.pengpengdd.cyou/gtwshoxfrp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yangfankeji.com/gtphnztjxj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.snrcjt.cn/gtsdyrqdtn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ybcxt.top/gtprjhoeec.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.feifeiyinyue.top/gtoddstmyl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jlsjyb.cn/gtmmqoohgk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.gzhubu.top/gtcfacoqmo.html

[L06] 解析响应为 JSON
来源：http://hz.yj202588.top/gtlimypgmk.html

Py:   resp.json()
来源：http://hz.havefunace.top/gtrrhfjxuw.html

PHP:  json_decode($body, true);
来源：http://hz.0kj1m.cn/gtcfjemdzy.html

JS:   await resp.json()
来源：http://hz.guowangkeji.top/gtbhvwecyi.html

TS:   await resp.json()
来源：http://hz.xingfuxueyuan.xyz/gtyibrzkne.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.nanxinkj.top/gtwzrxegxa.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.nanxuanxn.top/gtoeikdgcx.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhixingplan.top/gtirgonaed.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.wangdashe.top/gtpnxdsiaw.html

[L07] 处理 HTTP 状态码
来源：http://hz.smart0.xyz/gtwjkxuiit.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.aibaodan.cn/gtlicddvrq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.xziqi.cn/gtfniyeosj.html

JS:   resp.ok;  resp.status
来源：http://hz.jianghu66.top/gtcaztgkrl.html

TS:   resp.ok;  resp.status
来源：http://hz.zycfv.cn/gtictswevh.html

Java: resp.statusCode()
来源：http://hz.jinghuilouyu.cn/gtjkhnjzoi.html

Go:   resp.StatusCode
来源：http://hz.guowangkeji.top/gtdwqmrntc.html

Ruby: resp.code.to_i
来源：http://hz.meibo888.top/gtwwzacopq.html

C#:   (int)resp.StatusCode
来源：http://hz.tian-w.cn/gtmlcxjsgj.html

[L08] 并发请求多个地址
来源：http://hz.daria6918.cn/gtlobihbve.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jinqigfzy.top/gtijrwpxwm.html

PHP:  curl_multi_init() 系列
来源：http://hz.shanyushiyangtech.top/gtckvxlrhy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.aizwys.cn/gtbobzxfsc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.dashuyun.cn/gtuedgxgvy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.cheryme.top/gtoyqiicrw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hysaishi.cn/gtztinzein.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yj20258888.top/gtiykhuhkg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yj20258.top/gtqyfukyzw.html

================================================================================
来源：http://hz.zhixingplan.top/gtsusmksya.html

M. 命令行 / 进程 / 环境
来源：http://hz.yonumen.top/gtihjnduef.html

================================================================================
来源：http://hz.chenlongwang.top/gtsdwekxan.html

[M01] 读取命令行参数
来源：http://hz.iojbl.cn/gtsyhqsetf.html

Py:   sys.argv[1:]
来源：http://hz.tian-w.cn/gtvvrpdnng.html

PHP:  $argv;  $argc;
来源：http://hz.ydzc1.top/gtarukkhar.html

JS:   process.argv.slice(2)
来源：http://hz.tanke756.top/gtudigqacy.html

TS:   process.argv.slice(2)
来源：http://hz.nanxinkj.top/gtbhsdjymn.html

Java: args 数组（main 方法参数）
来源：http://hz.guowangkeji.top/gtgovgbwud.html

Go:   os.Args[1:]
来源：http://hz.yanxiufei.cn/gtragnfjpo.html

Ruby: ARGV
来源：http://hz.zhiwuduotai.top/gtuzxemnvc.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ydjk.org.cn/gtsirneigh.html

[M02] 读取环境变量
来源：http://hz.hysaishi.cn/gtcgoibipb.html

Py:   os.environ.get("HOME")
来源：http://hz.cucudq.cn/gtpvadadyq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.gotoacloud.top/gtthggohty.html

JS:   process.env.HOME
来源：http://hz.pycfn.com/gtziyeihjf.html

TS:   process.env.HOME
来源：http://hz.zhongyouzk.top/gtbcdpjlgf.html

Java: System.getenv("HOME")
来源：http://hz.wangdashe.top/gtsbiylepn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.sufxvd.cn/gtqwphigvq.html

Ruby: ENV["HOME"]
来源：http://hz.meibo888.top/gtjkqedrwg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.feifeiyinyue.top/gtwgiuygwp.html

[M03] 执行外部命令
来源：http://hz.cqqwz.cn/gtpkzadhah.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.52xcode.cn/gtjkynivji.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yuanzhike.top/gtflatkqhj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yongpay.top/gtastnoaek.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zdqjudy.top/gtylkwqhut.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.xziqi.cn/gtdbigrcfj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.xziqi.cn/gtfajttsgy.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.nanxinkj.top/gtdhtqgqzu.html

C#:   Process.Start("ls", "-l");
来源：http://hz.nanxuanxn.top/gtuiubicqc.html

[M04] 获取当前工作目录
来源：http://hz.chenzaomai.com/gtvootykdm.html

Py:   os.getcwd()
来源：http://hz.ppjwa.cn/gtsxzosxsi.html

PHP:  getcwd();
来源：http://hz.mhx1999.top/gtrxzaucni.html

JS:   process.cwd()
来源：http://hz.yanxiufei.cn/gtsiyidems.html

TS:   process.cwd()
来源：http://hz.xinyue.icu/gtnfupzrbb.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.sweek.top/gtcqdrthcd.html

Go:   os.Getwd()
来源：http://hz.kuanghao11.cn/gtshsnygbg.html

Ruby: Dir.pwd
来源：http://hz.tanke756.top/gtnibulhck.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.nwbrower.top/gtjoivdvnh.html

[M05] 设置退出码
来源：http://hz.redwolf501.top/gtfsidgesg.html

Py:   sys.exit(1)
来源：http://hz.jiagoushi.top/gtcruocznr.html

PHP:  exit(1);
来源：http://hz.ydjk.org.cn/gtwrsvihng.html

JS:   process.exit(1)
来源：http://hz.tian-w.cn/gtipxissse.html

TS:   process.exit(1)
来源：http://hz.zycfv.cn/gtmrxdviti.html

Java: System.exit(1)
来源：http://hz.nanxuanxn.top/gtrlinwpnp.html

Go:   os.Exit(1)
来源：http://hz.yvedp.cn/gtuhqmoukf.html

Ruby: exit 1
来源：http://hz.yonumen.top/gtkskgupzy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.316326.xyz/gtelfrcpec.html

[M06] 向标准错误输出
来源：http://hz.yj202588.top/gtszeiawrl.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ppjwa.cn/gtxzgobnbj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.redwolf501.top/gtvgrywnoe.html

JS:   console.error("err")
来源：http://hz.xinyue.icu/gtgizfvvwj.html

TS:   console.error("err")
来源：http://hz.zycfv.cn/gtinmownuz.html

Java: System.err.println("err")
来源：http://hz.xingfuxueyuan.xyz/gtnuvcvxqz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yongpay.top/gtstsjnvhr.html

Ruby: warn "err"
来源：http://hz.mhx1999.top/gtjvltophz.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.dianchejie.cn/gtkkntxhlt.html

[M07] 判断是否为主入口
来源：http://hz.nanxinkj.top/gtugprwvmi.html

Py:   if __name__ == "__main__":
来源：http://hz.sxryk.cn/gttwjksxtr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.redwolf501.top/gtdrqnmsxy.html

JS:   require.main === module
来源：http://hz.nwbrower.top/gturwficqj.html

TS:   require.main === module
来源：http://hz.jinghuilouyu.cn/gtjjapyipv.html

Java: public static void main(String[] args)
来源：http://hz.0kj1m.cn/gtngklxgpe.html

Go:   func main()
来源：http://hz.zdqjudy.top/gtapekegmj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.quarkkingdee.top/gtdvxehkhi.html

C#:   static void Main(string[] args)
来源：http://hz.jiagoushi.top/gtczxgzjcb.html

[M08] 获取系统与运行时信息
来源：http://hz.cucudq.cn/gtvvqoqlye.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yueranfly.top/gtrophcnbl.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jinqigfzy.top/gtvlvmfbbz.html

JS:   process.platform;  process.version
来源：http://hz.sxryk.cn/gtrsvjeffb.html

TS:   process.platform;  process.version
来源：http://hz.vqdsnc.cn/gtipeyjtuf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.gaohongyu789.top/gtnlgshwes.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.52xcode.cn/gtrcfaycvl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.aibaodan.cn/gteyonbtwo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hnxiangtu.top/gtyulxosgy.html

================================================================================
来源：http://hz.daria6918.cn/gtxxjzamck.html

N. 数据结构与算法
来源：http://hz.zhaomingkeji.xyz/gtduukliry.html

================================================================================
来源：http://hz.xylfe.cn/gthpmlzgoh.html

[N01] 二分查找（有序数组）
来源：http://hz.9152youxi.cn/gtbihrhiwo.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xziqi.cn/gtrgwxixhv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.dianchejie.cn/gtbzrjaqny.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yj20258888.top/gtybhhvktb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sxryk.cn/gtpzqdygeo.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jqgufenzy.top/gtuncpiayc.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jqgufenzy.top/gtpgvonnwl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.birdmap.top/gtyjpmpplf.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zhoulong.xyz/gtxnmhgjif.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhaomingkeji.xyz/gtbfqaaxxt.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shanyushiyangkeji.top/gthbedkgkb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.snrcjt.cn/gteqqddqsq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hnqzz.top/gtyxiepmdg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hongshengwenyu.top/gtmmyiurzw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hfpthk.cn/gtxtnftann.html

Go:   slices.Sort(arr)
来源：http://hz.zhengqikj.top/gtvjujygbl.html

Ruby: arr.sort
来源：http://hz.guannengcc.top/gtmfzzcyop.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhiwuduotai.top/gtxubgkcwi.html

[N03] 快速排序（分治示例）
来源：http://hz.zhaomingkeji.xyz/gtfsfmemkq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zycfv.cn/gtsfkvwdvo.html

PHP:  // 递归实现，或用 usort
来源：http://hz.ywan-chungtsiang.top/gtwwtjpjsn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ywan-chungtsiang.top/gtsojfuqpo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nanxinkj.top/gtwpgkubxd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jlsjyb.cn/gtpehnctkx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.wangdashe.top/gthykmsfkf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ywan-chungtsiang.top/gtgnrqobsc.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yj20258.top/gtlhnwyyvx.html

[N04] 斐波那契数列
来源：http://hz.yonumen.top/gtygqlbfba.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.sweek.top/gtfbktumlk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.sysykeji.top/gtorzjxouy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hammf.cn/gtqvhoehmt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.smart0.xyz/gtlftulrjh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.redwolf501.top/gtgeheferr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.gotoacloud.top/gtsdelrtnr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.nanxinkj.top/gtsaxibvcd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.ydzc1.top/gtdobomtph.html

[N05] 最大公约数
来源：http://hz.zhixingplan.top/gtlutvepsg.html

Py:   math.gcd(a, b)
来源：http://hz.yanxiufei.cn/gtztpizlqd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.gzhubu.top/gtksadwpls.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yvedp.cn/gtbflarcpk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yj20258.top/gtdfxaajyv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zhixingplan.top/gtlhdtgetm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.c1oappe.top/gtrqbhaica.html

Ruby: a.gcd(b)
来源：http://hz.mhx1999.top/gtbstltmbr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.bjfxy.top/gthyzruivr.html

[N06] 判断回文字符串
来源：http://hz.cdnleiting.top/gtsofkwqyg.html

Py:   s == s[::-1]
来源：http://hz.yanxiufei.cn/gtfsiqybkh.html

PHP:  $s === strrev($s);
来源：http://hz.sweek.top/gttgmtbtyt.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jianghu66.top/gtqptgikwk.html

TS:   s === [...s].reverse().join("")
来源：http://hz.sxryk.cn/gtzzqbtgmu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.shanyushiyangkeji.top/gtmoeyypjo.html

Go:   // 双指针从两端比较
来源：http://hz.jianghu66.top/gtajkgsnic.html

Ruby: s == s.reverse
来源：http://hz.zhoulong.xyz/gtdopgjmkc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ydjk.org.cn/gtdnzcvchu.html

[N07] 两数之和（返回下标）
来源：http://hz.9152youxi.cn/gthqsptokp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jinghuilouyu.cn/gtwrrxfenr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hysaishi.cn/gttdzhekjn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.guowangkeji.top/gtlhqdnpim.html

TS:   // 手写 Map<string, number>
来源：http://hz.52xcode.cn/gtzixxtopj.html

Java: // 手写 HashMap
来源：http://hz.hnqzz.top/gtxzobdcet.html

Go:   // 手写 map[int]int
来源：http://hz.dianchejie.cn/gtpdjeibee.html

Ruby: // 手写 Hash
来源：http://hz.zhixingplan.top/gtabpimxjd.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.shanyushiyangtech.top/gtmtkfbmwv.html

[N08] 生成全排列
来源：http://hz.xziqi.cn/gtxvqqnatw.html

Py:   itertools.permutations(arr)
来源：http://hz.guowangkeji.top/gtprjekkih.html

PHP:  // 手写递归交换
来源：http://hz.cqqwz.cn/gtrxlqovpx.html

JS:   // 手写回溯递归
来源：http://hz.xinyue.icu/gtekiebjgs.html

TS:   // 手写回溯递归
来源：http://hz.daria6918.cn/gtcwpzzafp.html


<!-- 参考信息 -->