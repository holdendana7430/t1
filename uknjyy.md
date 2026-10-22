代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2svektavf.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2gfcvrwbe.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2koiqicka.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tlyyppob.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2snjjsdqr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2zalrnvmj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2nintclkr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2jhyldgob.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2ixfuvron.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2eaapuwdu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2vbokbvqp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cgcddjmg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2hebmgulb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2nrelpaxi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2tswglqpm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2vfwxurzd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2edkxjzvu.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2vsqyycic.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2nryxtnuk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2madvkrbn.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2leakwsqe.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2dnlcprtp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2tzevqkvj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2seminbdj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2qzxatmra.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kjfpdjep.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2wrzxurdi.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2kjryzaqj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2gooxzayd.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2aqrldgfm.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2qeleidfb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2qwaljskj.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2iuuztdzo.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2bvuebgxh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2bvfiidvs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rfeyjbnz.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2oakmztqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2imqfehnp.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2byravgqe.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2nejkrmrq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2rzsodhhr.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2atwloyks.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2zwoekgcz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2ngzsspaj.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2lcsrfnhi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2hjvdjywp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2elixomiw.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2cqcwgued.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2zguruetr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2cnusutns.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2grdvhcyh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2wjwdfxjo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2mtjgldyo.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2ulwmtrfu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2sppcidqy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2qncetvuz.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2lhtyomtl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2mkozlpiw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2tbjkqtza.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2oimgznqg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2hiidwmbl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2vgqyafrb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ecglivgc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2tpdjdmcg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2rrqbdelf.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2hqzjtten.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2zweufgtn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2ukbxagzw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2sonejndh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2kbxrjebp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ldwmzkme.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2bcxegvte.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2xtziwabj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2uvmpuznh.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2hyuifwwe.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2ozprbkax.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2xirtikyz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ioptvhoe.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2hsliicib.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2xlpipbnb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2pgpqmzwe.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2erffulvm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2llaefsqs.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2srjwqrrc.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2qzseekda.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2puippwip.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ktgqnzfq.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2orbcplrl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2rqijpaun.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2akbodyfa.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2kbzxelkr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2widchwwg.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2koheosqz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2qyvohzlu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2yiajdnso.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2myzxhsql.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2beswaynn.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ctkujuqo.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2kudbcdoc.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2sjksdkht.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2jsqlhdyt.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2dejkagbk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2hapwvava.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2xjtmwtti.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jwlmpkod.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jtcmtoez.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2ztqmfxqb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2gopyyogo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ifceaaur.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2mxccgijt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rejuhbiw.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2qjgvjreo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nwacdmor.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2mymdantv.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2rkyhulgp.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2ryhujjlr.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bmgrjqwx.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jiwmiuwj.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2hlhwgcba.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2kyfreyig.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2lmneukaz.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2htpwchcb.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ldjsjjzn.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zinkexju.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2rfpkgqut.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2itttfwhx.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2yirkyxqf.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tuvwsztq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ieodqwvq.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2yzcrvaym.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xpchylqv.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2fpglrwqa.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lvtrraje.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2gphxtbjt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2yvxmgein.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hujmgtxp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2sgvabefr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2cjluaydb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2flgggael.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2koxyaqea.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2loqdecse.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vwdwdenr.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2vchxxwcc.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lulkmnzd.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2plvdzrcz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2solaxmzx.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ceyplceh.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ifhloxoe.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2xohnlhpj.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2yzbauzlb.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2plinsoiy.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2anvigrcq.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zlefxyxe.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2erxuseyg.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ozyattue.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kvcevvlo.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2xdruparp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2cxydqfqd.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2korvcfhn.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2bdudshjx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2itawliri.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lkkwkupp.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zukjexbi.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2lfjtfawp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2wpqsduor.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2zpizjbqk.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2jluidpei.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2vnxyodnr.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2vlxkkajo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2yqmttsaq.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2axenifdn.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2pobvhsdb.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2dqmbzltm.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2zrzifsai.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2mevaiwac.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2depeajyy.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2kkuyvwas.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2uiiogabh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2tzdpormb.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2pyvaqhrl.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2zzqnjhgq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2tgfqdbuo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2hxgxywfe.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2xgghqvyw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2bffqurne.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cjavqjnr.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2hyeuvymv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lveqxemk.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2oksfadta.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2doxkvwyg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2raflobsx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2cohllsiq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2cxzevbfm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2aiicjmqk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vcbpmwtu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2sqhuhztt.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jdprrbtx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2mitqoryv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2bdzpsyhu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2juigaufe.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2qrakfyec.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2bpczmbzq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2fnnhuhjt.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2tpmaayua.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2rvpnrucc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2knrzriuy.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2dsqknzhh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2metpyayn.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2vimbsezj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2yctaysva.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2poedllpp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2rbweokwn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2yslbnzkc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2uidticsm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2nsnqzftv.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2jikkgazb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2egeirhsh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2doocselb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xkzmgqjw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2aefkpwaj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ykmjjjdu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2qvnokmrt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2wstjcpcx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2fbmieevi.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2kepjtwnj.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2imvmsvey.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2quwxtdjp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2krzolmcx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vflsdygt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2opvixvhg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2frtklhgc.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2cxxjklsh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ckbrnoxd.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jbaaisvb.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2bukgpkrq.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2tdfiufln.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bdztysoy.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zgrwcxja.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2jnqmokdy.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2zctvdgbj.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2qlaeconv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2skhssbkg.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2gagrrxqu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2ncixnwmj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2euxmpiub.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2atoiloyc.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2npgczzva.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2rkuitfcf.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2fhujsyob.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ipqqhtnt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2jeujfqsj.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2wxftkmqr.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2slvzldkj.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2ysqkliql.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2eumyepvz.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2azghjfcl.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qvaxsyax.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cjhwbffw.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2pleejvdd.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vgkpdptx.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ufwypdue.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2hznvzsci.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xhhcyult.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vazmghhl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2fbxwsgje.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2xzcjneuo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2chgxgwyd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2vlukmple.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2jmryysyr.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2qkvuytpm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2ryutlmee.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwdcrpjq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mfzvihzu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2wwjgqstd.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2hcmxnxfs.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2iqltinzc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2bkukbqek.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2wgaymnrv.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2xyopfxft.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2sztgfbzs.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2kudjumwc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2axsxkydw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2batqzuyk.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vkmbizdw.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2yaxfrmye.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2yvjqsdhg.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xqnroczd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2jigecwjs.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2thvgtvks.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2jpyywwmq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2vozkxzxb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2vzdclvxm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2wgkvzjyk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2kunxdrgq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2vxzpzadw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2mmyrquxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2exjrnhpl.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2afaohzif.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jjrhlbrl.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2dkocyyuz.html


<!-- 参考信息 -->