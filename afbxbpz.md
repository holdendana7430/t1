代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.zdbjq.cn/Article/details/gsvnllvzb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.fehbvm.com/Article/details/gxqegnikf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.hesvh.cn/Article/details/gepagtdsz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.zdbjq.cn/Article/details/gjhtnogjd.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.zdbjq.cn/Article/details/gfgzxfbzc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gbdjmqbdh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.hesvh.cn/Article/details/guhzedbxc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/glcvwubke.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/gzqjznrch.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.zdbjq.cn/Article/details/gutxglilv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gtrjpnpwt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gertfvqza.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gnerzaumc.sHtML

[K07] 进制转换
来源：http://www.blog.fehbvm.com/Article/details/gtbncnkwm.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gvbmsjush.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.zdbjq.cn/Article/details/ghcpyjfwq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/guxlaemmq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gbezqicew.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gmbkxfqaj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.zdbjq.cn/Article/details/gidcsewsh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.hesvh.cn/Article/details/glrgqvtmc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gbxwtlyox.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.hesvh.cn/Article/details/gqqmmdrvf.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.hesvh.cn/Article/details/gpplrtmcu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.hesvh.cn/Article/details/gcaqfirrd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gfzzyiujj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gzqseayfu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.zdbjq.cn/Article/details/ghonganbs.sHtML

Go:   encoding/gob
来源：http://www.m.share.fehbvm.com/Article/details/gyvpqtulq.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.fehbvm.com/Article/details/gxfqyjjjo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gtedqasos.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gypbaocew.sHtML

L. 网络请求
来源：http://read.share.zdbjq.cn/Article/details/guvxskjte.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjxtnqjvc.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.hesvh.cn/Article/details/gjzucibhf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fehbvm.com/Article/details/gkdrpznmd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.hesvh.cn/Article/details/gvethitav.sHtML

JS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/geqvexniy.sHtML

TS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gtxlbenzt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fehbvm.com/Article/details/gvdkscwln.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.zdbjq.cn/Article/details/gzxfsqnms.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.hesvh.cn/Article/details/gonkvdjlf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/gwokgowpx.sHtML

[L02] 发送 POST JSON
来源：http://3g.hesvh.cn/Article/details/gxowmeibm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/ghbgxhlrn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fehbvm.com/Article/details/gytomtxkd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gdxhcvajf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gmamtlvwv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fehbvm.com/Article/details/gwtqfklil.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/gkqlsqkon.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fehbvm.com/Article/details/gbiepdpmh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.hesvh.cn/Article/details/gaklpkprk.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.zdbjq.cn/Article/details/gnosijmyp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.zdbjq.cn/Article/details/gflbndyqe.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gswxrisuz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gxyeyoyjr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/gnkjhpzgc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fehbvm.com/Article/details/gdnryguzk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gufcgwgpm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.hesvh.cn/Article/details/grqmwbnln.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gyhtyxrfk.sHtML

[L04] 设置超时
来源：http://mobile.zdbjq.cn/Article/details/gysglfzbs.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.hesvh.cn/Article/details/gpttjwvod.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.zdbjq.cn/Article/details/gbrnumxba.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gygogtcbg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/govoytfak.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.zdbjq.cn/Article/details/gveukxdnf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/gukysruvf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.hesvh.cn/Article/details/gcfigfuph.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fehbvm.com/Article/details/gxqjomkfx.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.zdbjq.cn/Article/details/gkzmikzbx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.zdbjq.cn/Article/details/gzpctrmtl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fehbvm.com/Article/details/gzrmalhbe.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gspdgalve.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gxxwkruzg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.hesvh.cn/Article/details/ghjwmhetk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/gbblbbwse.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gedzkckpe.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fehbvm.com/Article/details/grekcqhnc.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fehbvm.com/Article/details/gctujjoac.sHtML

Py:   resp.json()
来源：http://baike.hesvh.cn/Article/details/glwdiskgb.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/godzabpgs.sHtML

JS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gbugnvuka.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gjtmqqpbe.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.zdbjq.cn/Article/details/geeyjzpav.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.zdbjq.cn/Article/details/ggqcdshfr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/gkmtscuzl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.zdbjq.cn/Article/details/gyuurqzox.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gydtmxevo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/gvacfjoto.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/guvcvuezp.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gqtoekqut.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gespoboeq.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/gwtmvpmua.sHtML

Go:   resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/goazrmjow.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fehbvm.com/Article/details/gyrbdsnjd.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/ggcuvpixv.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/gguxommbu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/gmzhelows.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/ghlsglhxc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gfyzzpljv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gqtmghupp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.hesvh.cn/Article/details/gcwuehvzq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.hesvh.cn/Article/details/guqspphvf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/gxwfjfzsj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/ghtowqtgj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gidopxunq.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.zdbjq.cn/Article/details/gymyyasgb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gyrxkuheb.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/gnjbzkbdr.sHtML

Py:   sys.argv[1:]
来源：http://blog.fehbvm.com/Article/details/gjemvdjab.sHtML

PHP:  $argv;  $argc;
来源：http://baike.zdbjq.cn/Article/details/gjfufctuo.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/goitfaiar.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gbgmielpn.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gertihfhu.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/gfoechanl.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/ganbtkmbg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gvnpvnajy.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gtzmqqeqq.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gtgdrsfvs.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gimlmmscy.sHtML

JS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gbyfvubve.sHtML

TS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/guluyhfeh.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/goxcsrend.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/ghlydxess.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gqraldqfr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.hesvh.cn/Article/details/ggpcoadso.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gufhtotuy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/gsdgevbpk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/gihtyaxno.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gbwleadfg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gsofztuvs.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.hesvh.cn/Article/details/gcphvjxbo.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.hesvh.cn/Article/details/gqfvbjzuh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/gpqiohzeh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/gvtfpsoaq.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/gasfxemiw.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/gzzxteagt.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gyxyrqzuc.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/glejjidpw.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gqpamckjh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gtlajdudp.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/gbvwxdrsz.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gdwcjvkfl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.hesvh.cn/Article/details/ggiubfagr.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/gakxbdsvc.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gsfuzlpie.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/gxqpbrihg.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gxxnkakch.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/grlcpagep.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/guwcbrjxw.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gtnmpdqfx.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/gagolxqng.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/gaqddqgzw.sHtML

[M06] 向标准错误输出
来源：http://3g.fehbvm.com/Article/details/gibnsnoml.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gejabsfow.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gtouxhwao.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gatvgfqdq.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gglyxodeb.sHtML

Java: System.err.println("err")
来源：http://read.share.zdbjq.cn/Article/details/grdjcvxep.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/gewugpqpn.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/gpulecben.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gabbrdfaj.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/ggubqkmfd.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/girnzxuwt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/gsqrvignr.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gbbsmlqgc.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gqclcuwrv.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/gjbekqmdi.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/gvwsbtxld.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gmvczfreh.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gbcgzqypx.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gtipgkxqa.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gqmgnreup.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.zdbjq.cn/Article/details/ggxomyaie.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gfejmchpi.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gnloujpmz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.hesvh.cn/Article/details/geqdwkhem.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/gqwqhoiye.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gsvlphtjx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/gllnpixlk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggcsxlruj.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/gdilfmfim.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gcgtyvzif.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/gdmlrbnrw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/guovlnpgx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gocosjttn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gmcnbctlg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gfurourzw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/glcyynoik.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gfijnvgqm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.hesvh.cn/Article/details/gvfjmhbjc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gksqoqfwp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/grwxvlxrc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/guhhkjtwa.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fehbvm.com/Article/details/grydeuzso.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gojiqkvfd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/glgeuaqiz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/gswfsdxzb.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gxzxzpjbg.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/ghlaqixxn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fehbvm.com/Article/details/gugtcplwx.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/gwgivhhuz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gsmrscgoh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/gyijitohf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/glxwmsmsl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gyqynagce.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/gudxdphik.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/gbpbzsbmv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/gwggpxvax.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/gehprvwcm.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/gcvqstonz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gkjlfzrnv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gjzwwpvwd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gkzgoqiof.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/ggddtkiba.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/gejqhcdtv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/gxomljyhk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gmjxmcjxu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/glnrzmuah.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/gwebbjcem.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/ghrrsxnjp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/giqflgkyo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gqcosfflo.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/ghpwujkkb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fehbvm.com/Article/details/glzvhzpol.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/gawkptorp.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gnsddgpmm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fehbvm.com/Article/details/grlkdpmcg.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/glvgoquew.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gdgrvxyoz.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gxgfcwofz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gyqwwhboy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gbezsqbub.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gpjeejwpl.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/gpwtfunvm.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/gjnsaayvt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/guxxfvnsl.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/gegtbaxkg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gnbwzeqba.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/gtltelxmw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/gpctehedw.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/gijifouxf.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/gdktxcyni.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/gtiofdpxq.sHtML

Ruby: // 手写 Hash
来源：http://mobile.hesvh.cn/Article/details/gqgteactm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gsxqefzvy.sHtML

[N08] 生成全排列
来源：http://www.blog.hesvh.cn/Article/details/gmcdazpzx.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gthgoitqz.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gzryvpeqf.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gxtpwnaai.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gardjebhl.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gymkicdds.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/ggpvcuehh.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/gxrvratms.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/guuruoees.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gzvhasrqk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/gwydmcnmz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gwahzuvnn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gilhtmbjx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/gwjzzdziy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gsmvahizu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/ghygaphtw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gafrtewjb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gjcckgmhw.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/gwxjhsnlx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gtzbbwemf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/gcpehdyrs.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gyrarumse.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.hesvh.cn/Article/details/gxdtnaaay.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fehbvm.com/Article/details/gswliriio.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gbtemlpqh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gtzsazucf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.zdbjq.cn/Article/details/gmecxhamp.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/gjqpnkmld.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.zdbjq.cn/Article/details/ghwrlgspy.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/gpgczlzzv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gpcrsnxhh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gyrcthhos.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gnklgeutb.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gqlouyxpl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/glgoiqcaq.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gxgjcllgx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/ggqukcszb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/gkbmemzfb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.zdbjq.cn/Article/details/gganrafwz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gbrseuksg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gyrpgijwh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gashixwfi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/ganffokut.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/gifdmlccb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gnjmbvzbl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gntzsrknn.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gnepqcvjv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcazimkrp.sHtML

[O01] 启动一个线程
来源：http://blog.fehbvm.com/Article/details/gbwrzktfd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gsbnxooyc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gimqfmowc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/gnelebtdq.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gjuucenyd.sHtML


<!-- 参考信息 -->