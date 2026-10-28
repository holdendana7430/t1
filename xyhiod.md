代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.smart0.xyz/gtjcinddyu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.chenlongwang.top/gttbxgbyty.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gaohongyu789.top/gtwikdolcx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.vqdsnc.cn/gtpbvwlyvn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.fengsongda.top/gtezbrxrzt.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.meibo888.top/gtsxiygidn.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.nwbrower.top/gtvcowcuvy.html

[K05] 深拷贝对象
来源：http://hz.aizwys.cn/gtzaltccza.html

Py:   copy.deepcopy(obj)
来源：http://hz.yj20258.top/gtvecbipxx.html

PHP:  unserialize(serialize($obj));
来源：http://hz.redwolf501.top/gtmoxbarbx.html

JS:   structuredClone(obj)
来源：http://hz.shzxlz.cn/gtlebgmqgq.html

TS:   structuredClone(obj)
来源：http://hz.wangdashe.top/gtuqydbfsz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.cucudq.cn/gtikjjkrsk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jyoumei.cn/gtkyralnej.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.gotoacloud.top/gtwsnqsxpo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.gzhubu.top/gtdycbmqgc.html

[K06] 解析 URL 查询串
来源：http://hz.aibaodan.cn/gtvcpgpegn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.dianchejie.cn/gtjruxkzii.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.316326.xyz/gtkggstfww.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.wangdashe.top/gtrdtphtib.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ydjk.org.cn/gtgvponvmp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.316326.xyz/gtzmnmiiof.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jinyuanbaomall.cn/gtyargczvg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.sxryk.cn/gtvcvlskmg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.sufxvd.cn/gtyspafonp.html

[K07] 进制转换
来源：http://hz.yuxming.cn/gtrnseweje.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.tianlin.xyz/gtlommyrnn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xuetiantiany.cn/gtxynsixfv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hysaishi.cn/gtgilupgtq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yuanzhike.top/gtylpfuuqf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ybcxt.top/gtskyegeqq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.ybcxt.top/gtirbdejjs.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.nwbrower.top/gtdzpmezcd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.daria6918.cn/gtrellimho.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.aizwys.cn/gtniaatvmx.html

Py:   pickle.dumps(obj)
来源：http://hz.ybcxt.top/gtvxqunkfo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zycfv.cn/gtfbumohnc.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.haohaochexian.top/gtowqlgwiw.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.shanyushiyangkeji.top/gteoejsxhy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hongshengwenyu.top/gtynhdwuhf.html

Go:   encoding/gob
来源：http://hz.cqqwz.cn/gtzgwsydzk.html

Ruby: Marshal.dump(obj)
来源：http://hz.zycfv.cn/gtibvcdkml.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.dianchejie.cn/gtofhpvije.html

================================================================================
来源：http://hz.xuanzx.com/gtwexptbgd.html

L. 网络请求
来源：http://hz.chenjidiqi.icu/gtlgezhszr.html

================================================================================
来源：http://hz.gzhubu.top/gtnqoyuxjf.html

[L01] 发送 GET 请求
来源：http://hz.guowangkeji.top/gtprigszgd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.ehwqpu.com/gtsmnouwco.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hysaishi.cn/gtuymptpqa.html

JS:   await fetch(url)
来源：http://hz.wangdashe.top/gtttprdwwk.html

TS:   await fetch(url)
来源：http://hz.zhongyouzk.top/gtfzisllwh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.vqdsnc.cn/gtvlywahqj.html

Go:   resp, err := http.Get(url)
来源：http://hz.dashuyun.cn/gtgcyjqdtb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.fengsongda.top/gtpggnisao.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ehwqpu.com/gtuxkadtug.html

[L02] 发送 POST JSON
来源：http://hz.iojbl.cn/gtjclgwfkg.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.kuanghao11.cn/gtyoczjgwf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.sweek.top/gtejoanrpp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hnqzz.top/gtnicuztua.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.nanxuanxn.top/gtgjhgftml.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.xylfe.cn/gtpxhgmzur.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.svipenyu.cn/gttmqcotwz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.bjfxy.top/gtqgachlnr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zhiwuduotai.top/gtdtxkppvk.html

[L03] 设置自定义请求头
来源：http://hz.shanyushiyangtech.top/gtppgzvaug.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.tian-w.cn/gtuzvhwvgg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.cheryme.top/gtjpaeuuim.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.redwolf501.top/gtrjkkssrf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cashguo.top/gtbshrcnsb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ywan-chungtsiang.top/gthoqbicri.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hnqzz.top/gtsevlyuus.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhoulong.xyz/gtvowjvqww.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.cucudq.cn/gtvcbmcyfh.html

[L04] 设置超时
来源：http://hz.yvedp.cn/gtgtdwhlas.html

Py:   requests.get(url, timeout=5)
来源：http://hz.tian-w.cn/gtdqgfotom.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.redwolf501.top/gtmeqkxdbp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nwbrower.top/gtsorvtxoq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gotoacloud.top/gtjiiluvnc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.aibaodan.cn/gtpsqnjdmd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.wangshuangyany.cn/gthjfcsmwq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.aizwys.cn/gtbjqlvydk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhoulong.xyz/gtgqlvpupe.html

[L05] 上传文件（multipart）
来源：http://hz.316326.xyz/gtdneolabz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.andypj.xyz/gticzajbku.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.pengpengdd.cyou/gtbmlbiprj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhongyouzk.top/gtqbzvrdsf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.nanxinkj.top/gtuulvrzzh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.cashguo.top/gtrmxzopfh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.kuanghao11.cn/gtacpwhvjg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.daria6918.cn/gtutbdryqg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.sxryk.cn/gtyrbxcjmd.html

[L06] 解析响应为 JSON
来源：http://hz.pycfn.com/gtwpdrphfm.html

Py:   resp.json()
来源：http://hz.daxiang520.top/gttbpncgbu.html

PHP:  json_decode($body, true);
来源：http://hz.ydjk.org.cn/gtfotixqtp.html

JS:   await resp.json()
来源：http://hz.sxryk.cn/gtettkbggo.html

TS:   await resp.json()
来源：http://hz.hysaishi.cn/gterqjoibk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.chenzaomai.com/gtdwptcftj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.guannengcc.top/gtwwcfkdxv.html

Ruby: JSON.parse(resp.body)
来源：http://hz.daria6918.cn/gtjsqeyngq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.aizwys.cn/gtuidkyuos.html

[L07] 处理 HTTP 状态码
来源：http://hz.iojbl.cn/gtjxzaibjp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.meibo888.top/gtnsijgbbl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.cdnleiting.top/gtqnfhycfi.html

JS:   resp.ok;  resp.status
来源：http://hz.sweek.top/gtjxzyytpm.html

TS:   resp.ok;  resp.status
来源：http://hz.yvedp.cn/gtveefztof.html

Java: resp.statusCode()
来源：http://hz.cheryme.top/gtwoxncrvw.html

Go:   resp.StatusCode
来源：http://hz.andypj.xyz/gtbskotfbv.html

Ruby: resp.code.to_i
来源：http://hz.nanxinkj.top/gtnmxqffdw.html

C#:   (int)resp.StatusCode
来源：http://hz.hammf.cn/gtqpovrpjy.html

[L08] 并发请求多个地址
来源：http://hz.jinqigfzy.top/gtwzlockqj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.vqdsnc.cn/gtodijeoti.html

PHP:  curl_multi_init() 系列
来源：http://hz.yvedp.cn/gtbzntomqe.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.9152youxi.cn/gtiiriwfko.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.smart0.xyz/gtkeeuchhv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.vqdsnc.cn/gtsiaegilp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.snrcjt.cn/gtttsmjeas.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.0kj1m.cn/gtomkqssow.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xziqi.cn/gtrntppxgt.html

================================================================================
来源：http://hz.meibo888.top/gtvrcnpybj.html

M. 命令行 / 进程 / 环境
来源：http://hz.jinghuilouyu.cn/gteexqkeqt.html

================================================================================
来源：http://hz.zhongyouzk.top/gtalsgnmpc.html

[M01] 读取命令行参数
来源：http://hz.nwbrower.top/gtndpclzcd.html

Py:   sys.argv[1:]
来源：http://hz.shanyushiyangtech.top/gtnyyrerfm.html

PHP:  $argv;  $argc;
来源：http://hz.dashuyun.cn/gtzgxidfse.html

JS:   process.argv.slice(2)
来源：http://hz.aibaodan.cn/gtxidrwkor.html

TS:   process.argv.slice(2)
来源：http://hz.sufxvd.cn/gtzcetcsyc.html

Java: args 数组（main 方法参数）
来源：http://hz.wangshuangyany.cn/gtqwmpetom.html

Go:   os.Args[1:]
来源：http://hz.hywenlv.cn/gtsfxwbqmt.html

Ruby: ARGV
来源：http://hz.ydzc1.top/gtllugjbkn.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jqgfzy.top/gtfywqitpt.html

[M02] 读取环境变量
来源：http://hz.ydjk.org.cn/gtleengbhk.html

Py:   os.environ.get("HOME")
来源：http://hz.52xcode.cn/gtwrpbolat.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yvedp.cn/gtijjceqbb.html

JS:   process.env.HOME
来源：http://hz.hongshengwenyu.top/gtmbnuhmkw.html

TS:   process.env.HOME
来源：http://hz.zhongyouzk.top/gtfuhaulnl.html

Java: System.getenv("HOME")
来源：http://hz.vqdsnc.cn/gtlmxwevlz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.fengsongda.top/gtadidkemu.html

Ruby: ENV["HOME"]
来源：http://hz.cheryme.top/gtqjqdarhe.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jinyuanbaomall.cn/gtqfwnsnlo.html

[M03] 执行外部命令
来源：http://hz.zhongyouzk.top/gtbybmctwv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.sxryk.cn/gtsidocjov.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ydjk.org.cn/gtyefnkepd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yangfankeji.com/gtjobzkwkd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hywenlv.cn/gtwjzeoslw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.haohaochexian.top/gtpcumnahl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.sufxvd.cn/gtscdliwhc.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.cheryme.top/gtvzzddpbt.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yuanzhike.top/gtxktayfbo.html

[M04] 获取当前工作目录
来源：http://hz.tanke756.top/gtfdqybibh.html

Py:   os.getcwd()
来源：http://hz.quarkkingdee.top/gtjdhhnelo.html

PHP:  getcwd();
来源：http://hz.sweek.top/gtssrnhwmx.html

JS:   process.cwd()
来源：http://hz.shangyingyoupin.top/gtrmdpepaa.html

TS:   process.cwd()
来源：http://hz.svipenyu.cn/gtpdcxhteh.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.haohaochexian.top/gtgjqcizhg.html

Go:   os.Getwd()
来源：http://hz.haohaochexian.top/gtxbidhowb.html

Ruby: Dir.pwd
来源：http://hz.yj202588.top/gtrtlnxryz.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.redwolf501.top/gtdyypictf.html

[M05] 设置退出码
来源：http://hz.xinyue.icu/gtykjfrtwi.html

Py:   sys.exit(1)
来源：http://hz.xuanzx.com/gtzcmgngxw.html

PHP:  exit(1);
来源：http://hz.yongpay.top/gtfndhtkwm.html

JS:   process.exit(1)
来源：http://hz.nanxinkj.top/gtkueehwjj.html

TS:   process.exit(1)
来源：http://hz.zhoulong.xyz/gtnmwgwkgt.html

Java: System.exit(1)
来源：http://hz.zdqjudy.top/gtaljtnxdp.html

Go:   os.Exit(1)
来源：http://hz.pycfn.com/gtwnfhxjem.html

Ruby: exit 1
来源：http://hz.hongshengwenyu.top/gtftrqelvq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.wangshuangyany.cn/gtnndzwxmj.html

[M06] 向标准错误输出
来源：http://hz.xuetiantiany.cn/gtozgbbilc.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ydzc1.top/gtbohemdnk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yongpay.top/gtmtrgqtzl.html

JS:   console.error("err")
来源：http://hz.jinyuanbaomall.cn/gtqrjezprb.html

TS:   console.error("err")
来源：http://hz.cdnleiting.top/gtxgzyhori.html

Java: System.err.println("err")
来源：http://hz.chenzaomai.com/gtxkwbubzh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.pycfn.com/gtqcnfjdfo.html

Ruby: warn "err"
来源：http://hz.jianghu66.top/gtvdfklozs.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.fzhhl.top/gtohntiymd.html

[M07] 判断是否为主入口
来源：http://hz.ydjk.org.cn/gtodozmpgm.html

Py:   if __name__ == "__main__":
来源：http://hz.cdnleiting.top/gtwmawlqxs.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yj20258.top/gtueqdvyij.html

JS:   require.main === module
来源：http://hz.gzhubu.top/gtckznnoji.html

TS:   require.main === module
来源：http://hz.zhixingplan.top/gtbonmazbt.html

Java: public static void main(String[] args)
来源：http://hz.hammf.cn/gtwtpeazes.html

Go:   func main()
来源：http://hz.jyoumei.cn/gtznisfqyo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.xingfuxueyuan.xyz/gtpmvbgtsj.html

C#:   static void Main(string[] args)
来源：http://hz.jianghu66.top/gtirxfnhlp.html

[M08] 获取系统与运行时信息
来源：http://hz.jinqigfzy.top/gtohcefyrp.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ivvv.top/gtgyjeepwr.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.chenlongwang.top/gterbgouxz.html

JS:   process.platform;  process.version
来源：http://hz.gzhubu.top/gtnwfyjwat.html

TS:   process.platform;  process.version
来源：http://hz.yuxming.cn/gtnwkithql.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.feifeiyinyue.top/gtwquboshz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.tianlin.xyz/gtdwpoxrrn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.vqdsnc.cn/gtxeiaekxt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.daxiang520.top/gtzltiscqh.html

================================================================================
来源：http://hz.0kj1m.cn/gtlosmjugo.html

N. 数据结构与算法
来源：http://hz.fengsongda.top/gtughuuupu.html

================================================================================
来源：http://hz.vqdsnc.cn/gtjkvyqxtk.html

[N01] 二分查找（有序数组）
来源：http://hz.316326.xyz/gttrmiadpj.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yj202588.top/gtlkszoriw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.guannengcc.top/gtcababhkf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jlsjyb.cn/gtajclumaz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cdnleiting.top/gtljzdghcq.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.gaohongyu789.top/gtenpsjfzs.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zdqjudy.top/gtpzrblnnt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.shanyushiyangkeji.top/gtzanxxrsr.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jinqigfzy.top/gtbjmnwljk.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yj20258888.top/gtactcwozi.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhengqikj.top/gtkooerulr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.ywan-chungtsiang.top/gthpitzboz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jqgufenzy.top/gtxdxiupgr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.chenzaomai.com/gtqyhmarbw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.mhx1999.top/gtjfevmeon.html

Go:   slices.Sort(arr)
来源：http://hz.shanyushiyangkeji.top/gthnccbxsr.html

Ruby: arr.sort
来源：http://hz.jinqigufen.top/gtdaeqyxvb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.chenjidiqi.icu/gteosciryj.html

[N03] 快速排序（分治示例）
来源：http://hz.sweek.top/gtyyzyzuxa.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.fzhhl.top/gtwhgnmsxh.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zhengqikj.top/gtzkoqcjbm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yanxiufei.cn/gtvhspashb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhiwuduotai.top/gtvtjdumwq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.wangshuangyany.cn/gtkdngvxii.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.aibaodan.cn/gthwkqgfmo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.daxiang520.top/gtefodioyt.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.cashguo.top/gtocxqwiej.html

[N04] 斐波那契数列
来源：http://hz.zhiwuduotai.top/gtmpqrundm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.vqdsnc.cn/gtechhdyyj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.tianlin.xyz/gtxliinxjg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.tian-w.cn/gtjawftxuj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hnxiangtu.top/gtqyrzgnkg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.xinyue.icu/gtdvxlfgpk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.gogol.net.cn/gtcawwnuzt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.iojbl.cn/gtztcsjmql.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jinqigfzy.top/gteepmiifc.html

[N05] 最大公约数
来源：http://hz.cheryme.top/gtdhlthejp.html

Py:   math.gcd(a, b)
来源：http://hz.zhongyouzk.top/gtcsqksugc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.sweek.top/gtcbomihxg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sxryk.cn/gthfezvlxw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cashguo.top/gtaywjsdud.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.tianlin.xyz/gtzqbllmzv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.316326.xyz/gtazqyvufa.html

Ruby: a.gcd(b)
来源：http://hz.zhijiandao.cn/gtirvsemyx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.xylfe.cn/gttirgmoxq.html

[N06] 判断回文字符串
来源：http://hz.smart0.xyz/gtvcuwuqwa.html

Py:   s == s[::-1]
来源：http://hz.dianchejie.cn/gtwermkcqy.html

PHP:  $s === strrev($s);
来源：http://hz.wangdashe.top/gthvetarso.html

JS:   s === [...s].reverse().join("")
来源：http://hz.9152youxi.cn/gtuubzqnzh.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yonumen.top/gtucjhdazp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.c1oappe.top/gtqhrzsibe.html

Go:   // 双指针从两端比较
来源：http://hz.fzhhl.top/gtiatgkiwi.html

Ruby: s == s.reverse
来源：http://hz.chenlongwang.top/gtfxldtflc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.guowangkeji.top/gtjneggkjz.html

[N07] 两数之和（返回下标）
来源：http://hz.feifeiyinyue.top/gthjafaguo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ppjwa.cn/gtkliwcvio.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.9152youxi.cn/gtoywfzdas.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.nanxinkj.top/gtrvlnbqyq.html

TS:   // 手写 Map<string, number>
来源：http://hz.yonumen.top/gtlfybrrop.html

Java: // 手写 HashMap
来源：http://hz.quarkkingdee.top/gtkfrthtnc.html

Go:   // 手写 map[int]int
来源：http://hz.redwolf501.top/gttubnspgh.html

Ruby: // 手写 Hash
来源：http://hz.jinqigfzy.top/gtzpiopdmq.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hammf.cn/gtnrrbzzlj.html

[N08] 生成全排列
来源：http://hz.ybcxt.top/gtvyhtihte.html

Py:   itertools.permutations(arr)
来源：http://hz.jinqigufen.top/gttogpcdjr.html

PHP:  // 手写递归交换
来源：http://hz.nwbrower.top/gtyzkujxgf.html

JS:   // 手写回溯递归
来源：http://hz.tian-w.cn/gtjkgvxuun.html

TS:   // 手写回溯递归
来源：http://hz.birdmap.top/gtbaschrbo.html

Java: // 手写回溯递归
来源：http://hz.xinyue.icu/gtaajmdprp.html

Go:   // 手写回溯递归
来源：http://hz.dashuyun.cn/gthbpdhgiw.html

Ruby: arr.permutation.to_a
来源：http://hz.daxiang520.top/gtvpsmvhrz.html

C#:   // 手写回溯递归
来源：http://hz.yj202588.top/gtsluasupz.html

[N09] 栈与队列
来源：http://hz.tian-w.cn/gtlrsewybf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jinghuilouyu.cn/gtecsazoiw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.guowangkeji.top/gtfzoaktkj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yueranfly.top/gtywmewojk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yj20258.top/gtxqkixdqb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.xingfuxueyuan.xyz/gtggunatey.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhengqikj.top/gtwtehssdf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.bjfxy.top/gtiausbkfz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.chenjidiqi.icu/gttnrwqblx.html

[N10] 链表节点定义
来源：http://hz.bjfxy.top/gtmhxetuwk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.sysykeji.top/gtfzannnso.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.tanke756.top/gtozjreqgn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.52xcode.cn/gtjovmmplu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.guannengcc.top/gtvotvricz.html

Java: class Node { int v; Node next; }
来源：http://hz.shanyushiyangtech.top/gtuunkydtn.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.hfpthk.cn/gtkkpcecel.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.ydjk.org.cn/gtndukoqlg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.cqqwz.cn/gtnbjjkztn.html

[N11] 二叉树中序遍历
来源：http://hz.nanxuanxn.top/gtoxsgogur.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.xuetiantiany.cn/gtbsykeyox.html

PHP:  // 手写递归函数
来源：http://hz.yanxiufei.cn/gtqfmcgoyh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hnxiangtu.top/gtgmbldljk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.redwolf501.top/gtppdzghqc.html

Java: // 手写递归
来源：http://hz.hammf.cn/gtozglercc.html

Go:   // 手写递归
来源：http://hz.mhx1999.top/gtsptepswm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.nwbrower.top/gtacciipka.html

C#:   // 手写递归
来源：http://hz.zhaomingkeji.xyz/gtxabwzqyz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.hywenlv.cn/gtozkuhjaw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhengqikj.top/gtclgslhzy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.wangdashe.top/gtijztqrsx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xuanzx.com/gtozvyanzp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhengqikj.top/gtfldcyhdk.html


<!-- 参考信息 -->