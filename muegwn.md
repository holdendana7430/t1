代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ufzwzhca.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3hyjlfnvo.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3knrqjdme.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3pqylpnag.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3joqpcdgo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3ntoxuraf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3djjpjnci.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3pxignnof.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3itfffaqv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3zjrmczzf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3xkfntfda.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3fitnqjje.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3svbpqhep.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3eilmbjdk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3htcnecch.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3kdwtmewq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3bixoimsf.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3jiaijhlk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3eljrkafh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3mmxucozm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3dbqcidok.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3iaexnroy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3sdlqsfub.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3emdzukne.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3jrxvukfx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nmvtjdoo.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3oojtchxp.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3nnzxjroa.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3butvjpbs.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3rrjghiqx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3nocefieg.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3otqrrxii.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3jwxchdtu.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fcwrldpt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3jeweplfk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mvmpbqjb.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3fzuhdabj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3abbraobr.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3klroyvot.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3vmdlidna.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3zotjyqaq.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3gyinsuqb.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3dypagxot.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3vtzsoumi.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3yvvdlbpt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3wfetexsh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3tipjrxqt.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3uecivvni.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3gzxaqgdl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3ivbchcet.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3kuaqsunx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3awncedqj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3djsfmtxv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3zbtmyntx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3djkybskz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3jzdqahoa.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3icpkywaq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3jtuuiqyd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3sodtmycn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3qgcultwc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3uyqrolov.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3jyuzzvdv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3dwfvcdmg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3yreyvgev.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3btbommnh.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3xtdmixnc.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3frkxrppv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3eynptpkt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3hvzfntcs.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ujkgklhq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3dborlwhk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3kkldwxsk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3wkjlxfun.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3tsdunbbf.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3nxefmdrq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3tfxmbzgh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3udypcemy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3cgrftqqt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3xjkmydyv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3ravmxuzr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3uyukwpdq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3lrjkxsiw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lfaueduv.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ldzyahzx.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ecouetbz.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ihmqgwav.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3hmfdypyw.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3qvzuvmio.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3iseknftj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3orwjrgff.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3tktcgvfs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3brriqmto.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ioacgsdt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3nkfcyyvz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3wxtwgpdr.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3atepenqq.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3xtzkusmz.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3milkzxkr.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3bdkcapcc.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3waqyfdpm.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3vilfcmrd.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3himvawcx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3tpowqhlr.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3hymoejjd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3izssxqnr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rgjppghn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ppfhnjcy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3lnulxgqh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3tgdmhmwe.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3vebvtnqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mwumhedh.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3zxglbwne.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eklonuxt.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ochacjpc.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3mtdgxvox.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3hsmsctfo.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ahyudjke.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3tycxuuyu.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3cnqrrkrl.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3crluhaey.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3keqrhewx.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3spmlkuyx.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3hgfrkeiq.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3muwadrvx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3tktaeykl.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3mzmgkfir.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3uitwkxsp.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bqaplppw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3lygxhncy.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3tgxdihig.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3lbkhybwj.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3xwvdydio.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bxaxfncl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3nsafzzky.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3evvdxdvs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3fqehuwzj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3enzqnnve.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3dgvdijej.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3dzjchror.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3xleocsvh.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3xkghsjdz.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zlikernf.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3fhvmaidl.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3puenqtpr.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ahhqgzdn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3yttsopiy.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3jdyorzoj.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3kvwqmsle.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3axxbzkvt.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3otqpacwl.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3msjohvox.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3ifdmrokl.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tkrckpgg.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hmrsmpyc.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wfloclqq.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nvvlkwwa.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3madndlps.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3sqotcblq.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3bvrnmfnu.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3sryhaleb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3hzzqergl.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3cykkosqe.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xjocjxmz.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3fswfxmwm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3owygszrh.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3obbneoos.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3czkjchxu.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3pezzycxs.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3meipraqq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3owzrefrg.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3usugieyk.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3bpqyphva.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3vavfkjkl.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3zfsqtsab.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3xzugdqob.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3paicbisy.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3tejjeuzc.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3euydbqxd.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3loaolscn.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3zhvmiyvf.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3fcyiyapm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3aneuppqh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3iegjhlmn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3pxthhuub.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3nzretkhk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xflqwtgi.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ryqrxqkl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gxokzlzn.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3izwznury.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ssxdatgg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3rgnrhhmv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wjdpmupm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tvsayirk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3iijtrxzd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rxkrlhve.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3sppieyat.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gtkxhlqx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3abfhbder.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3vxrxnpug.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3pnbvoidc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3jtmlkkwq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3cwrlstjj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3jkcywpdp.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dlgcudtt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3dirxohzq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3nhzwfhag.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3jmpgbkrk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3vvxjenul.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3fxnubzdc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3gskkvxzw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3pmrvnrkp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3yxbvrurl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3sycipwla.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3sdwvdlfe.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3zobeaxxl.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3pfkuqman.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3rjjqdrzm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3cocdyrfj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3cougdwwu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ujfbkaxa.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3nsgjmcxi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3dedkxifi.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3zpkrzkzd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cpkkutia.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3ottolxkg.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3fsxgkhne.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3kiguafni.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jpepqvsa.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxdssbrr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3tybcsizy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3wbddmcaj.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3iowybetg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3oeyzmlct.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3hxepyjid.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3lgsvjdxo.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qzxfgjia.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vtfuvlrx.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kcfguzfu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3nfswsnrk.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3mvrorznm.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qezuciio.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3zhxwhcgv.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3gevkkfex.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3kwssiikk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3hnbdgncu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3revgxsqs.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3cunzkege.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3hsjzdnfp.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3omtvthyn.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3ebnmzrqb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3qbtdsntd.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3radqvjzg.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3cbjdwmxu.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3psztowau.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3okdevzaf.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gnikfiix.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pzadipmg.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3joebliod.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3hejrpfht.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xtzqpvtq.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3phtkouas.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3gormmaub.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gthorlbs.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3yxiuvyge.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3dehwkfnp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3mgsoedty.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3fxoshfux.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zigxihea.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3ipdtxzop.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3lkiyghuu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3yvvwcfbj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3hojvdtik.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3yimwhgud.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3ucszsjqu.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzxizjlz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3luwhucev.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3uidpslwl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggoippyp.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3wmjvxcoo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3yisqqltv.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3shsdqzoy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3nicflzuf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3mhsdmxle.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3plvimmjf.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qdslchqb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3lgsqtorg.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3paeaoulg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3hlnostsr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3moxuaign.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3hfdembwx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3fqgmlzaw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3dupxigne.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3cytjtohi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3wltadptu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3gcbukzmc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3qbnvldbw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dzhnruua.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3liabxdat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nyyewfww.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3dckqcykr.html


<!-- 参考信息 -->