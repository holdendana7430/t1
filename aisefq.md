代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3htbrpgvh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3lmunmzra.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3icxizmmx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3jkvfcnsz.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3gzwtqxbs.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3aqxosftd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3kusbagkh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pztxdqfw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3mbjurbxx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3wqaqdfea.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ofitkwkv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3fuokxxmn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3qeyjsmhj.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3lgcutmzt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ytlkzslf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3ewkydksu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3dzoujzfa.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hflcuoha.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ryewwcod.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3aoowcotn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3yobvcbkz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zstzrnaj.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3oldvmqkt.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3yhtouxzo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hnhyaevm.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3hgzkbiuy.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3utagnvpl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3wnrvfjkw.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3uwjzpijj.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3nfxiovfw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3bzjprbbi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pxufjlem.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3dwalyxzb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vyebmzrs.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3utgfdapr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3pyvtumun.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3ezbpdddm.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3znheonug.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3cprwhtjg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3qxyomvco.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3nxapznxd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3pgnqbjvy.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3xrdcvuzr.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3pncepgtu.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3nfvoxlat.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3oysjsodw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3wjcsvkxo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3oljubkop.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3gzcrtsmx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3gduvasvq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3cfnghmim.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3piejqwhj.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3udjrykuk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3lmapaigj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fxypwmrh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3nfwsxotd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3jgniojzx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3ffyounil.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3zlonrjsj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3uebuwmvy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3osyecdqw.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3fyidumvb.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3ydcpqhuw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3xbanmxii.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3hmdgudul.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3voofhnft.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3bfqlahij.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3bmvywejn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3mdxrtedf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3lsuigydp.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3dajjkdyp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3itvgktbs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3bfhmsrmb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3grchtjrt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3klggcifg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3ifenytxk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3izpnwccm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3erwjxthd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wuhtpkrw.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3vtnhzerl.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3krisuzcy.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3scbbvkha.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3senntfyk.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ieajugzy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3kfvnlonj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3cqvgjubs.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3vixpzxxi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3flyggxmn.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3fkkanoft.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3ibhjnedo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3doxjygcv.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ppsrmacz.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3enjdsjfe.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3wxudrhit.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3gmwdtzac.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3zhijgnnj.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3jefyyqxd.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3piutluww.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3evzgjzhj.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3zbftykjk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3udfeyjfx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3aiuwhqpq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3fiejrzyg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3rlpoxchu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3hzzxtmmy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bhoqryis.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nfdzfvzi.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3jlkpftua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rjlbravt.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3nppomvmn.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3yvupxyap.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3nfjiqska.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gbvaimmw.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3jjonfdhz.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3epmgtmqv.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3vovvhubg.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3nffplpcc.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3zzxsllvi.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3cnxghcvf.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cwrbjfpd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3lamtmugs.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3kbwgksxl.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3yovarmfe.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zxrjhhca.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zxlfuosm.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3dcnzwlxn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vhekfczu.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3ooqxcvij.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3tetaramk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3chjahkzt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3yfkjlyej.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3gezdetof.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3grhyudas.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3fvcichyw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3cqulmohs.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3iwpnrksq.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3uqfdzbak.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mlxobhhx.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3fkvkuwsw.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3qcpnrakz.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ugfzcttu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3jgaowjob.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ubehjfis.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3rgljaeux.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3tkdqjltb.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3kdtgxlec.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tjofwino.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3igjrdcyy.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tdgmrdgc.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fvqxgiva.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kblfiuxn.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3drmahmam.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3rhrvdxbb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3hbuldhsg.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3feajrlju.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3erzulkma.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ectsecak.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wwcwagsd.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3tknaxdfw.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3pxznntvh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ensejdix.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3otnzxvwu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qcciglck.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3uldoifug.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3cdhuayxf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3ujdsruzm.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3tdbrvbvt.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3zklhqlqd.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3fvbolgbr.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3kxqwlybu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3ugbxeudi.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3vbbbkxau.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3rwzcrjmo.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3nscnprby.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3dnillcdn.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3zsiwbopz.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3vcbnkeja.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3tknrptla.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3sijhjhfc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3ossbkeqt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3vyqapmlf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tgnhicoi.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3zaqfhqzt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3crojkdbd.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3fzioobgd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dmkjwooy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3cxutkzrs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3yjauxebr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3pojzvnpg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3oiojtyia.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3usugfivs.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3rrrrybpi.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3oqtjdyld.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3thrgdezj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3xsmvktqd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3udilewqm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3sgrefgcr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3lxxwtpxa.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3zvshjxjq.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wfaybush.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3zjztabkk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3gephpstk.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3nkrmdodd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3chmnwtex.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3fdfycfii.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3zolywgey.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3jsmaxeih.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qtzrntfm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3exoxrmps.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3ibxyjmwp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ycydptwp.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3rtstrwyu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rwaibfyt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ysmmxxzu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3hvspaxuu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kguglrfp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3wysmivek.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3nagpzftt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3odkxvlef.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vroprgbz.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3blqvllfb.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3hbotkkjg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3igqxvrfw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3iairtpgp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3yunvedbx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3ajpwxxiw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3vwwbwwfs.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3lawhcdjn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3oilxrthc.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3lxxzwnqj.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3wptrvyxn.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xzoirpad.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3tsyoqjcy.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kqoapqsg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3sezdelja.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3xvlxklfd.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3dbzsicem.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3usoyeexr.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3jkrfmhxa.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ppbhfdoq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3huqqxrzv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ykipvmyf.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3velfveoq.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ndvftrsi.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3zbaqkrse.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3kmbwidvn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3wkfuaglm.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3lslmfviz.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3miuvwidb.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3tmxanmhh.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ebcytnvg.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nwxexwir.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3psicgere.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vwovmycf.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3gfndybhv.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qkhvckdr.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3rwihpddz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3fvyubgid.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3oojuujhp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ciiahhyq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3rpeiohmw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3bbsulmpa.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3mmzhkkej.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3vgrpvwzm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3kauogkkc.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3fieiixvb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3qtxftiog.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwbmndol.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3jwhdujld.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3rkkrmwpb.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3rpsqwcjr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3mxwxehuh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3zyocozsk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3pkszlbrp.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3zwtbbpcd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3zbeyloiu.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3dptnpfvm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3indcvnjj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3lwbnevgc.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3gahtbiei.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3cosvzxlh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3gpvpfreu.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qtjgbfkw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3zyafzrmh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3qwdgvacw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3ytvtycxz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3menrotsg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3etkrffsv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3xocotisn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3yugqmjrd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3jxbjnzlz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3mjnwwtpl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eljpucee.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3bfsqbwxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qcvyvwta.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3wfowxjab.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3pkzlgusu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3spotgwjx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3bqicczhx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3fgwpylrc.html


<!-- 参考信息 -->