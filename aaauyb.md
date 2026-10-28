代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.nwbrower.top/gtzadcjpfc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.snrcjt.cn/gthvzmrjzd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.9152youxi.cn/gttjryaxuc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yj20258888.top/gtkjlagzgh.html

================================================================================
来源：http://hz.sweek.top/gttupcdpke.html

K. JSON 与序列化
来源：http://hz.hnxiangtu.top/gtentcawmz.html

================================================================================
来源：http://hz.hnxiangtu.top/gtxgxsifwv.html

[K01] 对象转 JSON 字符串
来源：http://hz.yvedp.cn/gtszrzowms.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ydjk.org.cn/gtbwdhfyub.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.pycfn.com/gtsldodncz.html

JS:   JSON.stringify(obj)
来源：http://hz.jqgfzy.top/gtzblzqtbg.html

TS:   JSON.stringify(obj)
来源：http://hz.jinqigfzy.top/gtjuqhhjmc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.9152youxi.cn/gtvsmvptds.html

Go:   json.Marshal(obj)
来源：http://hz.bjfxy.top/gtamzhaxzk.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.52xcode.cn/gtecczylld.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.sxryk.cn/gtpdwoztet.html

[K02] JSON 字符串转对象
来源：http://hz.jinqigfzy.top/gtkmubjrgh.html

Py:   json.loads(s)
来源：http://hz.jianghu66.top/gtyxtjzchz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zdqjudy.top/gtjvusrdla.html

JS:   JSON.parse(s)
来源：http://hz.iojbl.cn/gtubeodvvf.html

TS:   JSON.parse(s)
来源：http://hz.redwolf501.top/gtqnzdhdxl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yj20258.top/gtzspkqknc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ehwqpu.com/gtowtlwbvg.html

Ruby: JSON.parse(s)
来源：http://hz.jinqigufen.top/gtdulgnshq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hnxiangtu.top/gtpnseidsx.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zycfv.cn/gtkzmnpgkn.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.quarkkingdee.top/gtzdxywhwu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.shuidangran.top/gtoqrxxxsk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.mhx1999.top/gtwmngwwym.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj20258888.top/gtsrmidrwi.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yueranfly.top/gtajzulabl.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zycfv.cn/gtqnnotazj.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.vqdsnc.cn/gtkpsihprz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hysaishi.cn/gtrdwomxpq.html

[K04] 读取 JSON 文件
来源：http://hz.shzxlz.cn/gtppqplalx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.guowangkeji.top/gtzgkksnyr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ywan-chungtsiang.top/gtjtmraies.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.pengpengdd.cyou/gtiaxjwzsu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ppjwa.cn/gtsglbsjri.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.xinyue.icu/gtntgfpeej.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhijiandao.cn/gtkzkbasfr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.gaohongyu789.top/gtkguuwzai.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.shangyingyoupin.top/gtgcxfrvez.html

[K05] 深拷贝对象
来源：http://hz.nwbrower.top/gtfwkujlaf.html

Py:   copy.deepcopy(obj)
来源：http://hz.ehwqpu.com/gtjxiydcth.html

PHP:  unserialize(serialize($obj));
来源：http://hz.52xcode.cn/gturswrkdq.html

JS:   structuredClone(obj)
来源：http://hz.smart0.xyz/gtvnvjvhgn.html

TS:   structuredClone(obj)
来源：http://hz.tian-w.cn/gtrnjxuoai.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.shangyingyoupin.top/gtyctxvbme.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jinghuilouyu.cn/gtuukikgyp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yj20258.top/gtzbbxfryx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhaomingkeji.xyz/gtmbwzpkav.html

[K06] 解析 URL 查询串
来源：http://hz.vqdsnc.cn/gtveuuxkuf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xinyue.icu/gtispdekls.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xingfuxueyuan.xyz/gtujmcfomo.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xuetiantiany.cn/gthcgryxxa.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hongshengwenyu.top/gtrcmuefkr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yvedp.cn/gtxmtgjyjj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jianghu66.top/gttgklzglh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yongpay.top/gtaaqkfocu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.nwbrower.top/gtjvwdtqjo.html

[K07] 进制转换
来源：http://hz.jinqigfzy.top/gtiurdvmcn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ydjk.org.cn/gtjaqzzqwe.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.guowangkeji.top/gtufaslolg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.meibo888.top/gtfktulass.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.chenjidiqi.icu/gtgiarvvxt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.iojbl.cn/gtvrzwalqx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.vqdsnc.cn/gtykszuzfd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zhijiandao.cn/gtevdyiybs.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.fengsongda.top/gtsshcucda.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.xylfe.cn/gtasbfyika.html

Py:   pickle.dumps(obj)
来源：http://hz.smart0.xyz/gttfeiuqek.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.tianlin.xyz/gtexgusess.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.quarkkingdee.top/gtufingmuz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.dashuyun.cn/gtofsqxivi.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ybcxt.top/gtkuecqrus.html

Go:   encoding/gob
来源：http://hz.yvedp.cn/gtkaauymeh.html

Ruby: Marshal.dump(obj)
来源：http://hz.birdmap.top/gttymawhyx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.gaohongyu789.top/gtgrugxgqk.html

================================================================================
来源：http://hz.meibo888.top/gtsevfwmgq.html

L. 网络请求
来源：http://hz.shangyingyoupin.top/gtrbofxxza.html

================================================================================
来源：http://hz.zdqjudy.top/gtdxtncfor.html

[L01] 发送 GET 请求
来源：http://hz.nwbrower.top/gtmyxikhtd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.chenjidiqi.icu/gthfcwmgpn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.shanyushiyangkeji.top/gtvmbuovgd.html

JS:   await fetch(url)
来源：http://hz.dianchejie.cn/gttujvnbzg.html

TS:   await fetch(url)
来源：http://hz.mhx1999.top/gtvqlxfvdi.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hnxiangtu.top/gtimmlobcr.html

Go:   resp, err := http.Get(url)
来源：http://hz.52xcode.cn/gtyjpzqmdh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhoulong.xyz/gtitrtrvtj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.xingfuxueyuan.xyz/gthnznhmvg.html

[L02] 发送 POST JSON
来源：http://hz.hywenlv.cn/gtvnxmuinx.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.nanxinkj.top/gtktnbrncx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jyoumei.cn/gtnjsaqljq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jiagoushi.top/gtqcwaelrg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yangfankeji.com/gtvvapdmzs.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.0kj1m.cn/gtgkfpakxb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.shanyushiyangkeji.top/gtlmmkoxfc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.pycfn.com/gteyetbkmv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xinyue.icu/gtklgijfgi.html

[L03] 设置自定义请求头
来源：http://hz.jinghuilouyu.cn/gtcgghmwbr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ydjk.org.cn/gtiiiznads.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.feifeiyinyue.top/gtqzgqcyjm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhengqikj.top/gtnzrubehe.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yuxming.cn/gtlrpyzbjq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.fengsongda.top/gtznzctilk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.meibo888.top/gtrazlcexv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.cucudq.cn/gtkohjvmco.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.nwbrower.top/gtzenrnanw.html

[L04] 设置超时
来源：http://hz.52xcode.cn/gtbjfwwsez.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yueranfly.top/gtvlckcokk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.hfpthk.cn/gtdhwbmzon.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.daria6918.cn/gtneoxzqic.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yueranfly.top/gtpdtqwukl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.bjfxy.top/gtxfdmsbuu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.cucudq.cn/gtkzurgltc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.birdmap.top/gtznxmkuoh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yuanzhike.top/gtqnarizts.html

[L05] 上传文件（multipart）
来源：http://hz.hammf.cn/gtxbyztamd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.ydjk.org.cn/gtztngagjw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhiwuduotai.top/gtyousqtcj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.wangdashe.top/gtpgfojurh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.tianlin.xyz/gttpalmxpz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.gotoacloud.top/gtfntrifvl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.9152youxi.cn/gtcmwwvgdy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.smart0.xyz/gtztcodzws.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.52xcode.cn/gtptexdzzl.html

[L06] 解析响应为 JSON
来源：http://hz.xuetiantiany.cn/gtduqrlolm.html

Py:   resp.json()
来源：http://hz.guowangkeji.top/gtecnewenv.html

PHP:  json_decode($body, true);
来源：http://hz.vqdsnc.cn/gtkgnyovzv.html

JS:   await resp.json()
来源：http://hz.pycfn.com/gthchdortp.html

TS:   await resp.json()
来源：http://hz.xuanzx.com/gtbcsnomhg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.pycfn.com/gtqbdzorcz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.smart0.xyz/gtyadkaruo.html

Ruby: JSON.parse(resp.body)
来源：http://hz.cheryme.top/gtvcokhugm.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hammf.cn/gtdoiqpxgm.html

[L07] 处理 HTTP 状态码
来源：http://hz.nwbrower.top/gtzyrswmgm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.sysykeji.top/gtcgcahibs.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.daxiang520.top/gtonjfceqo.html

JS:   resp.ok;  resp.status
来源：http://hz.ppjwa.cn/gtgjxeeqgt.html

TS:   resp.ok;  resp.status
来源：http://hz.mhx1999.top/gtgjhbiuhc.html

Java: resp.statusCode()
来源：http://hz.pycfn.com/gtyezhniit.html

Go:   resp.StatusCode
来源：http://hz.tian-w.cn/gtvheharch.html

Ruby: resp.code.to_i
来源：http://hz.zhaomingkeji.xyz/gtfqietskq.html

C#:   (int)resp.StatusCode
来源：http://hz.chenjidiqi.icu/gtjojpkrpy.html

[L08] 并发请求多个地址
来源：http://hz.9152youxi.cn/gtyehggtxw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.tianlin.xyz/gtryufafvc.html

PHP:  curl_multi_init() 系列
来源：http://hz.andypj.xyz/gtdxzsslzm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sweek.top/gtgyoznshm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tian-w.cn/gtogdsmdzz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.bjfxy.top/gtozvewkit.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.aizwys.cn/gtwkjhpepy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.smart0.xyz/gtbvhidsia.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jinghuilouyu.cn/gttivbknhr.html

================================================================================
来源：http://hz.jiagoushi.top/gtrpvdwzba.html

M. 命令行 / 进程 / 环境
来源：http://hz.hfpthk.cn/gtfhkyscae.html

================================================================================
来源：http://hz.pycfn.com/gtnbvcqznj.html

[M01] 读取命令行参数
来源：http://hz.iojbl.cn/gtbjmjshhw.html

Py:   sys.argv[1:]
来源：http://hz.cucudq.cn/gtquzbzbci.html

PHP:  $argv;  $argc;
来源：http://hz.chenlongwang.top/gtuxprxybc.html

JS:   process.argv.slice(2)
来源：http://hz.yongpay.top/gtlvlbivxu.html

TS:   process.argv.slice(2)
来源：http://hz.jinqigfzy.top/gtdsfpzwrt.html

Java: args 数组（main 方法参数）
来源：http://hz.hysaishi.cn/gttcvcqnvr.html

Go:   os.Args[1:]
来源：http://hz.hnxiangtu.top/gtahsoyaxj.html

Ruby: ARGV
来源：http://hz.ywan-chungtsiang.top/gtoqpjmxrh.html

C#:   args 数组（Main 方法参数）
来源：http://hz.shanyushiyangtech.top/gtydzqwwmx.html

[M02] 读取环境变量
来源：http://hz.hnxiangtu.top/gthtcodhza.html

Py:   os.environ.get("HOME")
来源：http://hz.xylfe.cn/gtriglsjxs.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.daria6918.cn/gtegfkubew.html

JS:   process.env.HOME
来源：http://hz.guannengcc.top/gtypexdstq.html

TS:   process.env.HOME
来源：http://hz.fzhhl.top/gtkcmzozhg.html

Java: System.getenv("HOME")
来源：http://hz.hammf.cn/gtnpvaxyzh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hfpthk.cn/gtrzcmwkfx.html

Ruby: ENV["HOME"]
来源：http://hz.iojbl.cn/gtnpvggzgv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.aibaodan.cn/gtqhrotgbw.html

[M03] 执行外部命令
来源：http://hz.jqgufenzy.top/gtngunqibg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yonumen.top/gteekgosxb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.quarkkingdee.top/gtoyjwyysg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.gogol.net.cn/gtsdbmktbt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.kuanghao11.cn/gtiahsqzdo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.birdmap.top/gtmqwpaikt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yj202588.top/gtsvubmitx.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.svipenyu.cn/gtgeqooeav.html

C#:   Process.Start("ls", "-l");
来源：http://hz.guowangkeji.top/gtyglweazd.html

[M04] 获取当前工作目录
来源：http://hz.sufxvd.cn/gtknnyfhpy.html

Py:   os.getcwd()
来源：http://hz.hongshengwenyu.top/gtcnejpmii.html

PHP:  getcwd();
来源：http://hz.iojbl.cn/gtdrvgvkyf.html

JS:   process.cwd()
来源：http://hz.jqgufenzy.top/gtoaxkfvym.html

TS:   process.cwd()
来源：http://hz.vqdsnc.cn/gtyjanospd.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhoulong.xyz/gtymvqobda.html

Go:   os.Getwd()
来源：http://hz.chenlongwang.top/gtbwbcddxb.html

Ruby: Dir.pwd
来源：http://hz.dashuyun.cn/gtoaoymytj.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.aibaodan.cn/gtfnbmpekh.html

[M05] 设置退出码
来源：http://hz.yanxiufei.cn/gttbkkwade.html

Py:   sys.exit(1)
来源：http://hz.dashuyun.cn/gtizcewzfz.html

PHP:  exit(1);
来源：http://hz.sufxvd.cn/gtsbbpkcyx.html

JS:   process.exit(1)
来源：http://hz.xinyue.icu/gtievhnuzr.html

TS:   process.exit(1)
来源：http://hz.smart0.xyz/gtikwznzzx.html

Java: System.exit(1)
来源：http://hz.cashguo.top/gtxegaflhl.html

Go:   os.Exit(1)
来源：http://hz.jiagoushi.top/gtxzkhwofy.html

Ruby: exit 1
来源：http://hz.hfpthk.cn/gtzphivekk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.feifeiyinyue.top/gtrmjgnhmu.html

[M06] 向标准错误输出
来源：http://hz.dashuyun.cn/gtdrdbnowi.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yueranfly.top/gtevvyvexw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yonumen.top/gtjqixjtlt.html

JS:   console.error("err")
来源：http://hz.mhx1999.top/gtwbyjjotf.html

TS:   console.error("err")
来源：http://hz.shuidangran.top/gtpfiubngz.html

Java: System.err.println("err")
来源：http://hz.cashguo.top/gtzmsssvfj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.dashuyun.cn/gthgsspqkh.html

Ruby: warn "err"
来源：http://hz.zhixingplan.top/gtbkibvrhn.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.gotoacloud.top/gtfoierfdk.html

[M07] 判断是否为主入口
来源：http://hz.jinyuanbaomall.cn/gtisqzxopm.html

Py:   if __name__ == "__main__":
来源：http://hz.pycfn.com/gtpmjohovn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.hywenlv.cn/gtbubxxdce.html

JS:   require.main === module
来源：http://hz.jinyuanbaomall.cn/gthjolwjme.html

TS:   require.main === module
来源：http://hz.gotoacloud.top/gtbnwtotxd.html

Java: public static void main(String[] args)
来源：http://hz.ybcxt.top/gtixqvfqry.html

Go:   func main()
来源：http://hz.sufxvd.cn/gtbkpvhonj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yonumen.top/gtpzwzzcno.html

C#:   static void Main(string[] args)
来源：http://hz.jinqigufen.top/gtxijyoxmd.html

[M08] 获取系统与运行时信息
来源：http://hz.ehwqpu.com/gtyogeklrg.html

Py:   platform.system();  platform.python_version()
来源：http://hz.cheryme.top/gtpffjsgao.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.nwbrower.top/gtstznefpp.html

JS:   process.platform;  process.version
来源：http://hz.hnxiangtu.top/gttzudakso.html

TS:   process.platform;  process.version
来源：http://hz.birdmap.top/gtlcgbkqpt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.quarkkingdee.top/gthzgsefjt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.gaohongyu789.top/gtrjyutloc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.daria6918.cn/gtmiurvtpi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.tianlin.xyz/gtervinyjt.html

================================================================================
来源：http://hz.cashguo.top/gtuldjsmrc.html

N. 数据结构与算法
来源：http://hz.yueranfly.top/gtfhzpvxen.html

================================================================================
来源：http://hz.hfpthk.cn/gtfxnstxay.html

[N01] 二分查找（有序数组）
来源：http://hz.zhijiandao.cn/gtnzffrkmj.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yj202588.top/gtmicdkzhy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhoulong.xyz/gtkvoqmmer.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ppjwa.cn/gtpnrhsgmw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.nanxuanxn.top/gtopkuuzvr.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.shanyushiyangtech.top/gtcgenqhdo.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ywan-chungtsiang.top/gtjracddze.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yongpay.top/gtmiflwotg.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.daxiang520.top/gtahqkgcwj.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yongpay.top/gtsrojefxj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cdnleiting.top/gtqhukidvy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.xylfe.cn/gtcyxrexha.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yanxiufei.cn/gtmgjuuizi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nanxinkj.top/gtdxebohol.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.shanyushiyangtech.top/gtvyarmuqn.html

Go:   slices.Sort(arr)
来源：http://hz.xziqi.cn/gtcczrxrta.html

Ruby: arr.sort
来源：http://hz.zhengqikj.top/gtnmazqwcg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.chenlongwang.top/gtsrzfglsw.html

[N03] 快速排序（分治示例）
来源：http://hz.zycfv.cn/gtmgjomgjd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.aibaodan.cn/gthpshzsjn.html

PHP:  // 递归实现，或用 usort
来源：http://hz.iojbl.cn/gtwfqunphy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.redwolf501.top/gtfjuhqawe.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xuetiantiany.cn/gtwmapsdhf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.shangyingyoupin.top/gtonrhecbd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhongyouzk.top/gtozutinal.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.cashguo.top/gthwavpyfz.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.smart0.xyz/gtrlqgouxb.html

[N04] 斐波那契数列
来源：http://hz.ywan-chungtsiang.top/gtzftqcovq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.dianchejie.cn/gtgacoucnz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.daria6918.cn/gtcuuyodqq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.gaohongyu789.top/gtmqslcqae.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.birdmap.top/gttdbccxvt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.chenzaomai.com/gtxlpvgfip.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.sufxvd.cn/gthnxnrewg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ivvv.top/gthlfbmbyc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.sufxvd.cn/gtolppygdr.html

[N05] 最大公约数
来源：http://hz.yj202588.top/gtlimeusax.html

Py:   math.gcd(a, b)
来源：http://hz.yueranfly.top/gtrprisexv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.chenlongwang.top/gtaqdjeots.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gzhubu.top/gtdgpptamo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ydzc1.top/gthevsgkyt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.vqdsnc.cn/gtoulyzjjp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.sysykeji.top/gtnubifsdb.html

Ruby: a.gcd(b)
来源：http://hz.xingfuxueyuan.xyz/gtmxthxocb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.andypj.xyz/gtaoqedlhy.html

[N06] 判断回文字符串
来源：http://hz.jqgufenzy.top/gtuhjeibfb.html

Py:   s == s[::-1]
来源：http://hz.hongshengwenyu.top/gtzltarkrd.html

PHP:  $s === strrev($s);
来源：http://hz.chenzaomai.com/gtnwuirzso.html

JS:   s === [...s].reverse().join("")
来源：http://hz.9152youxi.cn/gtlnkjhguy.html

TS:   s === [...s].reverse().join("")
来源：http://hz.guowangkeji.top/gtxbjbocmt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.bjfxy.top/gtxszuvimw.html

Go:   // 双指针从两端比较
来源：http://hz.ydzc1.top/gtfdmaucbq.html

Ruby: s == s.reverse
来源：http://hz.shangyingyoupin.top/gttjcajvqr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.xuetiantiany.cn/gtujhbkpep.html

[N07] 两数之和（返回下标）
来源：http://hz.xingfuxueyuan.xyz/gtoxsbnyto.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.52xcode.cn/gtnnyiqouk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.bjfxy.top/gtrimvektm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.cdnleiting.top/gtuifbfeoi.html

TS:   // 手写 Map<string, number>
来源：http://hz.xuanzx.com/gtcdubqsoz.html

Java: // 手写 HashMap
来源：http://hz.shanyushiyangkeji.top/gtpxmuikyb.html

Go:   // 手写 map[int]int
来源：http://hz.hnxiangtu.top/gttnguqvdt.html

Ruby: // 手写 Hash
来源：http://hz.jinqigufen.top/gtzgpzsgqn.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.guowangkeji.top/gtaowbiqyk.html

[N08] 生成全排列
来源：http://hz.zdqjudy.top/gtkavilotw.html

Py:   itertools.permutations(arr)
来源：http://hz.zhongyouzk.top/gtdodchzkr.html

PHP:  // 手写递归交换
来源：http://hz.xuetiantiany.cn/gtioyxvwsp.html

JS:   // 手写回溯递归
来源：http://hz.gogol.net.cn/gtaxvaqgzh.html

TS:   // 手写回溯递归
来源：http://hz.dianchejie.cn/gtpybiextp.html


<!-- 参考信息 -->