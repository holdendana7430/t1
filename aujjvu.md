代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2igurxosx.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2ksknznov.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2wluzwkdd.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gvvmtkmn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2sprsrgwv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2fprqivbz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2vqxpfeec.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2wvqdjdrr.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2rxweuulq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2tlgkzxnz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2muqxuqel.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2hnhfayuy.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mwpirmmm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2bxknxpxo.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2fvauqdqf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2oknpmhis.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2bfmxuyib.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2jjgsasyb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2tylpnzfg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2mhwsfaob.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2oneysvux.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qnsmkhvn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hcydgknj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2vnwygbug.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2ykewxpfr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2uqkfghkr.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2nqjygtup.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wbjwugwh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lrcbussu.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2onnfpjet.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2bhaymfsw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2qxklzjbs.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2rkoirbac.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2saxgwcth.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2sbktiyfb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gisjdgwl.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2gpdlffgl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vfkdyeme.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2qsutuguo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2esropmjl.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2ecldtzdz.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2dpiieeym.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2rhmgwfkv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2iqhtgigj.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2dszbbxue.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2chjurrca.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2emhzjswk.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2kqgkzypa.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2kvbchazg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2lguaqdht.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ozgiebgi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2taznacqp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ejuvsxgj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2mlovokdg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2uxcckemz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2ukaiyfrn.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2pnizyxfy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2zzlzmqkj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gceszmmd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2kugtpzfs.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ndbsbxrt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2pxnlazwu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2xhirfnwg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2evjskexl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2rlgeibdi.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2rteymjhl.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2aorgigtb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2kczpclvw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2fcabeywx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2dpnegrid.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2rvoyxion.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2xhykhwtj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2kzsvrbsf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2tmzuzlnb.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2wlasmnwt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2njhebxsh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2rcokpvol.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2uviwpiyc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ndxfrtxz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2irjrqqki.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2xqtjpxhh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2qgqjoube.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2feemdsrm.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ssdujzgg.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2shzojavc.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2qcpuyzyz.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2cfjonwxr.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2crhfaoww.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2oscuglnp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2kkhvewfu.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2fjsvaogh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2mqvekpxg.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ewtvwxgo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2sibxpunb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2exzwhzya.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2yuiofebc.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ipitjlqx.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2rnkopewk.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2qbugchod.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2zkqxucvt.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2hquipmzb.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2jxlfrlwk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2qbiebgcx.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2teadpkms.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qakjzlij.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fafyttmy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2ubqqbrld.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2cbqwqvej.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2pfhjbxdo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2nfikvtjo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2narklffc.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2xamhklch.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wwvzgqvp.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2hduixflf.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zvosgcqw.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2tadcujkh.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wajxuzcd.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fzjafkeq.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2fgqkwosu.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ryghlikz.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2wkeenfmf.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2edtljdhv.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2fugafwtk.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zpdenoxv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2alekznij.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2vqoloiev.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2cptrlewi.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qwqsfrnl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ebvvkdfh.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2hemtbbuo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vxinzrgh.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2svslmgci.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2qhxfcase.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2ipziypax.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2uossdiyn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2rzzkewos.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2biemadur.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2wmppjkja.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2pcjcmrbu.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2kddtgnxq.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2umnmkypt.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2epnhyklj.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2vhhhgamn.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2rkllkckj.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ymyyxcqv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2aujcunlj.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2tnxyhthz.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2labbkgrj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2dfrgwvru.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ggqtbkcc.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2iwkqxlff.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2kwhagkbm.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zyzcsqzq.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hbjtjmaw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nqydofrn.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vhsojgcr.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2zbbrmhnt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2fcjkedvn.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2jpobaqid.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2mkfcvoau.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2dfccsmfv.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2paaceaas.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2cldrtjns.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qvkdsqop.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2oiuvzzbw.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2ygczllwc.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gvwykuzi.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2bbquxcvd.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2glnsogid.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2exfhrpxy.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2fgelzxiz.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2zyoyprxo.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2jmhxjmvv.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2aksmpqxm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2ysrnhmcu.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2lofqjubs.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2annsneug.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2rqsqnjau.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2eybjsbzc.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2wcqbhttu.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ieleltle.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2aaxkkldq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2mnmkdtlc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2dherxsnq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2fmbmcmuo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pozwoaex.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2mehtduve.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oqnngfqq.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2heelfrho.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2coiodkwq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2eclyqhul.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2imciktjm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wztckwsz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2icbvugrh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zlevinkl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2ccbmevks.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vzycqsro.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2quudxwfy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2bpusqeuv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2cekmwnwc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xqsuvysn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2hhzafzco.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2qffiujcn.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2xhcwkfey.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qqjusbib.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2juvwpoby.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2hcorezhs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2pqbrgxqi.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2glrbjewe.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2zmtqvskz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2xmarpyxx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2blqksuog.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2bifgyrox.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2qtcorxkt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2nyuuhswy.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2bkxmmvbe.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zjsvmuoo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2sqvoljfn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2bzlaksmx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2phevodgt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2hvjsdnts.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2unzmkffq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2zvqxviqc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tpwwgrch.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2puwuidst.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rgtbzdyo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wpednure.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2fsdizsar.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdcidxcq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2atvrgmpj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2ndflmuuy.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2rnuumqjj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2eyianayt.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2delyflmx.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2nnvrxfnk.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2awniehll.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jimwuume.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2odqpcyea.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ghrwoudm.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2qlxzfdmh.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2rxhiqken.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2hpqifnlr.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2rxwroqka.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2ierqbdmz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2murtynim.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2znngnnok.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2rqlftxza.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2dkjggxwk.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2isvvrsbt.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2zvluvbvt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2fysrjsjd.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2xkceakmi.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tkpchypb.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2oimjeoeq.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pkiomytk.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2urrugjqr.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xtwbadlj.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ijjsfkss.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2ikullirp.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kjayvndt.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ioxtygva.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2goijyrqi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2aptczkvo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2qlhuhsvk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2zdpspyvx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2bkhwtfgt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2merlxnab.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2sindbpdy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2loanuixj.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2dbsyrnor.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2vbtoodjq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2zepxmqrg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bibpslnc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2htvndhvd.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2nwekkqyk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2cmojivpm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2cjqwdpnd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2uwjwvfbu.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2lbxiktie.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2yehzgbsc.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2vajaazmf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2pbyzeuao.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2gcdmzqln.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zzejsxvz.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2waxindzn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2inlnxute.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2wyfgtsay.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2heiagtaw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2lenchubr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2jnrcojpn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2evsaxnah.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ffijixze.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2gosgypfh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2qkmnvpec.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2zpbpwoow.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2hgyockli.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rizdmoyn.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2vffltjxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ienssmqm.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2wlvsyene.html


<!-- 参考信息 -->