代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qorconsr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2dzmmfuem.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ywpzjlfh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2fcmercev.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2motxquvk.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2datnwajf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mhfqwhmj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2uoktcmtj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2exjcgkbz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2uyqvthof.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yvumtxcb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2mhdafgap.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ijeebfuz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vclqfwzt.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2mamvxbci.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ahncdlev.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2sxshkdny.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2wlglltld.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2lekhgvzk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2arqjeipo.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2ynrgymox.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2ylxskvqz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ryipewlf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xrpfzphs.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2fdvmrmiv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qtqjdkpb.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2qewrsoat.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2jtgnkhng.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2syfgvnef.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2rpyiihzu.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2lmxemnnj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2ajqqeaps.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2aqrmtmxp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2fajjzvks.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2kvaconzw.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2gyewjgic.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2xtbkzcbr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2ojmvfbqc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2zaodrpzq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2xchypkyu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2eruyuzbg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2etetdtog.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2qgvwvzcy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2onfsjpex.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2llbqxpoe.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2dojirizp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vldgdupy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2bwgwovuq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2plclfbjp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2ustsacgb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ihgaxrmz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2jwmsucam.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2bbkjmcfa.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2wbketght.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2izueyqtk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2hwycfpmw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2tqtvjwev.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2lcwkdxrh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2mfqqpfwz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2lwzrcsjl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2zyqahjvl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2dhdhykwr.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2egllwrvo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2jwszmqii.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2pojfnyze.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2nnztpbvg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2boliarjy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2saidtine.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2vqiuodsm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2kthkbqob.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nhrqbena.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tlokfcln.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2bnvxmyet.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2curshgdi.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2usgktkwt.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2wzatcatp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ehotqrqs.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2zybroqoy.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2avghtrvs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2upbwycoc.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2rebqfeix.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2xeginnyl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2dyirplqr.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ghcggrep.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ybktxkku.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2qrmspiem.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2epyagloz.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2elixnsoz.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2hhhbqavj.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2hivojspf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2jisujuos.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2bdyymyup.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dftaunpy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2kwctkfew.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2sfmderoj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2pjwgwbaa.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2tgsrkdxe.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2oynlqoxx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2urgdzhix.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ruvutejx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ivjlqmip.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2hibepnbw.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2dupequcq.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2cdocgqhk.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2xojfgzby.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jekdlelf.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2frbcbxtw.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2cljhoetg.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2yeejaeqi.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2wskjyldt.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2mqffpvuq.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ricwajsi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ttdpnzsa.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2nkkteuis.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2rzjtjdls.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qmrgamnv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cxhxasbd.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ampnozqe.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tejubwal.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2utrvdzlx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fsdmcenn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2udaamjfx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2kdxdbatm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2baafoips.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2iopjpgut.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2fgpqvfpz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2ajgedtlq.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2pvgpbihj.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2vrgwhgrh.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dyiyspkt.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2bwzvydta.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ivznxxyh.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jckdifcj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2ghmfnwrb.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2duvmdrtf.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2psclfhkg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2tlffmphk.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ocilhssq.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gehkkpdr.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2zdoujxxi.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mcxfmbie.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ypqjznzx.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2exyiusjk.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2othnfdnw.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2ejhfejor.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2kieftbec.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2tciauaif.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2afjsynsl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2fnpvepsf.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2jnfsyyhp.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2moqnpief.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2yjviwwjn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2icnhgbli.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2aqgprivq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2jrncrzbz.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ztogxnxv.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2zfhoruzp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2bawakjzu.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2xinbegpm.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2gtfbwins.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2koyweigi.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2sbzhjwjj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2fkdfdczr.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2xxsfwvni.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ahollttm.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2sejuvknt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2yrtdphlg.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2vilgrmvj.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2vdlgczym.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2rldohkcl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2lkktllit.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2muunfflr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2sajdkrxz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aeblrttb.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2bsudpkzn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eaqdzfbr.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2wxfhlunt.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dxlriddy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cfvupuqu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2veosxoye.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hcsophuh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2warjvidn.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sghsqujk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2nlkpodkz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hcnbljhw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2ydwtdokl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2haeymwdb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2cnhlqljs.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jdgjdhph.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2asqulnsf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2vfyhplnn.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2uagpbaul.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2qnpcmvot.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ximldmek.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2ejeazlpo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2lazqucgl.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2jjbdbwdo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2upkwdiho.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2chgsurat.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ncdmngjq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2sjuhavub.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2vlqgsgvz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2nuxftxdw.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2wsgrwlnw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2iqoarktl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2gxjwzmep.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pfprfspc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bywxchei.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2lyhgtqtw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2dxlrdhpn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uusjoxsp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2amygmawu.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2hvsjszga.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2nxwozami.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkegzzay.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2msomwkxs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2faczhesc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2gayzanzv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2gewgmwbl.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2pxwgpzzq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2utgqyhwm.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2mfsyvryu.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2feyyecxl.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lwgwizpp.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2knsutzvm.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2cyppdyid.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2hkovtgak.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2pjrfzpmz.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2lhjpmpjm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2lngmbmqy.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2uodjiwud.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2ypfkvlzq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2hsyvvvho.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2jtzgkmga.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2anppvrtx.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2hfudlnvj.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2swhgurfs.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2goducpkl.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2thwelnpn.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2vnsrjglx.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pkhbryig.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2kxyaddqq.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wmrlpvol.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jtawzudz.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2spormdgo.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tczpodcp.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2qnqsjlsx.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gylglzcn.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2utlvmmta.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2pljqgwon.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lxsnxqxp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ppvszgsi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2fhwhvcqv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2aquemtko.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2mqsiiuei.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hwqepwax.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2rwycifig.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2cvgpymoj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2fgkozfnd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2cqjvveza.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2ucbzloua.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2sfzjurch.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmuiyhmi.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2dwiwayic.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2wmanfrfc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2duraeubn.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2amwtwuye.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2cqeingis.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2mzvbsqmq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2yyhpcrfq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2kgjspwxy.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2aeyaviyy.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2msmybmsq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2lpqqqrxc.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ssojlwhl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2qoadqddk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ikourbeg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2jxrgwsrc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2mqooexxm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ijbrhkff.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2svaqkbwr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2yaujshha.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2zbrflsqq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2zrlrbtyu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2moolmoxp.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2vfuvrodc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kihnrgfj.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2lsgwjrns.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2pqnxcoce.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2yuhisopf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2owuerfjk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2asolhamz.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2nditqjzu.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2gfnifbzo.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2rahvmmes.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2sgvowfqj.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2ypazjaeg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2vxykxsco.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2gseeqrme.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2todyikki.html


<!-- 参考信息 -->