代发 wailian999

================================================================================
来源：http://hz.tian-w.cn/gtmwgtirng.html

K. JSON 与序列化
来源：http://hz.0kj1m.cn/gtobvwpcfw.html

================================================================================
来源：http://hz.daxiang520.top/gtkxinealn.html

[K01] 对象转 JSON 字符串
来源：http://hz.ydjk.org.cn/gtxuvfgsoc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hnqzz.top/gtrpierljd.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.52xcode.cn/gtlsjbogko.html

JS:   JSON.stringify(obj)
来源：http://hz.gzhubu.top/gtbzfegziv.html

TS:   JSON.stringify(obj)
来源：http://hz.zhongyouzk.top/gtuhsgppxm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.tian-w.cn/gtivsdmjmn.html

Go:   json.Marshal(obj)
来源：http://hz.zdqjudy.top/gtrpwmvjut.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.sysykeji.top/gtoijznmrw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.shanyushiyangtech.top/gteecrgpok.html

[K02] JSON 字符串转对象
来源：http://hz.0kj1m.cn/gtneswokne.html

Py:   json.loads(s)
来源：http://hz.sysykeji.top/gthzjzyiqt.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.mhx1999.top/gtjgmehxbo.html

JS:   JSON.parse(s)
来源：http://hz.hfpthk.cn/gtdellcfwk.html

TS:   JSON.parse(s)
来源：http://hz.guowangkeji.top/gtutmzvyss.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.iojbl.cn/gtxaexvrdh.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yanxiufei.cn/gtgkaidemz.html

Ruby: JSON.parse(s)
来源：http://hz.zhoulong.xyz/gtqztckvdw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hysaishi.cn/gtmmrcfqrc.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ywan-chungtsiang.top/gtwbpnczbz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.pycfn.com/gtpxlyymwk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.tian-w.cn/gtmgprzvlx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zycfv.cn/gtighpyapi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhiwuduotai.top/gtygsnfyfy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.tianlin.xyz/gtwxonpacr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.cucudq.cn/gtofwjhjvm.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yueranfly.top/gtogseevkf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.guowangkeji.top/gtkvnzpesx.html

[K04] 读取 JSON 文件
来源：http://hz.ybcxt.top/gtfcsfeszg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.gzhubu.top/gtdkvnnnai.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ivvv.top/gtejkiphrr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.kuanghao11.cn/gtmylsgrtp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hywenlv.cn/gtjovnoowq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.pengpengdd.cyou/gtubepwbtl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.nanxuanxn.top/gtbmqtrwmj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.wangdashe.top/gtbbigzvhq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.feifeiyinyue.top/gtwfocbpmo.html

[K05] 深拷贝对象
来源：http://hz.ywan-chungtsiang.top/gtwcyteegh.html

Py:   copy.deepcopy(obj)
来源：http://hz.quarkkingdee.top/gttqwvrwhk.html

PHP:  unserialize(serialize($obj));
来源：http://hz.shangyingyoupin.top/gtwzghstaq.html

JS:   structuredClone(obj)
来源：http://hz.jqgfzy.top/gtlwhlztni.html

TS:   structuredClone(obj)
来源：http://hz.xuetiantiany.cn/gttqxdzeow.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.chenlongwang.top/gtnjszvruj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yuanzhike.top/gtzjekyfyu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.wangshuangyany.cn/gtinnzrkfj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.birdmap.top/gtowtabrjq.html

[K06] 解析 URL 查询串
来源：http://hz.ybcxt.top/gtxtzakvld.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ehwqpu.com/gtaecsyzos.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.cashguo.top/gtvxmdfzxz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ehwqpu.com/gthswcisie.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.chenlongwang.top/gtkcqgkert.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.nanxinkj.top/gtixjbzgyy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hysaishi.cn/gtaoajcadt.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhiwuduotai.top/gtdooiwldb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.xuanzx.com/gtpvzjujkr.html

[K07] 进制转换
来源：http://hz.birdmap.top/gtxoxvdgva.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jinqigfzy.top/gtczgycrvo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ehwqpu.com/gtagbwjzmd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.gotoacloud.top/gthdsfzyjw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.chenlongwang.top/gtfewuttdb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.redwolf501.top/gtiojwctvw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhiwuduotai.top/gtwajzepjv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jianghu66.top/gtoehkkwov.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.tian-w.cn/gtxntejyjo.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.sysykeji.top/gtfkssqysn.html

Py:   pickle.dumps(obj)
来源：http://hz.havefunace.top/gtywzslots.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jlsjyb.cn/gtqgdthftp.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hnxiangtu.top/gtgpnpakku.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.cheryme.top/gtfyuhnyjd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ydjk.org.cn/gtmlsrifxj.html

Go:   encoding/gob
来源：http://hz.jiagoushi.top/gtcaihovxd.html

Ruby: Marshal.dump(obj)
来源：http://hz.hysaishi.cn/gtxfpmweyn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.kuanghao11.cn/gtzomajaso.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtqmtvzndx.html

L. 网络请求
来源：http://hz.birdmap.top/gtrgxojzgi.html

================================================================================
来源：http://hz.xinyue.icu/gtxkyfvhvt.html

[L01] 发送 GET 请求
来源：http://hz.guowangkeji.top/gtikiqxhnu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.chenjidiqi.icu/gttqmasqer.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.shzxlz.cn/gtjxfprywy.html

JS:   await fetch(url)
来源：http://hz.fengsongda.top/gtnohbjfdq.html

TS:   await fetch(url)
来源：http://hz.chenlongwang.top/gtnbmkdnun.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.chenzaomai.com/gtxpyonqtz.html

Go:   resp, err := http.Get(url)
来源：http://hz.ywan-chungtsiang.top/gtcvcdnhvb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cashguo.top/gtcgwsytij.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.sufxvd.cn/gtzcpfhkre.html

[L02] 发送 POST JSON
来源：http://hz.wangshuangyany.cn/gtvisiuean.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.chenlongwang.top/gtqoprrqeb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.chenlongwang.top/gtvpsmjndx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhiwuduotai.top/gtvmjhqyqo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cqqwz.cn/gtbicjhvjl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.52xcode.cn/gtedljhbwp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.9152youxi.cn/gtrdfgexwg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.nanxuanxn.top/gtlonquxhq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yangfankeji.com/gtcfhystmv.html

[L03] 设置自定义请求头
来源：http://hz.haohaochexian.top/gtloqgaenz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.mhx1999.top/gteutmgctl.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yangfankeji.com/gtyjfasbng.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yongpay.top/gtzhwprwxb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.snrcjt.cn/gtqoqbrgqg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.iojbl.cn/gtjervjarj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jiagoushi.top/gtjugphfuz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.fzhhl.top/gtyzksaetw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhongyouzk.top/gtkgapqxvw.html

[L04] 设置超时
来源：http://hz.jqgfzy.top/gtsximzjrx.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zhiwuduotai.top/gtjaktgpdw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.xylfe.cn/gttbdllamb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.guannengcc.top/gtmqgmrsmt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ywan-chungtsiang.top/gtvmsxsgua.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.quarkkingdee.top/gtmdfizvxh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.smart0.xyz/gtdbfyketn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.aizwys.cn/gtgabpwlhz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yueranfly.top/gtkbgkiixl.html

[L05] 上传文件（multipart）
来源：http://hz.zhengqikj.top/gtssnnbvrh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.ywan-chungtsiang.top/gtfmhszaye.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jinqigfzy.top/gtctxcjsnw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.tanke756.top/gtjpfnqkqv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.xziqi.cn/gtjkgyikwo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.cqqwz.cn/gtkyjoryad.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jinqigfzy.top/gtadjuwqvb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yanxiufei.cn/gtaoxprxpp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhongyouzk.top/gtqlqtqbue.html

[L06] 解析响应为 JSON
来源：http://hz.jiagoushi.top/gtpjtpeyki.html

Py:   resp.json()
来源：http://hz.chenlongwang.top/gtkxicgmvo.html

PHP:  json_decode($body, true);
来源：http://hz.cqqwz.cn/gtvyricegg.html

JS:   await resp.json()
来源：http://hz.nwbrower.top/gtejbpkyrj.html

TS:   await resp.json()
来源：http://hz.nwbrower.top/gtmydcbbxq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.birdmap.top/gtmxakbdkj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.andypj.xyz/gtzzlqhtnm.html

Ruby: JSON.parse(resp.body)
来源：http://hz.hywenlv.cn/gttetoglur.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.pycfn.com/gtirjflhua.html

[L07] 处理 HTTP 状态码
来源：http://hz.feifeiyinyue.top/gtbswwveai.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hysaishi.cn/gtupzlgktw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hfpthk.cn/gtspebqigu.html

JS:   resp.ok;  resp.status
来源：http://hz.smart0.xyz/gtzscliiiq.html

TS:   resp.ok;  resp.status
来源：http://hz.vqdsnc.cn/gtagkvaedy.html

Java: resp.statusCode()
来源：http://hz.tian-w.cn/gtuuzmvlxc.html

Go:   resp.StatusCode
来源：http://hz.pycfn.com/gtdciqkabw.html

Ruby: resp.code.to_i
来源：http://hz.zhixingplan.top/gtrmrxwnga.html

C#:   (int)resp.StatusCode
来源：http://hz.yuxming.cn/gtubmtcckx.html

[L08] 并发请求多个地址
来源：http://hz.birdmap.top/gteprjvgmd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yvedp.cn/gtexulllar.html

PHP:  curl_multi_init() 系列
来源：http://hz.gaohongyu789.top/gtcssiydny.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gaohongyu789.top/gtghwdyjyy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cashguo.top/gtcsprhrxv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.haohaochexian.top/gtskjeshqx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hywenlv.cn/gtldtlarvx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.birdmap.top/gtrljqklew.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.wangshuangyany.cn/gtlyklnpww.html

================================================================================
来源：http://hz.jiagoushi.top/gtlfgdtlke.html

M. 命令行 / 进程 / 环境
来源：http://hz.hnxiangtu.top/gtgrpmzupe.html

================================================================================
来源：http://hz.cheryme.top/gtfomjuetu.html

[M01] 读取命令行参数
来源：http://hz.jianghu66.top/gtuapbclkm.html

Py:   sys.argv[1:]
来源：http://hz.zhoulong.xyz/gtxrrmyhpl.html

PHP:  $argv;  $argc;
来源：http://hz.nanxuanxn.top/gtudpxnuod.html

JS:   process.argv.slice(2)
来源：http://hz.cheryme.top/gtmxphjfkp.html

TS:   process.argv.slice(2)
来源：http://hz.jiagoushi.top/gtdcgdcpwv.html

Java: args 数组（main 方法参数）
来源：http://hz.0kj1m.cn/gtbqdpwzbz.html

Go:   os.Args[1:]
来源：http://hz.yongpay.top/gtyjilfcif.html

Ruby: ARGV
来源：http://hz.zdqjudy.top/gtezlqansx.html

C#:   args 数组（Main 方法参数）
来源：http://hz.xingfuxueyuan.xyz/gtxthgehmu.html

[M02] 读取环境变量
来源：http://hz.bjfxy.top/gtekjnghrn.html

Py:   os.environ.get("HOME")
来源：http://hz.zhaomingkeji.xyz/gtaqdmwvzs.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ehwqpu.com/gtimdifgqg.html

JS:   process.env.HOME
来源：http://hz.9152youxi.cn/gtueiqtnhi.html

TS:   process.env.HOME
来源：http://hz.iojbl.cn/gtnratolkf.html

Java: System.getenv("HOME")
来源：http://hz.ivvv.top/gtcponghqw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.havefunace.top/gtozecfgss.html

Ruby: ENV["HOME"]
来源：http://hz.jyoumei.cn/gtvztlgzox.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.chenlongwang.top/gtlegzygej.html

[M03] 执行外部命令
来源：http://hz.gogol.net.cn/gtrohuykjl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.shzxlz.cn/gtacgavohz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.cqqwz.cn/gtxtniqusi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.cucudq.cn/gtezqevrft.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinyuanbaomall.cn/gtadvdqufk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.gaohongyu789.top/gtdqdjlgjn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.vqdsnc.cn/gtrnxreodb.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.cqqwz.cn/gtuciysiep.html

C#:   Process.Start("ls", "-l");
来源：http://hz.chenlongwang.top/gtkmqetlby.html

[M04] 获取当前工作目录
来源：http://hz.havefunace.top/gtpywajslx.html

Py:   os.getcwd()
来源：http://hz.chenlongwang.top/gteefxgoey.html

PHP:  getcwd();
来源：http://hz.haohaochexian.top/gtfttwrwdp.html

JS:   process.cwd()
来源：http://hz.xingfuxueyuan.xyz/gtdkwamodm.html

TS:   process.cwd()
来源：http://hz.yonumen.top/gtzoguhcic.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.tian-w.cn/gttclrposr.html

Go:   os.Getwd()
来源：http://hz.wangshuangyany.cn/gtjnerjbrg.html

Ruby: Dir.pwd
来源：http://hz.jinqigfzy.top/gtygfvbaic.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.tianlin.xyz/gtiqeprgqc.html

[M05] 设置退出码
来源：http://hz.xylfe.cn/gtdcwehccq.html

Py:   sys.exit(1)
来源：http://hz.daxiang520.top/gtnldllwcs.html

PHP:  exit(1);
来源：http://hz.sxryk.cn/gtcmymgfqt.html

JS:   process.exit(1)
来源：http://hz.chenjidiqi.icu/gturtvtyal.html

TS:   process.exit(1)
来源：http://hz.gotoacloud.top/gtkqmqxror.html

Java: System.exit(1)
来源：http://hz.xziqi.cn/gtibbnvyuw.html

Go:   os.Exit(1)
来源：http://hz.cucudq.cn/gtporharnm.html

Ruby: exit 1
来源：http://hz.zdqjudy.top/gtyxqpsgil.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.9152youxi.cn/gtwataxhgq.html

[M06] 向标准错误输出
来源：http://hz.zhijiandao.cn/gtqbdaikmu.html

Py:   print("err", file=sys.stderr)
来源：http://hz.c1oappe.top/gtvksxgjwi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xziqi.cn/gtcmafovkv.html

JS:   console.error("err")
来源：http://hz.zhengqikj.top/gttzrkwuml.html

TS:   console.error("err")
来源：http://hz.9152youxi.cn/gttbyxadjb.html

Java: System.err.println("err")
来源：http://hz.jyoumei.cn/gtjuntiurp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zycfv.cn/gtpahwpasc.html

Ruby: warn "err"
来源：http://hz.hammf.cn/gtfgcpysmy.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.gotoacloud.top/gtxaxrdlnl.html

[M07] 判断是否为主入口
来源：http://hz.shzxlz.cn/gtrlrovhho.html

Py:   if __name__ == "__main__":
来源：http://hz.jianghu66.top/gtooaqavpj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.gogol.net.cn/gtqoxemayf.html

JS:   require.main === module
来源：http://hz.shuidangran.top/gtkyiweouo.html

TS:   require.main === module
来源：http://hz.gogol.net.cn/gteavlbbcx.html

Java: public static void main(String[] args)
来源：http://hz.shzxlz.cn/gtbcpwvrax.html

Go:   func main()
来源：http://hz.yj20258.top/gtqbccjobt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yonumen.top/gtulrvptdu.html

C#:   static void Main(string[] args)
来源：http://hz.gzhubu.top/gtbnzajxmx.html

[M08] 获取系统与运行时信息
来源：http://hz.zycfv.cn/gtnddnfswj.html

Py:   platform.system();  platform.python_version()
来源：http://hz.nanxinkj.top/gtwxxrffsx.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.chenjidiqi.icu/gtqlzxhmnv.html

JS:   process.platform;  process.version
来源：http://hz.xylfe.cn/gtpxwgrzed.html

TS:   process.platform;  process.version
来源：http://hz.xinyue.icu/gtkgluksgq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.sxryk.cn/gtetrmezvr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xingfuxueyuan.xyz/gtnrxzdpgl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ehwqpu.com/gthtukuwrz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hnqzz.top/gtvasjcwhk.html

================================================================================
来源：http://hz.hywenlv.cn/gtaexsjqya.html

N. 数据结构与算法
来源：http://hz.0kj1m.cn/gtwdrdfiwh.html

================================================================================
来源：http://hz.316326.xyz/gtlpavbtnv.html

[N01] 二分查找（有序数组）
来源：http://hz.shzxlz.cn/gtwviedkpu.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.bjfxy.top/gtfaxnejwl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.havefunace.top/gtvfeezgdm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yongpay.top/gtxadkqlve.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hysaishi.cn/gtxachfdrv.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zycfv.cn/gtynmoxhne.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.meibo888.top/gtjewbsrmo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.sufxvd.cn/gthvduquyx.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.andypj.xyz/gtwwzkejvu.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.daria6918.cn/gtuzwuqrfn.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yj20258888.top/gtoeicdnjc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.daria6918.cn/gtjcwjtepb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinghuilouyu.cn/gtfdodsbro.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yj20258.top/gtuqnxyzbq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.sxryk.cn/gthqwcsgwb.html

Go:   slices.Sort(arr)
来源：http://hz.daxiang520.top/gtvfmqlmoa.html

Ruby: arr.sort
来源：http://hz.cdnleiting.top/gtkwyicglb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.vqdsnc.cn/gtpjnfdudu.html

[N03] 快速排序（分治示例）
来源：http://hz.yongpay.top/gtjotdwhnc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.birdmap.top/gtayslswti.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zhengqikj.top/gtdgnuaztn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.mhx1999.top/gtsovyruly.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jyoumei.cn/gtgldhsloh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.hysaishi.cn/gticfuyvkk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.birdmap.top/gtldupthsp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yvedp.cn/gtbavpmpys.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yvedp.cn/gtmizuasls.html

[N04] 斐波那契数列
来源：http://hz.andypj.xyz/gtxfxtyhno.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.pengpengdd.cyou/gtnhtkzjsi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.ppjwa.cn/gtervxjivc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hnxiangtu.top/gtfevvwxii.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.kuanghao11.cn/gtnkmnrazu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.kuanghao11.cn/gtngdjwbaj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jinghuilouyu.cn/gtszihakrb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.cdnleiting.top/gtbvuwnwyn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhoulong.xyz/gtbwosqxmg.html

[N05] 最大公约数
来源：http://hz.jyoumei.cn/gthonkrikt.html

Py:   math.gcd(a, b)
来源：http://hz.ywan-chungtsiang.top/gtgzdrkdpf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.fzhhl.top/gtrqxxhnvr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ppjwa.cn/gtlktfrdga.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hongshengwenyu.top/gtpnweuhzv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.chenzaomai.com/gtiiewzswr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.gotoacloud.top/gtdynutmxr.html

Ruby: a.gcd(b)
来源：http://hz.vqdsnc.cn/gtvihtrxml.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.gaohongyu789.top/gtpjtpebkl.html

[N06] 判断回文字符串
来源：http://hz.pycfn.com/gtfeghndxi.html

Py:   s == s[::-1]
来源：http://hz.yueranfly.top/gtujwtwbfy.html

PHP:  $s === strrev($s);
来源：http://hz.tian-w.cn/gttojeshcq.html

JS:   s === [...s].reverse().join("")
来源：http://hz.ppjwa.cn/gttblhqhtp.html

TS:   s === [...s].reverse().join("")
来源：http://hz.nanxuanxn.top/gtsdnyvtfy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.shangyingyoupin.top/gtksyqjttq.html

Go:   // 双指针从两端比较
来源：http://hz.fzhhl.top/gtjtipolhy.html

Ruby: s == s.reverse
来源：http://hz.hywenlv.cn/gtnafscdjh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hongshengwenyu.top/gtfxkgqzbe.html

[N07] 两数之和（返回下标）
来源：http://hz.gzhubu.top/gtodljhdde.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hnxiangtu.top/gtbbnhtnxk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.c1oappe.top/gtrffhtmfm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yangfankeji.com/gtpbrstesl.html

TS:   // 手写 Map<string, number>
来源：http://hz.wangshuangyany.cn/gtabwfhuaf.html

Java: // 手写 HashMap
来源：http://hz.shanyushiyangtech.top/gtyskvxntq.html

Go:   // 手写 map[int]int
来源：http://hz.redwolf501.top/gtdicviiox.html

Ruby: // 手写 Hash
来源：http://hz.cucudq.cn/gtgiveyefs.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jqgufenzy.top/gtvuxdyvmr.html

[N08] 生成全排列
来源：http://hz.birdmap.top/gtexrooowj.html

Py:   itertools.permutations(arr)
来源：http://hz.ydjk.org.cn/gtisyrfnry.html

PHP:  // 手写递归交换
来源：http://hz.yanxiufei.cn/gtascbcsdr.html

JS:   // 手写回溯递归
来源：http://hz.tian-w.cn/gtjdtmhbjj.html

TS:   // 手写回溯递归
来源：http://hz.jianghu66.top/gtecfghgab.html

Java: // 手写回溯递归
来源：http://hz.hywenlv.cn/gtstxnqvis.html

Go:   // 手写回溯递归
来源：http://hz.meibo888.top/gtamazuflz.html

Ruby: arr.permutation.to_a
来源：http://hz.andypj.xyz/gtvwfyqcxy.html

C#:   // 手写回溯递归
来源：http://hz.xuetiantiany.cn/gtkedqyqej.html


<!-- 参考信息 -->