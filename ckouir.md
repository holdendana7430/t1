代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3vlwmgxnb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3dmzmjquk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3gndlrjeo.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3enqrketq.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nzaqfrmf.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3mvxgacbc.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3zztmxcru.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pzunfaoe.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3xflclsuq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3jntxeyeg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3xsebqoxk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3pqlchovx.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3zwpqsnmn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ezvhvkbe.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3knzbsrjy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qyqwnmkg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3eaoykjfi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3cwyqkqqs.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3wlrhbwtw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3klkcyjel.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3klkgsuba.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3tcbmjico.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3taqkvnxs.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3ftsweiuv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3pbvbylch.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3liuhfdoh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3cetwybiw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3dircniyt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3gubwscse.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3krtfyhgx.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3ezbeqdkb.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pobmniky.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3kozavogv.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3vbubmvir.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3mwphhszr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3soewwpea.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3edthemqg.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cgklgvrt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3czsaeivp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zwdgedud.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3dcfbvaqq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dakfjnml.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3mkqovgqx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3jfoqmzdc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3lafhsisl.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3fhctspem.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3fnevgzra.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3ynsbktvk.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3gjchjyna.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3jyrjrcth.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3afgbpror.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3sutlclvc.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3lyvmgyrk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3rzzrqroy.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3selzzurn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3gltiaxqd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3wixrduxp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3ulunzwix.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3yyuhgdin.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3tjnczyex.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3dfpuyaqb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3jhnzdnge.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3dnsedvff.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3zrvrdwmg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ntnqqkli.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3kegzaixr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3khyqhgmr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3qowvyxhh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3kifizobu.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3uixbqjou.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3ofqejsyo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3nfmenedm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3xalwlcas.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3vghvlnqs.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3yjmapdlu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3odilrbpb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3bzscmyac.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3fvsntily.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3hzxrdauc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3prajnzwv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3mifuexrn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3mcucoabe.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3wusjfvrs.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3yxzxwvvy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3taquowij.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3eoxcrfik.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fpfmjpnf.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jmsdjaxc.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3drfriawp.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3sxmdirzr.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3thgtfufb.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3uhviesdi.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3epskpxkh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3icykckjn.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3rnrrfccc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3eqsliphk.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3vqpahjsd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3rywvtmvs.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3mydfielu.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3nubnmept.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3gsvjhiez.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3xnbccgmw.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3jarmhgcr.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3uycshluc.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3gzcmzcdv.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3wpcbywov.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3dfxebmod.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3twsghdpm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vovuxmok.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3hknydqgh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3pzzfzluf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3wmsspnrc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3sepnuobb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3kfavgshn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gohfhjnx.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3bviemjmr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jcdwwoga.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ajgtnkdy.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3argkayux.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3wfopfftb.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3yijjnmnk.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3renwomae.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3jdehsxoj.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3xzhmemtz.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3wgrfbmua.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3zdqobzcp.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3otyuuwhw.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3grhfqfuv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3kbqmnwmc.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3olrhuqbl.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3shguyyzp.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qjvfscge.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gnsergjv.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3mgcxbosr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jnrulgjo.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3lvnlnhua.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3hrafxnwn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3xdcjblhz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3roiomeub.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3chbneocf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3xcmdmtqw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3glsbdvxp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3mefnapcd.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ojdbjtbp.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3fbapmorq.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3gkhgbpfb.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3adlxnpdx.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3kuzhqmhs.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3nawzqgnb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3soviaekf.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3khiqbxbw.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3qrgbxifb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3imqsiyvz.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3gioawnqj.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3khzewhoc.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3otavoxdj.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kjhupebj.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ivmnsueh.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3snqxebji.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hsqmuanp.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3nxxcvkti.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3dmjccinx.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3wechgfib.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ynowcsrg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3vkfdurxy.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3zgiikhyp.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dzvwfozp.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3viksfyii.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3tnbrftnh.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ahtuhqte.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3khdknuwy.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ohkudaey.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3atywgegp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3vsuobpoi.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3gicesxqg.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3kdmftcdi.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3sunrmvvy.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3xbqjmqan.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3shrzxuap.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3agqohpli.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3vznhlbsy.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3vlmbcngh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3llewohde.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3hetkbywe.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3rslidsob.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3etfludoy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3lstttedl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3oywlbxnc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3fqelrbgs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rpzdqeot.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3zayfjdnd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sqiuyepf.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3juwmierp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ktffasoq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qyhfxaee.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3uaosrmrx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3lvtkavkr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zjqpvbro.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nefyjkhv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3kataekmd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nnigbfuq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3rcazakvf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3rvxgsymj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ehsjmoth.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3byzuuycz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ovmvnnqs.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3ejawqaof.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3dqvphblz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3dlxzpduj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3paqqpffu.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3gbgorqrq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3dgsclvjo.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3gyibhkje.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3dnmpzgrb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3fpwquepi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3nykwbled.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3ipzcmril.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3knsqeggs.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3sgnnzgbb.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3lxptfpyy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hzjphjju.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3vsokuxlw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3nssvsscb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3nxppkjtb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3mwsinpif.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3rcbkapep.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ennwjhed.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3phbxdvpx.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3pyppreer.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mpigbcew.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3sovpsjis.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3oknwmxta.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3azaxfaap.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3gvdmsmbw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3bhrjhunv.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3ywbmcanz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3ahcpeunf.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gsxdpnaq.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3zmjbubji.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3iczrwhqm.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gobjfllz.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dxgmlzab.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3xjwpnxda.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3tfhugchb.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3slkpkyue.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3xkwtzsgb.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3owxuwuso.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3iykldbsb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3rzwinnqw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3glwjivnw.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3boowpwzh.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3vcpkdudb.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3zjvwwtqh.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3fkxxzbds.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3qkwrizlb.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3rhcjjgsa.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ysopwtxb.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3utrjyrvo.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tgxvmqdq.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qatllslu.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pcubpoyu.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3uwzxkvzg.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3htdflrdi.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ofbiqwan.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3exjnqluw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hxcfiuzl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3jtfmjawa.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3tanoidya.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3dlfuidhr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3yqjvrazc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3fogyrjlm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3djcqxykm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3qpwgwwpa.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3zjidtgso.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3hdhtiqnr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwlmfqse.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cgizwblh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3nkejgokr.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3opepdmeh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3arpqroys.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ibnuhrfd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3tnfqmimv.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3hwdhpetm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3vitqfqxs.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3oiiagmlt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3xqrivwmb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3wsqizhgw.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ledrkyas.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ocdoiaqw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3dggmqens.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3uklaxsrh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3lvqudxcn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3yppfeuds.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3zfmcfztx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3boomlwvq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3nxugfddn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3tqlocoxy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3mcvrdlrx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3dkiejbxv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3hjkwnbld.html


<!-- 参考信息 -->