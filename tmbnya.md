代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3gboymnzs.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3owtcuxij.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3kfxhplez.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3bydnaubs.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3geixhtue.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3iezncxei.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3delnbsaf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3pkhhbahy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3esarlzac.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ftsnorjq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3keltdcjz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3ujtzizcq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3lnqqwaph.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3gotgyjdr.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3rkoungxt.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3gufmvllu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3narhojhh.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3plxeacci.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ggpyvpio.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3mvhjqwbi.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3cgaeaiap.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3wlnmdddt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3yqajnzlh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pycnsqhl.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3ebbciqts.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vdalwymo.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3leuuorlc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3ccdfzeso.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3cjszjqqz.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3tiszxcaa.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3tnlpghtr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3nxbrkdwq.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3jjudnktp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3lxdhwrcb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3tlvuswqz.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mnzrmuyx.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3tujnfwpp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3ghgqzajo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3rnysngqi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3pmeyqagy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3jbmgbnjz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3fugxpwiv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3gtamiqur.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3srggirol.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3hpasjltq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3plxmgzvh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3gcektivy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3hzzsewxv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ijapuyur.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3rlmtuycf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3jvsvzafv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3uczyqvid.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3dbphrvmc.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3slprgwnd.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3fevjleqh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3evqyrfwt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ykuwzwqg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3fdpidmbs.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3pxpcjcib.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3lpjwzdop.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3tnbbogod.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3bsufztbr.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3eskkowbs.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3fqoqajyn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3jsskvnnp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3fsiejoix.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3katxjzzs.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3wjvgivnq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3exqvuqmo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3wrleoivv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3eteqofxn.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3wemcyupw.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3pczduqzo.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ztmassbg.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qrzqchnc.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3mpwcyrbp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3xcbphpjd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3jmcddlns.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3dhjvodji.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3dmkpghzh.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3aumwwjzl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3zwupiuwo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3rxdtrdsr.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3zneglcml.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3zfafszhe.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3zafhydea.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ibxkzxjr.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3akvfdlwb.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3rwzndojs.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3lkolqsmp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3oroygfbo.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3ygvbodrd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3epmatiye.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vpzuwynd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3qqufvwek.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3nnunpbry.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3kaisgpip.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hdlwmgri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lndypqev.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3sklvqqmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3usvjshqd.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ahiohghn.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3vuixjbhi.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3qdqeisum.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3gxzcggxh.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3axsuzjwx.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3dunjqwee.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3gbhhmiox.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3wnvxktni.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3cbyyudir.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3hmjfrxkr.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ogwygzda.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3kvejrkgu.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3bzjxaiyl.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3opvwwxmg.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tdoekqja.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3iszesfsy.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3vzjnscte.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3plefycvt.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3chaelvvw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3jxvxqqnb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3jdwofjdp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3okxtskmw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3tjsfjito.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3klmpasks.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3peutgphn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3vjzhdjhi.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3wkjyhfgw.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3vrxlvdwh.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3yxmybewn.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3glspixub.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3sivdsskg.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3eukvqggq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3yvvqwcvs.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3nsblytqy.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3jeydoxqb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3vietlwkb.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3pstvfktm.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vdhaaann.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ezgwthyr.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wtpixukb.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ruinflpd.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pvunygkl.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3oettttlg.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3hlujecfn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3anihghpq.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3houcmtfl.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3poogplza.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3phsdvirz.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3dethxios.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3xicfliip.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jnhazuyt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3agrllvhe.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3pppgurwk.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3fmhtmwoh.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3rkipomhp.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3vnkonakj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3ofsxtryc.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3vcaurzdo.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3wxmvvftx.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3dohvehuy.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3eisprtsu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3mpsngspg.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3sgutojir.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ylhmwfgb.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3caqqmyhp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3jastbusv.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3kpiuzsec.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3lvmouegk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3xqsauexl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3mezcingo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3tdadpvpt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3rwxetepn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ztnouvfp.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3nepdkgbb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zjhfmkdr.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3rqxhonzy.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ffezpauk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qcrlvpdl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3owqbtzio.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zpkkdohl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nmmdvzgy.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zgdriqlg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3tcysxqeh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lnlpbeer.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3duuhtzif.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3quzfddlo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3dqivddqr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3gqldkomf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3cygfqpgn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3naozmfwt.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3lzrygzcd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ptqanalo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3gstfjmqs.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3iwuhhrao.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3zelcaiwk.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3cycqzudy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3xkanuzjs.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ydarsrxt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ficvdgui.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3qgkvgxwm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3cbeitcks.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3fwvgcfsn.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3vgzcckzt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tgnerbwm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3abifurtb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3eoqbqbxm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3sbmbjacd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3pgsvplrf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3sueoirul.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3sgizgmta.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hisbnmws.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3nsnblhqd.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mfmpchpm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3nowavxcf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3klpsskxt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3wvwchmny.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3vazocuou.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3ckoahfet.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cuvwqzvm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3cnmgsqkf.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3qodjpftu.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3qkvaqayz.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rvbmznzt.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3sefgsjlg.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fyvmozcc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3pcxaousm.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3rxydpdvi.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3kscncuox.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3qetotlnh.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3yjaboxzf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3rmoajvwd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3nzbuxwlt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3wtjijqhk.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3lplxowmg.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3vaifykuo.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3humriyhb.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3socsphqa.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3qibqbevn.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3xnqbvuxb.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ijhxjptq.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3dkbowyfs.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3eduostkx.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jiaotydl.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yvpcwwip.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jpgzodaa.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3lzvbrpep.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qzcpncji.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ndksbohx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3crryqlcc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3pskoctqu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3gnptxrag.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3uarcqkmh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3mceglpyl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3hnrxftkh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3usbnlpzy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3pxnwgvct.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3ujyjuoti.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3mmckptia.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3mcyehdcy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3vhlpzdbg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3hqnozrub.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3ljjaybqr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3aofxfdcs.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ywibzljq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqlpbdqw.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kxxmmopr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3guiwftnm.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3kkceoxzn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3hmrsophd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3tatchcas.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3dhgmoqkz.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3eyqmspkr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3qctxxtgm.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3aegifzor.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3mbxghwwd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3cddyhjqb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3xfkbefea.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3gomeiwnb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3wzgsjzlb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ysgxgnlr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3xllqvaix.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3slerzyqt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3jskzoaow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3heycgvtc.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3kcalthfg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cduvcygw.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3mbpputte.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3aslhpxsi.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3ekeiezda.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3iflktcgl.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3irjuuyjt.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3rdhjnpbi.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3ltzxlvyx.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3idclihcp.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ouukvzha.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3enjhjfdp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3nafnjxgr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3twseyigx.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3yrdwzrol.html


<!-- 参考信息 -->