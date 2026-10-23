代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3htnsgxtv.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3wmoxudxu.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3llvjkhex.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ykvtpiso.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3tbiycbax.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3hgqumvyj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3kvgqkcrq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3owpimazo.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3cykymfln.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ejjmselk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3cpkeegdq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3yuqidjgq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cgwhrzyl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3wsfcesqi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3rbnqwfuf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3vrfnqclm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3vwrppuiy.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3hvrxheef.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fhzorvrf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3mbfpkzad.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3uufyuykh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pmdfgjgo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3gdjqlxww.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3kukzfgaj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3nweowfct.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3aqmhvkty.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3ycxhilwd.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bejcraqf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3xxubofay.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3cuktowxy.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3eadnycuv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3oxwgloxq.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3fnjtzvyg.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3nelnavyc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3gohlbxtj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gkklesjo.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3yihcjbtk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jqasqybn.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3gaxlkqzw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3vzheovqe.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3raqwczua.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ktscjato.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3bggzlvnh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3pkgianvf.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3vhljybbs.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3ogdleuqu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3itepmexy.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3poamaecg.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ezadlarb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3suicmqqn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3lykhxxlm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3nvwysceg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3ghrnknpi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3cuovqocr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3auzkkshf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3bgcjrtfa.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3dyqhcduf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3tacwetng.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3xgenyqjb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ljukeuxt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3mvoxzabr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3afraffmt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3pcoezipx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3ytjwyksg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3uuddclhq.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3mylzhfgj.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3jxaamgfy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3bnzyoukl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3irsgeclc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3jrhtkjav.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3jerdpgkz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3tsqkkzfy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3lazhtxuv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3dhfkpwii.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3xuslxdpu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3kklrkhxw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3hkifqtmh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3jbqvwemm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3bvshpycq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3zthgtkuh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3osjglyhp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3jstwqibz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vqiuzwfd.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3nlnfpnhb.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3rtmryyxd.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ndbngdpt.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3imxpicxy.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3onrpedyr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3knqihoxb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3onizguey.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3szhgneou.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3zvtsdyiy.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3rlipamxp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3mebdglew.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3lcebccnj.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3vodhyavi.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3fxqudcgs.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3cphwpxwy.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3fqlucqcc.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3ackpxunl.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3xgkjzplb.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3ygkjqdbd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3fifewamh.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3vdhmoodj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3zjavcvpz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3otjysgux.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3wpregwfg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3xrhufrcb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3lnxnnrzh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nfbilxar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zjclopnz.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3yjwtcfeo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3utjqziwa.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3qoqxthks.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3vjrjvgzf.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ltwfhoju.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kuotvtvn.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ednaznsb.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3budezuit.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jibcaaqa.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3gjzxnanl.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3yzjtuexp.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3olmxerkd.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qkyurrmi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3kqtwmwck.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3kbvjttim.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3tndxdkhx.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vbnegknv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3momfytkj.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3conlidnh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mtxdpbfm.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3tefkekjx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zetkwmoe.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3jcskxzqg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3xojgwnjc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ztmlakga.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3ibryeqss.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3cbynlqrc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3xskzvufr.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3acxlsjme.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3pejdukvn.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dqzsdzqs.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3hthnicrl.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lyphgmnz.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dwhkkjtx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3mkxrqyth.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jjrdjbbq.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3grbdkiwk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3vptpyipq.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3mksznlbi.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3evyrkvtm.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3lrepthdy.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tafsuqyr.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3idcsbdxo.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sjwattzj.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ssqmlwmw.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3icemhwtn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3kvbpghnn.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3ndfxrste.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3zrklpags.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3urhxuwza.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qtpfnrof.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3wiabvbtz.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3lgkmuukb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3hzlejxgt.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3emjlfifx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3viqtivxc.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3xlnsjeoc.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3biqkkotu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3ageugbqr.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3oaizqnti.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3elmrufgs.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ihfrxdnf.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3jmjvybff.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3jlbwgbhn.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3vhacgydf.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3bqytnibl.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3fkoqweyd.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3liestegb.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3xndwnlag.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3cfelpjbe.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3gtycorba.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3lpporyxc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3ekunfddd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3pudfplty.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bfzzzwfq.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3zuomibch.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zpkogyic.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3ablfhjjj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ykybkbfp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3eznorsgg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3mxmskalb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vkyioyxo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gtxemdor.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3onbqpyul.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3qtlyeyht.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ycqnntdo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3oymehsbb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3gvggmysx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3zjcbtlkv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3jjdoneax.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3kobzjcfp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3jwgebttn.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3prjopzqi.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3wlpzhiwt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3jruzxrbw.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3dsoqvykr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3hpogzcxf.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3czmgewsc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3agwwhgdp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3zkxsgydn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bepwfgcn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3gysjkzvq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3nafeyjrf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3frgmwosi.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3emktannd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xpxgnvtq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3lpjfjcxj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qqqtrhey.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3yuxuyyjq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3mjklvtsn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3qkqkputd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3liyzzooc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3kzvqsuqe.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3echsgmqo.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3myhulgyx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3drfnixbi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3bimhgwer.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3vnrqcjfq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3worsqrqc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3wcegsphy.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3sbwastzk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3sqkvswxg.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wphvvucm.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3cltnfsoh.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3jplbmivq.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nvhrrmfm.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xdkfzher.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3qnsoaepk.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3mhbeylok.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ozdaksil.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3uabgqsfh.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3rvbupatf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3xtlmpkbo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3vhmbfdlb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3jnwaopts.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3zyydpuhc.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3rntmncdz.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3kaclljec.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3kvfqdxpn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3oymgwaqw.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3jtzmmvrs.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3pnbvrapm.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3gyebeths.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ltqwxozf.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pwjnalwz.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3usptpnuh.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fohekoyp.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3jouwwaok.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3brjefexl.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ndagwrrd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3vlxuqmfc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ojtigbta.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zbbzjmza.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3fzevzjmn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3gzhbtfjc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3tysqttke.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3edfzyzfc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3ggbwecup.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3ycnglhbi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3ruqnnnku.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3wenljmzd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3aypjwfpo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3mbizmvit.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3negkmtot.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3jscowfce.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3cbcgohqo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3dghselfv.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zvnfahti.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3buewpbhv.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3piskrkms.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3vcxlwhoc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ycehdfnd.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jiyjepvd.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3oxrawagd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3bhkumdlq.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3kswfieep.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3wbmgsnhp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3uilqjyhk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3vmxspaxq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3fwrskigd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3lbzsdamk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3fhfxvltz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3qilzlgoy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3wiwfybgd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3vcctsndh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mbxoyrvy.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3yirzzdsz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lkvuaago.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3hbdpnvlk.html


<!-- 参考信息 -->