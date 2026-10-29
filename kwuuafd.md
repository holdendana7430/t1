代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gnqafgfru.sHtML

[K07] 进制转换
来源：http://read.share.zdbjq.cn/Article/details/ghxfgnufx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gbzlafrfn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.zdbjq.cn/Article/details/ghammsaud.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gltfabbdb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gwekanmwl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gpqphkksw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.zdbjq.cn/Article/details/gslfjpvbk.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.zdbjq.cn/Article/details/genllwckz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gdglokxov.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.zdbjq.cn/Article/details/gvvglpeqw.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.zdbjq.cn/Article/details/gxvpjbcep.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fehbvm.com/Article/details/ghklhbmoj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gaiaixsze.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/ggroqivlt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.hesvh.cn/Article/details/gytlrdplj.sHtML

Go:   encoding/gob
来源：http://blog.fehbvm.com/Article/details/gczjooord.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.hesvh.cn/Article/details/gpgiilpqr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gpiuxgpbz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjqkwhvwe.sHtML

L. 网络请求
来源：http://mobile.fehbvm.com/Article/details/gvhuyuebj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gldtabgop.sHtML

[L01] 发送 GET 请求
来源：http://www.share.zdbjq.cn/Article/details/gqysuflms.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.zdbjq.cn/Article/details/gostuogen.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.hesvh.cn/Article/details/gsxgxmvbn.sHtML

JS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gcqotdtwh.sHtML

TS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/gdlokupya.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fehbvm.com/Article/details/gexsaazwy.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.zdbjq.cn/Article/details/gjntlxadl.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fehbvm.com/Article/details/gjlhawtjy.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.hesvh.cn/Article/details/gyagvugoj.sHtML

[L02] 发送 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gaesrfhip.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fehbvm.com/Article/details/gvxfsmrba.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.hesvh.cn/Article/details/gluslzifs.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gudeibpoc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gsdkprkeu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fehbvm.com/Article/details/gtlkynzik.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fehbvm.com/Article/details/ghyvugape.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fehbvm.com/Article/details/gucgdglmy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fehbvm.com/Article/details/grgiyfxwq.sHtML

[L03] 设置自定义请求头
来源：http://blog.zdbjq.cn/Article/details/gzxdygazf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.hesvh.cn/Article/details/gacxtxjqg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/gwrlqcjhz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gvtwpsfpu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gwwewwnrp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.hesvh.cn/Article/details/gydumllrd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gbuzdphex.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.hesvh.cn/Article/details/gysmcphgo.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gizlnzecr.sHtML

[L04] 设置超时
来源：http://baike.hesvh.cn/Article/details/ggpptfecd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.hesvh.cn/Article/details/gmpqudzti.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gxdtkdysl.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gscljbkyq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gahxrhfwm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/goolyluqc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.zdbjq.cn/Article/details/gxnnuorfw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.hesvh.cn/Article/details/gfpgpdory.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fehbvm.com/Article/details/gumknhunm.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fehbvm.com/Article/details/gltwvbtmz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fehbvm.com/Article/details/gcyvtirif.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fehbvm.com/Article/details/gjoznbjwg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gnbyhgnfq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/ghqnretkn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/gzkifosrz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.zdbjq.cn/Article/details/ggbepvdih.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.hesvh.cn/Article/details/gxqdwrmxa.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/gynntmgaa.sHtML

[L06] 解析响应为 JSON
来源：http://blog.hesvh.cn/Article/details/gpcmmofod.sHtML

Py:   resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gzmokxeee.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.zdbjq.cn/Article/details/guwjmxfyz.sHtML

JS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gthafqtfu.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gprpddjli.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gtckcsrom.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/gcvdhlbmi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.zdbjq.cn/Article/details/gwmdzrtyr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/gorqtgnxe.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gynzqmuaa.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.hesvh.cn/Article/details/gavvefjoe.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.zdbjq.cn/Article/details/gvxbzxkkv.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gldmksjus.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gdfnbmqbh.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/gvrkpnbmo.sHtML

Go:   resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/guxuzrmkh.sHtML

Ruby: resp.code.to_i
来源：http://m.share.zdbjq.cn/Article/details/glglbraxp.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gelasovob.sHtML

[L08] 并发请求多个地址
来源：http://blog.fehbvm.com/Article/details/ggreebeut.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.hesvh.cn/Article/details/gwjnkhmyv.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/gkpopuawm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gfitbxgss.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gdgilfmkk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.hesvh.cn/Article/details/ggagscphp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/gatircpbf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.zdbjq.cn/Article/details/glfxxtxxf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/ghlbkiznm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvucvhshz.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/gcjczqrsw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtifuimjd.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gdcfaainw.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/gmfwaubyd.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.hesvh.cn/Article/details/gruxalkab.sHtML

JS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gbdcyuxft.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gsjqlfkmy.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gknvazsnj.sHtML

Go:   os.Args[1:]
来源：http://blog.fehbvm.com/Article/details/gxiudxjvk.sHtML

Ruby: ARGV
来源：http://www.share.zdbjq.cn/Article/details/gppciugiv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gclatodyy.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/glnntqljm.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/gtxrqjfbj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fehbvm.com/Article/details/grwpvblld.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gkzxicrsd.sHtML

TS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gygaoexpc.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/geopclwaf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/gamrmczsj.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/gttdfhbpd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gqdrdvqzs.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gquapbqdc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gkqksglwk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/gjzarcwhs.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gytsfgesu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gqxncfugn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/ghjcffmth.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.zdbjq.cn/Article/details/gzdacgpyc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.hesvh.cn/Article/details/gmsuzunko.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/gagebnmfa.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/greqftcko.sHtML

Py:   os.getcwd()
来源：http://mobile.hesvh.cn/Article/details/gmwmaqnhf.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/grfytdkxc.sHtML

JS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gkmmxakqe.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gjugnxqpy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/ghkoaybhl.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gjkxdjfxb.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/gvljshitu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/gpuxlitia.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gvjonzpek.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gfticmmwv.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/gluiqpnim.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gnhkawhsw.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gbkxbncuu.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gzaxhjfsa.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gedjzkivr.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/grxrbegsr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/ghtlmfjfk.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/gmdfvkppq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gmatzrgdk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fehbvm.com/Article/details/gtdprsrlh.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gvgfczaht.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gaimqrmyf.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gssusgavq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.hesvh.cn/Article/details/gpctfhoai.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/ghbfnqfds.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/gftabcglg.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/gbdrnysia.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/gqabmbqjf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/guahcktgq.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gnlcmvtcw.sHtML

TS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gdthmaetv.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/giqaunkmh.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/gkkgpqbyk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/gugnbgmuf.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/grdywlgau.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/gblpneliq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.hesvh.cn/Article/details/ghpyqrwlv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gwhkdjhca.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gqytwpjva.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gjootafao.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/glfuccizj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/gpramzqrh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/gwnwjilbb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/gixqcedii.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtqhvovlw.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/ghbyrxvvc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsuypgznj.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/goeclwirb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gqrxrqcdt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/ghgmntfoy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/grmefybuq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gnpvovoow.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gusiciuva.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gefnqorqw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/glnctejon.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/goshivtqj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/ggokcgswc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gcyivkuai.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gdmppuqfd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gffusicyb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gdpuqzevf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/ggvubdqqr.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/guvtqxzof.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gkgjufime.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fehbvm.com/Article/details/glavoktbn.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gxpxizgxn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/ggswgzwst.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gxsagyeja.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gcdvlumzd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/guzgrskns.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/godfcetgi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/gmjnkjttk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.hesvh.cn/Article/details/gxzvvntqj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/ggchzkpvk.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/gdzvssmpj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gwfggoyyk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gcspykvsh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gblcnskjg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gjiyrytji.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/grszdfrtt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/gedwhermy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gljsvrdfh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/geosncxbv.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/gyouqndlg.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/ggkuvwhnh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/gtcpcpciv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/ghjvcculr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gzrbgnzga.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gwgiqbgjy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/grxkftlev.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/gwgkfeffe.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fehbvm.com/Article/details/gkqmtlnzv.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gjbtsrgsz.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gifjrleha.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/gazpadvfp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gzsgigtsr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gwsdgutfr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/guzgtkbgi.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.hesvh.cn/Article/details/gniiqisat.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/gzvcdgebq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gkxmipyky.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gnysqbunf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.hesvh.cn/Article/details/gcfblrlhu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/gbwkajajt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/ggjrmcabw.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fehbvm.com/Article/details/geuzxkrwa.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/gfrjcorzr.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/gpuqctnab.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/gdlvvieki.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gytnqridf.sHtML

[N08] 生成全排列
来源：http://www.m.share.fehbvm.com/Article/details/gifvyvamu.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gqrhsaxsp.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/glhrzwcgg.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gucefjxec.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gdfhujtff.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gtadybqxs.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/grqcbxaip.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/goprgptvo.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gzrbmyawp.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gyqergyxx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gpvgtmyzg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/guppqubap.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/grcctgxyg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/gghsnmbkh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gxuffrukz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/gbzoogpdz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gdwqwbmhh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.zdbjq.cn/Article/details/gzpxhlvgu.sHtML

[N10] 链表节点定义
来源：http://3g.zdbjq.cn/Article/details/ghqelwwjf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fehbvm.com/Article/details/gatydxxog.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/gwdazlczc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/guwqmslbz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/gflbkutbl.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gptvfiqio.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/giuhtdwzu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/gqbxpgzly.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/gkusbbaxj.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gnplrsefw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gaochfrgz.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/gyqmdfuyy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gddxqvpsa.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gaziffwrv.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/gvkdxhrxd.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gepstuhrs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/ghjgclvcn.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/ghufwcevu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/gduzsnjll.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/gesclngos.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/gziecdewl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gmbjqigld.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/ghesnaqyn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gkslcxbio.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/gjfpjsady.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gcjwfoyxy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gwihkbqvp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvavfqqst.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/gfbqainen.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqwmvxmfy.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gqbigymmd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/grmhhvjri.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fehbvm.com/Article/details/gefyqhcgd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fehbvm.com/Article/details/ggmedvlzz.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gvlaqwxaj.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/gjtnmjhte.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/gnrpsafjv.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/gumwxdvjo.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gcpxeokkb.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gxsrbbviu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gqwqctltw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gltnwnilg.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gwrqhngmk.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gdmbhnrhe.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/gebzkatqk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.zdbjq.cn/Article/details/glsokrxdo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.zdbjq.cn/Article/details/gpicgdipr.sHtML


<!-- 参考信息 -->