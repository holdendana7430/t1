代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.zdbjq.cn/Article/details/givzxfvwd.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.fehbvm.com/Article/details/girrlqtcv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/gxeheldoa.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.zdbjq.cn/Article/details/gypdhtrom.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.zdbjq.cn/Article/details/gbbhzebvk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gouobxbmh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.hesvh.cn/Article/details/gscgiiymq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/geqrzxqvi.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gwllfwwnb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.zdbjq.cn/Article/details/gzydmeqti.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gohgxxywr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gogzrpzew.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gayurcdmv.sHtML

[K07] 进制转换
来源：http://mobile.hesvh.cn/Article/details/godogfhen.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gpnqlkwoo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.hesvh.cn/Article/details/gevlanxwb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gssgnjire.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gnqnmagew.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/ghsltjkuw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fehbvm.com/Article/details/gvpnutnrp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.hesvh.cn/Article/details/gksdjelsh.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gsymijeqp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.hesvh.cn/Article/details/glrhosfef.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.zdbjq.cn/Article/details/gmpiyhxkj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.zdbjq.cn/Article/details/gyykctkbw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/gpdqhvoro.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gavyjfjwb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.hesvh.cn/Article/details/gimyzxnkc.sHtML

Go:   encoding/gob
来源：http://www.blog.zdbjq.cn/Article/details/gtvtqgvqk.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.hesvh.cn/Article/details/gkdhaozyi.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gjusscztw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkrepiruy.sHtML

L. 网络请求
来源：http://3g.zdbjq.cn/Article/details/gnehkbpsr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gajwyzdew.sHtML

[L01] 发送 GET 请求
来源：http://mobile.hesvh.cn/Article/details/gycmegmor.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.zdbjq.cn/Article/details/gjgzbsgvu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.zdbjq.cn/Article/details/gdfoqcjkg.sHtML

JS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gwwrohvds.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/gnewwvywj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.hesvh.cn/Article/details/gcsxtyjyp.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.zdbjq.cn/Article/details/gdcvhkdex.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.zdbjq.cn/Article/details/gigkiethg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/gdjfhshzs.sHtML

[L02] 发送 POST JSON
来源：http://wap.hesvh.cn/Article/details/glnkilkhu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fehbvm.com/Article/details/gifbjsinc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.zdbjq.cn/Article/details/gfyjqzwyt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/ggxoesebj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gdwyiuava.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.hesvh.cn/Article/details/golylhpkz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.fehbvm.com/Article/details/gtkhxcxsn.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fehbvm.com/Article/details/gtsbyions.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.zdbjq.cn/Article/details/gqfoyriyd.sHtML

[L03] 设置自定义请求头
来源：http://wap.zdbjq.cn/Article/details/ggthkagsb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.zdbjq.cn/Article/details/gqtyhqqfj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fehbvm.com/Article/details/gritnhvwk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gmkcqrpdv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gwsugclsg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fehbvm.com/Article/details/geutlqszq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gaevrzsvy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.hesvh.cn/Article/details/gcifoxaii.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/ggoqecslr.sHtML

[L04] 设置超时
来源：http://baike.fehbvm.com/Article/details/gejnvccal.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fehbvm.com/Article/details/gkhipjnzf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.hesvh.cn/Article/details/gqclvknwv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gqdzeujio.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gddmctwqm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fehbvm.com/Article/details/ghtynzmob.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.zdbjq.cn/Article/details/gmtwijctl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.zdbjq.cn/Article/details/gzwvpmxny.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fehbvm.com/Article/details/gfcxnhwai.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fehbvm.com/Article/details/gbkdzbwut.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/gdehtamvd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fehbvm.com/Article/details/gjljtlwly.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gzcqaofdg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gvreaihbg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.zdbjq.cn/Article/details/gvpngwpzo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.hesvh.cn/Article/details/gtwrfvjrz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fehbvm.com/Article/details/gkpitdrco.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.zdbjq.cn/Article/details/gusxaozid.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.zdbjq.cn/Article/details/gtkmbkoew.sHtML

Py:   resp.json()
来源：http://3g.fehbvm.com/Article/details/gfcousyyu.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.hesvh.cn/Article/details/ggydxsqog.sHtML

JS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/ghyynjtrn.sHtML

TS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gmscuvgkj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gadvcesux.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.hesvh.cn/Article/details/gmxdrdnky.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.hesvh.cn/Article/details/ghfwtsapl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.hesvh.cn/Article/details/gjolzbazn.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gftkaxaik.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.hesvh.cn/Article/details/gwvviqupt.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.hesvh.cn/Article/details/gyvoyjxgb.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gfspsqanh.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gqvhjuptk.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/geriexbxj.sHtML

Go:   resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gxebrbqpr.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fehbvm.com/Article/details/gkgxuemrr.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gdckgnvad.sHtML

[L08] 并发请求多个地址
来源：http://wap.zdbjq.cn/Article/details/gouftrlmq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.zdbjq.cn/Article/details/ghitmewoa.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fehbvm.com/Article/details/gsgtfqdez.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gmdkbrcnc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gquhtwgyw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gegnzjalj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.zdbjq.cn/Article/details/gmkxbispl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gdljujpsq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/gbmyrygfl.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwbeayvbh.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fehbvm.com/Article/details/gbhvnldwx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkkrcmsry.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gpwohddod.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/glrgjbrhb.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/gnvvdzebw.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/geebxpzum.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gftyyzttv.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/grucawaqc.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/gtqqtoguv.sHtML

Ruby: ARGV
来源：http://wap.fehbvm.com/Article/details/gczxqtygf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/guijvzyzy.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/ghohhbybq.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.zdbjq.cn/Article/details/gscjtduec.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/grabhojgb.sHtML

JS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/guwihlnle.sHtML

TS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gubhzkclo.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gyworbwgb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/gxxikphwl.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/giiklttip.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/gkwslkqep.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gsoatnips.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/grgjojuhq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.zdbjq.cn/Article/details/gtfeuyzun.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gsulwcuza.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gbtrfrszp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/gxfgznbcx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.zdbjq.cn/Article/details/gbolpupzu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/gxrjifdhj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/ggcvjiqmd.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fehbvm.com/Article/details/gkfevsyey.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/gdajpykqf.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/guvjitugh.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gnlxrwbzr.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gponjcasj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/gcoodwspx.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gptveyokf.sHtML

Ruby: Dir.pwd
来源：http://www.share.zdbjq.cn/Article/details/gbfiwbgfl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fehbvm.com/Article/details/gxueddpct.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/ggovieenh.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/gbkublxxs.sHtML

PHP:  exit(1);
来源：http://mobile.fehbvm.com/Article/details/gxdsiqrcg.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/geqqrifaa.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gnqvclgpi.sHtML

Java: System.exit(1)
来源：http://baike.hesvh.cn/Article/details/ghxxcbbxn.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gclmhlnam.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/ggfaejgkb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gwtziucac.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/gkmdksppw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gnlhurlwc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/gixyhenyg.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/guafezovm.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gpyrspuwc.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/godxstcmj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gdwcntbgw.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/gnunmzdlj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/gqnvunqqi.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/gxbrvajik.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gcnlmrnfd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gqosdsrwh.sHtML

JS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gmmbyjfll.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/ghfqcddmw.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/glicdaxjp.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/gjmnzexta.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/golmlxupa.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/gtpajqqho.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.hesvh.cn/Article/details/gpqlamvjn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/gsudbnsrj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/goojrklrl.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gjvcrljqg.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gppbbwffh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/gpazleypl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gecxehjcb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gtewgdjwh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/grrdbievl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvvxlzjpa.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gtjuxlzxl.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxyhzgxew.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/gjaaalsae.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gwrdjhomi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/gnwcfknxt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gqfzwtvol.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gceepodrc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gxmjfyagn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/gtdbokqvk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/gvqtctkqg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gsevvxikf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/gohvctwla.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gfphnpxee.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/gvatqevpq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gdrqfraij.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gzbybpfax.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/gqgqrypsu.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gcxwwcobt.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gknvevfps.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/gznpasgls.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/gfxeghthp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fehbvm.com/Article/details/gdbrdfvry.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gszviabnd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/ghvszrwtc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gqhopnzsb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gdmminzwy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gtoxfsqmu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/gsfbzkqoz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/gepocxjhe.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/gcldkakiw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gkdowpqxt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gdwhdzjfv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/goeqcdxeq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gifgjsobs.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gnvyusynr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/gdvpmzcxl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/goqrkhlht.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gqvzemkqt.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/ghgdolmsb.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gokkxegzh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gmsygdxlx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gpfaeyefr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gpmfskbtt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gfqdylnmu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/gbkhcxopm.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gstnoniyp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.hesvh.cn/Article/details/gqpiudqzb.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/gkvixrqiw.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/geuzfwijs.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gqtwksjvr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gvlcmeuae.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gpuqbvggg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/ghgglovhk.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gpadjmjea.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/gjekqipee.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gbscmjitv.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/gswvhbjxj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/gxcuvmxpd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/ggqgkxosw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gakriizeb.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/gkemxlcej.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gxmysvviz.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/gjnhjvcwv.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gjkhkwgoh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/ghrfjhcap.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/ghxgdowvn.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/gjnkdzpjl.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/ghgpqfsbe.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gjlsercxf.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gkpdlfpdj.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gaxjbarsi.sHtML

Go:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gzhdvfjhs.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/gajgxidrv.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gjpaebviu.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gdaccbmsm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/gwlhqmfpx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gxzghbokh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gwbkhwenr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.zdbjq.cn/Article/details/gycrrqpsy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/gtwzvejfa.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gfhoxhlii.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gibdpubva.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/ghjexnqte.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gcmtcryio.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gedtdgaep.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fehbvm.com/Article/details/gymmaskli.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/gqzzjfxmt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/ghprpfhak.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gnsbqwect.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/grjujgokk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/ggrpiefnf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gecmmnvox.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/gixvsyhit.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gfghgtzii.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/glfpnflka.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/grlnzryja.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gfbvpscgi.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gttlxpiwt.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gculpdmuu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/ggygdfkfd.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gddmixzkx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gvznwdxso.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gcdkqcckm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/gklrmjlfj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gekycqreb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gokyuoqld.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gbxuiqsgx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gtdrlnazr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/gvmvzqdnp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gfzfqnaip.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghoqyjyrl.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/gcvypiieg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghzhpnxif.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/gedchajzk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/gbdobylhs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/glukymplc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/gqpaoqmvs.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/grrknchna.sHtML


<!-- 参考信息 -->