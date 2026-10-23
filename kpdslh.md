代发 wailian999

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3ngbcdoio.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3sfmlpudy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3tkmvrwif.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3yxfsocbm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3btnivvll.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3ymcstdnc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3epksnsyv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3nnzfnodp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3uwlcvzyg.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3rykpoiao.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kknsekbs.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3mqkkwsvu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pblpszrc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3uwwsjuqp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ruwphfgx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3lrobtedy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3dgibeika.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fzmslogj.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3wzubjzzs.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3gibittwx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nkqmaqws.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3tojraedc.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3rgbzwtyi.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3kjxdirwi.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3hgxzjxwr.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wohgttlq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3mcmnuytl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fvfibvce.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3aewvxmyg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rctcspxw.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3fbyvgudl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3mgdoxdpp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3wpqybwpv.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3bxecleik.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jlerghbv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3vrwptcla.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3spexprxi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3yntypskq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3taaejjud.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3scoartcn.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ianumffj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3tvxhuwkv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3btmrvejs.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3bnffybpy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3jrxcxqee.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3rgpschxx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3ubkcurcj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3zmghsivs.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3bqaffqte.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3ogemwtro.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3altoycuu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3fcenepnf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3kcmkemxi.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3jrmlzrtk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3xdzupcuo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3jxryjgtn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3sutynzou.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3lsocdxbf.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3gevveosn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3dbndtefo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3cczizhgz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3yhzboerv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3grmbcdcb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3sdkbhpax.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3mnlscpoo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3hkwvtnmd.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3vfijcddz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3xkwihdlt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3gtamtkmq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3kbnhmkzf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ybxpkges.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3apynnkep.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3glhdzdxq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3ztuwirpu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vhkgzjys.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3amxnfnmp.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3lmkfzpgh.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3rrnudquc.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3shlphteh.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3humhpcoo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3uhsepvur.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3efqbjkan.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3bjqqzsdq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3eensoxnd.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3lcrejhzo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3gldwzwxa.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3uaijxhhu.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ftxlttro.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3zcaamhmc.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3uowcqeih.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3gkqmojae.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3dxktbxxz.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3obodeugr.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3jdvwdgvs.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ogurlkua.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3pghvzmez.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3qayxdtja.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3pxvjcboj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3bncijatg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3pvycmfrg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3gunutenq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3wdukpojj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3adkdmtdb.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3lniouqfu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fwzasdnc.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3zcwkxbbj.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3rtwobgvh.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3jlcgsmdz.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3wigvjsxk.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lndhaqfd.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3wpmyweif.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3pkrbjfit.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3hzfgaapm.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3uikjkghl.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3cgigcdnk.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3psnidhfa.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3sxianxad.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3tcrgcrzb.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3mldlzxlx.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ssiowflz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3yauyeobr.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3eypcterg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zagqivee.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3qqplkczu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3bltzmqsn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3oiclklgt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dmarxxxo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bdxqrcjx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3mwkqufqs.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ddtvuxfo.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3csoemqxs.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3fiqarvkt.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3hqsgxncp.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3quywusgk.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3yrhbvlqv.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3hkgmnjfj.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ulhdysuv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3zzmpsghs.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3cydabkgz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3xvkzpihp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3zvgiofgq.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ldwqqhcu.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nfxnsvua.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3kkrifjih.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bojzqarp.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dejitvxv.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3whabliel.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hwifknjt.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3mqndcwiv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3kmjqkuwd.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3yrhhtldt.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ptlozaqa.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3cqdzrvya.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3akixahav.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3xgltedrd.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3smssotcq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3sgrdwegr.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ouqmaczz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3bbzldzay.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3gtfngnbs.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3sczefgzb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3zozmqucm.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3cexrvahw.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3qkkdrzpp.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3tfxquhve.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3hpgmqrow.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3esibkvjd.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3dtmzfsym.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3rxsednku.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3rzgazbut.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3jloliyhw.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3xlcfdhqn.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ybpaolbr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3tehrlnyr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3djcozbas.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3sawdtzwg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3xydzurng.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nwsbgmey.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3nqsukfpz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pgrxpzrb.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3qzzvoees.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cyvigucc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3rgehbtqh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3pafjbamn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qyxnlltp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3doiwgkhp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vwgynqio.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3lomzithh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ejmovbmy.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3lxwbyjju.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3hoamlpzi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ioioubjy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ummsemvu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3fdbuvnzm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3wdddrmim.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3pstqoqds.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3jtbcfobq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3qxsrlgto.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3clfscvcx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3kmjfrccl.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3hrfchbeg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3nrvbulyh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3qyslvyja.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3swszlanq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3uqfrtwvs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3axhqdnpa.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3govlgvws.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ndikpxzm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rqtisvbf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3tymzmoyp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3jjcavzmq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3hpjwwnnp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ndhoveyh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3grlnxoun.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3kykwbvne.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3loeiazmb.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3drmbyapb.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3fswtnncu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3deoorymz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qubnltbi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtvemhmh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3ckdiewnw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3iilmtjmc.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3mmboekhi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3ihhlcgxi.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3aqojizbc.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3hsltccri.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3eaalxemn.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gewtlolx.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lvnjzzsw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3qyzynbuy.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3yqavfyzc.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3wadrzcyw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3etxttrfi.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3qzteyuhu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3bktrewoa.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3lewbvxhr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ghkmgngd.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3daabdvqs.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3kxhxourq.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3rsudiazi.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3xqyrmmnz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3kdkfdzac.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3ymzpbbln.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hjbvxtht.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3zpekqmsg.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mebeoqgd.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hchtuzjm.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lgqwtllb.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3izfbiiya.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3fatzejlv.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3earpmpae.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3svqorlda.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fxrsfnna.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3pumbfygn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3abnqnsdp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3xwggrjkn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3nzlcpzwf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3kfmjupbs.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zxayydoo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3vfrjxgyp.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3osjimbxh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3ywbdthjb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3iioiktxn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xqdilplh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3mzqdbrxs.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3musvnwac.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3uytnqsjd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3xjddyytk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3rtkuptjq.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3oqbuefff.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3rlcbixgt.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3xsgsbovu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3lwwfkgyn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3lopjzmdx.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3sxyukttw.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3uhatveiw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3ldivuujp.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3zsjhmyqg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3oypmwkgf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3wzjrouwf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3wgpfygtf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3fvloyqrv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3zwalupum.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3zzdlybar.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3ftsknbcv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3hpizrree.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3hrzbmeke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fmsmpxgz.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3lluyrbaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uojkhoig.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3xoihmplq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3tkkthewe.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3saplckoe.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3lzpodjeo.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3izigwwln.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3cscqgaay.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3uamqqavp.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ojmfqila.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3aolpihuc.html


<!-- 参考信息 -->