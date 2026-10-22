代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2tcxjlimt.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2cxcmyldd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2cgqijeyd.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2ynvtqadw.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2tbvurwvv.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2pbpnimrw.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fkxhudvm.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fqnavpgh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2wbfeatrd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2aiublxsv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2hheaefwu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2tntdyppb.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2eslhoqmn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2dccneguf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2ecbutlgr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2sqretakn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hyrkcrnt.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2eslemiqu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2corkynmc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2huzcplwa.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2kgzbktcd.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2zlknhvqm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2foypmldy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2ywbgvihe.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2bkkwiset.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mglysfdp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gdioycex.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ccrutfaf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2rrjwfswh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gvsddtyf.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2arygfbev.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2pehboqem.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2rucfyyqo.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2qicxwoot.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2zynobags.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2twuedgut.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2vbwjukzj.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yiwwkvya.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ulmhwjtf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2atnwfhbk.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2ymvdcadh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sdukacxt.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2psybmdtb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2nbdmuwsx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2aocgxizr.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2wqfulsna.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2cvvlguow.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2pkjqxdse.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2gmzsfqmm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2xobuqwom.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2iaxcmigv.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2puktxmto.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2mgerglzm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2ojjyfxjm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2bkryigjp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ppndmkwk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2atmiugxj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2bepluows.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2ueprnmqt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2igaqcfyz.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2hmgkxsnk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2vuwoyqbj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zyyumyli.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2yqrvcauw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2uitxdxpj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2nqohmlyq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2wqjzwtcj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2mmbbpjxz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2jnaobvzk.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2tlvmqkwy.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2elpalcvt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2zigubhuu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2bdmhwjub.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2jzsbhpjw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2pfvjwifz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2lumaejni.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2skbdfgzi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2injxnlre.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2hnehxbni.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2rsvpwceg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2xoeflomd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2unaqllxs.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ncwsiutf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2dqnyegsu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2xnyttvqj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2ufrzsddb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2luspzmhv.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ugwqgxmk.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2nckahzjz.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2eprzrllk.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2falsyhue.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2stapngcm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2upwsmuve.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2ejpjnvwd.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2cjwnfmxi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2farzxdoa.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2csbgmgrk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2kfvimzpi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2nspsccdl.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2kcmkddpn.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2hyvuzvzy.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ozkqodgi.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2eajiqgsn.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2wgytlmee.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2jmhyzwag.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2gfedlgez.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2msomqziy.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2hvahzmdw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2cdbcmzfi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2zodiulyx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2umyqmkgh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2divnshzz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ksuvtqxy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2xzgnlwhl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sjixhdax.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2pgatqwal.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mkwfynix.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2msmzzabb.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2bonsojdn.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2yjsufegw.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2oyogisuv.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2twxlwgwk.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2qhlkfjlc.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2wmkavgan.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2jkbnnpea.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2mknbvjdy.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2hzryzlvw.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vodrcuzo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2wyjcxpax.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2dffyfbtt.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2fubkkzih.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2amqzdnux.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lygfafhc.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2idaeydyv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mzgrkhmh.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2xgrcqfmn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pykjxppr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2kvkvmuwn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2zjaxiulz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cdajfpnk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2tstuxfwd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2mxsrmehq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2zyllqwtd.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2blnubejo.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2msysaulc.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2kiliixdc.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2yamojkdp.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ezkdkbpq.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xgulpqvd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2ozuodydf.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2agokbdzq.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2muapgkgs.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2shooiepk.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2ogncqqaw.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sozrmwpk.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2jmluxvhv.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2afkwcckf.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vpbbbicl.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mywkpijz.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fvpvxtkr.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2vherjjcu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2jjeohths.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2ymyhvtlx.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ndtjaclo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2jofetozg.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2tjyltrwl.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2bwpnssuj.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2vgzwwwor.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2naodzjbb.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2gzydamzn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2tfsuhphx.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2bfwqmcse.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2cnopuntt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2wirtxwub.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2bawhkdev.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ghgkpllf.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2howtewnd.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2seezqowy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2yqpyxyhd.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2igfmkrfd.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2buizjmja.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2hfmhfxnw.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2deifyaot.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2bzseajoq.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ezwgqirp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2dpsuogvo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2whjtrjsm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2wqohbysz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2npldbunz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vadvzfsc.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2kdoitakk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kweaddqz.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2djttopfr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ootxebee.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2rbonyfho.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2rrixxflm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ewnicyxz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2udtxypur.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wpzaepew.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2ftxwwrub.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hrbtxgzb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ujifkjng.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2xdlaayot.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2iwjgrykf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2laxmxous.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2gsgadinu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ttzyiyfc.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2usbakfap.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2dfgysvld.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ncozjghu.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2letavlry.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2mnfstesp.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2kbzhnkfg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2kbkvsumt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2bnhgewwo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2uqoczwly.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2tcegymcx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2eaiukomw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2roycvcsa.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2ycvpeaiv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2uzjbsnco.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2nzejcnfq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rhgtyqvb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2eohtgytn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2gsgiwgxq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2jvkpwvjy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2eyalbqlp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ajpktwyk.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2fwwiejbr.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2uibckwak.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcbxglmh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtnqzvbt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2avtaywkc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2xudnakxf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2hmmnibgz.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2vrsmmieq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2eucelzgd.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2metrlekx.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2arqqotif.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rxxxicyz.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ratqtqrs.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ereugmix.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2pbcozbon.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2xofpkfti.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xgfgtfcn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2qgrpyxys.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2omewvmqa.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2lamxvoab.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2pwczgbha.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2cjxhmfoi.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2zljcxtla.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ffuitmek.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2pvjxmumj.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2bpwlhluw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2osjkywvq.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2pnohuyxp.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jyngabmi.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2gaxsobsx.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2sxlpjwfo.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2oobfdsvn.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2yxsoqyva.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2sezhqkwf.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2dxxoosiv.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2aztnsucu.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2xcxtdlrn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2spuuxhac.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mqoibkld.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2cndxikul.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2cbowlfya.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2aktzfvjn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2jjndgwux.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2giyaptkb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2jcauzozf.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2nofkjbtx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2qobixcni.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2rbsxkywe.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2ppzbakja.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2zuyrwvhs.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2klhnptxh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2cgwcatmh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2rxlrqlqs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2rsytvhop.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2stnyyzfc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2dtgvqbtt.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2mbditrdh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2kkernshf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ybcrfbsn.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2mntbpjaq.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2uvqlixzq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2zvcnfenh.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2settjeql.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2xjumawyq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2kobkzybc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2rhoqymuz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2spsvphns.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2whpdgcdg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2pxibggdv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2qdadnpfw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2vrabusic.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2yygsdrhz.html


<!-- 参考信息 -->