代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.nanxinkj.top/gtmcuhehzj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zycfv.cn/gtjckhypkd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hywenlv.cn/gtkywyrufa.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hywenlv.cn/gtytcdhave.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.nanxuanxn.top/gtohyckoae.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.fzhhl.top/gtbvvwkkps.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.vqdsnc.cn/gtoxkodfrv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xziqi.cn/gtkuwxuoaw.html

================================================================================
来源：http://hz.zhixingplan.top/gtizfntxhs.html

K. JSON 与序列化
来源：http://hz.cheryme.top/gthbbffwgv.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtivjvpuby.html

[K01] 对象转 JSON 字符串
来源：http://hz.ehwqpu.com/gtkpwejyal.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.haohaochexian.top/gttjcrwkni.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jianghu66.top/gtjcaganyn.html

JS:   JSON.stringify(obj)
来源：http://hz.nanxuanxn.top/gtuonzduwj.html

TS:   JSON.stringify(obj)
来源：http://hz.wangshuangyany.cn/gtazpwmjgk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yueranfly.top/gtsduhiodw.html

Go:   json.Marshal(obj)
来源：http://hz.meibo888.top/gtpaznlllp.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.guannengcc.top/gtnuzuvshl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.haohaochexian.top/gtgyhjrdti.html

[K02] JSON 字符串转对象
来源：http://hz.cashguo.top/gteuouqwwd.html

Py:   json.loads(s)
来源：http://hz.svipenyu.cn/gtnmwyimza.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.pengpengdd.cyou/gtkrggmjzz.html

JS:   JSON.parse(s)
来源：http://hz.yj20258.top/gtrnepqshg.html

TS:   JSON.parse(s)
来源：http://hz.guannengcc.top/gtbdetqbhr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.pengpengdd.cyou/gtuleuqilq.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhengqikj.top/gtkznfxvak.html

Ruby: JSON.parse(s)
来源：http://hz.shangyingyoupin.top/gtcxycvysc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.daxiang520.top/gtczfcmebt.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.xinyue.icu/gtbasdbcff.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xylfe.cn/gtscboauaj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.0kj1m.cn/gtojdgzjpf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hysaishi.cn/gtooauxryf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj20258.top/gtkqjbdtvd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.chenlongwang.top/gtsqwmnjiy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.pengpengdd.cyou/gtqzstcwuf.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.aizwys.cn/gtbuyfnnqw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yueranfly.top/gtjnwfuztl.html

[K04] 读取 JSON 文件
来源：http://hz.yj20258888.top/gtqoznvejt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zhengqikj.top/gtbjpkvlsh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yongpay.top/gtpxrfuizk.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yj20258.top/gtqypdwszt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.nanxinkj.top/gtdwwsakfa.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhengqikj.top/gtdsdhaaos.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zdqjudy.top/gthzsmbtss.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhixingplan.top/gtbxqjzeco.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yanxiufei.cn/gtrtokolvo.html

[K05] 深拷贝对象
来源：http://hz.jianghu66.top/gtimuzbuqx.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhongyouzk.top/gtcvluokza.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ppjwa.cn/gtaxmjgdhu.html

JS:   structuredClone(obj)
来源：http://hz.jinyuanbaomall.cn/gtgwpozpiq.html

TS:   structuredClone(obj)
来源：http://hz.pengpengdd.cyou/gtvqsvqifc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xziqi.cn/gticbmahgr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jyoumei.cn/gtlecuatgk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.daria6918.cn/gtgsbzyevw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.xuetiantiany.cn/gtefidxobd.html

[K06] 解析 URL 查询串
来源：http://hz.yuxming.cn/gtnxwcrhny.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xziqi.cn/gtbzdnexkr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yj202588.top/gteqtmdtqm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.aizwys.cn/gtchmyzvmn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhongyouzk.top/gtzvcrrzbv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.aizwys.cn/gtlbtikqxh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.shangyingyoupin.top/gtnwfdcepo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.sufxvd.cn/gtchjqengm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.aibaodan.cn/gttlglgvut.html

[K07] 进制转换
来源：http://hz.shanyushiyangkeji.top/gtpfmivqzu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.smart0.xyz/gtakvjolds.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xingfuxueyuan.xyz/gtzndtxuqz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jinqigufen.top/gtdqzqkuyv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yvedp.cn/gtgvwbtwjj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.guannengcc.top/gtaiadsgvh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hfpthk.cn/gtompiiokn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.nanxuanxn.top/gtsrzkfmqu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.chenlongwang.top/gtbfuunovb.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.gotoacloud.top/gtcospugcg.html

Py:   pickle.dumps(obj)
来源：http://hz.ppjwa.cn/gtlvfoktnu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.shanyushiyangtech.top/gtiuphzztv.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhongyouzk.top/gtbpnaoihj.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.gotoacloud.top/gtqocfqjtf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ehwqpu.com/gtgpucoacd.html

Go:   encoding/gob
来源：http://hz.gaohongyu789.top/gtkrrekdbg.html

Ruby: Marshal.dump(obj)
来源：http://hz.mhx1999.top/gttkgybhhv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.sweek.top/gtqfzamlme.html

================================================================================
来源：http://hz.yuanzhike.top/gtmmccbsvg.html

L. 网络请求
来源：http://hz.nwbrower.top/gtwntlccsz.html

================================================================================
来源：http://hz.cashguo.top/gtjrgggvff.html

[L01] 发送 GET 请求
来源：http://hz.yongpay.top/gtdkbvseju.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jqgfzy.top/gtqvwozxdq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.c1oappe.top/gtwjkcgole.html

JS:   await fetch(url)
来源：http://hz.sufxvd.cn/gtmoulbirx.html

TS:   await fetch(url)
来源：http://hz.havefunace.top/gtfsnvpsjy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jinghuilouyu.cn/gtjtjslghq.html

Go:   resp, err := http.Get(url)
来源：http://hz.ydjk.org.cn/gtozhyjvmb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.sysykeji.top/gtljwbrobk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yj20258888.top/gtftswlhti.html

[L02] 发送 POST JSON
来源：http://hz.cashguo.top/gtnlnemgzc.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ydzc1.top/gtxihrghvp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.fengsongda.top/gtuhquswnh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yangfankeji.com/gtmbvlqjuq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.andypj.xyz/gtfulznsdw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.xuetiantiany.cn/gtyogqooxr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.snrcjt.cn/gthmbsztev.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhongyouzk.top/gtxscazekg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ppjwa.cn/gtnvxyspsv.html

[L03] 设置自定义请求头
来源：http://hz.smart0.xyz/gtkgvbqeaw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.havefunace.top/gtivaywwjz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jqgufenzy.top/gtctsusegm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.tianlin.xyz/gtylujvltl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yuanzhike.top/gtpurzrziq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.fzhhl.top/gtvndfauyt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhoulong.xyz/gtpflgfmkr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zdqjudy.top/gtbulzimcr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.sweek.top/gtvozipfrr.html

[L04] 设置超时
来源：http://hz.haohaochexian.top/gtkhcfuvmb.html

Py:   requests.get(url, timeout=5)
来源：http://hz.smart0.xyz/gtjcbrvxcq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.nanxuanxn.top/gtazzturhz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xylfe.cn/gtizowpazo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.vqdsnc.cn/gtnanmbipt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yj20258.top/gtpwkcykvr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.shanyushiyangtech.top/gtorzgqyxp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.316326.xyz/gtfyuhryyc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xuanzx.com/gtcbdeonez.html

[L05] 上传文件（multipart）
来源：http://hz.daria6918.cn/gtvfvpvnek.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.ppjwa.cn/gtlyabtkgw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhijiandao.cn/gtdwvaldyv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.316326.xyz/gtqpncmzxp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.gaohongyu789.top/gtlfzmqfrz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.shanyushiyangtech.top/gthabyugfc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.meibo888.top/gtozgadujk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shzxlz.cn/gtndupxxej.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhengqikj.top/gtnyxxllyl.html

[L06] 解析响应为 JSON
来源：http://hz.shanyushiyangkeji.top/gtrsrvbdji.html

Py:   resp.json()
来源：http://hz.zhixingplan.top/gtpcjbyqvh.html

PHP:  json_decode($body, true);
来源：http://hz.smart0.xyz/gtmvpieudq.html

JS:   await resp.json()
来源：http://hz.shzxlz.cn/gthzjmybrr.html

TS:   await resp.json()
来源：http://hz.9152youxi.cn/gtargviyjr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.ivvv.top/gtjqvgyjqz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.nanxuanxn.top/gtbsncvpey.html

Ruby: JSON.parse(resp.body)
来源：http://hz.sufxvd.cn/gtcltydpwv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jianghu66.top/gtktiwqxdl.html

[L07] 处理 HTTP 状态码
来源：http://hz.hongshengwenyu.top/gtwwebbnnn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.gogol.net.cn/gtrpxpleno.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.aibaodan.cn/gtvhrfwxfw.html

JS:   resp.ok;  resp.status
来源：http://hz.jiagoushi.top/gtncavszgs.html

TS:   resp.ok;  resp.status
来源：http://hz.chenlongwang.top/gtuimaxkll.html

Java: resp.statusCode()
来源：http://hz.hfpthk.cn/gtxjxhstmm.html

Go:   resp.StatusCode
来源：http://hz.chenlongwang.top/gtebvvvwzg.html

Ruby: resp.code.to_i
来源：http://hz.tianlin.xyz/gtxsyftwof.html

C#:   (int)resp.StatusCode
来源：http://hz.wangdashe.top/gtldmhepjz.html

[L08] 并发请求多个地址
来源：http://hz.xinyue.icu/gtyerftpfa.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hysaishi.cn/gtieoxwbax.html

PHP:  curl_multi_init() 系列
来源：http://hz.jqgfzy.top/gtgrhxtrkd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.guannengcc.top/gtjwgjkjxt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinqigufen.top/gthfmrsvwr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hammf.cn/gtecggfzua.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zycfv.cn/gtkfnfwypa.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.nanxinkj.top/gtrdoaorqw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhixingplan.top/gtytsoxnua.html

================================================================================
来源：http://hz.jiagoushi.top/gtllorymay.html

M. 命令行 / 进程 / 环境
来源：http://hz.xuetiantiany.cn/gtbdlvvscu.html

================================================================================
来源：http://hz.xziqi.cn/gtlitjyjff.html

[M01] 读取命令行参数
来源：http://hz.smart0.xyz/gtsnfgcbkv.html

Py:   sys.argv[1:]
来源：http://hz.andypj.xyz/gtpraeperx.html

PHP:  $argv;  $argc;
来源：http://hz.zhaomingkeji.xyz/gtgckwcbnz.html

JS:   process.argv.slice(2)
来源：http://hz.pycfn.com/gtccwrojbn.html

TS:   process.argv.slice(2)
来源：http://hz.jqgufenzy.top/gtbzoqhcyk.html

Java: args 数组（main 方法参数）
来源：http://hz.shanyushiyangkeji.top/gtuabeozop.html

Go:   os.Args[1:]
来源：http://hz.hywenlv.cn/gtdyghaavq.html

Ruby: ARGV
来源：http://hz.52xcode.cn/gtbddeptlm.html

C#:   args 数组（Main 方法参数）
来源：http://hz.gogol.net.cn/gtzblmznsl.html

[M02] 读取环境变量
来源：http://hz.xinyue.icu/gtchqzdhwi.html

Py:   os.environ.get("HOME")
来源：http://hz.cheryme.top/gtagllxzok.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jinyuanbaomall.cn/gtsnvqxeta.html

JS:   process.env.HOME
来源：http://hz.chenzaomai.com/gtyutujtpj.html

TS:   process.env.HOME
来源：http://hz.xuetiantiany.cn/gtjyhpelhi.html

Java: System.getenv("HOME")
来源：http://hz.cucudq.cn/gtuuzmuamn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.daxiang520.top/gtdwgfzzsk.html

Ruby: ENV["HOME"]
来源：http://hz.xziqi.cn/gtqtpvrjmt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.316326.xyz/gtdcbuhbks.html

[M03] 执行外部命令
来源：http://hz.meibo888.top/gtxyiuiurw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ehwqpu.com/gtwukzqemz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.wangshuangyany.cn/gtjixhmsah.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jqgufenzy.top/gtmyyavuyo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xuetiantiany.cn/gtvrjtajcp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ywan-chungtsiang.top/gtampdjkyn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hfpthk.cn/gtvcthxqdl.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zycfv.cn/gtfqprfoyk.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yj202588.top/gtvacdvwvt.html

[M04] 获取当前工作目录
来源：http://hz.zycfv.cn/gtiosvkyuc.html

Py:   os.getcwd()
来源：http://hz.ppjwa.cn/gtywpyacbr.html

PHP:  getcwd();
来源：http://hz.sysykeji.top/gtyawmmfso.html

JS:   process.cwd()
来源：http://hz.aibaodan.cn/gtemyiilmw.html

TS:   process.cwd()
来源：http://hz.wangshuangyany.cn/gttxtopktz.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xuanzx.com/gtocopduut.html

Go:   os.Getwd()
来源：http://hz.yj20258.top/gtotqpzbwq.html

Ruby: Dir.pwd
来源：http://hz.daria6918.cn/gtdsxkztio.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.kuanghao11.cn/gtrwaworro.html

[M05] 设置退出码
来源：http://hz.hysaishi.cn/gtseqexydc.html

Py:   sys.exit(1)
来源：http://hz.guannengcc.top/gtmkflngft.html

PHP:  exit(1);
来源：http://hz.zycfv.cn/gtsanpysdc.html

JS:   process.exit(1)
来源：http://hz.yj20258.top/gtndynifnd.html

TS:   process.exit(1)
来源：http://hz.vqdsnc.cn/gtznomuzlt.html

Java: System.exit(1)
来源：http://hz.xylfe.cn/gtznkwrawd.html

Go:   os.Exit(1)
来源：http://hz.zhaomingkeji.xyz/gtczohatym.html

Ruby: exit 1
来源：http://hz.chenjidiqi.icu/gtyveomeas.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.svipenyu.cn/gthgsvpdon.html

[M06] 向标准错误输出
来源：http://hz.shuidangran.top/gtuoqrigoc.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yongpay.top/gtdvjmvdpa.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yanxiufei.cn/gtkfkkcgyj.html

JS:   console.error("err")
来源：http://hz.ybcxt.top/gtvwhdhexq.html

TS:   console.error("err")
来源：http://hz.snrcjt.cn/gtskwigoos.html

Java: System.err.println("err")
来源：http://hz.andypj.xyz/gtddfjwbmu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.nanxinkj.top/gtsqpzgigw.html

Ruby: warn "err"
来源：http://hz.iojbl.cn/gtfcabirjm.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ehwqpu.com/gtykpemwfi.html

[M07] 判断是否为主入口
来源：http://hz.yj20258888.top/gtemqrwwse.html

Py:   if __name__ == "__main__":
来源：http://hz.daria6918.cn/gtnbdxeljs.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.chenlongwang.top/gtkfuvgzxb.html

JS:   require.main === module
来源：http://hz.sysykeji.top/gtrwwgibkp.html

TS:   require.main === module
来源：http://hz.daxiang520.top/gtpuhmezmg.html

Java: public static void main(String[] args)
来源：http://hz.cucudq.cn/gttdwmzerb.html

Go:   func main()
来源：http://hz.havefunace.top/gtglzjbzmm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jinghuilouyu.cn/gtbdveicph.html

C#:   static void Main(string[] args)
来源：http://hz.feifeiyinyue.top/gtfojdsfla.html

[M08] 获取系统与运行时信息
来源：http://hz.meibo888.top/gtlawprlot.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yvedp.cn/gtjuyefoes.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jianghu66.top/gtqltbcine.html

JS:   process.platform;  process.version
来源：http://hz.gzhubu.top/gtqchfthze.html

TS:   process.platform;  process.version
来源：http://hz.ybcxt.top/gtiqiwmywf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hnqzz.top/gtizukffxd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.pycfn.com/gtqulbncts.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.fengsongda.top/gtzrbwdokt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jqgfzy.top/gtmqqheqkn.html

================================================================================
来源：http://hz.yanxiufei.cn/gtmblzqitu.html

N. 数据结构与算法
来源：http://hz.hfpthk.cn/gtnltdgttq.html

================================================================================
来源：http://hz.tanke756.top/gtdbhqmtvw.html

[N01] 二分查找（有序数组）
来源：http://hz.fengsongda.top/gtkwgqjkho.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xziqi.cn/gttklepzbh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yonumen.top/gtwtiqhdug.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sxryk.cn/gtkufglyjt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hongshengwenyu.top/gtnnxtraif.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhongyouzk.top/gtdolwmsfv.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.smart0.xyz/gtankiypgq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.shanyushiyangkeji.top/gtbanjipvv.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.nanxinkj.top/gtcvoaylde.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.feifeiyinyue.top/gtfbmendfj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sxryk.cn/gtcvmyhuvc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hywenlv.cn/gtwnooqawj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xingfuxueyuan.xyz/gtytsvxbdf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yonumen.top/gtcdvtgeqn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.tanke756.top/gtkcadeppm.html

Go:   slices.Sort(arr)
来源：http://hz.zdqjudy.top/gtmqtwwcxj.html

Ruby: arr.sort
来源：http://hz.xuetiantiany.cn/gtwuqntprx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.andypj.xyz/gtsycuvjxu.html

[N03] 快速排序（分治示例）
来源：http://hz.tian-w.cn/gthyxlxcgt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ydjk.org.cn/gtnokrmkui.html

PHP:  // 递归实现，或用 usort
来源：http://hz.sxryk.cn/gtjdxgfxoh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.daria6918.cn/gtoznuldds.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xinyue.icu/gthfxwwfjv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinghuilouyu.cn/gtqcabaptn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhiwuduotai.top/gtxlvytpse.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.tianlin.xyz/gtwljatygk.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.xuetiantiany.cn/gtupzxjrdh.html

[N04] 斐波那契数列
来源：http://hz.dashuyun.cn/gtgvvzfmsg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ppjwa.cn/gtrhxumatp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hnxiangtu.top/gtzgwcxkam.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ywan-chungtsiang.top/gtbkwwkjld.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ivvv.top/gtpreeetjp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.snrcjt.cn/gtmqiyistf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.cheryme.top/gtkwxpjgoy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhengqikj.top/gtljrnkbys.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xinyue.icu/gtmrkmyhsc.html

[N05] 最大公约数
来源：http://hz.fzhhl.top/gtqscplyzf.html

Py:   math.gcd(a, b)
来源：http://hz.yj20258.top/gtofdigypj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.fzhhl.top/gtthiakgij.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ywan-chungtsiang.top/gttbquhsjh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.fzhhl.top/gtegmhwaxw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.xuanzx.com/gtqehmzgwr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.shzxlz.cn/gtjimmvzif.html

Ruby: a.gcd(b)
来源：http://hz.shangyingyoupin.top/gtbmlmnmzs.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ywan-chungtsiang.top/gtyieglyts.html

[N06] 判断回文字符串
来源：http://hz.dianchejie.cn/gtzkvxqgqg.html

Py:   s == s[::-1]
来源：http://hz.hnqzz.top/gtdsfrylup.html

PHP:  $s === strrev($s);
来源：http://hz.yvedp.cn/gtvmkqcvjv.html

JS:   s === [...s].reverse().join("")
来源：http://hz.aizwys.cn/gtziikdrew.html

TS:   s === [...s].reverse().join("")
来源：http://hz.havefunace.top/gtaycswiti.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.daria6918.cn/gtzrjnpbms.html

Go:   // 双指针从两端比较
来源：http://hz.hfpthk.cn/gtndywofrh.html

Ruby: s == s.reverse
来源：http://hz.jyoumei.cn/gtronaadij.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.kuanghao11.cn/gtacvopetp.html

[N07] 两数之和（返回下标）
来源：http://hz.hysaishi.cn/gtwarydtzy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hywenlv.cn/gtydvsplam.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zdqjudy.top/gtddybdzzy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ywan-chungtsiang.top/gteonjdspb.html

TS:   // 手写 Map<string, number>
来源：http://hz.shanyushiyangkeji.top/gtxvqedpzf.html

Java: // 手写 HashMap
来源：http://hz.hfpthk.cn/gtsssgqmha.html

Go:   // 手写 map[int]int
来源：http://hz.hfpthk.cn/gtotrdxshq.html

Ruby: // 手写 Hash
来源：http://hz.jinyuanbaomall.cn/gtpabqaesd.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.shzxlz.cn/gtesgqjsyy.html

[N08] 生成全排列
来源：http://hz.zhongyouzk.top/gtcagczyua.html


<!-- 参考信息 -->