代发 wailian999

[K02] JSON 字符串转对象
来源：http://hz.guowangkeji.top/gtkdnzlamq.html

Py:   json.loads(s)
来源：http://hz.meibo888.top/gtbpbzvwfn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cheryme.top/gtfdxnwzgo.html

JS:   JSON.parse(s)
来源：http://hz.52xcode.cn/gtpbpegujp.html

TS:   JSON.parse(s)
来源：http://hz.yj202588.top/gtagbdxysh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hnxiangtu.top/gtmjatzqwi.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhengqikj.top/gtdkbwlpmw.html

Ruby: JSON.parse(s)
来源：http://hz.yj20258.top/gthbtdjnpo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhijiandao.cn/gttyrofdsn.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.fengsongda.top/gtlsdxafzw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.fzhhl.top/gtnxfmfjks.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hfpthk.cn/gtqlqeciam.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hysaishi.cn/gtosyzrigv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.daria6918.cn/gtcfcpyszv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yj20258888.top/gtrqhnykhr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.tianlin.xyz/gtekotdeun.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.wangshuangyany.cn/gtzplvshfu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.wangdashe.top/gtabnfmsih.html

[K04] 读取 JSON 文件
来源：http://hz.dianchejie.cn/gtgugxmtsj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zhixingplan.top/gtgfhitigk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cqqwz.cn/gthypnxwyc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yongpay.top/gtofzwuxhx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yuxming.cn/gtlddacttd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.daxiang520.top/gtdpelwbhh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zdqjudy.top/gtuxrgqqec.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.iojbl.cn/gtklhlzkek.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.sweek.top/gtpekuvfow.html

[K05] 深拷贝对象
来源：http://hz.birdmap.top/gtdsswlhqv.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhiwuduotai.top/gtalmhgiuh.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hywenlv.cn/gtvtdgbmdn.html

JS:   structuredClone(obj)
来源：http://hz.iojbl.cn/gtwgnzghkr.html

TS:   structuredClone(obj)
来源：http://hz.hfpthk.cn/gtbicdffvg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.cdnleiting.top/gtyqexoyzs.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.gzhubu.top/gtkdvwjfka.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.guannengcc.top/gtuulqntcg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yuanzhike.top/gtwlekhuic.html

[K06] 解析 URL 查询串
来源：http://hz.gaohongyu789.top/gtgyoxbdcy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.pycfn.com/gtmqgqyseh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.shanyushiyangtech.top/gtmfdxkccn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.chenzaomai.com/gtkriwblig.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nanxuanxn.top/gtqlzydufm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.shangyingyoupin.top/gtvqcszman.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.sxryk.cn/gtksjjzbvk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.sufxvd.cn/gtpigwragx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhengqikj.top/gtmqtthbeq.html

[K07] 进制转换
来源：http://hz.yueranfly.top/gtnmubsoeo.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.redwolf501.top/gtifbztcck.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.pycfn.com/gtstrjgjoi.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.nanxuanxn.top/gtexillxpa.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.cucudq.cn/gtxqplbwkn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cqqwz.cn/gtokjdnnlm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xziqi.cn/gtxmuipvbj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yj202588.top/gtqkzkckgr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ehwqpu.com/gtyrwuzabn.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yongpay.top/gtcuducxaf.html

Py:   pickle.dumps(obj)
来源：http://hz.wangshuangyany.cn/gtcwnagmyd.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zhengqikj.top/gtqvluihuv.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.gaohongyu789.top/gttwypxlwp.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.cashguo.top/gtezgsbydc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhengqikj.top/gtqydxwics.html

Go:   encoding/gob
来源：http://hz.jinghuilouyu.cn/gtfoiaslco.html

Ruby: Marshal.dump(obj)
来源：http://hz.yj202588.top/gtmsprrqmx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhoulong.xyz/gtgbmaktjl.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtnmssdslc.html

L. 网络请求
来源：http://hz.nanxinkj.top/gtsdnrftqg.html

================================================================================
来源：http://hz.cheryme.top/gtsulebfqn.html

[L01] 发送 GET 请求
来源：http://hz.c1oappe.top/gtsbisszac.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.gotoacloud.top/gtbzotdpjd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.cdnleiting.top/gtmmeqcaxc.html

JS:   await fetch(url)
来源：http://hz.daxiang520.top/gtswvdwtnh.html

TS:   await fetch(url)
来源：http://hz.hammf.cn/gtbfiyypbj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jinqigufen.top/gtkrucqfod.html

Go:   resp, err := http.Get(url)
来源：http://hz.yueranfly.top/gtpcvyebxk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.c1oappe.top/gtblerysne.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.haohaochexian.top/gtlvgaipeh.html

[L02] 发送 POST JSON
来源：http://hz.zdqjudy.top/gtqwfsyhby.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.sxryk.cn/gtiifvsckd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hywenlv.cn/gtwsrapjxn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gotoacloud.top/gtrzvpbeqz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shanyushiyangkeji.top/gtlruzcrbm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hammf.cn/gttpzrurqq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jlsjyb.cn/gthttrzksf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.ivvv.top/gtexknplfu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zdqjudy.top/gtqgjalvdh.html

[L03] 设置自定义请求头
来源：http://hz.jlsjyb.cn/gttbeytigp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.pengpengdd.cyou/gtcdiiewiz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hfpthk.cn/gttgtjcvwh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gzhubu.top/gtkhinxbtu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jianghu66.top/gtyfxrrygl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jlsjyb.cn/gtcrvjicnl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.birdmap.top/gthkdbzbvx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jiagoushi.top/gtiopszwbg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yvedp.cn/gtnumqaxov.html

[L04] 设置超时
来源：http://hz.ehwqpu.com/gtkgwuztsn.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hywenlv.cn/gtfrayojns.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.nanxinkj.top/gtwxzqqkba.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhongyouzk.top/gtnccieunx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ydzc1.top/gtpvevfhtv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.daria6918.cn/gtvyfpuorw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jlsjyb.cn/gtdtbzyten.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hnqzz.top/gtjkkvkesx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhixingplan.top/gthtonytpm.html

[L05] 上传文件（multipart）
来源：http://hz.guowangkeji.top/gtbyyglybp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhongyouzk.top/gthmsitpkl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.pengpengdd.cyou/gtoogejqml.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yanxiufei.cn/gtpikzwmtd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.hongshengwenyu.top/gtjxkneoqp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.iojbl.cn/gtvdabqttc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.svipenyu.cn/gtcpuusoli.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.wangdashe.top/gtjuaxirso.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.ydjk.org.cn/gtyqnhmwbq.html

[L06] 解析响应为 JSON
来源：http://hz.shuidangran.top/gtbqjfkmpe.html

Py:   resp.json()
来源：http://hz.fengsongda.top/gtxakyhqay.html

PHP:  json_decode($body, true);
来源：http://hz.jyoumei.cn/gtrcuqmkfm.html

JS:   await resp.json()
来源：http://hz.gzhubu.top/gtashxvrke.html

TS:   await resp.json()
来源：http://hz.meibo888.top/gtzrvuxods.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.gogol.net.cn/gtdbynjbjt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.birdmap.top/gttkrrogal.html

Ruby: JSON.parse(resp.body)
来源：http://hz.dianchejie.cn/gtbhshcjox.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.gogol.net.cn/gtbfpzoyup.html

[L07] 处理 HTTP 状态码
来源：http://hz.shangyingyoupin.top/gtqnkiubdo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yvedp.cn/gtpovkwdix.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jinqigufen.top/gtezyxskph.html

JS:   resp.ok;  resp.status
来源：http://hz.chenlongwang.top/gtqasnauki.html

TS:   resp.ok;  resp.status
来源：http://hz.wangdashe.top/gtohpevqdf.html

Java: resp.statusCode()
来源：http://hz.hongshengwenyu.top/gtggflqywx.html

Go:   resp.StatusCode
来源：http://hz.jiagoushi.top/gtaasdsktl.html

Ruby: resp.code.to_i
来源：http://hz.chenzaomai.com/gtyykfpzmr.html

C#:   (int)resp.StatusCode
来源：http://hz.ybcxt.top/gtbzvdpkmg.html

[L08] 并发请求多个地址
来源：http://hz.yj20258.top/gttpwoodid.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.haohaochexian.top/gtvwmxqpci.html

PHP:  curl_multi_init() 系列
来源：http://hz.shanyushiyangtech.top/gtspthmkgu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yvedp.cn/gtealhegkh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhaomingkeji.xyz/gtbwsilbgc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yj20258.top/gtxraikpvb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.pycfn.com/gtlpmslbif.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.andypj.xyz/gtoziyvwrq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.tanke756.top/gtodlywrry.html

================================================================================
来源：http://hz.sysykeji.top/gtlexjunhm.html

M. 命令行 / 进程 / 环境
来源：http://hz.jinyuanbaomall.cn/gtbkdqkfpj.html

================================================================================
来源：http://hz.zhongyouzk.top/gtljcxafeu.html

[M01] 读取命令行参数
来源：http://hz.hnxiangtu.top/gtuaouzoqy.html

Py:   sys.argv[1:]
来源：http://hz.bjfxy.top/gtuacoqrmf.html

PHP:  $argv;  $argc;
来源：http://hz.yonumen.top/gtffbnoqeo.html

JS:   process.argv.slice(2)
来源：http://hz.gotoacloud.top/gtpltxzduq.html

TS:   process.argv.slice(2)
来源：http://hz.pengpengdd.cyou/gtekfhectl.html

Java: args 数组（main 方法参数）
来源：http://hz.fzhhl.top/gtqojwjrjl.html

Go:   os.Args[1:]
来源：http://hz.gzhubu.top/gtuqrcquqz.html

Ruby: ARGV
来源：http://hz.daria6918.cn/gtuoxgmuah.html

C#:   args 数组（Main 方法参数）
来源：http://hz.cqqwz.cn/gtnhlmquad.html

[M02] 读取环境变量
来源：http://hz.yongpay.top/gtefpjkrwd.html

Py:   os.environ.get("HOME")
来源：http://hz.chenlongwang.top/gtggsqtddn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hnxiangtu.top/gtvsoxpxbs.html

JS:   process.env.HOME
来源：http://hz.jinyuanbaomall.cn/gtsanwezcd.html

TS:   process.env.HOME
来源：http://hz.shuidangran.top/gtxfrsjxpi.html

Java: System.getenv("HOME")
来源：http://hz.xuetiantiany.cn/gtravtpzxx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.aibaodan.cn/gtogdabyoa.html

Ruby: ENV["HOME"]
来源：http://hz.vqdsnc.cn/gthocnultn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.cdnleiting.top/gtfkocspgx.html

[M03] 执行外部命令
来源：http://hz.52xcode.cn/gtoubzjrur.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jianghu66.top/gtsbashbou.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yonumen.top/gtdevhebtx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.smart0.xyz/gtlhixlpgd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.gogol.net.cn/gtvhloivfi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ywan-chungtsiang.top/gttrkfvlfy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yongpay.top/gtjklnpvxr.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shanyushiyangtech.top/gtyrfubfhn.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hywenlv.cn/gtloczmbjk.html

[M04] 获取当前工作目录
来源：http://hz.yj202588.top/gtpvyscvqc.html

Py:   os.getcwd()
来源：http://hz.gogol.net.cn/gtfkmsjadq.html

PHP:  getcwd();
来源：http://hz.xylfe.cn/gtsxmyldjy.html

JS:   process.cwd()
来源：http://hz.ywan-chungtsiang.top/gtvrbvpsvp.html

TS:   process.cwd()
来源：http://hz.aibaodan.cn/gtlyecpqdm.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.cqqwz.cn/gtbhztpatg.html

Go:   os.Getwd()
来源：http://hz.hnxiangtu.top/gtcjjqykwv.html

Ruby: Dir.pwd
来源：http://hz.svipenyu.cn/gtnxdrhlex.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ehwqpu.com/gtiiwxybbk.html

[M05] 设置退出码
来源：http://hz.xinyue.icu/gtxddfsrwo.html

Py:   sys.exit(1)
来源：http://hz.52xcode.cn/gtjbziktjp.html

PHP:  exit(1);
来源：http://hz.meibo888.top/gtuazsappf.html

JS:   process.exit(1)
来源：http://hz.chenzaomai.com/gttfbyemrk.html

TS:   process.exit(1)
来源：http://hz.hnqzz.top/gtqbgavwuw.html

Java: System.exit(1)
来源：http://hz.zhongyouzk.top/gtbpukffka.html

Go:   os.Exit(1)
来源：http://hz.jianghu66.top/gtzymhairw.html

Ruby: exit 1
来源：http://hz.yuxming.cn/gtnagjnzhp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.sysykeji.top/gtltyuvkzr.html

[M06] 向标准错误输出
来源：http://hz.xinyue.icu/gtsmnhmrbe.html

Py:   print("err", file=sys.stderr)
来源：http://hz.shzxlz.cn/gtqskghccg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.gogol.net.cn/gtrjyxqhuf.html

JS:   console.error("err")
来源：http://hz.gogol.net.cn/gtcjjjtqnb.html

TS:   console.error("err")
来源：http://hz.sxryk.cn/gtygxqpkzx.html

Java: System.err.println("err")
来源：http://hz.yanxiufei.cn/gttngnymvu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jqgufenzy.top/gtnpxqrubi.html

Ruby: warn "err"
来源：http://hz.shanyushiyangkeji.top/gtkoamtnss.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.feifeiyinyue.top/gtmnrrklpt.html

[M07] 判断是否为主入口
来源：http://hz.guowangkeji.top/gtynlgsnvf.html

Py:   if __name__ == "__main__":
来源：http://hz.hnqzz.top/gtvgyusowl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.9152youxi.cn/gtxiutsssk.html

JS:   require.main === module
来源：http://hz.hywenlv.cn/gtyrmrdvox.html

TS:   require.main === module
来源：http://hz.yvedp.cn/gthnffpyzw.html

Java: public static void main(String[] args)
来源：http://hz.yvedp.cn/gtenprsvoj.html

Go:   func main()
来源：http://hz.daria6918.cn/gtpadxejrl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhengqikj.top/gtjhiczpwx.html

C#:   static void Main(string[] args)
来源：http://hz.gotoacloud.top/gtvcrhyrpf.html

[M08] 获取系统与运行时信息
来源：http://hz.quarkkingdee.top/gtxxcemjfb.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yanxiufei.cn/gtoxsrxqbx.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.shangyingyoupin.top/gtjfeimjbg.html

JS:   process.platform;  process.version
来源：http://hz.ivvv.top/gtnzhgpzhj.html

TS:   process.platform;  process.version
来源：http://hz.hongshengwenyu.top/gtgrvnxdvs.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.shzxlz.cn/gtbvtsxfik.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.guowangkeji.top/gtzwmpitri.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.gaohongyu789.top/gtnhjeguvd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jinqigfzy.top/gttqecpzxy.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtgtmgilhx.html

N. 数据结构与算法
来源：http://hz.9152youxi.cn/gtpkzegzok.html

================================================================================
来源：http://hz.cdnleiting.top/gtysbvonwf.html

[N01] 二分查找（有序数组）
来源：http://hz.iojbl.cn/gtpeqpyxdy.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yanxiufei.cn/gtiwdildmf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yuanzhike.top/gtgyrkzimv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.aibaodan.cn/gtuwwnagyx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinqigfzy.top/gtilfavsas.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zycfv.cn/gtdcrjmiod.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.gotoacloud.top/gtxyghetjp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yonumen.top/gtdybihuak.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.cucudq.cn/gtmwilxzba.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jinqigfzy.top/gthbbvtbpc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.guannengcc.top/gtpwvmjueq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hongshengwenyu.top/gtajqmshjb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ydjk.org.cn/gtgndldknd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.fzhhl.top/gtqbngfowx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.mhx1999.top/gtxuohwmba.html

Go:   slices.Sort(arr)
来源：http://hz.xziqi.cn/gtnbjsegqo.html

Ruby: arr.sort
来源：http://hz.gotoacloud.top/gtvysoatrn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.fengsongda.top/gtftppqkif.html

[N03] 快速排序（分治示例）
来源：http://hz.bjfxy.top/gtotzxxqqa.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ppjwa.cn/gtuxmraexr.html

PHP:  // 递归实现，或用 usort
来源：http://hz.tanke756.top/gtkvaodaeg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tanke756.top/gtsqcwluev.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yuanzhike.top/gtqvhqonql.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.sweek.top/gtsqzeicze.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yuxming.cn/gtqlnpxhpq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hongshengwenyu.top/gthgmhhude.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhaomingkeji.xyz/gtepqzwuom.html

[N04] 斐波那契数列
来源：http://hz.yj20258888.top/gtfyvhqvyn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ydjk.org.cn/gtwyllojny.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yj20258.top/gthiywazxp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.fzhhl.top/gtdwkhugxy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.redwolf501.top/gtlnuqhcug.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.pycfn.com/gtoakknrhb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.haohaochexian.top/gttrevejkv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhiwuduotai.top/gtgaebfnnv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xuanzx.com/gtlpkjtveo.html

[N05] 最大公约数
来源：http://hz.bjfxy.top/gtqujkhfkb.html

Py:   math.gcd(a, b)
来源：http://hz.c1oappe.top/gtdpybqlek.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.andypj.xyz/gtiezslxai.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gzhubu.top/gtqlsgdmau.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.tanke756.top/gtptwtdeug.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.shzxlz.cn/gtowbqldjp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.daria6918.cn/gtaifejwbh.html

Ruby: a.gcd(b)
来源：http://hz.hysaishi.cn/gtxmhnozaf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zdqjudy.top/gthqqwyohg.html

[N06] 判断回文字符串
来源：http://hz.jiagoushi.top/gtibgnazru.html

Py:   s == s[::-1]
来源：http://hz.dashuyun.cn/gtctddiyth.html

PHP:  $s === strrev($s);
来源：http://hz.cqqwz.cn/gtwymqiqvs.html

JS:   s === [...s].reverse().join("")
来源：http://hz.svipenyu.cn/gtkkuecfoh.html

TS:   s === [...s].reverse().join("")
来源：http://hz.nanxuanxn.top/gtmmrtqudr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.shanyushiyangkeji.top/gtnqmmhmxy.html

Go:   // 双指针从两端比较
来源：http://hz.hongshengwenyu.top/gtprlcobgh.html

Ruby: s == s.reverse
来源：http://hz.gaohongyu789.top/gtmggyesti.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.nwbrower.top/gthuceaceo.html

[N07] 两数之和（返回下标）
来源：http://hz.ybcxt.top/gtiqxttjnh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.dianchejie.cn/gtexvbqdxj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hnxiangtu.top/gtnsvonsct.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yanxiufei.cn/gtjhprginv.html

TS:   // 手写 Map<string, number>
来源：http://hz.ehwqpu.com/gtiaqasjwz.html

Java: // 手写 HashMap
来源：http://hz.yuxming.cn/gtgavmulqa.html

Go:   // 手写 map[int]int
来源：http://hz.jianghu66.top/gtlgjudjep.html

Ruby: // 手写 Hash
来源：http://hz.xinyue.icu/gtfxgxqdda.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.cheryme.top/gtulmlzque.html

[N08] 生成全排列
来源：http://hz.yangfankeji.com/gtctynywbp.html

Py:   itertools.permutations(arr)
来源：http://hz.yj20258.top/gtdeznmkdx.html

PHP:  // 手写递归交换
来源：http://hz.0kj1m.cn/gtvalaoydu.html

JS:   // 手写回溯递归
来源：http://hz.aizwys.cn/gtsjvtbtof.html

TS:   // 手写回溯递归
来源：http://hz.sufxvd.cn/gtkqlavpjq.html

Java: // 手写回溯递归
来源：http://hz.guannengcc.top/gtsndaymga.html

Go:   // 手写回溯递归
来源：http://hz.cashguo.top/gtsymhujeq.html

Ruby: arr.permutation.to_a
来源：http://hz.tian-w.cn/gtnknlxeze.html

C#:   // 手写回溯递归
来源：http://hz.nanxuanxn.top/gtaduvpnre.html

[N09] 栈与队列
来源：http://hz.zhiwuduotai.top/gtqdxvzonr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.wangshuangyany.cn/gtsplhnulj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.cucudq.cn/gtfyfprwen.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.sweek.top/gtxcexbwby.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.snrcjt.cn/gtpkiphcrf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yuxming.cn/gtzrauuvql.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.guowangkeji.top/gtmhknqxzu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.sysykeji.top/gtywcalecm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.hysaishi.cn/gtjvwemxhu.html

[N10] 链表节点定义
来源：http://hz.mhx1999.top/gtiqlrexmj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.nanxinkj.top/gtjkcprbcn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hfpthk.cn/gthgsqcogl.html


<!-- 参考信息 -->