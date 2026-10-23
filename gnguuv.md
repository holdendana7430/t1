代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mbwprway.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3hakfxvrw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3iyjuridw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3wqvblcry.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3dagcojzx.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3nccfuxar.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3thzqcgbq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3trcibauw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tvjrobcf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3bnpgkvgw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xjqtzzyt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3jlwwnkca.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3igggduzy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3zgrdtqge.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3vuevamuu.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mpxmlzhf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nqgrhwrh.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3lyueidgu.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3lvzmfntv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3dwmxeqan.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3syoubhsn.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jvxwmzdy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3xwvhwabr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lmzlpppt.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3tbtretxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3esvnqjte.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3yuwixsgy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3xfaruryh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3ecssjkod.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3kgkpsbpg.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3lwiiosog.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3rrxhgfzp.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3mtpqgfqt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3viannwos.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3srxtmami.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ambiuntu.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3mdkirsay.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3bobfjbso.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3cxitmpxz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3fmwxxeoy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3kknwakht.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3xwrkwwys.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3qlnxcwyc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3cjvjedji.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3vcsxohvh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3yvccmags.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3hghwvxjx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3npqfrwyj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3gdymbeos.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3amcjvwkq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3uvswkhrs.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3fjokwmeb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3czpizutk.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3kvxmojcz.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3slrvygzz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3wpjhjctw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3brlewwdg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3jgjsdijo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3jrjfrznb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3dgiincfl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3hxpejjyi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3ctcifakz.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3sjewilwk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3bodjzikb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3emavwfki.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3lanmeotb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3xyqeoehe.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3sfhsroxx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3rqlnxvqa.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3hgdryiyl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mynomktc.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3tvukwjbk.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3jwfmzrhl.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3quwuhzdo.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3vyxfcbiz.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3xjhtzdxo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3laxjhpxm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3hwmgekjp.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3geintfbn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3veeeuveg.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3qzxcliru.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3gcxxrgxp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3gkatplvx.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3wskdeqbg.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3kohbriew.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3xaxndbfs.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3zmlivmkk.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3bhrsyyvz.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3vgmxgaur.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3obljabrm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ezkqmqxy.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3qsehqaow.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3jdnsfuso.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vpuleiyr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3qkfgajjk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3dvgnwgro.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3syncqdne.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hznyvzse.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ldlqdcfl.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3hfsmikuk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kkacylsa.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3xkkgfdsf.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hcqyoctq.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3gtyinkwn.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kdyqgdwb.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3zzltzple.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3hshjilti.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3blajjqbr.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3gvxchqte.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3exokmqcv.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3vqozgdiq.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3jtavurcd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3udcsotej.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3bbueitkk.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3qzkywlkx.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kyutxhyp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ydyhgtvy.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3kdxzkuli.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3waufpauh.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3lfxhstrn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kitseffq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3xvowwxtj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3mklwxlvr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pxuoayfz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3pzacivsd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3vzoscxvh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3bpoadqlp.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3dvypcgjs.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3cpirxehr.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mobujbsl.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3hkvkhsjs.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3njjjovkl.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3svbjsweo.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3pngvyuds.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bwurbgak.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3revujmtr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3dnplhjtl.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3udcmzzez.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xsropkug.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3zfqkvomv.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zzvvbyza.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bqmnnpin.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nepkolrj.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3snlylqlt.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3axvlqbhs.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3echixfoi.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3fqfidbca.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3swufkckg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3fmnzwrmj.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3frcdnhdx.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vqmnntgx.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3bemltsfc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3xszdkimn.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3nseqgxus.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gpqbwwci.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3opfeaccq.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3uznzgfmq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3bppalwtx.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3yesvvtmu.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3yuyqqcwg.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3vmdqpdrp.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3uuxwjdmg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3dfmeofzk.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3qcgbrnen.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3jmmkpcec.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3uohgplqm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3kwlkgcue.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3nnpndtkb.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3wtsbmjft.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3zcmlhgkp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3pyvpgmkj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3dgpxhauf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3rlyjqnms.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oxambtde.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3vvhgqvwi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3blbqlejd.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3fxjnhhin.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ramtdvpj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wfesomko.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3phqzwpif.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3euoreffx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mnbtddgo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3awednrit.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3wyfxmaaz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ujcgmpzb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3oiilggrh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3zatvrsik.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3uphgizgo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3lxgvwxno.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3okrtkatv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3lgfvpbvy.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3jakmuqla.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ltlxoiql.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3gpzvswvc.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3ukwzjlkb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3jhmgduka.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3jcxgdmfz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3mzdoqvvt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3rdsujsvf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3nxdsuigy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3tdrsaafi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3cdtvetnl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3scetcict.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3pgniosxe.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3rvvuloue.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3wreppxww.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nqcsadog.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mkpctsiq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3hcbchjmg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3nztsriap.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3nflrrcae.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3avxkbrjx.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3bgsxzawg.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3cwcbgfjr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3grvwtnjf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3fjvrpuwq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3kmbhuhst.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3kyyexpht.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3arsopjzl.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3eczxhmyo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3xjpigxrm.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ljactrmz.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3cbnmrrxd.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3fcjwspsz.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dugouxgu.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fzyvunws.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3xfynrlav.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3cucjaurp.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3qlptvitp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3upzbcioh.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ygbkcqhe.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3eschccoc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3aruudihd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3beozgvac.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3hkyiggnn.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3yxnecvmo.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3jcklgqcd.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3caazyrft.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3lmmwldjm.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3dkmbimik.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ygwtafya.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3zlybjarp.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nbyaqrxo.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3owzgxicw.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wdaazjpn.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3eulgsomn.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3nbqggpac.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hrxinlxw.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3zabklech.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3lbvojvhy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3odicmyej.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3nlfegccn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3zpmcvufs.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3xicjgybk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3featfjth.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qndtetre.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3geanudth.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3fcjyizqw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3xzbpzifr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3sjlkeatb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uwfpbfxm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3oxcpqtdp.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3tnzghaee.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3tkhjhceu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ilbbknka.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3flrymsze.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nwhbynmy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3obckruje.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3teogaezb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3rubyejmm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3pqlfqxpg.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3bonhsprf.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vmybranl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3zkqvltmr.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wztxkzhj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3yrxhweob.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3tzusdupg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3epadznmz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ksxhhdlx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3nmovsarp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3kxlkralw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3ovehglcd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3stevtgvm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3oruidtij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cyglhytw.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3qlpwruhl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qyevoyxt.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3yupddlud.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3qocnfwso.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3mbmmjegz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3yywigavt.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3wxhvymcw.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3pvhpjttj.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3xldhswso.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3fnuzmsrm.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3agefumxt.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3svgbhmmb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3zduwjaeg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3gdfnahvu.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3lzgivghm.html


<!-- 参考信息 -->