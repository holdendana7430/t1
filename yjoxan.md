代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2zsemdzjz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2guqbpdvv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2zwrxoqpn.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2vkghmbod.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2lgtgycsq.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2nqamhgru.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2vatcffgi.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qglcedhp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2eqewzvnm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2rmibcokg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2cxasbtdh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2yvgtvuoo.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2ropkmgkf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2jkppdkpq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2nksjnlrx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qnnlsjav.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wksepcbo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2jovmvmzd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2maqykrpf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ztbucomq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2xztfrqhx.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2yfxutxls.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wtvdmzql.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2yvrdrcop.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2uwunlnqq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ermodqqp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2papxdqtp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2jumytwcj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2fbdredwg.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2cxraesiy.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2cqyyozzk.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2fogwtmwa.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2tpfnbsyl.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ewvearbb.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2wchspgwa.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2cmohltvh.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2fhyamtzb.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2svbuiuwq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2txsjhtmn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2omsonaop.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2hyaconyj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rondkupr.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2bawgjovu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2nwrfyier.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2jbmwooli.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2vejacnwu.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2lpbubdmi.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2snudnazl.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2svvrrogw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2tojeugwk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2dzcicwxb.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2twntcmxq.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ynrgeryv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2nirovfib.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2jraertsx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2dlavouuj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2snodjsrg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2qzvghhdb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2kqaavmwr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2tbbszgbl.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2dypxrylp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2ptyetmhx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2cmqvcscu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ekgrquov.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2vnfmjbqj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2iovfgyqp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2kswnnevi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2bxnadjtz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2oxioywcs.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2lbzqymyc.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2iccdwuqm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2bcxsxoyn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2xefmotxu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2lcyeumzt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2zbcozvgr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2gfyyqkho.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2dfvuokhc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2mpycohbg.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2dvpjqhlv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2akcmcard.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2ixzjwmfd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2dbmcwrpm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2abdyfrml.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2nvgcjsvn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2godpudsg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2nwcfuzon.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cqsnfifi.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2bakxyzgy.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ggfqymmc.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2yncvscxe.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2eloqvdsb.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2iisjorsz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2mdhkhggk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2tyfuhicn.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2vjkjwucw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2rdodenky.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2cxyjqfkr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2wqpjoifo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2bnyovklk.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2lmpgweuk.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2qvhnbeeo.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2xvjulnny.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2aqyghcdo.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2bcjfadak.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2wnuzvlqe.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2llgmmawu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2fsxxlljm.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2mwtkvjdf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2kdvkdplv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2yfnoslep.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2hfajtimj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2tqljwlfq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2hqfzctxp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qonfpbvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cuapwngx.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2wymqtrps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ryafmouu.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2mhooelbq.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2myelkspo.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2ehkrujmi.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2klceeeep.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vlxtvuhp.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2msownzhz.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2fkhpsucd.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2uqlwtwyo.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2yrnudeew.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2nqsyhilv.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lptfymbz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2jpzolmzf.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2vijbkhto.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2wowlfejf.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dwoljcbo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2buceqyeu.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2hrlhjwpo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zfsedywr.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2hrvfhjvx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gjhlktnk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2jeupsetk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2achpzkfq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uevfplfm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2hdgclnqm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ewbtyxvj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2mfqwtwhp.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ncdasble.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2rpziscde.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2cnqntedo.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2xtfqwoux.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2khmgjyjg.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2xoxesmvz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2sfnzwyyk.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lrnjalns.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2jnubrflf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2gaokwoph.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2hcalvjda.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lzmlykqt.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2owyfllqs.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gdjsdxxa.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zdssxqam.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2forxgjon.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pvrtadqk.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2jqyiuips.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2tjslublr.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2qgpsfkwe.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2fldcnzyt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2htxxnueg.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vjraetba.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pqnyjwdv.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2zgkaeyur.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2qehepkkp.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2iuknvnag.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2mmfhuxpt.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2gokvbmwx.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2mtfauvwg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ncnywjis.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2vkjhpcnj.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2gqmruslt.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2uzphvyds.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2iprlfnqi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2hhryusdi.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2rvztdizd.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2fkcpjcfz.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ivaamomb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2nnojveeq.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ylaxbdam.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2hpdfpixt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2jbjwogjk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2lbgemqrr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2mawjesab.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2tvvdkpii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qjqinegh.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2suknroiq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oxwofcrj.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2uihsnvvc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ecuboqju.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zofizlos.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kuvocbfu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jrxbctuc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ctgdvvsc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pjgiutbi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2nzangkej.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dpneeyvf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2efteqyae.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2qrjqbvmj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2hjycxqaw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2qdcsyvfz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2kvqvhgdo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ktfjaqwq.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ucloshfr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ijuhciec.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2nigqvrpt.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2vadfhsqw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2rnpbkkvp.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2kcbezeyi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2oljgcdlr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2akhmbzxh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ffexgmnk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2fzvficxn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2dtqxklwk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2alqwihvq.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2rktijmoo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ataplqly.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2uulawriv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2nxmysfxe.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qhkyuhgj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2htzjllrn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2axqsfunt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pbvlhstd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2wradwsks.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2vgvpmmij.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2wurbauiw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvpotkzt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjrkqlkh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjngpcfy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2utwaoqrm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2dhbbckjz.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2nnjdfgyn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2bpuwbdyu.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2hsawhpvz.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2fesonfzq.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mhmynvaj.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2oyzedrpy.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yhsxmyfp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2qsbpwwrn.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2puopxrgu.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2aaskrgih.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2zjpwzlbj.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2ogxufoid.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2evxbqqdk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2fhzfeggr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2aewmgfrl.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2fseazkqa.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2ovbvydgp.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2ycvqxjly.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2nlcmduey.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2zodnjngz.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2ueaeidyl.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zeexcykb.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2nhbijvxc.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2swbsigsi.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hgsrwnzk.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mfqnajtv.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cxrnsxkq.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2dbroccte.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pyndweiq.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2amcocxio.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2virjlmrc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2uwsijmrq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ihvsxzwu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2tolwztll.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2nicbnvjs.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2ouvbdacy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xacpagnb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2dhjgaktp.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2cbpwvsfh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2eigeddlu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ckvuitbu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2yashxmos.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2jujtlhmp.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2qqyxixtu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2szdzzarg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2onavgnwq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2mjunsgpn.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2ofpcakpu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2daopgobn.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2qkasicmf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2svprnufd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2hvnnyimu.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2lnpzepbi.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2lcghcbmr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2ishjsfpv.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ulepwcxi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2dqrzihml.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2cgmyurxo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2oeqlqoos.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2dhghpdju.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2nqnuhxup.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2hbzyhciv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2zvxpypoj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2lszmtudr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2pymfjrhq.html


<!-- 参考信息 -->