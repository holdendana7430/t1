代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3sbixrhly.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3pmmhdjgr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3tfcnpqjl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3ryinvvpq.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3kyywtvaz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3cdesexga.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3exmoogoa.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3ueujjbmb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xqsdiarx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3wuexjvql.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3occigwep.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3odebcvxl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3tdxelkus.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3mnsuqvbn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3uybojchm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3lqxvfzcw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3wwuihyzh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kixzdebo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3soivbdrf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3xygsxfss.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ceczppsa.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tllzcuqy.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3sniyugro.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ilrecrzu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wusosskw.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3jdflutyx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ifokdjwk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3gpinxqyp.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3ztkzxbji.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kqobdlkl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3xvbdsuss.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pumkqxka.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3jcrkrrib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3anjxbzgh.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3mktkihfo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3akpfvgxu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3uvgorfno.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ftnvpvsz.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3nytndmfa.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3vuaafjej.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3wilhmasz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3fcndwiia.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3eilecros.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3rlyxkckf.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3jbwmbxuk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3quwmhjme.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3siyytycv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3mxnrxsmi.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3rrqpbzfl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3jfnszpwy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3mohtbhfd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3raeidjks.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3wpfrmmto.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3olngayxh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3vqpkknpq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3nbjwgnkw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3uekwtswe.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3kdwpxmjd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3cdqehuje.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3lsagkomu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3gxyvtofc.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3nmzlhkuq.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3ogtudqhy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3oievhjpq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3mjniyuqe.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3etzbxoiv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3wjrskkos.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3dmulrmpu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3scxippjw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3adjmlkuc.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3qorbfhlq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3axcbspwb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3thfddniz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3cdozrgxa.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3iuspcwsx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3rfmhchxh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3zvcgkhvb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3ezhtzxcl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3aulmwvrj.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3iggzeorl.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3fvqghmrw.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3gudnrzsn.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3mfyaqwti.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3nkentitj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ksoncoxk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3toxiyadx.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3dkhrrkom.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3znwtnqfh.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3rrijvkev.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3tvmygrtc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3npblgowx.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3xlgryuvr.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3vvmmgfbq.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3wutmrtsa.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3dyoelawr.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3bjlnnkky.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3guihasmk.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3cbhyucmp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3emccbasy.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3biqkszme.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3wlhxsilu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tiwddnlq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3kkxqgeui.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3evvgvvml.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3xkxznvib.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xhbryakf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ruvfncjq.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3cmeiciog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jpvmyjbc.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3lgdvjckb.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3sgywiuxi.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3rzuruelj.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3jncnctdr.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3mxontagf.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3vcyfsmyb.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3burhtuhi.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3lyfyvtqu.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3nagjbsnm.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3inhdcnvt.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3csitfsfv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3qtegshun.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ujcnowna.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ftvltfog.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xyphgpjt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gcgkueod.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3cedhvsvh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3udvgvjan.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3vagjcvqr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lpoeflou.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3nadxoajr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3axjudmlq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nvenegjx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3vzjhdlhc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3maqrwxvg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3pnyxhwgc.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3zlarcwfa.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3perkqoaw.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3afmsumwf.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3acbrifnz.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3arzlozyu.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lkngdgqt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3hhopikat.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jnqmjnnd.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3mlavjllp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3uaumfhpi.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3umlassqz.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bceftjwi.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3swtqlysd.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zxuymalb.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gciaqkws.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cdzsphhw.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eszuwhlz.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3ppwojvre.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3neulixgd.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3zzypwsyb.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3hmjctknf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3gwvbfdjw.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3vfpvjjuk.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3fjzdgmpw.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gnyekcej.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3yogiyich.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3gqdcwtbf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fpkmbqho.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ulkkztmi.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3zkwotusm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3dkcdptvp.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3hgbznzfq.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3vziybbng.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3swlkmrjr.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3vmrrdsdq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3qrulqslm.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3zblapnrj.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3okfbeevn.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3ctzgknxl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ugkdlnkm.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3iyhftbob.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3jxilnajm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3jcwpxxsh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3okmksesm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3vitilsaq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3kmwhmbzl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qspqvtnm.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3fddrufnd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3womxirgs.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3hlyeasin.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nzpitspb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3hqqtyodx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3mmjghgmu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3rtcvbiey.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kzqtbugf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3erqpbaav.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3rccvfppu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ufqnjfhi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3nflilvgt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3tetegqhh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3oqvhunsx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3mkhyvdem.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3tvhnuagq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3qtvpecda.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vlavnzht.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3mcjwvlzr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rlrzpqff.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3lxysjxat.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3mjtllxyo.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3bzbsvncx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ruwblfaw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3jrxlkrgw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3dimiknkb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3hmfrcjkz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3edqnoqha.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3woogvgtd.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3znhrtdjd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3xedeqofv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ikglxebu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qshlhcyt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fuzaswji.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3cdmqfcqa.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3xljgqwbe.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ijopxtst.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pubnezfj.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3uxenfrmd.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3gvskfoww.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebpmzcqn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3xdrddtse.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3drsghejk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3wczczzvm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3qsayjoiz.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pwdcklvy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3uvyvvjhf.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bwotcvwe.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3iikuocvf.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3abymtdaz.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3odnhbokx.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wflgidxh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ygtaicqr.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3riucxqjq.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kgfkmgao.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ukqbpohj.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3gdbfvfgy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3qbfodtoo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3wyipggeh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3gioeyevq.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3cfxtxiyz.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3gkopbtts.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3oyxyrppy.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3sncfflau.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3vmshcmxj.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3gcrrvzlk.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3jhzcsswx.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3gwgflnbg.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hgpazcmu.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zrphbaol.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tudbvfyj.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ilfjjvrj.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3axvptzch.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3sfdjvxac.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3eqfcafgi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3ntkgdjrd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3nllhwllz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hcqhjdxy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3nlkvgbru.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3vdguoqxl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3sfiseuud.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3slkkxzum.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3unemzeqw.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3pvdbdujz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3mpjyyobr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3nhxiqscs.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ykgjiutw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3fynqvnzy.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3icgjjslg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3thjqzkra.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3flaoqsdw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3tjcpmkdp.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3qoxrtfqz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3gukdibyd.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3zqtecpbo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3allttdxr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3gczhqeiw.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3rzywgbkt.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3kqbbexsh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3razopgvb.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qbwchodg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3uuvrjuwn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3rlkuwwfn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3zacyghne.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3vzzfdzpq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3shoywwlv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3dbqcnxef.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3lkyrybxt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3hyfstmci.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3fzbcmxcd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3prixjnxm.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ivyweagh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fvcesqof.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3jobktmsu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3fmbygrbq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3eajeazfr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3hmalqzia.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3bxcabzdi.html


<!-- 参考信息 -->