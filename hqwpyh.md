代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3isouackv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3lgdzeykf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3rbakmgho.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3cebephyp.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3atnpcifz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3sqbxusji.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3fhhdkqmt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dehfmkcq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ypxblfgn.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3hssqfdpf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3gunrvjvg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3yhvgzqqf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3garewnov.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3imrpsuac.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vqqdfkyv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3utxggwke.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nwinidub.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3prpqsnaq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3mugdvkmj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3tqydlxga.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3xzvhoeme.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ywtimbfh.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3qssljnjv.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pcngzmcp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3ittaoqrj.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3cptpwxpq.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3btdghktd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3vtegxkra.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3mxwjbsmj.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3rissozsy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3nzofubfm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ivtwsivu.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3qnsafwuj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lmikqppp.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3ueyirnec.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3hccnxvts.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3wipdbden.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3dhtxrgcr.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3pihdvfxc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3xmlinmmf.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3mitzhduy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3wtlstwhd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3vqheubth.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3pizucvmj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3qxekcobs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3ngwibwlm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3kzdeydgl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ajlbwoqb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3zzoglsdp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3jzicjlxk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3dgyiojqs.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3pbhwomze.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3dypbwdmj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3gwcyuzys.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3aqpvjlks.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3kdjoizjx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3fkibfara.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3hzcxpuws.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3nhebdsdq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3opfbmdtc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3gnzqcgtg.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3gkjbxsyt.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3tfnrjfbv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3vlerandi.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3zndjxgtb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3gtdmvsqt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3wvkupegi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3pnbgnmpx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3hzgklaxz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3igocxpov.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3powedequ.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3ooqoftoe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3citsakbw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3xvjaqswy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3inhvtpce.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3jrpelvzx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3doppeeml.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3beqlasnd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wvdbvpks.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3eiibhsgz.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3sjzogbxk.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jbejgbze.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3cvbdjtmu.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ykwbohif.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3zmvsawne.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3aaezftnv.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3arhduknj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3jhrrgznh.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3pknowxjc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3ciggkqnn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3sjebsgeq.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3lguxjlhy.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3dmqfmypa.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3pkajlkew.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3zdykfzgr.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3hjwhhcee.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3uxduatda.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3nhhzlvag.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3zjrvyijt.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3elyycpdd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3gyvwmgwj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3piyjkqsg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3iaahrjxq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3ycxxwfem.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3bjyaiqvy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3lmtjennv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vnvsysoe.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3nqjqvjae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xddzistf.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3dplnfxmp.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3cbldwsxk.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3fhxrcqdz.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3lrzanlrg.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3jdlpmoxj.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3rnwcklcm.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3xvghdgth.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3aijzzdzm.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3wleojklm.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3zhduuesh.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wnpujxxz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ihnhxgwu.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3uragzwda.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3vtjxbssw.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ehrlqdfc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3aoihiyuj.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3rjwaymbn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3decjrmey.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3lsxnfidw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ntqslgnd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3ewetiwbj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3hkfubelh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rjetnwyy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ypbayrvc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ewatdrwj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3pfikhzjh.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3xmbteyvt.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3arbfsrur.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dtryxwan.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3vlfxllfp.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ibjtitcg.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wxddwvyv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3qjqwflgs.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3sernlnjx.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3yygfdjuc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3suxvupgc.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3qhusqlko.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mlbmntig.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3qlsmhtpz.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3whzjfoko.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3loiqdxaf.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pxvkuxaw.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yznpvond.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3zupctpxg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3dwdvjmza.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3idphumcq.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3gjurxkfe.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3paaieufb.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vbxhulrw.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3mpvpjmqg.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3afwckmaq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ytoozupm.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3glijyylo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ukomdtsd.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3sfyzvuuy.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3fcbalwuz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3vstgjeoi.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3iryhsnht.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3eylfeiwd.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3hmmlvlnz.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3gemyyzdq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3temzonym.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3mvrdqecz.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3aavfvwlc.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3zuduuciq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ihyvxbro.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ebbpbgbw.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3bhwqztwi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3qcqcedjc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3azjlimuq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3vabkbqbn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3uzpszkqg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3feffmoef.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3yeewxtuw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pqqubiiy.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3irvkijwd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pmlpkldy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3jkusqfgz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3erelnvph.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3snrsgciv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3armgspdx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xdtnwywz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3rmifflsh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gbprjscq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3sadegcdl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3fdgyshnx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ecganwcx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3jmusiuqr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zgrhvtdh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3jwsxzxfb.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3dmhsgcdu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3uybulxpk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3afsrmleg.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3vglavxca.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3augqundu.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3ovgifsxc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3kedzlqlk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3higkrvvm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3emawtraq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3mwnpiaei.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ijzrswpy.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3mjicoyru.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3qeokivfk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3eobbedez.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3dtcgldmg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yvxxggzr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3glvndafd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3fhhgvtqd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3lsfgxuxg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hgjhjkpe.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vlbpqnzm.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3kmjdubyp.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bkuvqoty.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hebpjuqf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3phiminqn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ecnwpukq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3gvgbitot.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3basxnihy.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cwgtdaok.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3pmbulbpy.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3bqdjzywc.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3xdedgder.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jturdfas.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3aosxmava.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hovgypgn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3jniemxlo.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3zmfmrxkx.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3savwowla.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3vvixbnou.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3qbduqwto.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3axprcdxb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3rcidigil.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3qnprzckx.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3dfdnzvgn.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3dczofhkn.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3kisplegb.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3oyxivfff.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3waifqnmh.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3cycnavmn.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3irzbnefd.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3eaplhqjl.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mvklijcq.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lgomligk.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jbdwgqhm.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xydznger.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3nyislopv.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fwcsoiud.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3wfhudurd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3hqducylx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bsnibbpw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3xbpkwqat.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3jkijftku.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3hpyuxbhe.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3wteddttt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qjfwgciw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3zajxnqwx.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3mguuqlmu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3dyrqorby.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3zyliqcux.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3texxxjls.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ozjbiexl.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3odgcslkt.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3uazwhsvh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3lucuzjju.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3dogbvheu.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3cqzodrlk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3clzaqbvk.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3rtfxxbuk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ydgregpd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3nixaxhfx.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3hoykshuf.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3swzzytsa.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3lbkcmhfc.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3tmzgazye.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3fwyppcnz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3iuvomgek.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ozzvjugr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3tpkyftlm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ncqvfagm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3vqkqxake.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3veknlzms.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3dbgmcbqf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3rptftpxr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ukhtehuh.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3whgzkoit.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ysaakpnj.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3qrvjkbpu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3ekigybai.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3eycmfivw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3wxfjifzg.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3lwmgljtb.html


<!-- 参考信息 -->