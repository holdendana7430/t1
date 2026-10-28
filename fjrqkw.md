代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.andypj.xyz/gthirdpucg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yongpay.top/gtfebghzii.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zycfv.cn/gtwxftwxqd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yuanzhike.top/gtngvgcoxy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.cdnleiting.top/gtqhqrrmnb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.nanxuanxn.top/gtrpncbggt.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ybcxt.top/gtcllfnaue.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.daria6918.cn/gtcjxjnwex.html

================================================================================
来源：http://hz.sufxvd.cn/gtxoembiin.html

K. JSON 与序列化
来源：http://hz.ydjk.org.cn/gtodghmlnr.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtkopdqznu.html

[K01] 对象转 JSON 字符串
来源：http://hz.chenlongwang.top/gtaxkywzpj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shanyushiyangkeji.top/gtsdoxlizr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.nanxinkj.top/gteqqfxllr.html

JS:   JSON.stringify(obj)
来源：http://hz.haohaochexian.top/gtairnnrll.html

TS:   JSON.stringify(obj)
来源：http://hz.kuanghao11.cn/gthoahxxgv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hysaishi.cn/gtzlxsnxzt.html

Go:   json.Marshal(obj)
来源：http://hz.hnxiangtu.top/gtvzdkmoxw.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.xuetiantiany.cn/gteormsejx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.sxryk.cn/gtiznsrepw.html

[K02] JSON 字符串转对象
来源：http://hz.yuanzhike.top/gtjgkmojii.html

Py:   json.loads(s)
来源：http://hz.wangshuangyany.cn/gtpuetuipl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.0kj1m.cn/gtgdbrwwqs.html

JS:   JSON.parse(s)
来源：http://hz.chenlongwang.top/gtlqnahqdh.html

TS:   JSON.parse(s)
来源：http://hz.xuetiantiany.cn/gtbfcszhih.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yangfankeji.com/gtqztbbvix.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.aibaodan.cn/gttpzwndvr.html

Ruby: JSON.parse(s)
来源：http://hz.svipenyu.cn/gtrwvrpkok.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.nanxuanxn.top/gtdmrmibau.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.smart0.xyz/gtjpvjmygl.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.svipenyu.cn/gtzcbmirmo.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.316326.xyz/gtqyjxeakp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.svipenyu.cn/gtvtfgqxdt.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.vqdsnc.cn/gtcogepmod.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yj20258888.top/gtavybljpg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhengqikj.top/gtctqqnnuy.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.tian-w.cn/gtfqddosyw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.feifeiyinyue.top/gtcyntbymu.html

[K04] 读取 JSON 文件
来源：http://hz.ivvv.top/gtsbsvjtqp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.mhx1999.top/gtawiyuwhe.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.hysaishi.cn/gtkojahrjp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hywenlv.cn/gtnoqmqzxi.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hysaishi.cn/gtidhqvtcq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.havefunace.top/gtuwuvzvpr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.shuidangran.top/gtnhzntvog.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.nwbrower.top/gtityhkezl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.shzxlz.cn/gtusqodsya.html

[K05] 深拷贝对象
来源：http://hz.snrcjt.cn/gtbrmifjsg.html

Py:   copy.deepcopy(obj)
来源：http://hz.cqqwz.cn/gtensierjt.html

PHP:  unserialize(serialize($obj));
来源：http://hz.wangshuangyany.cn/gtqgieuxin.html

JS:   structuredClone(obj)
来源：http://hz.pengpengdd.cyou/gtyttblkoh.html

TS:   structuredClone(obj)
来源：http://hz.wangshuangyany.cn/gtesyjnmqz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jqgufenzy.top/gtjsyobzyj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ydjk.org.cn/gtyemlbqxy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ivvv.top/gtiuqyygcp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.gogol.net.cn/gtddpbmqmy.html

[K06] 解析 URL 查询串
来源：http://hz.316326.xyz/gttcanmssa.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xziqi.cn/gtmkrmkujk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xingfuxueyuan.xyz/gtsnfzvahk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.aibaodan.cn/gtvjvjcnym.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.pycfn.com/gtbidtfbgr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yanxiufei.cn/gtiftquhub.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.tanke756.top/gtjuqlllnw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jyoumei.cn/gtxblbmlxl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.sysykeji.top/gtglcichev.html

[K07] 进制转换
来源：http://hz.hongshengwenyu.top/gtpviouhep.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zdqjudy.top/gtzxzxkiuh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hnxiangtu.top/gtrqystgig.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hammf.cn/gtdjzgckao.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.snrcjt.cn/gtusijlajg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hammf.cn/gtpuhdlxeq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.chenlongwang.top/gttppdwadv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jyoumei.cn/gtfpfcoozt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.cucudq.cn/gtvfpeqobw.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ppjwa.cn/gtlyaniafu.html

Py:   pickle.dumps(obj)
来源：http://hz.tian-w.cn/gttvuljjyz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.meibo888.top/gtdqpdgami.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.nwbrower.top/gtfkxqsmri.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jiagoushi.top/gtvbdsfhke.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.snrcjt.cn/gtjmzygoax.html

Go:   encoding/gob
来源：http://hz.daxiang520.top/gtlxgskoxc.html

Ruby: Marshal.dump(obj)
来源：http://hz.sysykeji.top/gtanoazeqy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.andypj.xyz/gtqqauthhw.html

================================================================================
来源：http://hz.0kj1m.cn/gtocuogath.html

L. 网络请求
来源：http://hz.andypj.xyz/gtpisfcbml.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtyywchneg.html

[L01] 发送 GET 请求
来源：http://hz.meibo888.top/gtjigjmbkf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cqqwz.cn/gtzylhtvum.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hywenlv.cn/gtqwknpjzk.html

JS:   await fetch(url)
来源：http://hz.jinghuilouyu.cn/gtxrvbtvil.html

TS:   await fetch(url)
来源：http://hz.shangyingyoupin.top/gtvspgbtao.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jqgfzy.top/gtllasuteq.html

Go:   resp, err := http.Get(url)
来源：http://hz.wangshuangyany.cn/gtnhawcgpm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhaomingkeji.xyz/gthzezhncw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.pycfn.com/gtcnhibqil.html

[L02] 发送 POST JSON
来源：http://hz.vqdsnc.cn/gtirophpzq.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.snrcjt.cn/gtwqldypuq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.aizwys.cn/gtkvtirius.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jlsjyb.cn/gtkqzrxsjl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.fengsongda.top/gtncpgbbxq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.sysykeji.top/gtvgiyanzn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.guannengcc.top/gtztiruthq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jqgfzy.top/gtvxycrkqf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.meibo888.top/gtxzydmrow.html

[L03] 设置自定义请求头
来源：http://hz.xingfuxueyuan.xyz/gtkkiipqfm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jiagoushi.top/gtmlscbexo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.redwolf501.top/gtjoqcknfk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zdqjudy.top/gtkvtlxjmr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yuanzhike.top/gtoyubedso.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zycfv.cn/gtywdmraaw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.cucudq.cn/gtgafjatne.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.cashguo.top/gtdvjzsxni.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.nanxuanxn.top/gtachpdqyq.html

[L04] 设置超时
来源：http://hz.jqgfzy.top/gtpxvtcvod.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zdqjudy.top/gtvofigvar.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jyoumei.cn/gtlcjmquqn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yongpay.top/gtdyoroojn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yuanzhike.top/gtlzdgyxsc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hammf.cn/gtedylwxjx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.shzxlz.cn/gtqjxskamc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.dianchejie.cn/gtwouljhdj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhaomingkeji.xyz/gttnchunjg.html

[L05] 上传文件（multipart）
来源：http://hz.andypj.xyz/gthmrynxco.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.daria6918.cn/gtifcxfuuf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.shanyushiyangtech.top/gtcxfpigkx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zdqjudy.top/gtonrdsixk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yueranfly.top/gtxerteuzy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.pycfn.com/gttoqtcncb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.daria6918.cn/gtlskpzcry.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.cqqwz.cn/gtpbtbzxbt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.pengpengdd.cyou/gthpeipzfe.html

[L06] 解析响应为 JSON
来源：http://hz.redwolf501.top/gtsdbtyqii.html

Py:   resp.json()
来源：http://hz.yongpay.top/gtajwswnyr.html

PHP:  json_decode($body, true);
来源：http://hz.zhengqikj.top/gtoowqoerk.html

JS:   await resp.json()
来源：http://hz.xingfuxueyuan.xyz/gttgyniytk.html

TS:   await resp.json()
来源：http://hz.gaohongyu789.top/gttfjgglgf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.dashuyun.cn/gtixqrjxja.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.shuidangran.top/gtylbkopdp.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhoulong.xyz/gtspzbgdtp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.chenjidiqi.icu/gtfbgzpslf.html

[L07] 处理 HTTP 状态码
来源：http://hz.sysykeji.top/gtflysegzj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zycfv.cn/gtlrfiuayd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.cheryme.top/gtssbbyffo.html

JS:   resp.ok;  resp.status
来源：http://hz.zhoulong.xyz/gtwqdgefiq.html

TS:   resp.ok;  resp.status
来源：http://hz.hnqzz.top/gtzpxndtru.html

Java: resp.statusCode()
来源：http://hz.ydjk.org.cn/gtkpggnlui.html

Go:   resp.StatusCode
来源：http://hz.zycfv.cn/gtdiufzath.html

Ruby: resp.code.to_i
来源：http://hz.ywan-chungtsiang.top/gtptymodwc.html

C#:   (int)resp.StatusCode
来源：http://hz.chenlongwang.top/gtcgwgzsya.html

[L08] 并发请求多个地址
来源：http://hz.hongshengwenyu.top/gtrpjplrno.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.daria6918.cn/gtdofbdvme.html

PHP:  curl_multi_init() 系列
来源：http://hz.andypj.xyz/gtuaebumph.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cucudq.cn/gtnebelpjk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cdnleiting.top/gtsctsjtgv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.guannengcc.top/gtozeyowlu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.daria6918.cn/gtqdtlkbmw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.cheryme.top/gtymgbicur.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.cheryme.top/gtkzyrreos.html

================================================================================
来源：http://hz.ybcxt.top/gtvaprgprl.html

M. 命令行 / 进程 / 环境
来源：http://hz.yangfankeji.com/gtiuvnuivx.html

================================================================================
来源：http://hz.hnqzz.top/gtiqnrgpde.html

[M01] 读取命令行参数
来源：http://hz.cashguo.top/gttcqxixko.html

Py:   sys.argv[1:]
来源：http://hz.hfpthk.cn/gtaybhhfut.html

PHP:  $argv;  $argc;
来源：http://hz.hongshengwenyu.top/gtjgadyjib.html

JS:   process.argv.slice(2)
来源：http://hz.zdqjudy.top/gtwssxgpha.html

TS:   process.argv.slice(2)
来源：http://hz.kuanghao11.cn/gtorhtimzb.html

Java: args 数组（main 方法参数）
来源：http://hz.guowangkeji.top/gtkybzjxxv.html

Go:   os.Args[1:]
来源：http://hz.redwolf501.top/gtqvshhylz.html

Ruby: ARGV
来源：http://hz.xziqi.cn/gtmcuhtgfa.html

C#:   args 数组（Main 方法参数）
来源：http://hz.daria6918.cn/gtglnsyawj.html

[M02] 读取环境变量
来源：http://hz.fzhhl.top/gtfgdwxtet.html

Py:   os.environ.get("HOME")
来源：http://hz.xylfe.cn/gtyomtkmnl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hysaishi.cn/gtmrxflwjb.html

JS:   process.env.HOME
来源：http://hz.gzhubu.top/gtwvemqlhp.html

TS:   process.env.HOME
来源：http://hz.smart0.xyz/gtpohpbxze.html

Java: System.getenv("HOME")
来源：http://hz.gaohongyu789.top/gtzwxyrzin.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.snrcjt.cn/gtvvsadvan.html

Ruby: ENV["HOME"]
来源：http://hz.cashguo.top/gtdljrdpuu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jqgufenzy.top/gtphoyonle.html

[M03] 执行外部命令
来源：http://hz.shanyushiyangtech.top/gtgndwsiod.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.nanxinkj.top/gtngffdzse.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.gotoacloud.top/gtztqxaqyg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hfpthk.cn/gtauhohhrs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.cheryme.top/gtfezaecwz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.feifeiyinyue.top/gtlhskrjkd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.snrcjt.cn/gthkbozznh.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhengqikj.top/gtrfasybyj.html

C#:   Process.Start("ls", "-l");
来源：http://hz.9152youxi.cn/gtbmzjcklw.html

[M04] 获取当前工作目录
来源：http://hz.yuxming.cn/gtfvaripvi.html

Py:   os.getcwd()
来源：http://hz.fengsongda.top/gtkqqesfsq.html

PHP:  getcwd();
来源：http://hz.ydjk.org.cn/gtbriolzfu.html

JS:   process.cwd()
来源：http://hz.yj202588.top/gttwasguly.html

TS:   process.cwd()
来源：http://hz.dianchejie.cn/gtoeeoknnc.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hnxiangtu.top/gtqoobpiau.html

Go:   os.Getwd()
来源：http://hz.xinyue.icu/gtyenypoco.html

Ruby: Dir.pwd
来源：http://hz.hysaishi.cn/gtrbynpoeg.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jinyuanbaomall.cn/gtjynwnayh.html

[M05] 设置退出码
来源：http://hz.aizwys.cn/gtyvhelcft.html

Py:   sys.exit(1)
来源：http://hz.aibaodan.cn/gtmphigqug.html

PHP:  exit(1);
来源：http://hz.sufxvd.cn/gtvxzjadnv.html

JS:   process.exit(1)
来源：http://hz.xylfe.cn/gtipnlglqt.html

TS:   process.exit(1)
来源：http://hz.gaohongyu789.top/gtndxrjrab.html

Java: System.exit(1)
来源：http://hz.chenlongwang.top/gtxsiqladk.html

Go:   os.Exit(1)
来源：http://hz.yonumen.top/gtimeejnio.html

Ruby: exit 1
来源：http://hz.yuxming.cn/gtlmwykkuh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jianghu66.top/gtvnlirlax.html

[M06] 向标准错误输出
来源：http://hz.xylfe.cn/gtladpptxm.html

Py:   print("err", file=sys.stderr)
来源：http://hz.pycfn.com/gtbpzfljqp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.aibaodan.cn/gtjyjbpxqx.html

JS:   console.error("err")
来源：http://hz.hongshengwenyu.top/gtbsnsjssp.html

TS:   console.error("err")
来源：http://hz.hongshengwenyu.top/gtlxdpyudi.html

Java: System.err.println("err")
来源：http://hz.chenzaomai.com/gtikjvojje.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.cheryme.top/gtbzbywgzt.html

Ruby: warn "err"
来源：http://hz.zycfv.cn/gtsuhzjusy.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.shanyushiyangtech.top/gtgrwrcbph.html

[M07] 判断是否为主入口
来源：http://hz.yj202588.top/gtsxjqwrke.html

Py:   if __name__ == "__main__":
来源：http://hz.yj202588.top/gteyttnwtl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xinyue.icu/gtfvewyzbq.html

JS:   require.main === module
来源：http://hz.zhijiandao.cn/gtxigjflso.html

TS:   require.main === module
来源：http://hz.aizwys.cn/gtwhlourkt.html

Java: public static void main(String[] args)
来源：http://hz.cdnleiting.top/gtaeagahaw.html

Go:   func main()
来源：http://hz.gzhubu.top/gtmsgyuuus.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.quarkkingdee.top/gtcuqupsov.html

C#:   static void Main(string[] args)
来源：http://hz.jyoumei.cn/gtylckhleq.html

[M08] 获取系统与运行时信息
来源：http://hz.shanyushiyangtech.top/gtdsaonzts.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ydjk.org.cn/gtryamubqr.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.pengpengdd.cyou/gtejwikwsk.html

JS:   process.platform;  process.version
来源：http://hz.shangyingyoupin.top/gtzrsxrbej.html

TS:   process.platform;  process.version
来源：http://hz.jinyuanbaomall.cn/gtfvyuprdr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhaomingkeji.xyz/gtnajkgsow.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jianghu66.top/gtwizlqyxs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ivvv.top/gtewzvawmz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.vqdsnc.cn/gtuespnowk.html

================================================================================
来源：http://hz.yanxiufei.cn/gtfsnwtcyh.html

N. 数据结构与算法
来源：http://hz.jinqigufen.top/gtjcugrrnr.html

================================================================================
来源：http://hz.zhijiandao.cn/gtydfzqfaq.html

[N01] 二分查找（有序数组）
来源：http://hz.yongpay.top/gtpsaomnjf.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.sweek.top/gtpwdgfqqz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.redwolf501.top/gtlseovalg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.vqdsnc.cn/gtfzissiip.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sufxvd.cn/gtnodylltn.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhongyouzk.top/gtwtaiymfu.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jiagoushi.top/gtfcfmfklk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.wangdashe.top/gtkrvmtbaf.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.cucudq.cn/gtuzbtkwjj.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jianghu66.top/gtzeteatae.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ydjk.org.cn/gtqkgsgyoh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.tanke756.top/gtvrywqvuj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shangyingyoupin.top/gtddkputsd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.svipenyu.cn/gtizufplls.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jinghuilouyu.cn/gtdnwvkqbk.html

Go:   slices.Sort(arr)
来源：http://hz.zhaomingkeji.xyz/gtrvhzkpit.html

Ruby: arr.sort
来源：http://hz.jinghuilouyu.cn/gthssaahqg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jinghuilouyu.cn/gtxoqaskyu.html

[N03] 快速排序（分治示例）
来源：http://hz.guowangkeji.top/gtdxsekylq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.snrcjt.cn/gtxijzarxi.html

PHP:  // 递归实现，或用 usort
来源：http://hz.bjfxy.top/gtthnribdi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhixingplan.top/gtdcppsspw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shzxlz.cn/gtucuniqna.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinqigfzy.top/gtvwhwekhh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.hnqzz.top/gtdrgmlcia.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhijiandao.cn/gtqardanlx.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ivvv.top/gtdeecuruh.html

[N04] 斐波那契数列
来源：http://hz.wangdashe.top/gtofprwsgm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.shzxlz.cn/gtejfuykpl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.52xcode.cn/gtpqthxowc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shzxlz.cn/gtcewyzvay.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yvedp.cn/gtcwhfsjdf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yj20258.top/gtgernxnkk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hfpthk.cn/gtsiukquzu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ydjk.org.cn/gtrgijiybf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xuetiantiany.cn/gtsvqppgkm.html

[N05] 最大公约数
来源：http://hz.hongshengwenyu.top/gtqzaxiqiy.html

Py:   math.gcd(a, b)
来源：http://hz.daria6918.cn/gtiydhwhuy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.316326.xyz/gtdrwvhwox.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gotoacloud.top/gtwdihiebv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xingfuxueyuan.xyz/gtwxvfwqac.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zycfv.cn/gtcftfpyqr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.bjfxy.top/gtbuzdfcvs.html

Ruby: a.gcd(b)
来源：http://hz.zycfv.cn/gtihzafjcm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.andypj.xyz/gtkxfreneg.html

[N06] 判断回文字符串
来源：http://hz.yueranfly.top/gtjasnoixm.html

Py:   s == s[::-1]
来源：http://hz.yj20258.top/gtcqhicicp.html

PHP:  $s === strrev($s);
来源：http://hz.52xcode.cn/gtitficazb.html

JS:   s === [...s].reverse().join("")
来源：http://hz.kuanghao11.cn/gthmznlgiu.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ybcxt.top/gtyjpmdoqy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.9152youxi.cn/gthhrzhviq.html

Go:   // 双指针从两端比较
来源：http://hz.tianlin.xyz/gtrbturcsc.html

Ruby: s == s.reverse
来源：http://hz.guannengcc.top/gtnduyvwkv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.cdnleiting.top/gtjrsxqarr.html

[N07] 两数之和（返回下标）
来源：http://hz.chenlongwang.top/gtunpomkjj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.fzhhl.top/gtuaxgimev.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.ydjk.org.cn/gtrylyfywk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.havefunace.top/gtxqmbsgvm.html

TS:   // 手写 Map<string, number>
来源：http://hz.guowangkeji.top/gtdaxenlby.html

Java: // 手写 HashMap
来源：http://hz.chenjidiqi.icu/gthexhwcgf.html

Go:   // 手写 map[int]int
来源：http://hz.gotoacloud.top/gtkxozgznn.html

Ruby: // 手写 Hash
来源：http://hz.svipenyu.cn/gtnkfzyugg.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hammf.cn/gtuhalqaok.html

[N08] 生成全排列
来源：http://hz.jianghu66.top/gtgxprefcr.html


<!-- 参考信息 -->