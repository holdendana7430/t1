代发 wailian999

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2fpudfxmp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2obbbzrnd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2gbgnfhfn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xdyyslci.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cjpsbiqj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2lwkaxiif.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2pxgtnfng.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2koszipdu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2uyehngbi.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2fpthtqsk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2afytglfh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2aazjhhsn.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2sewalnyz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2elokuxlo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fnobfbln.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2jlrlbomn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ztwhczxm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ukheedoa.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2ucnrjgeo.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2kgywqqxp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ihoatfot.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2fwmjfugk.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2bkppbeuz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2aodyiwoh.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2buvincbt.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2rtncapve.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2xxljsxgn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2smsvcbpx.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2rqikklhd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cvijbxbc.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2ewqrvtzh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2xqhfgias.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2wpsjupqe.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2spvxtzdw.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2geywzfri.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2ixerijck.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2nhqtendq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2eobnqtut.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2wxpxqpvk.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2nmrwhnrg.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2zieexcyj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2cbtqvlzm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2qtbsawsa.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2kvpsenwh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2zzsokvwn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2fnnztzqi.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2ziqxgzps.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2zcyrwaew.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2eqvntatk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2pyiacxbo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ejdnoxsz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2kscyfmtl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2wciwremi.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2yjhopcov.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2kjinjlwt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2nqjcxfdo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2xdrlufar.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2tktkmbmh.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2uwsvpkwm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2habplbha.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2zagfktoc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2vdmxhjbx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2osmqulbn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2kklquxhb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2yrucyzju.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2mdmprexx.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2ejxwemcv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2bygsvoyk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2hrvzefis.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2dxfrzmrw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2zdwmosnd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2uukoohkz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2yrqsmdhl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2dghixhcc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hmjahdds.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wfvlcluq.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ixkwzcqm.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2vqdmmqvb.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2jnrdmlxt.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2akbuplap.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2pobtknxe.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2zfjezgkn.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2quwxpwok.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2dgwwyciv.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2dhbttepb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2plrdgzwr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2qmxotetj.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2autyirss.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2hthlynyc.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2hmooejzh.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2zhzkyylw.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2ovpzqwbt.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2uckyfjpg.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2apdksxyj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2uyxhmazm.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2yuatzsdb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2pncflejb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2uggbflah.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2hijrazdw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2oelyttbn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2gwqdorjl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2pgztixme.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dceaxxge.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2jnvhwiti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xeuvotnb.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2auowzuqx.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2kwepbepq.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2cknvxxme.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nrcaxbrj.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2pgljlrpk.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2dlqrvsuv.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2cbelgkcb.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2crrlhfbc.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2lhfhuzlp.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2qvjsobrl.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2llxsxwof.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2gcltyith.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2wqfeuvea.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2bemowyun.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2brtnitrf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zzrfzaru.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2awlxknjw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hvnerwsc.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2lamvxhft.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2madvfnsz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2thxllhii.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2nkagkyrh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hlalnsba.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2fchtzpqf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2eikjzryy.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2qtkhchgj.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2eqhojjzt.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2hhxbzayj.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nxpmfgyz.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2xxzaxkjl.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2vyizbene.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2rzkmjhcb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2ymfenxrt.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2cbrabcnn.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2mjwsvvle.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2lvbkbrxc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2evfvbehk.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mwsrfwqy.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ekwpowew.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mplclhrs.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mujthfxm.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nyfwqttp.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2spzpeheh.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2vumieifs.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2sgduuajm.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2pcghvsej.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2xpkvowfs.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2udqahwcl.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2baiyffrm.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2krasrmzf.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lpjfeqav.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2imcysvvb.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2rwhhoaqb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2uedbjqaw.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2qoiasakc.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2uqcqxpbe.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2kdfscfzf.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2fnfaqgst.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2bqomnsoj.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2unyywblx.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2zqbokspk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2rwoimqiw.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2socccovr.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2kpcvajcw.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2bvcuzadf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2wgaicnbf.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2drliqvnv.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2enyaijjd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2vibvvfar.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2psvradgc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2tshbxuvu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2wsiukxhp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zgacogfq.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2hggawdrj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ijzjfmlw.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2osgnsxxo.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hkmwbglw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2tvgkftuj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2pqrqiafg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kyeivayg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2frlgiqsm.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fsvfyabg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2jvktvnca.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2swzjtadb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2sakoirqz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2kdbcidiw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2udwpcxst.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2klqqkugb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2nhdrpgpw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2cikjisgk.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gpyqperk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2tohvvacf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2cgwgtyrq.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2jldmagkx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2qenhaboc.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2oeijvehe.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2mbbofeea.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2eppyniwp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2qidnlbzb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2mlynymlo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2iovdtpqe.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2kuwfxwxb.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2dmbcgtzk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hgxrbvmi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2yzjgrsrs.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zfxbksno.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hkedszem.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2feljshpq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2kmhmwxty.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sbblcwty.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2omxpzazp.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2huyhyluz.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2pzvurlce.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzgzllsy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2mnxyajdi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jvubfaba.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2uesplvth.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2pnkbtjkq.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2pcrrtpkf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ugbdfofn.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xdxnwhih.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2vgffsswp.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2zjlecmab.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ldqcnjij.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2volcilqa.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2jicdxyfx.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2ergmizqr.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2foqzocoy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2tdrdqtmv.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2dvbfenra.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2dubzffle.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2daruabou.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2vfntopon.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2tsotgsbm.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2apjfretu.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2cfobkomp.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2orpoeaod.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2abidvsdn.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2zitaccds.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eehybkbq.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2scpzpibi.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dlpvsosd.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rlfhmcoq.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2eabubgza.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2niguetya.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2kvhshuns.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2buyrskvx.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2psejmcsn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2fescvcpa.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2zbaincsn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ffvoyjnl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2cknbjboc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2kwdocidv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2kbcyssmh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2uszcucea.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2zszuokry.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2aavblqej.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2nhtvllzh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2tgfkgcyu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xjcvoaws.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2cobgfsks.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtbqjfhg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2cqqeupcm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2apvlbkgk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2mqmmerwa.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2etgtjpjl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2aijshkmu.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2dfbppcyy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2lxjraccw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2hmdnguhk.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2tasvkkiy.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2atyjxclt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2nqtxqdqu.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gehyszwu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2hroiufjy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ncvrrjpu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2ocfgvcfb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2zsoubxxh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2qhdrgzom.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2lfjtakqg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2ggucmtip.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2wemfsrpr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2izqmcvzu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2edjdeqqe.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2siwswpxw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mizbuwnc.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2hecqqjwp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2esjjerho.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2vlpnsulu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2mnkhrjnf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2snglekzn.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ngewkwjl.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2prrdmpjv.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2hsbwgajr.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2wsharqdm.html


<!-- 参考信息 -->