代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jlsjyb.cn/gtuuawpnqy.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jianghu66.top/gtcuypmqik.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.guannengcc.top/gtzycsgqva.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhiwuduotai.top/gtvydralct.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yj202588.top/gtgrrhfnjs.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.smart0.xyz/gthmmlvkgy.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhixingplan.top/gtrfmjljgv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.nanxuanxn.top/gtbpynuqen.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.daria6918.cn/gtxsfwmglr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.cheryme.top/gtlkdbhhum.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xuanzx.com/gtrwuwlsmr.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.hnxiangtu.top/gtpysxifvs.html

================================================================================
来源：http://hz.hammf.cn/gtylfxdwxd.html

K. JSON 与序列化
来源：http://hz.zdqjudy.top/gtzcjtvzie.html

================================================================================
来源：http://hz.ydzc1.top/gtishlwpnh.html

[K01] 对象转 JSON 字符串
来源：http://hz.sysykeji.top/gtrhnpuqvg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zdqjudy.top/gtmrgdinqb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yangfankeji.com/gtmusfktiy.html

JS:   JSON.stringify(obj)
来源：http://hz.zhiwuduotai.top/gtvsjbsuky.html

TS:   JSON.stringify(obj)
来源：http://hz.aizwys.cn/gtggwmyksw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jqgufenzy.top/gtvcieopkh.html

Go:   json.Marshal(obj)
来源：http://hz.yvedp.cn/gtqknirktr.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jqgufenzy.top/gtqwwzhmfi.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.sweek.top/gtolxdjzry.html

[K02] JSON 字符串转对象
来源：http://hz.hywenlv.cn/gtbvivvjam.html

Py:   json.loads(s)
来源：http://hz.redwolf501.top/gtlaruwftl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.daria6918.cn/gtcibuqwgj.html

JS:   JSON.parse(s)
来源：http://hz.pycfn.com/gtjkzpmazq.html

TS:   JSON.parse(s)
来源：http://hz.ydzc1.top/gtzufnnjgv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hywenlv.cn/gtxncenktb.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.sufxvd.cn/gtwakbmaim.html

Ruby: JSON.parse(s)
来源：http://hz.svipenyu.cn/gtbmhqhxjq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ehwqpu.com/gtvwtobort.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yuanzhike.top/gtlaqnsolk.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yueranfly.top/gtskkjfmdg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.daxiang520.top/gtqqiuszgm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ydjk.org.cn/gtgfssgwim.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.nwbrower.top/gtrcyrnnwl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ppjwa.cn/gtfqtdpuau.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.aizwys.cn/gtzwxzmfuv.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.pycfn.com/gtaycyuilb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jqgufenzy.top/gtzsrugwdo.html

[K04] 读取 JSON 文件
来源：http://hz.daxiang520.top/gtqypulenm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.wangshuangyany.cn/gtzirywxfc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.chenlongwang.top/gtivaqjiza.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jiagoushi.top/gtpwvtxbxf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xylfe.cn/gtohfabrvo.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhaomingkeji.xyz/gtsdewplbn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhiwuduotai.top/gtutufdibr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.cdnleiting.top/gtuhxjuizy.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.sweek.top/gtdygzuggb.html

[K05] 深拷贝对象
来源：http://hz.yuxming.cn/gtrjvujmzv.html

Py:   copy.deepcopy(obj)
来源：http://hz.yanxiufei.cn/gtutaufkie.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zycfv.cn/gtjsflvvfk.html

JS:   structuredClone(obj)
来源：http://hz.jqgfzy.top/gtdquclavf.html

TS:   structuredClone(obj)
来源：http://hz.xylfe.cn/gtqfqoarfe.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.smart0.xyz/gtvcpqhjym.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yj20258888.top/gtsgoiflwa.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.aizwys.cn/gtchxxytkj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jqgfzy.top/gthkntewaa.html

[K06] 解析 URL 查询串
来源：http://hz.shanyushiyangkeji.top/gtoiqemfaj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.kuanghao11.cn/gtwnzjbyqg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jinyuanbaomall.cn/gtfdruyhps.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.quarkkingdee.top/gtipkbfing.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.fzhhl.top/gtoptqjzdm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.tian-w.cn/gtlttwegwn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cucudq.cn/gtggecjsyk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hywenlv.cn/gtmwuajbky.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.iojbl.cn/gtkfbtqdxn.html

[K07] 进制转换
来源：http://hz.yangfankeji.com/gtvpaoyiqc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.iojbl.cn/gtxplfwfmh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xingfuxueyuan.xyz/gtvbpmuksq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.gogol.net.cn/gtcertlogu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.svipenyu.cn/gtrrhfvshk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jinqigufen.top/gtdtteemom.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhijiandao.cn/gtsiszzupk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.gzhubu.top/gtwbpuwxge.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.havefunace.top/gtaqwlhzgz.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.dianchejie.cn/gthxislzrw.html

Py:   pickle.dumps(obj)
来源：http://hz.andypj.xyz/gtsbnmjprg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.fengsongda.top/gtsoezhlta.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ybcxt.top/gtmsidaenw.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ydjk.org.cn/gtzpmdcasr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.sufxvd.cn/gtnbsqbowc.html

Go:   encoding/gob
来源：http://hz.chenlongwang.top/gtbsleihbb.html

Ruby: Marshal.dump(obj)
来源：http://hz.kuanghao11.cn/gtcbxbogwh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.guowangkeji.top/gtrkhsgkpm.html

================================================================================
来源：http://hz.tianlin.xyz/gtctgjfjnc.html

L. 网络请求
来源：http://hz.nwbrower.top/gtrhqqqtok.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtrtousuic.html

[L01] 发送 GET 请求
来源：http://hz.andypj.xyz/gthxbsgqat.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.xylfe.cn/gtzzoxruse.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.cashguo.top/gtzppraomw.html

JS:   await fetch(url)
来源：http://hz.xziqi.cn/gtwjctyscq.html

TS:   await fetch(url)
来源：http://hz.xuetiantiany.cn/gtqfdnmrem.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.andypj.xyz/gtprplhybm.html

Go:   resp, err := http.Get(url)
来源：http://hz.dianchejie.cn/gthhdwxhzu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xuanzx.com/gtxohaaexn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yj202588.top/gtmdkpkmad.html

[L02] 发送 POST JSON
来源：http://hz.sweek.top/gtfzjaiagc.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jinyuanbaomall.cn/gtweirnsew.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.vqdsnc.cn/gtcdnxmnjz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yangfankeji.com/gtjhlvxiht.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhongyouzk.top/gtzfnkehbr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.redwolf501.top/gtsazizhwz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hywenlv.cn/gtvffhjcnk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zycfv.cn/gtzctnzrqd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ehwqpu.com/gtrhbaqxgx.html

[L03] 设置自定义请求头
来源：http://hz.dashuyun.cn/gtfwokmjja.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.snrcjt.cn/gtosnfzkow.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.nwbrower.top/gtbxbnjgvf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ppjwa.cn/gtmtpropre.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.smart0.xyz/gtermzypun.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yj20258888.top/gtsiopkdyc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.smart0.xyz/gtlrxdjzdl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yanxiufei.cn/gttfiknmzq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.pycfn.com/gtrdmeabqe.html

[L04] 设置超时
来源：http://hz.chenjidiqi.icu/gtmjnvvnrh.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xinyue.icu/gtuuuklrtc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.sxryk.cn/gtgpsfpssr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shzxlz.cn/gtyawqdwyr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhoulong.xyz/gtzdnpcxgx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.feifeiyinyue.top/gtyjzalngp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yanxiufei.cn/gttfmnirfo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.dashuyun.cn/gtkhccbmvj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yj202588.top/gtfzgzmcvu.html

[L05] 上传文件（multipart）
来源：http://hz.yj202588.top/gtjvioeoel.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jinqigfzy.top/gtviyhbdig.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jlsjyb.cn/gtowugxcji.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ybcxt.top/gtonjqequl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.shanyushiyangkeji.top/gtysfntfqc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhongyouzk.top/gtwkqdqbgv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zdqjudy.top/gttbgkbvkj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.smart0.xyz/gtmlgrbjkf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.gogol.net.cn/gtoyavcdhl.html

[L06] 解析响应为 JSON
来源：http://hz.hongshengwenyu.top/gtpfdrrndq.html

Py:   resp.json()
来源：http://hz.ybcxt.top/gtnfmmiqoz.html

PHP:  json_decode($body, true);
来源：http://hz.ywan-chungtsiang.top/gtspzxxpdn.html

JS:   await resp.json()
来源：http://hz.bjfxy.top/gttbayrmsf.html

TS:   await resp.json()
来源：http://hz.hysaishi.cn/gtrmidxwal.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.guowangkeji.top/gtavgdjslt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.mhx1999.top/gtcbmcufte.html

Ruby: JSON.parse(resp.body)
来源：http://hz.daria6918.cn/gtsthnamvp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.andypj.xyz/gtficugjes.html

[L07] 处理 HTTP 状态码
来源：http://hz.xylfe.cn/gtccgcewwm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jqgfzy.top/gtrxnonayq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yj20258888.top/gtairoekgo.html

JS:   resp.ok;  resp.status
来源：http://hz.bjfxy.top/gtacnsxvby.html

TS:   resp.ok;  resp.status
来源：http://hz.jinyuanbaomall.cn/gtdizkhfvh.html

Java: resp.statusCode()
来源：http://hz.ydjk.org.cn/gtzqttybag.html

Go:   resp.StatusCode
来源：http://hz.nanxinkj.top/gtgdffehus.html

Ruby: resp.code.to_i
来源：http://hz.jyoumei.cn/gtsbwrtxia.html

C#:   (int)resp.StatusCode
来源：http://hz.zhoulong.xyz/gtjqwaumhr.html

[L08] 并发请求多个地址
来源：http://hz.chenjidiqi.icu/gtzetmtfof.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zhoulong.xyz/gtuxiwpiey.html

PHP:  curl_multi_init() 系列
来源：http://hz.jqgfzy.top/gtytbemiwf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ydjk.org.cn/gtnsfsjhsu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.dianchejie.cn/gtcysjcore.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yanxiufei.cn/gtazjduzee.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhaomingkeji.xyz/gttntyceua.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.c1oappe.top/gtguhkenwg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.daxiang520.top/gtzwtmcgvq.html

================================================================================
来源：http://hz.zhixingplan.top/gtyumtmykw.html

M. 命令行 / 进程 / 环境
来源：http://hz.gzhubu.top/gtubpdnaxu.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtqdrhtxag.html

[M01] 读取命令行参数
来源：http://hz.nwbrower.top/gtdcvtszfw.html

Py:   sys.argv[1:]
来源：http://hz.cqqwz.cn/gtslqdvnue.html

PHP:  $argv;  $argc;
来源：http://hz.jinqigufen.top/gtyknpyzah.html

JS:   process.argv.slice(2)
来源：http://hz.wangshuangyany.cn/gtlboeomfn.html

TS:   process.argv.slice(2)
来源：http://hz.cucudq.cn/gtbvrfgyxa.html

Java: args 数组（main 方法参数）
来源：http://hz.ybcxt.top/gtjnoxepme.html

Go:   os.Args[1:]
来源：http://hz.316326.xyz/gtxsskfhtw.html

Ruby: ARGV
来源：http://hz.daria6918.cn/gtzselfhmp.html

C#:   args 数组（Main 方法参数）
来源：http://hz.svipenyu.cn/gthiqcesmp.html

[M02] 读取环境变量
来源：http://hz.daria6918.cn/gttkfwrbpp.html

Py:   os.environ.get("HOME")
来源：http://hz.sweek.top/gttcvdkidf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yuanzhike.top/gtcsdcyciz.html

JS:   process.env.HOME
来源：http://hz.zhongyouzk.top/gtsnazlgtw.html

TS:   process.env.HOME
来源：http://hz.daria6918.cn/gtzjziczvr.html

Java: System.getenv("HOME")
来源：http://hz.zhaomingkeji.xyz/gtsbswzrth.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhiwuduotai.top/gthponkjsl.html

Ruby: ENV["HOME"]
来源：http://hz.yuxming.cn/gtfmegctom.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xuanzx.com/gtmgdizapx.html

[M03] 执行外部命令
来源：http://hz.zhengqikj.top/gtiwurxodd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.aizwys.cn/gtlvayiwpr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ydzc1.top/gtcbxnodnf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.52xcode.cn/gtfkcpezcw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.andypj.xyz/gtsgkppriv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.feifeiyinyue.top/gtcaldajos.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.52xcode.cn/gtobbumuvy.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.bjfxy.top/gtugqlkzqa.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xziqi.cn/gtkioppzfw.html

[M04] 获取当前工作目录
来源：http://hz.ydzc1.top/gtspxlmrht.html

Py:   os.getcwd()
来源：http://hz.c1oappe.top/gtniubjnkq.html

PHP:  getcwd();
来源：http://hz.yvedp.cn/gtplrwlbcb.html

JS:   process.cwd()
来源：http://hz.jqgfzy.top/gtihwsntuw.html

TS:   process.cwd()
来源：http://hz.snrcjt.cn/gtlnlkxbxl.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.daxiang520.top/gtvvasaast.html

Go:   os.Getwd()
来源：http://hz.cqqwz.cn/gtkmnrzgog.html

Ruby: Dir.pwd
来源：http://hz.ydjk.org.cn/gtwmvmazaj.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.chenzaomai.com/gtuizisxqw.html

[M05] 设置退出码
来源：http://hz.jlsjyb.cn/gtrtkhojaj.html

Py:   sys.exit(1)
来源：http://hz.hongshengwenyu.top/gtfnznasrv.html

PHP:  exit(1);
来源：http://hz.zhijiandao.cn/gtfrfzukov.html

JS:   process.exit(1)
来源：http://hz.xingfuxueyuan.xyz/gtzqnwdvhy.html

TS:   process.exit(1)
来源：http://hz.zhengqikj.top/gtosnwdwxi.html

Java: System.exit(1)
来源：http://hz.birdmap.top/gtmirulwvn.html

Go:   os.Exit(1)
来源：http://hz.zhixingplan.top/gtxxpdlamx.html

Ruby: exit 1
来源：http://hz.cqqwz.cn/gtjpeczgiv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.gotoacloud.top/gtangsnzil.html

[M06] 向标准错误输出
来源：http://hz.meibo888.top/gtkloopjeg.html

Py:   print("err", file=sys.stderr)
来源：http://hz.redwolf501.top/gtdxphthre.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.snrcjt.cn/gtwmmhnypv.html

JS:   console.error("err")
来源：http://hz.ehwqpu.com/gtliuoonwj.html

TS:   console.error("err")
来源：http://hz.ydjk.org.cn/gtuwnfafyn.html

Java: System.err.println("err")
来源：http://hz.sxryk.cn/gtuvyzwndk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.meibo888.top/gtvohabbwi.html

Ruby: warn "err"
来源：http://hz.dianchejie.cn/gtwhtrsmsa.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hysaishi.cn/gtuvlvdanf.html

[M07] 判断是否为主入口
来源：http://hz.sweek.top/gtjmumrbcd.html

Py:   if __name__ == "__main__":
来源：http://hz.gzhubu.top/gtllqhuuzq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.guowangkeji.top/gtxhtetnrf.html

JS:   require.main === module
来源：http://hz.9152youxi.cn/gtlkkxspyu.html

TS:   require.main === module
来源：http://hz.yueranfly.top/gtuqtjiaqx.html

Java: public static void main(String[] args)
来源：http://hz.daxiang520.top/gtplawnupn.html

Go:   func main()
来源：http://hz.smart0.xyz/gtexkzlzpp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jyoumei.cn/gtwccggtsr.html

C#:   static void Main(string[] args)
来源：http://hz.zycfv.cn/gthzjapkns.html

[M08] 获取系统与运行时信息
来源：http://hz.yvedp.cn/gtaopawjhc.html

Py:   platform.system();  platform.python_version()
来源：http://hz.sysykeji.top/gtsxaprckx.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.cashguo.top/gthjiotzsj.html

JS:   process.platform;  process.version
来源：http://hz.yanxiufei.cn/gthtzvwldo.html

TS:   process.platform;  process.version
来源：http://hz.tian-w.cn/gtgvkydacn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.guowangkeji.top/gtfvthpxmp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yj202588.top/gtwrwtbwcb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cqqwz.cn/gtmoeqdfdq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.mhx1999.top/gtgymphzql.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtwjusyjoz.html

N. 数据结构与算法
来源：http://hz.wangdashe.top/gtkaijjqeq.html

================================================================================
来源：http://hz.tian-w.cn/gtbanaspry.html

[N01] 二分查找（有序数组）
来源：http://hz.kuanghao11.cn/gtpewbqtbs.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.gaohongyu789.top/gtvhoxnbpz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhengqikj.top/gtxhiywayw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sxryk.cn/gtrengitnk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.tianlin.xyz/gtexwqvuar.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.fengsongda.top/gtphguoolr.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.shanyushiyangkeji.top/gtkoasbmjo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.sxryk.cn/gtkeaoqicw.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.tian-w.cn/gtwrhtgipp.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yj202588.top/gtsrnxvrbi.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinqigufen.top/gttubduzgr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.sufxvd.cn/gtvlhzncla.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nwbrower.top/gtaomoibpo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hfpthk.cn/gtvkzqqfwp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhaomingkeji.xyz/gtcenacdos.html

Go:   slices.Sort(arr)
来源：http://hz.ydzc1.top/gtsmqjaphf.html

Ruby: arr.sort
来源：http://hz.wangdashe.top/gtnvcuvbzw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.dianchejie.cn/gtipgqmgtu.html

[N03] 快速排序（分治示例）
来源：http://hz.guowangkeji.top/gteblzepoz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xuetiantiany.cn/gtwzpovjfj.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jinghuilouyu.cn/gtvccmmxrw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jlsjyb.cn/gtdrjstxty.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nanxinkj.top/gtnphmixrv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.xuanzx.com/gtrzhwfvvi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.0kj1m.cn/gtpyuwhfzd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.cashguo.top/gtceixhujv.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.vqdsnc.cn/gtkoyudkzq.html

[N04] 斐波那契数列
来源：http://hz.tianlin.xyz/gtyotgxyyh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xuetiantiany.cn/gtrvzvgarb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hysaishi.cn/gtnkctxivs.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.daxiang520.top/gtcfuurjfx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hongshengwenyu.top/gtbrrswnqt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.vqdsnc.cn/gtbivlgrql.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yangfankeji.com/gtlelofpnp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.aibaodan.cn/gtymdvcqsg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jyoumei.cn/gtiprvimyn.html

[N05] 最大公约数
来源：http://hz.wangshuangyany.cn/gtfjgirwtx.html

Py:   math.gcd(a, b)
来源：http://hz.shanyushiyangkeji.top/gtbmogbjxt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jianghu66.top/gtocaeiqzw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhoulong.xyz/gtllmkmnuh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zycfv.cn/gtnsnqzhwm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ywan-chungtsiang.top/gtcjbgwxue.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.iojbl.cn/gtmwhymmgy.html

Ruby: a.gcd(b)
来源：http://hz.c1oappe.top/gttlwwplse.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.vqdsnc.cn/gtdoebzish.html

[N06] 判断回文字符串
来源：http://hz.yueranfly.top/gtsyqsljtt.html

Py:   s == s[::-1]
来源：http://hz.zhiwuduotai.top/gtjiquwojq.html

PHP:  $s === strrev($s);
来源：http://hz.hywenlv.cn/gtnxwlnxbd.html

JS:   s === [...s].reverse().join("")
来源：http://hz.quarkkingdee.top/gttnvrimoi.html

TS:   s === [...s].reverse().join("")
来源：http://hz.nanxuanxn.top/gtjmqexnhc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.hysaishi.cn/gtjlimsipm.html

Go:   // 双指针从两端比较
来源：http://hz.yuanzhike.top/gtewezvbxf.html

Ruby: s == s.reverse
来源：http://hz.yj202588.top/gtwbkzvxra.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yj202588.top/gtquveyxlz.html

[N07] 两数之和（返回下标）
来源：http://hz.chenzaomai.com/gtylfyclbn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.c1oappe.top/gtarnvyycp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.kuanghao11.cn/gtjaoizxxw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.andypj.xyz/gtwjoaymyh.html

TS:   // 手写 Map<string, number>
来源：http://hz.daxiang520.top/gtrtehryqr.html

Java: // 手写 HashMap
来源：http://hz.jqgufenzy.top/gthsegwwty.html


<!-- 参考信息 -->