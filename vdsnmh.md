代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://hz.nanxinkj.top/gtkqmbvufz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cucudq.cn/gtasqjgnod.html

[K04] 读取 JSON 文件
来源：http://hz.zhixingplan.top/gtzodsopkg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jinqigfzy.top/gtscwiyltr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.guannengcc.top/gtobghbozr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.daxiang520.top/gtvbhmmuyq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhixingplan.top/gtcoyftxjb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.snrcjt.cn/gtemslthao.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.nanxuanxn.top/gtgstmhhkp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.tanke756.top/gtbcpbvqll.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ivvv.top/gtpehnhubg.html

[K05] 深拷贝对象
来源：http://hz.feifeiyinyue.top/gtwuyzvews.html

Py:   copy.deepcopy(obj)
来源：http://hz.9152youxi.cn/gtadipvbjj.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhaomingkeji.xyz/gtlfaxxlcb.html

JS:   structuredClone(obj)
来源：http://hz.cashguo.top/gtemcjikax.html

TS:   structuredClone(obj)
来源：http://hz.smart0.xyz/gtzznehnas.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.52xcode.cn/gtpjrqmhdo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.sweek.top/gtmwtjwkgj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zycfv.cn/gtolfapalh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.daxiang520.top/gtifcnshdo.html

[K06] 解析 URL 查询串
来源：http://hz.wangdashe.top/gtgaharcwf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.meibo888.top/gtmhbhlggh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.ydjk.org.cn/gtjymtxxau.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sxryk.cn/gtnfzltvhb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yongpay.top/gtcfvqzkdf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.fzhhl.top/gtgnlygtgn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhixingplan.top/gtturknmgq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.kuanghao11.cn/gtvlesdpqw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jqgufenzy.top/gtzcgqkmhy.html

[K07] 进制转换
来源：http://hz.yj20258888.top/gtqfwvzvtg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.sweek.top/gtxsorgdzz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yonumen.top/gthlyxrfdy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.gogol.net.cn/gtkuvvenux.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hfpthk.cn/gtjijunqpx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhijiandao.cn/gtrxbifqsm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.vqdsnc.cn/gtsmnuzgnf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jqgufenzy.top/gtlceqyzti.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yvedp.cn/gtwipabxqo.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.nanxinkj.top/gtzyykmnps.html

Py:   pickle.dumps(obj)
来源：http://hz.nanxinkj.top/gtutgynorl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.guowangkeji.top/gtujvtkblm.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.sufxvd.cn/gtcseousoa.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.iojbl.cn/gtesbylhjd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.daxiang520.top/gtlguivvpe.html

Go:   encoding/gob
来源：http://hz.birdmap.top/gtxrgkogqv.html

Ruby: Marshal.dump(obj)
来源：http://hz.gotoacloud.top/gtynaaqrqp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yj20258888.top/gtcxopmwte.html

================================================================================
来源：http://hz.yangfankeji.com/gtyyamxhvo.html

L. 网络请求
来源：http://hz.yueranfly.top/gtemgnzfdc.html

================================================================================
来源：http://hz.ivvv.top/gtwvmkuihf.html

[L01] 发送 GET 请求
来源：http://hz.ydjk.org.cn/gtqddqwulr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zhaomingkeji.xyz/gtmnsvcufp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hammf.cn/gtvebezuhy.html

JS:   await fetch(url)
来源：http://hz.xuanzx.com/gtuvbaaymq.html

TS:   await fetch(url)
来源：http://hz.cheryme.top/gtnlodzjdy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.aibaodan.cn/gtzhxekolb.html

Go:   resp, err := http.Get(url)
来源：http://hz.yueranfly.top/gttphgxdxw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.sufxvd.cn/gtjqfxuiko.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.c1oappe.top/gtfqhzesaz.html

[L02] 发送 POST JSON
来源：http://hz.meibo888.top/gtcbhurcur.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ppjwa.cn/gtbtrqsyxm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.dashuyun.cn/gttmyghogu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yj20258888.top/gtaoiajmmc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhixingplan.top/gtprblixll.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.tanke756.top/gtrieivzzq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jianghu66.top/gtydmnkxjn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.sxryk.cn/gtlzaezmnc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zhixingplan.top/gtujbkrhjz.html

[L03] 设置自定义请求头
来源：http://hz.gotoacloud.top/gtfbakmowa.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.mhx1999.top/gtfxgpnspz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.iojbl.cn/gtuukycoly.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cdnleiting.top/gtjnizwopy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ydjk.org.cn/gtuimrvugb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hnxiangtu.top/gtsccjalxt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zycfv.cn/gtjsubeedg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.pycfn.com/gtpgxnuusm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.daxiang520.top/gthqhepsqu.html

[L04] 设置超时
来源：http://hz.xingfuxueyuan.xyz/gtrcycqxji.html

Py:   requests.get(url, timeout=5)
来源：http://hz.pengpengdd.cyou/gtbfvzmscp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.52xcode.cn/gtfouknisg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.chenjidiqi.icu/gtlpbudovo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.0kj1m.cn/gtbtycwyoc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.shanyushiyangtech.top/gtiwpnwbau.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.shanyushiyangtech.top/gtqmigsutf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.nwbrower.top/gtxqvyafhw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hfpthk.cn/gtgcoozdke.html

[L05] 上传文件（multipart）
来源：http://hz.fzhhl.top/gtbkifktfg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.birdmap.top/gtlsrucelv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.ehwqpu.com/gtwwckfcas.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.52xcode.cn/gtzxhxncgy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ppjwa.cn/gtpboeaasu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.shanyushiyangtech.top/gtpevaqnrh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yangfankeji.com/gtzwdypoko.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.sufxvd.cn/gtdijmozyw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.xuetiantiany.cn/gtynomeesz.html

[L06] 解析响应为 JSON
来源：http://hz.shanyushiyangtech.top/gtaoqrmnty.html

Py:   resp.json()
来源：http://hz.aibaodan.cn/gtwyxusuab.html

PHP:  json_decode($body, true);
来源：http://hz.andypj.xyz/gtiqhxyarh.html

JS:   await resp.json()
来源：http://hz.yj202588.top/gtgipcwlha.html

TS:   await resp.json()
来源：http://hz.wangshuangyany.cn/gtbcsancdb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jinqigfzy.top/gtwqvpemhl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.feifeiyinyue.top/gtourmylph.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yvedp.cn/gtzyoinvah.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.aizwys.cn/gtyqswawvi.html

[L07] 处理 HTTP 状态码
来源：http://hz.zdqjudy.top/gtidgjjseo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.andypj.xyz/gthnozsucp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.daxiang520.top/gtivmxofkw.html

JS:   resp.ok;  resp.status
来源：http://hz.zhijiandao.cn/gtshvxtnun.html

TS:   resp.ok;  resp.status
来源：http://hz.andypj.xyz/gtzmtlvhfl.html

Java: resp.statusCode()
来源：http://hz.yanxiufei.cn/gtamwnlvef.html

Go:   resp.StatusCode
来源：http://hz.316326.xyz/gtrquuecyt.html

Ruby: resp.code.to_i
来源：http://hz.tianlin.xyz/gtfcxyyyqx.html

C#:   (int)resp.StatusCode
来源：http://hz.yanxiufei.cn/gtpxwlbcrs.html

[L08] 并发请求多个地址
来源：http://hz.nanxinkj.top/gtwdrndjkd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.kuanghao11.cn/gtspcnrwqw.html

PHP:  curl_multi_init() 系列
来源：http://hz.cqqwz.cn/gtgtkzobbp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hysaishi.cn/gtfrpkfphm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yuanzhike.top/gtnnornmko.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.gogol.net.cn/gthgxrilin.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jinqigfzy.top/gtdfbnqgyi.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yj20258.top/gtgshylfvs.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xingfuxueyuan.xyz/gtkscweusf.html

================================================================================
来源：http://hz.zhixingplan.top/gtygmiyqnv.html

M. 命令行 / 进程 / 环境
来源：http://hz.hnxiangtu.top/gtcogtgdwq.html

================================================================================
来源：http://hz.yongpay.top/gtcjhnnank.html

[M01] 读取命令行参数
来源：http://hz.c1oappe.top/gtrumidhur.html

Py:   sys.argv[1:]
来源：http://hz.316326.xyz/gtstgxqiyz.html

PHP:  $argv;  $argc;
来源：http://hz.yueranfly.top/gtfkdkpuvj.html

JS:   process.argv.slice(2)
来源：http://hz.bjfxy.top/gtiaccbcjg.html

TS:   process.argv.slice(2)
来源：http://hz.cheryme.top/gtzufgiicw.html

Java: args 数组（main 方法参数）
来源：http://hz.wangshuangyany.cn/gtnkcxtsjl.html

Go:   os.Args[1:]
来源：http://hz.cucudq.cn/gthksafxhr.html

Ruby: ARGV
来源：http://hz.zycfv.cn/gtmwrtsbdg.html

C#:   args 数组（Main 方法参数）
来源：http://hz.shuidangran.top/gtwssoberq.html

[M02] 读取环境变量
来源：http://hz.zdqjudy.top/gtyjuxqbrs.html

Py:   os.environ.get("HOME")
来源：http://hz.tanke756.top/gtngxpnlgc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.shanyushiyangtech.top/gtnzfqoofw.html

JS:   process.env.HOME
来源：http://hz.xuetiantiany.cn/gtdkxfpafi.html

TS:   process.env.HOME
来源：http://hz.aizwys.cn/gturgvwzzl.html

Java: System.getenv("HOME")
来源：http://hz.cucudq.cn/gtptekyotl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.fengsongda.top/gtcqbkpomx.html

Ruby: ENV["HOME"]
来源：http://hz.jyoumei.cn/gtrnbhksjx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zycfv.cn/gtobuewcua.html

[M03] 执行外部命令
来源：http://hz.jinqigufen.top/gtmjkxihrd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yj202588.top/gtsdqqaijf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hnxiangtu.top/gtdsirniwo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.shangyingyoupin.top/gtxxdhwafe.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.tian-w.cn/gthvfkqjmj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.sysykeji.top/gtyiddlcks.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jianghu66.top/gtzvyvuekw.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.birdmap.top/gtnffjahwo.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhongyouzk.top/gtttamxcrh.html

[M04] 获取当前工作目录
来源：http://hz.nwbrower.top/gtccnotdpa.html

Py:   os.getcwd()
来源：http://hz.zycfv.cn/gtdoiifiac.html

PHP:  getcwd();
来源：http://hz.dianchejie.cn/gtbynuqbsl.html

JS:   process.cwd()
来源：http://hz.mhx1999.top/gtdvqyiwyy.html

TS:   process.cwd()
来源：http://hz.redwolf501.top/gtzfiphnfo.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhengqikj.top/gtuipghbvw.html

Go:   os.Getwd()
来源：http://hz.tanke756.top/gtgusjyewz.html

Ruby: Dir.pwd
来源：http://hz.zhongyouzk.top/gtvrrxvzol.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jinyuanbaomall.cn/gtzyvwykbo.html

[M05] 设置退出码
来源：http://hz.dianchejie.cn/gttmdyghby.html

Py:   sys.exit(1)
来源：http://hz.zhaomingkeji.xyz/gtylyjndry.html

PHP:  exit(1);
来源：http://hz.hnxiangtu.top/gtaghcdqkc.html

JS:   process.exit(1)
来源：http://hz.316326.xyz/gtclaqaoeo.html

TS:   process.exit(1)
来源：http://hz.jiagoushi.top/gtwnqooidc.html

Java: System.exit(1)
来源：http://hz.zhijiandao.cn/gtwjbcqbdk.html

Go:   os.Exit(1)
来源：http://hz.yongpay.top/gtunwoxcoc.html

Ruby: exit 1
来源：http://hz.guannengcc.top/gtgnxvzqgj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.tianlin.xyz/gtrdfbmnpx.html

[M06] 向标准错误输出
来源：http://hz.sufxvd.cn/gtmppioizh.html

Py:   print("err", file=sys.stderr)
来源：http://hz.cucudq.cn/gteqvfjxsz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ydzc1.top/gtmnqsrtgt.html

JS:   console.error("err")
来源：http://hz.sxryk.cn/gtlesoirky.html

TS:   console.error("err")
来源：http://hz.9152youxi.cn/gtrgqzmshb.html

Java: System.err.println("err")
来源：http://hz.aizwys.cn/gtlwmasfwl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.52xcode.cn/gtpolqiipv.html

Ruby: warn "err"
来源：http://hz.yonumen.top/gtctrsimba.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.andypj.xyz/gtgwpzcufa.html

[M07] 判断是否为主入口
来源：http://hz.aizwys.cn/gtuvomdhdf.html

Py:   if __name__ == "__main__":
来源：http://hz.sufxvd.cn/gtsbinkxnx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cucudq.cn/gtzxgmuffc.html

JS:   require.main === module
来源：http://hz.yuxming.cn/gtpbpuqgfz.html

TS:   require.main === module
来源：http://hz.52xcode.cn/gtybzxlvii.html

Java: public static void main(String[] args)
来源：http://hz.fzhhl.top/gtskwdjufr.html

Go:   func main()
来源：http://hz.ydzc1.top/gtyqymhwwz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.daria6918.cn/gtcvppfltb.html

C#:   static void Main(string[] args)
来源：http://hz.jqgufenzy.top/gtfooczqmh.html

[M08] 获取系统与运行时信息
来源：http://hz.gogol.net.cn/gtansuocgz.html

Py:   platform.system();  platform.python_version()
来源：http://hz.gaohongyu789.top/gtacwhbbtr.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jianghu66.top/gtxzagxohn.html

JS:   process.platform;  process.version
来源：http://hz.hammf.cn/gtcdtnzgyu.html

TS:   process.platform;  process.version
来源：http://hz.ywan-chungtsiang.top/gtccnnqxxq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yangfankeji.com/gtqpebyqoa.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xziqi.cn/gtfenkywue.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yj202588.top/gtmtzlerbt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.snrcjt.cn/gtvsuoyoxf.html

================================================================================
来源：http://hz.cqqwz.cn/gtmjnpxuvz.html

N. 数据结构与算法
来源：http://hz.iojbl.cn/gtmlptiiho.html

================================================================================
来源：http://hz.redwolf501.top/gtiyrntjok.html

[N01] 二分查找（有序数组）
来源：http://hz.yongpay.top/gtxrxiowcm.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gtmsiusixc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.tanke756.top/gtlknvjysz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xuanzx.com/gtnvkvcqix.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.tianlin.xyz/gtxklqjlrt.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.haohaochexian.top/gtdimytown.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.tanke756.top/gtyyxfpsff.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yuxming.cn/gtekilmudi.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yonumen.top/gtchcfucyw.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yuxming.cn/gtpweuoard.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.daxiang520.top/gtzgthrdpm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.snrcjt.cn/gtezggqezj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.andypj.xyz/gtizborjyw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.daxiang520.top/gttksyjehv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hywenlv.cn/gtjibjfqwh.html

Go:   slices.Sort(arr)
来源：http://hz.xinyue.icu/gtucuvakyc.html

Ruby: arr.sort
来源：http://hz.fzhhl.top/gtodfzbaxn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.haohaochexian.top/gtwagnuopd.html

[N03] 快速排序（分治示例）
来源：http://hz.daxiang520.top/gtakdjctru.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xziqi.cn/gtrsdivjzj.html

PHP:  // 递归实现，或用 usort
来源：http://hz.birdmap.top/gthivvrlhk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.kuanghao11.cn/gtykpiqbqx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinqigfzy.top/gtkiaesoev.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jianghu66.top/gtvmjyplxg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.cheryme.top/gtbinznetc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.c1oappe.top/gtslcfqgbe.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.chenlongwang.top/gtpsyfdipe.html

[N04] 斐波那契数列
来源：http://hz.aibaodan.cn/gtuvvmqxyx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.fzhhl.top/gtynfmuoxf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhaomingkeji.xyz/gtokmmlouk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zycfv.cn/gtlfiiomry.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zycfv.cn/gtdsbvkqby.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.svipenyu.cn/gthlmcppnf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.snrcjt.cn/gtthrejzpk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.feifeiyinyue.top/gtxvkilejw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.daxiang520.top/gtgasntwnm.html

[N05] 最大公约数
来源：http://hz.9152youxi.cn/gtifmowfgm.html

Py:   math.gcd(a, b)
来源：http://hz.cashguo.top/gtmdoptehl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.sufxvd.cn/gtrygbbuyz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.chenzaomai.com/gtejxigfcx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.chenzaomai.com/gtzhbhvphe.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ydzc1.top/gtbwrwbxtk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.nanxuanxn.top/gtjfnqvxrf.html

Ruby: a.gcd(b)
来源：http://hz.sweek.top/gtmdhmxgse.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.svipenyu.cn/gthhhdsinn.html

[N06] 判断回文字符串
来源：http://hz.jinqigfzy.top/gtczcaqiek.html

Py:   s == s[::-1]
来源：http://hz.tian-w.cn/gtiuhuubto.html

PHP:  $s === strrev($s);
来源：http://hz.feifeiyinyue.top/gtacsprdtg.html

JS:   s === [...s].reverse().join("")
来源：http://hz.0kj1m.cn/gteukkszad.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ybcxt.top/gtprzxxtht.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yuanzhike.top/gtevwwsvyl.html

Go:   // 双指针从两端比较
来源：http://hz.cashguo.top/gtiwprhkht.html

Ruby: s == s.reverse
来源：http://hz.zhixingplan.top/gthzooeusq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.bjfxy.top/gtfpgwglyq.html

[N07] 两数之和（返回下标）
来源：http://hz.xingfuxueyuan.xyz/gtwycageyn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.kuanghao11.cn/gtylmdpdpj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zhongyouzk.top/gtuqrjkpbg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jinqigfzy.top/gtsqbtuwow.html

TS:   // 手写 Map<string, number>
来源：http://hz.jlsjyb.cn/gtbvvlrqoa.html

Java: // 手写 HashMap
来源：http://hz.316326.xyz/gtqkkmlkxn.html

Go:   // 手写 map[int]int
来源：http://hz.hfpthk.cn/gtwibvjsoo.html

Ruby: // 手写 Hash
来源：http://hz.ywan-chungtsiang.top/gtzmgtlmhw.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zhoulong.xyz/gtuvtiqkcx.html

[N08] 生成全排列
来源：http://hz.jinqigfzy.top/gtuhqzcitr.html

Py:   itertools.permutations(arr)
来源：http://hz.hammf.cn/gtxintmjzv.html

PHP:  // 手写递归交换
来源：http://hz.mhx1999.top/gthraoarja.html

JS:   // 手写回溯递归
来源：http://hz.xuetiantiany.cn/gtizjfzfrj.html

TS:   // 手写回溯递归
来源：http://hz.wangshuangyany.cn/gtmvuyohex.html

Java: // 手写回溯递归
来源：http://hz.hywenlv.cn/gtmetskcko.html

Go:   // 手写回溯递归
来源：http://hz.dianchejie.cn/gtmmxlknno.html

Ruby: arr.permutation.to_a
来源：http://hz.shuidangran.top/gttqqhvujr.html

C#:   // 手写回溯递归
来源：http://hz.cucudq.cn/gtprzgkztu.html

[N09] 栈与队列
来源：http://hz.jinyuanbaomall.cn/gtqmgbxrbg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jlsjyb.cn/gtikebyxzx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.wangdashe.top/gtwxodfynq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.ybcxt.top/gtpnbatynw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jiagoushi.top/gtgjrvukni.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yongpay.top/gtgpuhewkg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jqgfzy.top/gthmevhvds.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.pycfn.com/gtrjglcehn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.iojbl.cn/gtxufcmejc.html

[N10] 链表节点定义
来源：http://hz.yanxiufei.cn/gtldnsoaey.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ppjwa.cn/gtxhmeutjc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.vqdsnc.cn/gtgqgwznrj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ywan-chungtsiang.top/gtllctrqzc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.redwolf501.top/gtbjckteos.html

Java: class Node { int v; Node next; }
来源：http://hz.yvedp.cn/gtnuoguayv.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.guannengcc.top/gtictssfss.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.quarkkingdee.top/gteurxwltv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.sysykeji.top/gtbrsxzcno.html

[N11] 二叉树中序遍历
来源：http://hz.redwolf501.top/gtjgcqoxxz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zhixingplan.top/gtwurafmlv.html

PHP:  // 手写递归函数
来源：http://hz.zhaomingkeji.xyz/gtiofmzpwt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cdnleiting.top/gtoccumkkc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cucudq.cn/gtzkjnwhmh.html

Java: // 手写递归
来源：http://hz.bjfxy.top/gtlytqhvmf.html

Go:   // 手写递归
来源：http://hz.birdmap.top/gtxzkvegxg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.tanke756.top/gtrakiocgy.html

C#:   // 手写递归
来源：http://hz.ehwqpu.com/gtlxuupiwr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.iojbl.cn/gtachnkbgv.html


<!-- 参考信息 -->