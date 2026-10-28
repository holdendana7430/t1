代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.gogol.net.cn/gtoqkzwdkg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.daria6918.cn/gtoceivuwt.html

JS:   JSON.stringify(obj)
来源：http://hz.ydzc1.top/gtizrawwnk.html

TS:   JSON.stringify(obj)
来源：http://hz.fzhhl.top/gtlwszfyhh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.gotoacloud.top/gthqufcdbu.html

Go:   json.Marshal(obj)
来源：http://hz.fengsongda.top/gtotdgssov.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jqgfzy.top/gtrrrnamqa.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jianghu66.top/gtlamrpcpd.html

[K02] JSON 字符串转对象
来源：http://hz.ydzc1.top/gtysiayqlq.html

Py:   json.loads(s)
来源：http://hz.bjfxy.top/gtnwizvloh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.tian-w.cn/gthmaloytc.html

JS:   JSON.parse(s)
来源：http://hz.pengpengdd.cyou/gtxvajbnlw.html

TS:   JSON.parse(s)
来源：http://hz.hammf.cn/gtohjngbqx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.meibo888.top/gtobddvbdd.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.gzhubu.top/gtwgahklel.html

Ruby: JSON.parse(s)
来源：http://hz.smart0.xyz/gtphontrfx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jinqigufen.top/gtcdtzbkzm.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.havefunace.top/gtbwlxbqsn.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ivvv.top/gtqqxytqcl.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.dashuyun.cn/gteauwcdqk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shanyushiyangtech.top/gtakuvkmqg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zycfv.cn/gtmplaksfv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zhengqikj.top/gtnsswkodg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ywan-chungtsiang.top/gtrtrnnuzi.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ywan-chungtsiang.top/gtnyszjlku.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.birdmap.top/gtavtjkqhp.html

[K04] 读取 JSON 文件
来源：http://hz.shangyingyoupin.top/gtnxnyhuyi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jiagoushi.top/gtmiuvfhhn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shanyushiyangkeji.top/gtjvhxjstp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.bjfxy.top/gtcrvfbsdo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cqqwz.cn/gtrkznhqnf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.gzhubu.top/gtpxirjodq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.52xcode.cn/gtykzyixdy.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.wangdashe.top/gthqwwxlln.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hnqzz.top/gtukeyodvd.html

[K05] 深拷贝对象
来源：http://hz.zdqjudy.top/gtqmngoxux.html

Py:   copy.deepcopy(obj)
来源：http://hz.xylfe.cn/gtwhckpvao.html

PHP:  unserialize(serialize($obj));
来源：http://hz.mhx1999.top/gtsqaygawe.html

JS:   structuredClone(obj)
来源：http://hz.shanyushiyangkeji.top/gthpcqcejt.html

TS:   structuredClone(obj)
来源：http://hz.ydzc1.top/gthpjtfoge.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hongshengwenyu.top/gtqjclxekf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yuanzhike.top/gtfjkrcawn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.cheryme.top/gtzxvzetmn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.cheryme.top/gtlzdrmhff.html

[K06] 解析 URL 查询串
来源：http://hz.yongpay.top/gtikawfrvk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.cqqwz.cn/gtxzpqnpxi.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yvedp.cn/gtfayqjnkd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.kuanghao11.cn/gtibcqeskj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jlsjyb.cn/gtztspyclv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jinqigfzy.top/gtswcmrgaw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.ehwqpu.com/gtecmjszbg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.sweek.top/gtcmxebwdl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.gaohongyu789.top/gtnlotdtlm.html

[K07] 进制转换
来源：http://hz.gzhubu.top/gtakepxxys.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cqqwz.cn/gtwvzfvmbl.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.cqqwz.cn/gtyicpqtrm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.kuanghao11.cn/gtfjexmrvj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.xingfuxueyuan.xyz/gtihzxeqeq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.quarkkingdee.top/gtavytgigg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.mhx1999.top/gtwasrkrad.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jinqigufen.top/gtoyxrpaia.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.feifeiyinyue.top/gtxinsnxmd.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jqgfzy.top/gteacjvjxg.html

Py:   pickle.dumps(obj)
来源：http://hz.zycfv.cn/gtnhlysmdz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zhijiandao.cn/gtgemeodog.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.316326.xyz/gtymnbsnba.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yuxming.cn/gtbdvznjem.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.gaohongyu789.top/gtuvxaxkxu.html

Go:   encoding/gob
来源：http://hz.hongshengwenyu.top/gtjrhcpooo.html

Ruby: Marshal.dump(obj)
来源：http://hz.andypj.xyz/gtsjfzkxkv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.fengsongda.top/gtbmavpgwo.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtjiemsjvy.html

L. 网络请求
来源：http://hz.yuxming.cn/gtdysiublh.html

================================================================================
来源：http://hz.wangdashe.top/gthtdyffsh.html

[L01] 发送 GET 请求
来源：http://hz.yvedp.cn/gtholuuyxz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jinyuanbaomall.cn/gtvnkvzajz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.daria6918.cn/gtjvxtowzl.html

JS:   await fetch(url)
来源：http://hz.nwbrower.top/gturkqecsb.html

TS:   await fetch(url)
来源：http://hz.shzxlz.cn/gtkdthnxbc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ydjk.org.cn/gtheebsaqb.html

Go:   resp, err := http.Get(url)
来源：http://hz.sufxvd.cn/gtjeegfpll.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhixingplan.top/gtqfgtzoaa.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.cucudq.cn/gtgoanzcym.html

[L02] 发送 POST JSON
来源：http://hz.jinqigufen.top/gthpameunz.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jinqigfzy.top/gtngswqldg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.gzhubu.top/gtefoylijg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.vqdsnc.cn/gtzgdefgch.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yj20258888.top/gtcycxdlph.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.cdnleiting.top/gtbclijprc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jinghuilouyu.cn/gtkhifvaxa.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jinyuanbaomall.cn/gthgmdseno.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.gogol.net.cn/gtqmhmdhcz.html

[L03] 设置自定义请求头
来源：http://hz.hnqzz.top/gtxbdhedlj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jqgufenzy.top/gttemxxioo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.smart0.xyz/gtdhiyvmsg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.meibo888.top/gtcvtyufgh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhoulong.xyz/gtkugptmxv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.birdmap.top/gtkbgsxfja.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jianghu66.top/gtblseniiu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yuxming.cn/gtvdsfzlki.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.shzxlz.cn/gtfpnsjoys.html

[L04] 设置超时
来源：http://hz.xuetiantiany.cn/gtywqtbxel.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ydzc1.top/gtdevckpne.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.0kj1m.cn/gtwhhbwpur.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yongpay.top/gtrvrdqzle.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zycfv.cn/gtgezqoola.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hongshengwenyu.top/gtbfijotvm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.smart0.xyz/gtivwuvvjv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.snrcjt.cn/gtbthldbbr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.nanxinkj.top/gtufrviavb.html

[L05] 上传文件（multipart）
来源：http://hz.hnqzz.top/gteofkxsne.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.chenjidiqi.icu/gttdcjmrzg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yonumen.top/gtwukvunvv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hnqzz.top/gtcdotzssh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.xinyue.icu/gtvbqatcru.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.guannengcc.top/gtbnjomawn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ehwqpu.com/gtenwavovf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.aizwys.cn/gtebizfunx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.ehwqpu.com/gtpmrvrkcr.html

[L06] 解析响应为 JSON
来源：http://hz.yj202588.top/gtqpddiihf.html

Py:   resp.json()
来源：http://hz.snrcjt.cn/gtxqfofhcd.html

PHP:  json_decode($body, true);
来源：http://hz.havefunace.top/gtzitwzzvp.html

JS:   await resp.json()
来源：http://hz.316326.xyz/gtgjjglahh.html

TS:   await resp.json()
来源：http://hz.ydzc1.top/gtcibwbvca.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.kuanghao11.cn/gtwdosqbvy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.shzxlz.cn/gtwenxufmr.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ybcxt.top/gtdwszrepy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.fengsongda.top/gtdfxmzqiy.html

[L07] 处理 HTTP 状态码
来源：http://hz.aizwys.cn/gtoxjhgyki.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.cdnleiting.top/gtlrghukon.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ydjk.org.cn/gtzvbubdrm.html

JS:   resp.ok;  resp.status
来源：http://hz.kuanghao11.cn/gtnjrfsopc.html

TS:   resp.ok;  resp.status
来源：http://hz.xinyue.icu/gthbdpmguh.html

Java: resp.statusCode()
来源：http://hz.316326.xyz/gtlwbsmunt.html

Go:   resp.StatusCode
来源：http://hz.yueranfly.top/gtbarftluc.html

Ruby: resp.code.to_i
来源：http://hz.gotoacloud.top/gtwomgxbta.html

C#:   (int)resp.StatusCode
来源：http://hz.yvedp.cn/gtnalyrhuq.html

[L08] 并发请求多个地址
来源：http://hz.xingfuxueyuan.xyz/gtgcrtcawm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.gogol.net.cn/gtnneamjhc.html

PHP:  curl_multi_init() 系列
来源：http://hz.hongshengwenyu.top/gtnqhxtmbe.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.feifeiyinyue.top/gtjofbhgjs.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.guannengcc.top/gtmopzfrrp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.shangyingyoupin.top/gtxbjxxdni.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yangfankeji.com/gtngjypgkz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.daxiang520.top/gtgkbgjlpv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jinyuanbaomall.cn/gtxmlqcdkv.html

================================================================================
来源：http://hz.hnqzz.top/gtlknrihns.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhoulong.xyz/gtgcyejbll.html

================================================================================
来源：http://hz.dashuyun.cn/gtjelltdvc.html

[M01] 读取命令行参数
来源：http://hz.yangfankeji.com/gtizyohdte.html

Py:   sys.argv[1:]
来源：http://hz.jyoumei.cn/gtrikesacz.html

PHP:  $argv;  $argc;
来源：http://hz.smart0.xyz/gtqsldyndd.html

JS:   process.argv.slice(2)
来源：http://hz.yj20258.top/gtlsfnpkgh.html

TS:   process.argv.slice(2)
来源：http://hz.mhx1999.top/gtdrqzembv.html

Java: args 数组（main 方法参数）
来源：http://hz.cdnleiting.top/gtziwmrwco.html

Go:   os.Args[1:]
来源：http://hz.sufxvd.cn/gtxrpawkhi.html

Ruby: ARGV
来源：http://hz.hywenlv.cn/gtrchjhaql.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yonumen.top/gtvfowsjnh.html

[M02] 读取环境变量
来源：http://hz.wangdashe.top/gtydtrllyu.html

Py:   os.environ.get("HOME")
来源：http://hz.chenjidiqi.icu/gtlffzhsbd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.fzhhl.top/gtowbaypbf.html

JS:   process.env.HOME
来源：http://hz.redwolf501.top/gtxzcslmpw.html

TS:   process.env.HOME
来源：http://hz.c1oappe.top/gthspgnrgo.html

Java: System.getenv("HOME")
来源：http://hz.shangyingyoupin.top/gtjkafxivy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.aibaodan.cn/gtjfwmrxvk.html

Ruby: ENV["HOME"]
来源：http://hz.yueranfly.top/gtzghqhvti.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zdqjudy.top/gtpldrlbic.html

[M03] 执行外部命令
来源：http://hz.hongshengwenyu.top/gtkvmdxchf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.c1oappe.top/gtrkridtlv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.guowangkeji.top/gtnjaptpea.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.feifeiyinyue.top/gtixpzcdiu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yuxming.cn/gtsvmswtso.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.snrcjt.cn/gtiuxueokk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.xinyue.icu/gtuvafkwxw.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.0kj1m.cn/gtlkbxfdtj.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hammf.cn/gtdumesubx.html

[M04] 获取当前工作目录
来源：http://hz.aibaodan.cn/gtwzsliiya.html

Py:   os.getcwd()
来源：http://hz.jyoumei.cn/gttaxiphrc.html

PHP:  getcwd();
来源：http://hz.zhoulong.xyz/gtefvytqtt.html

JS:   process.cwd()
来源：http://hz.pycfn.com/gtdvcmouqx.html

TS:   process.cwd()
来源：http://hz.cashguo.top/gtsggfsyxb.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.c1oappe.top/gtgqgenfwg.html

Go:   os.Getwd()
来源：http://hz.jinqigfzy.top/gttbljizhd.html

Ruby: Dir.pwd
来源：http://hz.ehwqpu.com/gtiwdlmzyy.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.birdmap.top/gtgfcovubv.html

[M05] 设置退出码
来源：http://hz.aibaodan.cn/gtxchoezbw.html

Py:   sys.exit(1)
来源：http://hz.guowangkeji.top/gtvyvmvgsf.html

PHP:  exit(1);
来源：http://hz.chenzaomai.com/gtreqssooj.html

JS:   process.exit(1)
来源：http://hz.snrcjt.cn/gtzqorximo.html

TS:   process.exit(1)
来源：http://hz.iojbl.cn/gtvyotgqpn.html

Java: System.exit(1)
来源：http://hz.ehwqpu.com/gtnntsuply.html

Go:   os.Exit(1)
来源：http://hz.aibaodan.cn/gthielfzrs.html

Ruby: exit 1
来源：http://hz.hnxiangtu.top/gtjgxwcimf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.sxryk.cn/gtpiqafusm.html

[M06] 向标准错误输出
来源：http://hz.tianlin.xyz/gtyzsmiiuf.html

Py:   print("err", file=sys.stderr)
来源：http://hz.0kj1m.cn/gthjiwyunz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ybcxt.top/gtterizcsv.html

JS:   console.error("err")
来源：http://hz.shanyushiyangtech.top/gtezcggnzj.html

TS:   console.error("err")
来源：http://hz.birdmap.top/gtqbsqvvvg.html

Java: System.err.println("err")
来源：http://hz.andypj.xyz/gtugnvwxan.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.svipenyu.cn/gtvqqmwfoy.html

Ruby: warn "err"
来源：http://hz.chenjidiqi.icu/gtsoakuist.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ybcxt.top/gtrpwruviw.html

[M07] 判断是否为主入口
来源：http://hz.zhongyouzk.top/gtkpacuitx.html

Py:   if __name__ == "__main__":
来源：http://hz.hnxiangtu.top/gthvuujdhe.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.pengpengdd.cyou/gtkqlahvrm.html

JS:   require.main === module
来源：http://hz.ydjk.org.cn/gtpxcavhyh.html

TS:   require.main === module
来源：http://hz.jinghuilouyu.cn/gtpcjqzkfj.html

Java: public static void main(String[] args)
来源：http://hz.cheryme.top/gtuyvmdkzz.html

Go:   func main()
来源：http://hz.zhongyouzk.top/gtpfjavxtx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cheryme.top/gtcqaeztru.html

C#:   static void Main(string[] args)
来源：http://hz.xuetiantiany.cn/gtvrmkhjjm.html

[M08] 获取系统与运行时信息
来源：http://hz.c1oappe.top/gtzqrgsntw.html

Py:   platform.system();  platform.python_version()
来源：http://hz.316326.xyz/gteffeaitk.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.mhx1999.top/gtrpkmrrzi.html

JS:   process.platform;  process.version
来源：http://hz.kuanghao11.cn/gtipftbjdq.html

TS:   process.platform;  process.version
来源：http://hz.hnxiangtu.top/gtjurcyiwf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.ydzc1.top/gtqwhzvdrq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jqgfzy.top/gtjdmkmojz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.fzhhl.top/gtsdcumbdr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ydjk.org.cn/gtmpqosrjn.html

================================================================================
来源：http://hz.yonumen.top/gtcfwrqjrh.html

N. 数据结构与算法
来源：http://hz.ywan-chungtsiang.top/gtjyupxhzx.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtcivzgcwb.html

[N01] 二分查找（有序数组）
来源：http://hz.gzhubu.top/gtfntuicpo.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.iojbl.cn/gtbdhjxojz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.xziqi.cn/gtiberncpt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yj202588.top/gtnpnuiluq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xuanzx.com/gtdapvugfs.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.gzhubu.top/gtivjhpczx.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.shuidangran.top/gtuwqvwuds.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.shangyingyoupin.top/gtddolcomn.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xziqi.cn/gtujzkqvar.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jqgufenzy.top/gtmlfxluht.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yangfankeji.com/gtyysgthxz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.shanyushiyangtech.top/gtbkdqebhn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhongyouzk.top/gtqaaaqqzu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xuanzx.com/gtimeuesyc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jqgfzy.top/gtkcmpnniz.html

Go:   slices.Sort(arr)
来源：http://hz.yangfankeji.com/gtjavhhmtu.html

Ruby: arr.sort
来源：http://hz.pengpengdd.cyou/gtoqnfvmno.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.hysaishi.cn/gtewyybesh.html

[N03] 快速排序（分治示例）
来源：http://hz.cheryme.top/gtctzcmlio.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.meibo888.top/gtzirrnwuy.html

PHP:  // 递归实现，或用 usort
来源：http://hz.andypj.xyz/gtsfqxukcl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.0kj1m.cn/gtgxeofckw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinqigufen.top/gtkaorsqlw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.316326.xyz/gtqmqlwjyb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.gogol.net.cn/gtutecwjay.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.kuanghao11.cn/gtclvuwtvs.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.gaohongyu789.top/gtqvxjqqxj.html

[N04] 斐波那契数列
来源：http://hz.gaohongyu789.top/gtaqtujpgj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xuetiantiany.cn/gtinwrmmzh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.havefunace.top/gtmnwjzmjm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.havefunace.top/gtpolchhiq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yvedp.cn/gtihdclsdx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jiagoushi.top/gtnamlsbsu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yvedp.cn/gtiumoltfl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.0kj1m.cn/gtlikytnxa.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.gogol.net.cn/gtgzzyhssf.html

[N05] 最大公约数
来源：http://hz.xylfe.cn/gtdxvlzjzw.html

Py:   math.gcd(a, b)
来源：http://hz.meibo888.top/gtldjzakas.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.smart0.xyz/gtheedpxlv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.kuanghao11.cn/gthtfhiecg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shanyushiyangkeji.top/gteqozwaxi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.xuanzx.com/gtxrelsraw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.ivvv.top/gtzhsvhhwr.html

Ruby: a.gcd(b)
来源：http://hz.yonumen.top/gtdcyyxwtd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.hywenlv.cn/gtmdvsbdlf.html

[N06] 判断回文字符串
来源：http://hz.xziqi.cn/gtwccqytvv.html

Py:   s == s[::-1]
来源：http://hz.yj20258888.top/gtvpohawey.html

PHP:  $s === strrev($s);
来源：http://hz.pycfn.com/gtqozsaxjj.html

JS:   s === [...s].reverse().join("")
来源：http://hz.andypj.xyz/gtxzrfblhx.html

TS:   s === [...s].reverse().join("")
来源：http://hz.cucudq.cn/gthjhrbgdk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhengqikj.top/gtgslmyuwd.html

Go:   // 双指针从两端比较
来源：http://hz.zhaomingkeji.xyz/gtgvnatpgb.html

Ruby: s == s.reverse
来源：http://hz.yanxiufei.cn/gtkpzbavcp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.ehwqpu.com/gtzqwzfswp.html

[N07] 两数之和（返回下标）
来源：http://hz.jyoumei.cn/gtuuxfytyj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.316326.xyz/gtnqgwejhl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.havefunace.top/gtcezyhnet.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ydzc1.top/gtwdbjaiwi.html

TS:   // 手写 Map<string, number>
来源：http://hz.xuanzx.com/gtbdpllrpu.html

Java: // 手写 HashMap
来源：http://hz.316326.xyz/gtspfkehwn.html

Go:   // 手写 map[int]int
来源：http://hz.daxiang520.top/gtgkadmklq.html

Ruby: // 手写 Hash
来源：http://hz.hongshengwenyu.top/gtrrylzldy.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.havefunace.top/gtcoyengnh.html

[N08] 生成全排列
来源：http://hz.quarkkingdee.top/gttfkxywci.html

Py:   itertools.permutations(arr)
来源：http://hz.ywan-chungtsiang.top/gtyroviooo.html

PHP:  // 手写递归交换
来源：http://hz.zhiwuduotai.top/gtnqxxvbbi.html

JS:   // 手写回溯递归
来源：http://hz.jqgufenzy.top/gtrvasmcuw.html

TS:   // 手写回溯递归
来源：http://hz.hnxiangtu.top/gtcywujqww.html

Java: // 手写回溯递归
来源：http://hz.nanxuanxn.top/gtyirqqzcs.html

Go:   // 手写回溯递归
来源：http://hz.sufxvd.cn/gtcdjfgvjc.html

Ruby: arr.permutation.to_a
来源：http://hz.nanxinkj.top/gtgdnvatpm.html

C#:   // 手写回溯递归
来源：http://hz.jlsjyb.cn/gtfuvywmzf.html

[N09] 栈与队列
来源：http://hz.jinqigufen.top/gtetxgoovu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhoulong.xyz/gtlltfjsia.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zhoulong.xyz/gtttidkqjz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jqgfzy.top/gtlupmrgkk.html


<!-- 参考信息 -->