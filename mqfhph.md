代发 wailian999

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2ekknmgff.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2equcqfsr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2laedzsbs.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ezgiyalq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2berligjt.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2iusylmou.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2bucnylur.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2nrucpjmv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2iftvhxpp.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2nzbayhut.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mlkvwtbj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2tasdzwai.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2upzpdsge.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zifzboun.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ztxnqpuo.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2ptydtgvh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2excdvwyr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qgjdklpd.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2bkngepqo.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2oxnctufu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bbqfiatl.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zmoiygwc.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2dcoylsnw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2azakteqt.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2excenfii.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2ppuhwywz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2raqizzcs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ftaadfkn.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2xzlvmmop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pmjlqahu.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2pmobadvh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2hpxedjah.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2eftilwcz.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2dxiqwxks.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ibmtrzjq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2sdtywips.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2einbwkiz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2dynbmkpr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2yyvleavp.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2fdyrfspr.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2pfzgqusn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2jtncdkyi.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2qwojjxhk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2tpvljawi.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2aevdreif.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2oooopzyw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2antvjciq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2wseivlbj.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2rjakxaql.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2mwgcaoyc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cptrljwu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2suenwmhv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ajqqvxug.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2nojacxfv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ruqlvzvg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2czgcirlz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2cmtigapi.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2noiufytp.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2pmipuwsn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2owssqlxv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2dchguhzw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2stgmzbgm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2ajmxgyul.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2nhyyvnrd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2btiivjeo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2efceyhls.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2elpjtnga.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2cvcpsnte.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2wwgozxpi.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2susuhsig.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ggwvcabp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2ejgtbnpj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2ylnvtlhz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2fxsiabfl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nlbcxkoq.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2crnlicps.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2apxlpjhf.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2avliffai.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ybxphvrz.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2bubrknfz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2puinkace.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2tadofoou.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2puixxsqk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2ckritvyy.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2cldfshmd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2ptpzwbua.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2kdeyxhsz.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2iogrmujd.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2hhadeglz.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2xktuplmg.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2lgxtqpuw.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2drnonxeu.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2zjkqdpag.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2qpdiqdfu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2gqdowotx.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2lpjledyk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2edawxeom.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2leqerzwp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2fpkydgaj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2nkyxzxnu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2hlrlejis.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2uezmrnrv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qhnbiood.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2qxvabwtu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kexwyjum.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2oiiibpub.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2mlnbetqo.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2skdoghyh.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cbaianyq.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hcxvaijn.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2mxzdcyys.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2rvxjsuwu.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2rndmympb.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2cdyocloj.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2syfxwrdg.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fpbismzs.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2kijrpsiw.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2unmyjcbi.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2jrcrxbtm.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xfpwrovx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wirytvqj.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2blafcgfq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kbsgkzho.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2iymupmua.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ucegjhcz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2cjanqggb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2kjcoridg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2wmeiamye.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2drfpnrcj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2hnvbozyf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2otzzymxg.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2tvrrkcro.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2sfmqokvy.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2zuamiumd.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2zagkerjg.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2bmniuthp.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2vsdqruvu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2nvmlyzze.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yszdmrly.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2fpwifjjl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ekkabain.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2aipnpgtw.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jcpsrszf.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2ojzdvdwp.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fdxycorx.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nrurymzw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2docnqwdq.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rlzxrjup.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2yjgyjiqu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2tzyohawj.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2dfurhhdf.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2cvobmbeq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2aleqfkjh.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ulzzdinm.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2iaxxoyun.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ivuqwehv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2oidbxmvg.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ubywwxjr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2gtdagajw.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2mbrmbsnp.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2gkoxdesr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2lunperea.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2fwxgyfmg.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2tidbsbuk.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2obyqntzd.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2sepzddcz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2roagyvhl.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2fpmngigt.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2vwiycvof.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2okwnqslf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2vvtyapvd.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2wtshpjdk.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2kcelenyn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2oxqcdcvz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2nviqcngc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2leqpgdnb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2ktmygemu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ovgreqio.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ivqgezjm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vaqtkuia.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2bjoocewe.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2aekvtdee.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2mtuqczpk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xqplomqc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2mmimbpdh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ynzrslvs.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kmybzopm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2fbriiirl.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pgbzjgch.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2xxwlmtvu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2uapbawlu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2yxbsfund.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2fvfordsx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2atstrtup.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2bgfybgnh.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xvatgxis.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2syvfxfje.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2sptjzkan.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2nfofcxzs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2pgrwqlss.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2vicoedgo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2dmxssejf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2kvxnbnbz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2egcnrzpx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2blktwtem.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2pbxtkhpt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2zmtfjtmf.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2jusyaggv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2xacoavwp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2qjyfoqay.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2syfskryk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2oqqmyvff.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2xfxlhpew.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2qnqptpdp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hgebzekd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2nknzxklp.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2aroimduc.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2aknpqbnp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2fcteogns.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2kilbgedb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2sjbiecfo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ilkqlqoc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2dtqyxdxt.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2plnbreku.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2kfzwwmvi.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rcbfntyw.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2asouqnlw.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ewtkrvpm.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2svzgjwlt.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2etbailtf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2zlygogzr.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2dvtnoazo.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2plekldil.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2txdthyow.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2cxjepwrj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2yztqmhtp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2zvqfjsjs.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2jwmunzgg.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2syniutut.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2skynkuav.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2ronrnvcd.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2zioupkpd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2bxclhxsj.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2wznpzlvr.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ghwwvhav.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2tsarfdgr.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2szglpbta.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2odemifpa.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2atjzslwi.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vqcfpmod.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2uoqjbfvx.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2clbelogn.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2wjcimhye.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2fnjdszyt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vvjfeivg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2sfuogrbm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2uvnjfjau.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2siflhfsr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2xsqzdojc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2eiyzawgu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2cmyjxulo.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2sywzizyh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2tfastvzo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2xpelxrdo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2losxgvrc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2vocvzymt.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2tfgcevqz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2dnlgaijy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2auzsrkqg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2xxujbvza.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gftukgrx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2etuhnand.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2xoszlbvl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2gosfqtdv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2eoizdbou.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qyijwnfj.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qjsazgtm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2uohpyikv.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2uawagfqf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2iloffkxw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2irwmaedu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2ozlpbsgz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2dzikaxoq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2uptntlcr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2abdqmtvi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2ozltmlrg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ylgohkma.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2nipekvty.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fdnbjbrw.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2ogjlkqap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hjcikcxt.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2jbufmxil.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2khnwnibo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2tidswtkc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2himkltxu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2aotvbffp.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2kwfapbyg.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2trkaxokx.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2ivexolfb.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2crnqwsfz.html


<!-- 参考信息 -->