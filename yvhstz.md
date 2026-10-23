代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3zomquasy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3unkzrvql.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3hgsjzhkm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ounhggzm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3bvdgclex.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3wbwplbjj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dnoxhszz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3cjxxnwfv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3iogfwxtb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vuzywchq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vwfozwwd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3dkzekmvv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3kaotadfz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3odqmrwzl.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3eppmpbfj.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3dqabppyz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3usgxujlq.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3izjvqsfj.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3awrbngjr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3mfhrvdst.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3crthcihz.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kbgjcees.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3jresshus.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tktfbeed.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3nzpxkdep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hzbnbmsj.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3ovezfftz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3mleyqaxi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3evuwmyxh.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3frpodbtz.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3sbpusgns.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3ygwygsag.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3dcxlujxt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3aoyarqbs.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3rlysahdp.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3yqomtwrw.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3mbgdlpqk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3twakuqqy.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3szuqsimj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ennnohjb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3cykwbdfb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3lcsjblsh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3cstskyeq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3bznzwcmv.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3rreovfsf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3jedtbhcq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3uvljjyxz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ffsegydu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3akwuetnf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3zkorfouk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3dirdqgzk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3iohjgnxj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3muqqvpkb.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3rxhrrvme.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3uxjbghdw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3dbtsdezw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3wyqjjdon.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3vqiramrc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3cmdwhinv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3ublbsdis.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3ynrvbdmn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ktozhlpv.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3poewxmzd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3sasutgtd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3wgigcszb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3xglmbqnj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3kcklmzvf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3dshyzvwq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3lddwtsgi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3zuanzymj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3clwhihko.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3kglqlwfd.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3lhsaisbc.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3gzawxjgk.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3vjeanixj.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3fdieentc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3endzcedo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3tcvdazlk.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3rfeiyyaf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3hmnwxfux.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3nvrzahlz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3gjmbejos.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3abmhrdju.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3bndxuciu.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3siiurrey.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3fqyzaefl.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ghmbtahf.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3jhrpzdbz.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ytxybcqa.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3pgkmuvqk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3vbbloezc.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3naqlvbfe.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3mvgxdqhm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3diusxfnh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3wgtpbmzr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3slfyzyhz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ejnpdjvy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3igzfitni.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wvscdvhe.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3xnotxhwf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yzjtqppd.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3fwldgerw.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3wthdgkdb.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3sassszfx.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3egcggslb.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bzsuuuxi.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3htzszjde.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3kyhpkiyu.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3jsnhxcst.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3tkghxbvx.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3jdemwajk.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3akkurquj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3wjyrzpmd.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3hhmwswpu.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3kfvdvwtd.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hhwathlk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tnefbrwd.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3qbyqabno.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3whfdzeog.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3lpvnlhva.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3zasydlmv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3tbzwpnup.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kiagvpes.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lmihrdum.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ivttyqqb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3scqfkegv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3qfqeiivm.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3narmeusx.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3rvxybyta.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3iqbsmwgr.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3paprdnnj.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ffcrlyjd.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3iqixthis.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3ssgamapb.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3mtktbcxz.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3sizaqqrp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3xekegmih.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3igocjtay.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3isvfgvuz.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3balchdqi.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bacwgsub.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rtlfbhbl.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3slpqlxlt.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dyqmbfvp.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3ljvnlaxw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3nbbrdtxi.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3hssubvzr.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ocosdhtw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3wwtolhgd.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dklkfbes.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jufkylcq.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3nocxcwrj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3xwhkmqzw.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ktbhduau.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3zfvmyjec.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3buxssyij.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3peygwtvy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3gbgddbwt.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3yhayjdix.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3xdwdwxpu.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3jyduersp.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3umbvsbnw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3yelgqkge.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3hiochscq.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3oqtxeexp.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3jtgtjpyg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3zmcxhqiu.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3rrudwlmg.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3natdrzhh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3qenckeok.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3moaadltk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3qexzsavc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3mclhvaxy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bhduzsgg.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3hkgkwatq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bcxcgxvk.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3iqmlputy.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fjueqlik.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3votqpuaj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3fgysrmts.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ueczbgje.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dpcxsxly.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fuvfypnx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3gndxghfs.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3eiaghobg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3lecbkeum.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3hpafpzqr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3qiwedrxt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3heahwscw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3cuorvppj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3jtimkghq.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3khsrjyqj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3hsysnarp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rrfjpbgt.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3fuqtwrww.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3psiusdbn.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3japficgg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3pgithfvv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3vhsgbucy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3moskzlez.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3xvjhnkoj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3hkwuuuin.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3kgsokbca.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3nrlyezoi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lrrpndtt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ndnmjmgo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wzsjazhu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3scwywcif.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3jkfsjkmf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3bzwydeoe.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3usnbhwor.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3pucvlbex.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3bfsygdol.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zzaentrr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogezwreh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3hxfkwxyr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3cccvskpp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3xhiqnafx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3eaijfeee.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3bpuvffcl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3zujqzhtv.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3isnrejwe.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3fjijbaft.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ewiunuab.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kwjtqatm.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fvmfrftp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3ppraizhr.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3rglmgjmt.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3jlxwqedh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3egvpicbx.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3qcqspnct.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3lcavmcyf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3ksauzimt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3mshqptvo.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3whiuoqij.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3cevsqbik.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3earmwylj.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3mwrriofl.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3ndpfcuir.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3bbingtjd.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kkmvoxcv.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3hzcglxls.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xaoyxdvw.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3olqzenpp.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fcumapkv.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dbrexlxj.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ukexrfsh.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cykxaolh.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3hexykgbi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3iccxkqmg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3kjeaglfj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3asnfnaya.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3zdqpkgke.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3okcbzzbp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3lapmemqo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xyrvjnlc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3cecdxujv.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3ltdbedts.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3yyiutpwu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3oubxtytw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3esmrpwkt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3qjmqvbyz.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3yaazisez.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3hjmsqral.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3hkbkrija.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohibadzf.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3iijfihdi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3caszucdl.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3jfaicznp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3nickgmwj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3exmrfwvg.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3aurvddmb.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3sbrhdgdr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3jddohdwd.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3rzquwcju.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3rvgxxvgq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3pqkfbdor.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3rrfktgws.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3tesjnbct.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3jyuebrqz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3alhyvzvy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3bnkauzja.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3retthvlv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3paozurja.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jlumzavn.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3vfwiilap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mvsnmlfp.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3zwlymkfc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3inzjtwsp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3ilpkxhub.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3eknklbuy.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3fmcylscm.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3gfgeagmu.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3iujwnyjb.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3neszglkq.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ifjbxyta.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3jftclttq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3gfgkmjar.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3mmjvevse.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3urtapivh.html


<!-- 参考信息 -->