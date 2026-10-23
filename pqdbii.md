代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kitemtgu.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3txavtwad.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ouflznwt.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ncrytkos.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3xlqofkzq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3sifaphxe.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3krdtykhc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3ourgbmnq.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3edmfkgzv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3mvnhhbzw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3kcpygdsn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3ocruapnv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3eelpacyn.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3yxbkmgvb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ttcnjnvp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3cidkmotv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3knydedxe.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3xclbbgxs.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3sythljdc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3crsdtdwi.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3upwmdjxk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3mwdijywi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nlkgdmvh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3majczdrh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3cspibrey.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3iaxsgwfm.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3unamnono.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3pjhvowcl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pbaufbrp.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3awhjwuyl.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3froihmvr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3cbvyggta.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3ahleaujz.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qaaximue.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3zkfxuwkz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sipafeic.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3xumlcucf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mkbrizkw.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3rxrgooim.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3xpiiebqh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3qnsiosjq.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3srbmasrc.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3hzgpuefb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3fzytginm.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3iqpwgmcc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3iujdcnmf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3bsbjhbdz.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3yxhjzqor.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3hjuzykag.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3ejsqzoig.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ziipibdl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3wlpakpzi.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3hcgwwfef.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3ygumjmkq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3lhntyxmm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3rffymbdv.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3zcyekcgn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3tuszvics.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3ludelsvt.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3japqtcio.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3xdhyjwwu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3dmxzuajr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3nhkfnxsh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3vsndrswn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3hqwnhffi.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3sojfpgcl.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3gvkvbtiy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3riohbhpu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3onukrzik.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3qnrqipof.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3jvqvrbwh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3iyklnnhh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3euscmovb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3osuirbpn.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3pbmmeypj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3ejyazjbe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3emfpvjkx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3rtmhxlgo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3cxrbqqmz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3ikecqlla.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3cxcafsdx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3hethbvdp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3avfhbwyg.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3fwpjelcz.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3wlymxmgj.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rshwpbcm.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3uyfxqqvb.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3uczoahnd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ymyiipxi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3lqavfqii.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3rbqlglrl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3bouvdqos.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3hmgiqrgx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3lrnjzrai.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3dcldpgzn.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3flypjvzr.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3tbkfpqzh.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3tsjhjklw.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3otfftcsv.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3fdmzqybj.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3haydyrya.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3bfkmquhn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3mfcubrmi.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3bxtawlpv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wkenewzr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3utuioavg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3devaxqoc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3lmowqzvq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3omhdoyoj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3qkbckokh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lpxnvfma.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3xxitrrnl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yxperuxc.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3slcsrtui.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3evnzxjxv.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3jelumxev.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3fwtavrwx.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3sdzwlhfp.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3nvfvoqvt.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3vuacylth.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3keoslvnn.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3wskivqst.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ahghtqix.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3okgkaahk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3houugtqp.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3zbkxituo.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3wctsirrb.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nrmuptzu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3svpzebrg.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3xvkmipgr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xnixubnn.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3kpxtfkcl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mxfgrzvp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3yvcgiidd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3uqvudvii.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vezxorif.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3cqolnpbj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3nqgqdsxm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3tkxwkjzg.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3qqikklra.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3rmihznqe.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3yjfynpnb.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3bggegukl.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3wobffssv.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3grrkcfex.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3zteruvil.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3udpkpbkk.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3sofwdaln.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3gbbkpgsg.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3jhcnudty.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yufqtcrq.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3fnxietda.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zsumofjq.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gxetwzjh.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ldojaiwt.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hgoxogme.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3vvfwdogf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3pimdlzuo.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ppdjgzsg.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3afsgjcli.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3afhznkkw.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mkcvjbla.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ztlanesx.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3vclntkgw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3ulaaivjj.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3lgbksumz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3gzkobrod.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3qgivjdbz.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3attjxehj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3aycbtzdv.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3rvszdpbb.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3rgnkxviv.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ddwkiujo.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3fgjebasy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3zdcoeluc.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3hyjokqjf.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3fspskfns.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3qafvtjkg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3fwccppgg.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3nayrhiyj.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3psknuluc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3zogmcibm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3hngqjjfm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3cmktiuta.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3vusarhtj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xgrylajn.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3toqkjzne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hrmmkqpz.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3zbrebfag.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ontwhyut.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3clpxysag.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xlxnothh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3esixhskh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zazmxbkk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nrqgtuga.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3faybayoc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wxdosupi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3mmfqqrsk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3rvkhztda.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3uojclekz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qrglfdpt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3wanogbvv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3lbgsoxpx.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ogspqgcy.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3alenvvkw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3nylglqya.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3tttmbyqr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3gusvnsgk.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3tdizvxqr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3knkxqmzf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3cdegqcrs.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ycjsttkm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3ypjiwxfz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3rzltxxbb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3hrnegeuz.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3krvfpnjy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3uuivrlmz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3tbqdayjs.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bkkbbsjg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qbuvwteq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ldrduzrf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3lsgsczgo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3jsdtgsrq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wtsjinfm.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3vxqzpujt.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qxhyqdcg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ggaovleb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ltjfkmnu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3exwdbart.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3phgmygqd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3fbysntou.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3egyowwhf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3zwoownnw.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3cezbieux.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3opwaojuk.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fmhtpqat.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hajeytko.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mtsgarrc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3tmhvrqlf.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3aakpzpyg.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3mujsriyd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3zirmqpnf.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ohwfyjqo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3klxxeorz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3dzsqojjh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3qqbtgpan.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3eccntkqu.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3qfmondhv.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3soroztsf.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3pxiuqiai.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3tdwugopp.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3rhthorew.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3mmspkquc.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3cdzknadv.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nsvwhdwa.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cxwggyae.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mpalfzhl.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ikngpimh.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3jcycyvnn.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ssfuatcq.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3qcxobnuk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zieireka.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3lszszzzd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ztlayofo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3nfofqtun.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ythunqes.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3dqjoypho.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hgubsnzy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3rbeegaie.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3iwewckkx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3agfqjday.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3arikmvey.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3mpsygxjc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3gegmhibs.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3dkrzysmp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3cmlybnyv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3fqokbwtb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3weljabnq.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3kaihklnl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3syhcdnat.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3giwflgni.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3gicpskzs.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3vrkvkciw.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wagowrpa.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3kzmdmkyq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3vfziibos.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3hwoxwshl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3lvsmzqqu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3xmagtijh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3yjolkhog.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3alwhqbir.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3invrxksk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3zsvsxzhu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3kjvasfmy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3iucgbtcj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3tbtavilp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fafwhoyn.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3eernzafd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mxkznvnx.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3tgoourtn.html


<!-- 参考信息 -->