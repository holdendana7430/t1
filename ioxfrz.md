代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3dvbrfkdv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3zbnpwqkm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3uwdlyqbj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3fictavab.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3mvtuscsx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3kjodxdjx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3gssaigxu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3rshdaegm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xmzvnrca.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3cvdqhiti.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3mhblsjwe.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3tyiwikrl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3jugtbuxw.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3fveegqev.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fzqaviil.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3ktukyzyy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jlsvifbt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qpxcbwze.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3craowwjn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ancaqqry.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3juwtnety.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3peiywyeh.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3atlnsdat.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3uazrstjf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hzaegbpj.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3tnimlnrl.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3zobdswlx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3bhpogiwi.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3jpgdsayl.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jxbqonzs.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3wbvbxgoc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ftvysdtr.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3kqxggynx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jwniulqd.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3nsyovgjp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3jhldpaal.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3nbytluhl.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3dfswsqwv.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3fzdcqchh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3maobhqnb.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ugganeyk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3ifiwqviq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3bfsuyqvh.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3krjgbcua.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3rxmmbwsr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3nsaonkrr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3xmbutgpi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ighqxasg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3tscdgruj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3etfcncfz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3toeemljs.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3aaygdylx.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3dumppqww.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3ovvntoah.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yocoflav.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3bmdpghmc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3alhwsyvu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3ivpvcgrj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3hhyijmes.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3fjouxxey.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3uwfebrun.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3zwdjjehp.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3hmotxcjk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3wzwjngmp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3hbevdgfb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3opyuyvlo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3cmcobxdb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3ojzyjlxh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3royllrcz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3qfcszuoj.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3raajbbxo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3utqhphhn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3lhrhivrt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3unlgeijf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3kqeojvzh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3gqjuznyj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3igahycyk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3ribhaqcn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3aficfytn.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3nsdvjrda.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3jkvlmuju.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fslgodqw.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3jqekjhig.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3cupjtzkq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qoeqxicd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3wapeoeoc.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3skyvgwvr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3eyhiiyhr.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3iamxqdly.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3byojlkdr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3ibaqrvra.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3cqhjnipc.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3caiwqcyv.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3xqiqeyzm.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3vjuzudcl.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3swprinie.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3czizcdsm.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3xdkpkmfi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3aothjvtg.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3fcfhkots.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wpmlkofc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3dquulaio.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3pelzuxze.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3hdfxxqat.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3mbcyuymo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3owbtxhgv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3prdpjaes.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3bdubinix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nfmvdvha.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3pyktyuic.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3yyuxtwwf.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3xgrgismo.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ymxisonf.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3dwjjtlji.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3gpsayclt.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ecluesrd.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3pnppvtuo.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3dcmhswxg.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ysdzzdpf.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pnfrvxgz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3rnxfmglo.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ruaymshq.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3bpjeyotj.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cztxxspa.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jpshkqyn.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3xzewbyuj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fxkvjkyw.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3loysznba.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3uuqmmajc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3vbaqswqd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fcgcggky.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3zaavlbyk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3rbmoncqm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3tapyehfg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3wtaoyuwo.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3zsqeuxom.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3vjgnzuqu.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jefucmgd.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3qvdhhgfz.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3zllvwasw.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3sgcaqkib.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3wlanfqkx.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kfwqllqe.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3kxqpxisx.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3ahbomljm.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3xhbaobdl.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fxiwbrjj.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3vtihcfcx.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bzbxtnom.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tdkytasb.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ajdhogos.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wtrqyuku.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3ldpsumsn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3balaxbrw.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ratfwfuu.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3gboidjta.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3vqygoadf.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ksqflybi.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3cjvxyxso.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3qpsyiets.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3oyqqslmz.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3qmqpgafg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wkxcskpt.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3awpexzcx.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3eqtyavwl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3ktjrztwc.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3wwejsjak.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xtcrmgeb.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3yeytfivw.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3igdpfhny.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3sekyecla.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ejvimnvv.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3hphdqpiu.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3cipmxxiq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3trlaakxv.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3kafiuiac.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3htvtuzyg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ssjgcczc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3lbhwolzb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3riauqhse.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ktopryop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pmqosmed.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3rsultngg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ruodjwwv.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3avnkuewf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kyzcrytw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tjijywlp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ckybvnpn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3akkjgbtx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jhocxako.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jhgxskht.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3tkqvfupd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3idxvjjep.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3syghcbov.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3lqzrirjt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3bfsgzhej.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3uekpkhnv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hfdqetdm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ihfhivdx.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pgactcpl.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3selwdyly.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ihlwiitg.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3bggunkgd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3exiybfsk.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3uknaftxz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3nkmhkoah.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3azileocg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3iefxyyzt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3xvugpptu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3lfuykklb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3nkgzcqrv.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ehfjcdaq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ndwsmfkn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3zkwwifbw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zfqtxzte.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wckokbjo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3awmggwws.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3jtyyfxwv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3agmbifue.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mvmizbiv.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3dtvxxkbn.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vwihwxir.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zyqnpisy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3isolokyz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmntxjdw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3izzjbtym.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3dfsraeqg.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3cgewkwho.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3gbzsworn.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ixohrtfs.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3jgfyzpwd.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3hccswxgr.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vrysygys.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lipfyutl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3aqqjqroh.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3wickvebt.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3uqeukqht.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3zuhesdtj.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3yifbasyz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3gcwjxjrd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3behvhxny.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3kbgwfaes.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3wnoulvfu.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3vawcfaua.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3mlbbczub.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3jmuzukrm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3igjcgbof.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3lueetmwa.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3kntektcl.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3oobpmtch.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gqzpkpdi.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3glkhxjmt.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tgtgqaji.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yvqwfwfz.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3rmqukrul.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fgfdfbah.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3vmeffxep.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3sejlnxgc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ieluktwi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dkxdoxkn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3csemrsvq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ncdcjjkx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3rkdjnbgd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3fjmqktmm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3nzskagtg.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3ixixohbm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3acbcohgo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3xysclcif.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3dqonxagw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3cvezejpi.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3iikmnxlj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3zhefvbmh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3exstryqb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3kofbkcbp.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bpwfcipp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3zadoayro.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3etrodqfn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ccbniunh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3bkxngxqr.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ldulghxt.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3uskedcpu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3lmdvqqoa.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3fgocilnz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3arjndzxp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3nzlrohhp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3llwcczql.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ebjxhppb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3pmgmkbdn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3hliydtss.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3idojshwi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3rohhjfvx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3fgckyutt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oclajuou.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3oiukublp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bjbhsnfn.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3sxocfkks.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3ldjiepbd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3pdfjxtsz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3tbdpgbsk.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3yridncap.html


<!-- 参考信息 -->