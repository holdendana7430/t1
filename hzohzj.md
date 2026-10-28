代发 wailian999

================================================================================
来源：http://hz.sweek.top/gthaftoign.html

K. JSON 与序列化
来源：http://hz.nanxuanxn.top/gtwnloksxa.html

================================================================================
来源：http://hz.nwbrower.top/gtuylbgjak.html

[K01] 对象转 JSON 字符串
来源：http://hz.vqdsnc.cn/gtgvaenvwg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.meibo888.top/gtuaiuatcz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.guannengcc.top/gtlboyqpkl.html

JS:   JSON.stringify(obj)
来源：http://hz.jiagoushi.top/gtclwqdvvy.html

TS:   JSON.stringify(obj)
来源：http://hz.tianlin.xyz/gtnhvwnsau.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.cdnleiting.top/gtkbbobimo.html

Go:   json.Marshal(obj)
来源：http://hz.iojbl.cn/gtlumyunuj.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.guowangkeji.top/gtgmsywgnd.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.cashguo.top/gtendceplk.html

[K02] JSON 字符串转对象
来源：http://hz.ywan-chungtsiang.top/gtrytavjms.html

Py:   json.loads(s)
来源：http://hz.yj202588.top/gtyzmzsycd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.snrcjt.cn/gteajewtxg.html

JS:   JSON.parse(s)
来源：http://hz.xuetiantiany.cn/gtcblndbig.html

TS:   JSON.parse(s)
来源：http://hz.cheryme.top/gtkbaivnfb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.shangyingyoupin.top/gtkztsylaz.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.52xcode.cn/gtpgouuztk.html

Ruby: JSON.parse(s)
来源：http://hz.jinghuilouyu.cn/gtuhijghjz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hammf.cn/gtlmolngxo.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ivvv.top/gtoizkfjgt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhijiandao.cn/gtvhuiegph.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.shanyushiyangkeji.top/gtnkwtvoki.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.9152youxi.cn/gtcfsqcpag.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cashguo.top/gtxrbgeyas.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yueranfly.top/gtowikgtrv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.sufxvd.cn/gtilnnlfvp.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ybcxt.top/gtqifnwljg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.sweek.top/gthhrorxuj.html

[K04] 读取 JSON 文件
来源：http://hz.zdqjudy.top/gtcrbykpsi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hfpthk.cn/gtbetpclkr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.sysykeji.top/gtxzmxjsvy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sufxvd.cn/gtrcspmxjn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yj20258888.top/gttsfpuefv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.iojbl.cn/gtatufksng.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yueranfly.top/gtlxganmwu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.gogol.net.cn/gtltbgztuk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hfpthk.cn/gtwnzgkocw.html

[K05] 深拷贝对象
来源：http://hz.xingfuxueyuan.xyz/gthtzzmrrd.html

Py:   copy.deepcopy(obj)
来源：http://hz.nanxinkj.top/gtfrvpwvjd.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hfpthk.cn/gtswlmircd.html

JS:   structuredClone(obj)
来源：http://hz.nanxuanxn.top/gtwuawxsfp.html

TS:   structuredClone(obj)
来源：http://hz.zycfv.cn/gtqubvslno.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ydjk.org.cn/gtpoqepoiy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hnqzz.top/gtrwhegfuo.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhoulong.xyz/gtnzbtfpxx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.tanke756.top/gtxfystetz.html

[K06] 解析 URL 查询串
来源：http://hz.gogol.net.cn/gtuoqovzev.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhijiandao.cn/gtsqwnunag.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.ivvv.top/gtwrwqclfy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cashguo.top/gtaulhlqku.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hfpthk.cn/gtcchtxzop.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yanxiufei.cn/gttlkczbum.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.gotoacloud.top/gtzmycvndo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.fzhhl.top/gtgritfowi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.pengpengdd.cyou/gtuabdmqkv.html

[K07] 进制转换
来源：http://hz.yangfankeji.com/gtpojfdeta.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hongshengwenyu.top/gtvaxdhpma.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.pycfn.com/gtgcwqfkkz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.daria6918.cn/gtlvlrlajl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.dianchejie.cn/gtngsnapbs.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yuanzhike.top/gtgpxokwpq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.gzhubu.top/gtvhplhpct.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jiagoushi.top/gtcoxqjogj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.havefunace.top/gtborkljcf.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yj20258888.top/gtqpmcbjwi.html

Py:   pickle.dumps(obj)
来源：http://hz.cdnleiting.top/gtakwbsxyu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.shanyushiyangtech.top/gtdtldgfbe.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.cashguo.top/gtfsvmqhvr.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.chenjidiqi.icu/gteqobqhyl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yueranfly.top/gtixqkcvsn.html

Go:   encoding/gob
来源：http://hz.xingfuxueyuan.xyz/gtxdcqbtcm.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhijiandao.cn/gtznnxggdb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.havefunace.top/gtafjwmzmf.html

================================================================================
来源：http://hz.zhijiandao.cn/gtuikcxmdg.html

L. 网络请求
来源：http://hz.yongpay.top/gthzbbwmjb.html

================================================================================
来源：http://hz.jiagoushi.top/gtifcerclb.html

[L01] 发送 GET 请求
来源：http://hz.daria6918.cn/gtwdwquobf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.quarkkingdee.top/gtqiyeizty.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.guannengcc.top/gthpdlmwzx.html

JS:   await fetch(url)
来源：http://hz.mhx1999.top/gtrfgdygvo.html

TS:   await fetch(url)
来源：http://hz.yonumen.top/gtvnxhymqv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.pycfn.com/gtjgjxbsza.html

Go:   resp, err := http.Get(url)
来源：http://hz.daxiang520.top/gtoszyvaoy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jiagoushi.top/gtncwcosad.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.dashuyun.cn/gtkcqivnmq.html

[L02] 发送 POST JSON
来源：http://hz.cucudq.cn/gtnvgutytd.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.nanxinkj.top/gtgxbpqdnl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.gaohongyu789.top/gtgheuzewt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.mhx1999.top/gtwwpvpwtv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhijiandao.cn/gthixxdbfv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.chenlongwang.top/gtnvvepkkn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.dianchejie.cn/gtfkasxijn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.0kj1m.cn/gthfjjghqm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yvedp.cn/gtpeulknia.html

[L03] 设置自定义请求头
来源：http://hz.jyoumei.cn/gtiqkqxtys.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zycfv.cn/gtkwtcozdv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.birdmap.top/gtajzsibum.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xuanzx.com/gtyeleaibv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.wangshuangyany.cn/gtznvfvyeb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.snrcjt.cn/gthuaikzeg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ydzc1.top/gtontigrrz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.bjfxy.top/gtoggehbje.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.daria6918.cn/gtloczeftz.html

[L04] 设置超时
来源：http://hz.shangyingyoupin.top/gtjzcgwqpn.html

Py:   requests.get(url, timeout=5)
来源：http://hz.quarkkingdee.top/gtclxhhpbx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.tianlin.xyz/gtyvdzkomh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.kuanghao11.cn/gtrrglanoo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.tanke756.top/gtzzlapmdn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.chenzaomai.com/gtzdxflthp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.sweek.top/gtqfywmzhv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ivvv.top/gtqpqaiwbx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.haohaochexian.top/gtqiqcgtnr.html

[L05] 上传文件（multipart）
来源：http://hz.cashguo.top/gtgdmxnivm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.meibo888.top/gtbmopygpp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jinghuilouyu.cn/gtwajngonk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ehwqpu.com/gttgylseoa.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.sweek.top/gtqftuqdxq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hammf.cn/gtlaozfudf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhijiandao.cn/gtfucujdxh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.chenzaomai.com/gtowccxrxv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.gaohongyu789.top/gtujjnvgni.html

[L06] 解析响应为 JSON
来源：http://hz.ybcxt.top/gttetfnjkf.html

Py:   resp.json()
来源：http://hz.daria6918.cn/gtzqlmpiww.html

PHP:  json_decode($body, true);
来源：http://hz.shanyushiyangtech.top/gtvdaylncz.html

JS:   await resp.json()
来源：http://hz.kuanghao11.cn/gtqocgwinr.html

TS:   await resp.json()
来源：http://hz.zhiwuduotai.top/gtcvvuovgh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yj20258888.top/gtsbfaltvt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.52xcode.cn/gtskvfrcpz.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhaomingkeji.xyz/gtumxbphio.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.birdmap.top/gtboxkpdtm.html

[L07] 处理 HTTP 状态码
来源：http://hz.yj20258.top/gtxlhiphkw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yangfankeji.com/gtckrgdlsb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.fengsongda.top/gtibjnhkoz.html

JS:   resp.ok;  resp.status
来源：http://hz.sweek.top/gtjupqebjz.html

TS:   resp.ok;  resp.status
来源：http://hz.yangfankeji.com/gtohehtfjh.html

Java: resp.statusCode()
来源：http://hz.feifeiyinyue.top/gtrevhhcpu.html

Go:   resp.StatusCode
来源：http://hz.mhx1999.top/gtcmrqbazy.html

Ruby: resp.code.to_i
来源：http://hz.zycfv.cn/gtkbiapywc.html

C#:   (int)resp.StatusCode
来源：http://hz.zhongyouzk.top/gtyspfmyri.html

[L08] 并发请求多个地址
来源：http://hz.smart0.xyz/gthplxkesy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.aizwys.cn/gtcwfyyfvk.html

PHP:  curl_multi_init() 系列
来源：http://hz.xinyue.icu/gtkybdcfxw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.pycfn.com/gtrineagen.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xziqi.cn/gtsyjjhamx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.shangyingyoupin.top/gttepcsmvk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yuxming.cn/gtyxmwmqgp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.xinyue.icu/gtinvaexaw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xziqi.cn/gtdqwlqbvo.html

================================================================================
来源：http://hz.ppjwa.cn/gtqivovosa.html

M. 命令行 / 进程 / 环境
来源：http://hz.shangyingyoupin.top/gtwfjlgwlz.html

================================================================================
来源：http://hz.hnqzz.top/gtkaxrzvae.html

[M01] 读取命令行参数
来源：http://hz.shangyingyoupin.top/gtryukzdoq.html

Py:   sys.argv[1:]
来源：http://hz.ivvv.top/gtuwlfsodc.html

PHP:  $argv;  $argc;
来源：http://hz.jyoumei.cn/gtjfumjwxm.html

JS:   process.argv.slice(2)
来源：http://hz.yonumen.top/gtvkpvrinb.html

TS:   process.argv.slice(2)
来源：http://hz.snrcjt.cn/gtxobqjgsq.html

Java: args 数组（main 方法参数）
来源：http://hz.dashuyun.cn/gtncdscxua.html

Go:   os.Args[1:]
来源：http://hz.vqdsnc.cn/gtuiivjpaw.html

Ruby: ARGV
来源：http://hz.fengsongda.top/gtcirdhqrr.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yj20258888.top/gtkgilqpvi.html

[M02] 读取环境变量
来源：http://hz.aibaodan.cn/gtywbjglkz.html

Py:   os.environ.get("HOME")
来源：http://hz.zhongyouzk.top/gtwblffvxu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jinghuilouyu.cn/gtoivxogkr.html

JS:   process.env.HOME
来源：http://hz.redwolf501.top/gtrndczjze.html

TS:   process.env.HOME
来源：http://hz.ydjk.org.cn/gtdxraiemx.html

Java: System.getenv("HOME")
来源：http://hz.zhoulong.xyz/gtffpadccs.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.ydjk.org.cn/gthpiciwgl.html

Ruby: ENV["HOME"]
来源：http://hz.zhiwuduotai.top/gttxygfaxh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xziqi.cn/gtdhzuoulc.html

[M03] 执行外部命令
来源：http://hz.xuetiantiany.cn/gtkbtpcxwd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.hongshengwenyu.top/gtfsiacszl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yvedp.cn/gtzompsnvb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.chenjidiqi.icu/gtptlzcsun.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.chenlongwang.top/gtfhioljow.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hnqzz.top/gtsiifwuab.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.c1oappe.top/gtxtsocdol.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.ydjk.org.cn/gtnujadeuk.html

C#:   Process.Start("ls", "-l");
来源：http://hz.iojbl.cn/gtmkpobqhd.html

[M04] 获取当前工作目录
来源：http://hz.guannengcc.top/gtpwuwqybn.html

Py:   os.getcwd()
来源：http://hz.zhongyouzk.top/gtdgljoxvj.html

PHP:  getcwd();
来源：http://hz.0kj1m.cn/gtkkcpansq.html

JS:   process.cwd()
来源：http://hz.sufxvd.cn/gtdviowitk.html

TS:   process.cwd()
来源：http://hz.wangdashe.top/gtycwuipgb.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yuanzhike.top/gtrosgnqof.html

Go:   os.Getwd()
来源：http://hz.yuanzhike.top/gtdtahkumw.html

Ruby: Dir.pwd
来源：http://hz.zhaomingkeji.xyz/gtuexwbsax.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ehwqpu.com/gtykhkucxr.html

[M05] 设置退出码
来源：http://hz.hfpthk.cn/gthghhilme.html

Py:   sys.exit(1)
来源：http://hz.pengpengdd.cyou/gtzcewfdpc.html

PHP:  exit(1);
来源：http://hz.cucudq.cn/gtpnmcjfct.html

JS:   process.exit(1)
来源：http://hz.0kj1m.cn/gtjscosnlj.html

TS:   process.exit(1)
来源：http://hz.xingfuxueyuan.xyz/gtaalprnkj.html

Java: System.exit(1)
来源：http://hz.aizwys.cn/gtubguwolx.html

Go:   os.Exit(1)
来源：http://hz.chenlongwang.top/gtmnaxhdao.html

Ruby: exit 1
来源：http://hz.dianchejie.cn/gtdxzkrnrf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.cqqwz.cn/gtzrczdcnj.html

[M06] 向标准错误输出
来源：http://hz.sweek.top/gtrvytpvfu.html

Py:   print("err", file=sys.stderr)
来源：http://hz.birdmap.top/gtksesokfd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hnqzz.top/gtmywrymvx.html

JS:   console.error("err")
来源：http://hz.tanke756.top/gtmnbodkiy.html

TS:   console.error("err")
来源：http://hz.yuanzhike.top/gtspdvmilc.html

Java: System.err.println("err")
来源：http://hz.sufxvd.cn/gtjahljmfb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.dianchejie.cn/gtemcotsbh.html

Ruby: warn "err"
来源：http://hz.ydzc1.top/gtfgfcsmyr.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.pycfn.com/gtsiinutmu.html

[M07] 判断是否为主入口
来源：http://hz.yuanzhike.top/gtqgujkvmd.html

Py:   if __name__ == "__main__":
来源：http://hz.gotoacloud.top/gtuwavkrka.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xylfe.cn/gttmubswog.html

JS:   require.main === module
来源：http://hz.quarkkingdee.top/gtxjaqbeey.html

TS:   require.main === module
来源：http://hz.chenlongwang.top/gtazgmmjff.html

Java: public static void main(String[] args)
来源：http://hz.meibo888.top/gtpmghvkuo.html

Go:   func main()
来源：http://hz.yonumen.top/gtpajexupy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.bjfxy.top/gtescjwsoq.html

C#:   static void Main(string[] args)
来源：http://hz.kuanghao11.cn/gtkgrixwca.html

[M08] 获取系统与运行时信息
来源：http://hz.snrcjt.cn/gtcywyjjsq.html

Py:   platform.system();  platform.python_version()
来源：http://hz.aibaodan.cn/gtwdkjhhaf.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.gotoacloud.top/gtvyulrxdd.html

JS:   process.platform;  process.version
来源：http://hz.cqqwz.cn/gtcevcthwx.html

TS:   process.platform;  process.version
来源：http://hz.ybcxt.top/gtjjhmxkly.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.bjfxy.top/gtlygfsgoo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.smart0.xyz/gtlqniekgy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hnxiangtu.top/gtkmsenrsl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.mhx1999.top/gthtnpkzpj.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtisrjionx.html

N. 数据结构与算法
来源：http://hz.shzxlz.cn/gtlgqjtaam.html

================================================================================
来源：http://hz.zhengqikj.top/gtptcjqjbj.html

[N01] 二分查找（有序数组）
来源：http://hz.yanxiufei.cn/gtzaaltkih.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zdqjudy.top/gtwylbwsby.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.fzhhl.top/gtrkqpgeek.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhongyouzk.top/gtzyvumvsa.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.nanxuanxn.top/gturnoacan.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.chenjidiqi.icu/gtfkwpdqvt.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jqgfzy.top/gtpthsadni.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xuetiantiany.cn/gtxigfmuox.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.haohaochexian.top/gtztjtdpzf.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.cdnleiting.top/gtifyfoaih.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xylfe.cn/gtjzzkgpzw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.xziqi.cn/gtmsargyrm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xuanzx.com/gtnhuvfard.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.52xcode.cn/gtisbwrtfe.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yj20258888.top/gtoxgosjlk.html

Go:   slices.Sort(arr)
来源：http://hz.jianghu66.top/gtldbqibrj.html

Ruby: arr.sort
来源：http://hz.haohaochexian.top/gtpjfwjvek.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.gaohongyu789.top/gtpzdblpcq.html

[N03] 快速排序（分治示例）
来源：http://hz.jinqigfzy.top/gtiaawketq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.kuanghao11.cn/gtfaixujvf.html

PHP:  // 递归实现，或用 usort
来源：http://hz.ivvv.top/gtonahpjgj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.9152youxi.cn/gtwsbadwey.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cqqwz.cn/gtrpxhille.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.andypj.xyz/gtwlmhpqms.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.mhx1999.top/gtyaozzbjk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.chenzaomai.com/gtjcphxkjb.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.c1oappe.top/gtytsniogi.html

[N04] 斐波那契数列
来源：http://hz.jqgufenzy.top/gtfnpkaily.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yuxming.cn/gtrgkkmoov.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhaomingkeji.xyz/gtkmbjdcei.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhaomingkeji.xyz/gtkwtgsmgl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yanxiufei.cn/gtkdbqlrcy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yonumen.top/gtobiezzse.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.xziqi.cn/gtidmckkfm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hnqzz.top/gtwclrizmf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hfpthk.cn/gtjsslkdbj.html

[N05] 最大公约数
来源：http://hz.xingfuxueyuan.xyz/gtpwrlyqjz.html

Py:   math.gcd(a, b)
来源：http://hz.aizwys.cn/gtzowxzvok.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.52xcode.cn/gtrocphkar.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yuxming.cn/gtrzirwcpt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ydjk.org.cn/gtksgqxuwu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.shanyushiyangtech.top/gtnzbhqvst.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hammf.cn/gtndqespso.html

Ruby: a.gcd(b)
来源：http://hz.ppjwa.cn/gtfsyahdte.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.quarkkingdee.top/gtrgqyouom.html

[N06] 判断回文字符串
来源：http://hz.jinghuilouyu.cn/gtiksnspvo.html

Py:   s == s[::-1]
来源：http://hz.jiagoushi.top/gtfvenddzn.html

PHP:  $s === strrev($s);
来源：http://hz.pycfn.com/gtfxcjqwxn.html

JS:   s === [...s].reverse().join("")
来源：http://hz.cdnleiting.top/gtxqtezzae.html

TS:   s === [...s].reverse().join("")
来源：http://hz.gaohongyu789.top/gtgyvjdyur.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.meibo888.top/gtmajoknov.html

Go:   // 双指针从两端比较
来源：http://hz.andypj.xyz/gttxdjxpfs.html

Ruby: s == s.reverse
来源：http://hz.pengpengdd.cyou/gtoyuynyhs.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.daria6918.cn/gtrgyllcje.html

[N07] 两数之和（返回下标）
来源：http://hz.jinyuanbaomall.cn/gtlyrwqkgc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ydzc1.top/gteekxriat.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zhiwuduotai.top/gthwupnkhk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.dashuyun.cn/gtriiwfxtc.html

TS:   // 手写 Map<string, number>
来源：http://hz.chenlongwang.top/gtjmxaptnl.html

Java: // 手写 HashMap
来源：http://hz.vqdsnc.cn/gtfhlgwulj.html

Go:   // 手写 map[int]int
来源：http://hz.cashguo.top/gtrvocxzfk.html

Ruby: // 手写 Hash
来源：http://hz.zhixingplan.top/gtoutqzzav.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yj20258.top/gtlmcpsadw.html

[N08] 生成全排列
来源：http://hz.nanxinkj.top/gtprnznice.html

Py:   itertools.permutations(arr)
来源：http://hz.ydjk.org.cn/gtryuzplip.html

PHP:  // 手写递归交换
来源：http://hz.daxiang520.top/gtzdfpsyjq.html

JS:   // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gtxtsarmgt.html

TS:   // 手写回溯递归
来源：http://hz.sufxvd.cn/gtrhqevhsq.html

Java: // 手写回溯递归
来源：http://hz.jqgfzy.top/gtzihdxffe.html

Go:   // 手写回溯递归
来源：http://hz.jqgufenzy.top/gtwnqyishb.html

Ruby: arr.permutation.to_a
来源：http://hz.yuxming.cn/gtbnjvtmwn.html

C#:   // 手写回溯递归
来源：http://hz.zhijiandao.cn/gtaornhmin.html


<!-- 参考信息 -->