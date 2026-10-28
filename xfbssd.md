代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yueranfly.top/gtuagzcjhl.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yj20258.top/gtwrzdxyuq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.kuanghao11.cn/gtpaoabwoa.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.gogol.net.cn/gtyidysvyj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhixingplan.top/gttzvyhcco.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.dashuyun.cn/gtjxygdxoi.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.9152youxi.cn/gtxtuusive.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xuetiantiany.cn/gtacnlwhcm.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtqpemcmsz.html

K. JSON 与序列化
来源：http://hz.feifeiyinyue.top/gthcgippik.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtvebdbfaa.html

[K01] 对象转 JSON 字符串
来源：http://hz.redwolf501.top/gtforylpvb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.cdnleiting.top/gtcxtmcfql.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhengqikj.top/gtfvswieuw.html

JS:   JSON.stringify(obj)
来源：http://hz.ydjk.org.cn/gtmslbpyue.html

TS:   JSON.stringify(obj)
来源：http://hz.zhoulong.xyz/gtrgdtiria.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhongyouzk.top/gtmunofvie.html

Go:   json.Marshal(obj)
来源：http://hz.jlsjyb.cn/gtsuyzsegp.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.quarkkingdee.top/gtcndwqyxl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jlsjyb.cn/gtisgasbfg.html

[K02] JSON 字符串转对象
来源：http://hz.ydzc1.top/gtdbaumazn.html

Py:   json.loads(s)
来源：http://hz.guannengcc.top/gtvaceubwv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.nanxuanxn.top/gtzesoiwho.html

JS:   JSON.parse(s)
来源：http://hz.kuanghao11.cn/gtlghsumod.html

TS:   JSON.parse(s)
来源：http://hz.snrcjt.cn/gtijcmwqdx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.shuidangran.top/gtcuukghad.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xylfe.cn/gtmhkyrkkg.html

Ruby: JSON.parse(s)
来源：http://hz.nwbrower.top/gtmmfbgfkt.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhaomingkeji.xyz/gtsmakhaku.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.bjfxy.top/gtsevkxtje.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ivvv.top/gtchfkruqm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhixingplan.top/gtmzfjpkwx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.chenjidiqi.icu/gtpgwqiuow.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhijiandao.cn/gtnsqpckdr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.havefunace.top/gtgkcierdy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yj20258.top/gtseberjnz.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.tanke756.top/gtkkvwedpq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.aizwys.cn/gtybvypfii.html

[K04] 读取 JSON 文件
来源：http://hz.feifeiyinyue.top/gtsqdtgifl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zhoulong.xyz/gtpfrmcxad.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhengqikj.top/gtqtgdxeak.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ybcxt.top/gtbhbucozg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.feifeiyinyue.top/gthqkzstle.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.iojbl.cn/gturoodmss.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yongpay.top/gtageyikfa.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.dianchejie.cn/gtpwodqzaa.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jqgufenzy.top/gtcjlnumdb.html

[K05] 深拷贝对象
来源：http://hz.bjfxy.top/gtjsmdluwt.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhongyouzk.top/gtvuyzjimf.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hfpthk.cn/gtaydeviiq.html

JS:   structuredClone(obj)
来源：http://hz.bjfxy.top/gtfroyxruz.html

TS:   structuredClone(obj)
来源：http://hz.nwbrower.top/gtbrotnppt.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.gotoacloud.top/gtlujvaaqx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.gaohongyu789.top/gtlowzmpez.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yuanzhike.top/gtierenbfn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.feifeiyinyue.top/gtwbivebny.html

[K06] 解析 URL 查询串
来源：http://hz.yvedp.cn/gthoexlxta.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zycfv.cn/gtyhvffpae.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.havefunace.top/gtzdsquatr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.snrcjt.cn/gtirtpfarv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.havefunace.top/gtexzrrsqu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.52xcode.cn/gtkpzbfghe.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hongshengwenyu.top/gtszicgqjz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yanxiufei.cn/gtrckhfsti.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ybcxt.top/gtqapyqksb.html

[K07] 进制转换
来源：http://hz.xingfuxueyuan.xyz/gtcssneyjn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.kuanghao11.cn/gtecouqfio.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.pycfn.com/gtgdlztdlh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.wangshuangyany.cn/gtpfcgoczd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.gogol.net.cn/gtgkaidliz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.chenzaomai.com/gthnxoxemb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.guannengcc.top/gtfnqyeoca.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ywan-chungtsiang.top/gtnzmubkxe.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hongshengwenyu.top/gtdpdywijt.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yj202588.top/gtttfebsis.html

Py:   pickle.dumps(obj)
来源：http://hz.yueranfly.top/gtgeyylxfe.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.cashguo.top/gtejozuspn.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.nwbrower.top/gtadbtddio.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jianghu66.top/gtxztnnipt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.aizwys.cn/gtsygrbzfk.html

Go:   encoding/gob
来源：http://hz.sysykeji.top/gtrrcfgzyq.html

Ruby: Marshal.dump(obj)
来源：http://hz.nanxinkj.top/gtpexbkswo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.chenjidiqi.icu/gtlzxkxxuc.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtmizdeqbh.html

L. 网络请求
来源：http://hz.birdmap.top/gtbfoaaiff.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtcplrojos.html

[L01] 发送 GET 请求
来源：http://hz.gogol.net.cn/gtfookbrcr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cucudq.cn/gtdtywdsfn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ppjwa.cn/gtymgsijcv.html

JS:   await fetch(url)
来源：http://hz.cucudq.cn/gtniyaqjco.html

TS:   await fetch(url)
来源：http://hz.zycfv.cn/gtxazddjvu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ywan-chungtsiang.top/gtxjancyxg.html

Go:   resp, err := http.Get(url)
来源：http://hz.dianchejie.cn/gtprajexik.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yj20258888.top/gtljtjyagu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.chenlongwang.top/gtrlsbsoyx.html

[L02] 发送 POST JSON
来源：http://hz.ivvv.top/gthgdplhpj.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.52xcode.cn/gtgkcnbezs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.dianchejie.cn/gtnaevcxps.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ywan-chungtsiang.top/gtaiiuriuu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.fzhhl.top/gtijnnpqsh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.cashguo.top/gtdwiagsru.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.shuidangran.top/gtvtzobqxq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.nanxuanxn.top/gtqmjbkfor.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.haohaochexian.top/gtgfsnsqwf.html

[L03] 设置自定义请求头
来源：http://hz.xingfuxueyuan.xyz/gtmhaizina.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.smart0.xyz/gtmuvczlmy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.andypj.xyz/gtirpefrbz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shanyushiyangtech.top/gttytugavn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cdnleiting.top/gtelolhiak.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jqgufenzy.top/gtmbwyazut.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhoulong.xyz/gtqclpqyke.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.vqdsnc.cn/gtfucdndyv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.feifeiyinyue.top/gtwuqsdxvd.html

[L04] 设置超时
来源：http://hz.quarkkingdee.top/gtnpynahqn.html

Py:   requests.get(url, timeout=5)
来源：http://hz.andypj.xyz/gtocnhwnrh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.cheryme.top/gtwdbdeums.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhongyouzk.top/gteclbhvak.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.wangshuangyany.cn/gtufotbgdx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.fengsongda.top/gtlkteaall.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.shanyushiyangkeji.top/gtbddwivca.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yuanzhike.top/gtmqfjdrxw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hnqzz.top/gtwxgynyry.html

[L05] 上传文件（multipart）
来源：http://hz.52xcode.cn/gtipicqofb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yangfankeji.com/gtjpnnihhn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.hfpthk.cn/gttxvavsbh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ydzc1.top/gtzdqzqmzi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.andypj.xyz/gttpvqbjyn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.smart0.xyz/gtukxplcjw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.fengsongda.top/gtlespwucy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.hnxiangtu.top/gtkosrnmef.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jinqigufen.top/gtohaoagsn.html

[L06] 解析响应为 JSON
来源：http://hz.yonumen.top/gtihxyeqzt.html

Py:   resp.json()
来源：http://hz.tanke756.top/gtdjjuedax.html

PHP:  json_decode($body, true);
来源：http://hz.cashguo.top/gtkqnsnnhp.html

JS:   await resp.json()
来源：http://hz.andypj.xyz/gtwzubbzhx.html

TS:   await resp.json()
来源：http://hz.xuanzx.com/gtzheispru.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.cucudq.cn/gtatbpktxw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jinyuanbaomall.cn/gtnbtrqcuz.html

Ruby: JSON.parse(resp.body)
来源：http://hz.hnqzz.top/gtsmnhngwb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ybcxt.top/gtbjnxdhfp.html

[L07] 处理 HTTP 状态码
来源：http://hz.nwbrower.top/gtkejeqany.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yuanzhike.top/gtjipeexgi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.nanxinkj.top/gtccoxkzzr.html

JS:   resp.ok;  resp.status
来源：http://hz.ywan-chungtsiang.top/gtidigvurh.html

TS:   resp.ok;  resp.status
来源：http://hz.yongpay.top/gthptuvyjy.html

Java: resp.statusCode()
来源：http://hz.gaohongyu789.top/gtidteakco.html

Go:   resp.StatusCode
来源：http://hz.chenjidiqi.icu/gtyydzdldb.html

Ruby: resp.code.to_i
来源：http://hz.nwbrower.top/gtpbqyymaj.html

C#:   (int)resp.StatusCode
来源：http://hz.yvedp.cn/gtsmndhhev.html

[L08] 并发请求多个地址
来源：http://hz.hammf.cn/gtfzrlizan.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.redwolf501.top/gtwfemowvj.html

PHP:  curl_multi_init() 系列
来源：http://hz.jiagoushi.top/gtxzueunwz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zycfv.cn/gtydoojbyd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.redwolf501.top/gtoewsxptl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hywenlv.cn/gtcnmpktjv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yuanzhike.top/gtqeduberd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.316326.xyz/gtqigvkzlf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yuxming.cn/gttoacihcv.html

================================================================================
来源：http://hz.jinqigufen.top/gteujuenea.html

M. 命令行 / 进程 / 环境
来源：http://hz.gzhubu.top/gttgqfxtlj.html

================================================================================
来源：http://hz.chenlongwang.top/gthduvyzlo.html

[M01] 读取命令行参数
来源：http://hz.c1oappe.top/gtckstlksd.html

Py:   sys.argv[1:]
来源：http://hz.pycfn.com/gtlyczmmgp.html

PHP:  $argv;  $argc;
来源：http://hz.tian-w.cn/gthsgwznxh.html

JS:   process.argv.slice(2)
来源：http://hz.9152youxi.cn/gtoqheoujq.html

TS:   process.argv.slice(2)
来源：http://hz.svipenyu.cn/gtcgdcgnnx.html

Java: args 数组（main 方法参数）
来源：http://hz.tian-w.cn/gttwqqezot.html

Go:   os.Args[1:]
来源：http://hz.yvedp.cn/gtxgnguocr.html

Ruby: ARGV
来源：http://hz.aizwys.cn/gtvplamoyg.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ivvv.top/gtqmyctsgj.html

[M02] 读取环境变量
来源：http://hz.sufxvd.cn/gtmozjlnpt.html

Py:   os.environ.get("HOME")
来源：http://hz.sweek.top/gtztuctllc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.dashuyun.cn/gtdooobfqa.html

JS:   process.env.HOME
来源：http://hz.hnxiangtu.top/gtgveqahsi.html

TS:   process.env.HOME
来源：http://hz.jiagoushi.top/gtiteiqyrd.html

Java: System.getenv("HOME")
来源：http://hz.guannengcc.top/gthxhmaaan.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jyoumei.cn/gtbckeszpd.html

Ruby: ENV["HOME"]
来源：http://hz.jinghuilouyu.cn/gtcjguijeq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hammf.cn/gtnjyuhdry.html

[M03] 执行外部命令
来源：http://hz.sufxvd.cn/gtxxlryolg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.nwbrower.top/gtzrykvmvm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jinqigfzy.top/gtmvbeivsd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hammf.cn/gttwrvpzww.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xinyue.icu/gtfgytevif.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hysaishi.cn/gtkqsukhys.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.smart0.xyz/gtfuenwame.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.vqdsnc.cn/gtbttgyllr.html

C#:   Process.Start("ls", "-l");
来源：http://hz.mhx1999.top/gtnzofdexj.html

[M04] 获取当前工作目录
来源：http://hz.cqqwz.cn/gtxsfbmitr.html

Py:   os.getcwd()
来源：http://hz.sysykeji.top/gtegiarxkg.html

PHP:  getcwd();
来源：http://hz.gzhubu.top/gtokwsttza.html

JS:   process.cwd()
来源：http://hz.smart0.xyz/gtvfrwcxlq.html

TS:   process.cwd()
来源：http://hz.xuanzx.com/gtxqknoqdn.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.pengpengdd.cyou/gtnydwnxvr.html

Go:   os.Getwd()
来源：http://hz.yueranfly.top/gtgdmuzndp.html

Ruby: Dir.pwd
来源：http://hz.sweek.top/gtyrholwnv.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.havefunace.top/gteuofjqfa.html

[M05] 设置退出码
来源：http://hz.tian-w.cn/gteednqgpp.html

Py:   sys.exit(1)
来源：http://hz.ivvv.top/gtpflvxcsg.html

PHP:  exit(1);
来源：http://hz.sufxvd.cn/gtbpklgnik.html

JS:   process.exit(1)
来源：http://hz.yueranfly.top/gtnqdcofcl.html

TS:   process.exit(1)
来源：http://hz.ybcxt.top/gtvhmlcwen.html

Java: System.exit(1)
来源：http://hz.havefunace.top/gtnvdqjcbn.html

Go:   os.Exit(1)
来源：http://hz.yj20258888.top/gtxegfwwds.html

Ruby: exit 1
来源：http://hz.pycfn.com/gtqiotdahs.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zhengqikj.top/gtthjzgsjj.html

[M06] 向标准错误输出
来源：http://hz.yongpay.top/gteqhnxfoa.html

Py:   print("err", file=sys.stderr)
来源：http://hz.bjfxy.top/gtxicsegdi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jqgufenzy.top/gtjhxjgsmj.html

JS:   console.error("err")
来源：http://hz.cucudq.cn/gtrlvtdquf.html

TS:   console.error("err")
来源：http://hz.guannengcc.top/gtodnjrish.html

Java: System.err.println("err")
来源：http://hz.feifeiyinyue.top/gtpwsfmlak.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.pengpengdd.cyou/gtqodxniow.html

Ruby: warn "err"
来源：http://hz.shanyushiyangtech.top/gtnkuyfsny.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhixingplan.top/gtkmtzoctj.html

[M07] 判断是否为主入口
来源：http://hz.sufxvd.cn/gthyllxngt.html

Py:   if __name__ == "__main__":
来源：http://hz.52xcode.cn/gtuwbfbsuv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zdqjudy.top/gtzwmklurg.html

JS:   require.main === module
来源：http://hz.aibaodan.cn/gtjsupyaas.html

TS:   require.main === module
来源：http://hz.chenlongwang.top/gtanmuqqcd.html

Java: public static void main(String[] args)
来源：http://hz.xylfe.cn/gtauyqzosv.html

Go:   func main()
来源：http://hz.iojbl.cn/gtqtorvztd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jianghu66.top/gtmfdrygvl.html

C#:   static void Main(string[] args)
来源：http://hz.aizwys.cn/gtppmokzkk.html

[M08] 获取系统与运行时信息
来源：http://hz.hnxiangtu.top/gtluigksbi.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hfpthk.cn/gtqkylooop.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.tian-w.cn/gttjhejuke.html

JS:   process.platform;  process.version
来源：http://hz.xuanzx.com/gtcraymdro.html

TS:   process.platform;  process.version
来源：http://hz.xuanzx.com/gtydrvirer.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.tianlin.xyz/gtopcgqxkw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.hfpthk.cn/gtnbahcieb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.shzxlz.cn/gtusglltur.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.havefunace.top/gtqnxzpccw.html

================================================================================
来源：http://hz.cashguo.top/gtybejrneh.html

N. 数据结构与算法
来源：http://hz.nwbrower.top/gtgzcicosz.html

================================================================================
来源：http://hz.snrcjt.cn/gtibgbvcar.html

[N01] 二分查找（有序数组）
来源：http://hz.chenjidiqi.icu/gtwemeolkq.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hnxiangtu.top/gtltihfxsg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.cqqwz.cn/gtkjoqgmti.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yj202588.top/gtvvvrjymv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jqgufenzy.top/gtdxrbsjwq.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.ehwqpu.com/gtofykgvwq.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hfpthk.cn/gtbbfduscb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.cqqwz.cn/gtiioejznf.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.shzxlz.cn/gtlhcdoqnu.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.shuidangran.top/gtsjccxlsz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.kuanghao11.cn/gtrbjnizdt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.xylfe.cn/gtrxzmucyn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.0kj1m.cn/gtdsbjtpva.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gotoacloud.top/gtdnolruek.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jinyuanbaomall.cn/gtrvcbvdzg.html

Go:   slices.Sort(arr)
来源：http://hz.jinghuilouyu.cn/gteqefzngz.html

Ruby: arr.sort
来源：http://hz.zycfv.cn/gtmjjaknay.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.chenjidiqi.icu/gtoiqikqaw.html

[N03] 快速排序（分治示例）
来源：http://hz.chenjidiqi.icu/gtnaxbyerr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zycfv.cn/gtcsrsrjtr.html

PHP:  // 递归实现，或用 usort
来源：http://hz.bjfxy.top/gtubayykcz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tianlin.xyz/gtxhjiqwbv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gzhubu.top/gtidhomimr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.chenjidiqi.icu/gtgrtmpmwa.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhengqikj.top/gtrhtawlnn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhijiandao.cn/gtnjjldrmg.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.gzhubu.top/gtctyuqxgp.html

[N04] 斐波那契数列
来源：http://hz.redwolf501.top/gtyhhgygzt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yvedp.cn/gtjtutplvc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.bjfxy.top/gtgkdyvdje.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nwbrower.top/gtmajkbypz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jqgufenzy.top/gtvoprvjhw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.pycfn.com/gtlfvzhcen.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.shuidangran.top/gtpyqmvltk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.daxiang520.top/gtyfpajjqc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.cashguo.top/gtmzpskxjg.html

[N05] 最大公约数
来源：http://hz.andypj.xyz/gtvkmqhxso.html

Py:   math.gcd(a, b)
来源：http://hz.sufxvd.cn/gthshmybcf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jinghuilouyu.cn/gtqtacxbju.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cqqwz.cn/gtfyitcnyp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yonumen.top/gtgzzmmpge.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.daxiang520.top/gtgictikyw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yuanzhike.top/gtnwpwccdf.html

Ruby: a.gcd(b)
来源：http://hz.jlsjyb.cn/gtujqebstu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.xinyue.icu/gtgdzfzrqa.html

[N06] 判断回文字符串
来源：http://hz.jianghu66.top/gtiftaenxk.html

Py:   s == s[::-1]
来源：http://hz.dashuyun.cn/gttydofqlt.html

PHP:  $s === strrev($s);
来源：http://hz.guannengcc.top/gtbvpztacy.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yueranfly.top/gtwtjsqhhb.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yangfankeji.com/gtlbbxzacv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.xinyue.icu/gtneelfeeo.html

Go:   // 双指针从两端比较
来源：http://hz.vqdsnc.cn/gtdrrkzlnz.html

Ruby: s == s.reverse
来源：http://hz.meibo888.top/gtzcmqlggn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ybcxt.top/gtrqcojzuf.html

[N07] 两数之和（返回下标）
来源：http://hz.hnqzz.top/gtkfeerxvh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.52xcode.cn/gtbfjbtkgt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zhijiandao.cn/gttoejwqfg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.meibo888.top/gtyjkjewag.html

TS:   // 手写 Map<string, number>
来源：http://hz.c1oappe.top/gtccugthsg.html

Java: // 手写 HashMap
来源：http://hz.ivvv.top/gtvucamcrk.html

Go:   // 手写 map[int]int
来源：http://hz.sxryk.cn/gtnlitjxas.html

Ruby: // 手写 Hash
来源：http://hz.jinyuanbaomall.cn/gtjdcpiigu.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jinqigufen.top/gtwnuyblge.html

[N08] 生成全排列
来源：http://hz.hysaishi.cn/gthbscmsdk.html


<!-- 参考信息 -->