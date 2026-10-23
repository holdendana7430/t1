代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3frdeoago.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3krhecixu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3ogrrecvg.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3htuykntd.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bjbtmprn.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3lhllbynq.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3vplyzhmh.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3idgwgwbb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3tyebndyv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3xhwrlwlc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3phfawfia.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3mzdktfuh.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3uoaspfyn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3jxvzdiwa.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3murebdoj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3nkllcxzj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3ptnfcitq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3uzgqrpbp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ogdjcsyd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3jmaaleuk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3qshynqrn.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3mvtnclvf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xilvkikh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3arioanvx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3gnzuqqzy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3djuyxfkz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lbpifmmh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3nlgvyqpg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3nrvobxmk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wmfjwmua.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3fskctqvm.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3ptpnsnzh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cdrdvawh.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3tbgeivsb.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ozmhfxim.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3fcpttvel.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3tsvvoolk.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xrvclkjp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3nadejnxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zzqseojd.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3mwqgnkhy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xmwszkay.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3onoszbfv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3swbktqfu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3bnlunpsa.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3nohhskfn.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3mmghhlif.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3vsklqlti.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3yiqslcra.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3teoxvmzu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3cfdthpqs.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3evrlitjo.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3kcjzdley.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3boogofsh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3kksbuxll.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3uazgfhoa.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3imfvmroo.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3mfrmlcox.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3fyknrpqs.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3nijvjsah.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3sdiymudo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3zlofocgc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3euzvjpjn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3oquiaogo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3jsdwftnl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3gkagvciz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3abbkquis.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3gjzwczwk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3blyusgju.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3vhfbltgu.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3nmzpjyoe.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3zngvdmrz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ygkomoxw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3hrkopxuw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ndzoeuza.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3ibczshvf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3fwglohnl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3fzewiuhc.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3amyualjp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3azxylubr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3aewgqoxp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3vikbqmni.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3umwqwdty.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3ovuiwxve.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3ygiwfqkl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3irfkbxez.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hsblpnkz.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jkqatkix.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3netouwio.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3yfeevygr.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3hffkmslw.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3lctnaplq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3xlljzkyw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3prdorwmd.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3abbchtuy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3nzzhzrck.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3zlqitmla.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3bthmsxyu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3helqhrrw.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3hpoorhea.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3agyiipng.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3sgendddk.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3jzspmrho.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3mwikkyhl.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3lhgniqcy.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3jbjsyrwp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3fypjevru.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3junrfjuu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3aqbtafws.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3zkididtc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3jgqmzulg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3zjbbxnty.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3lzjqhtxq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vvacphms.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yckdtsju.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3vkwdtvct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xkvmtirz.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3rngtplst.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3kxspvgcj.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ikprjfmg.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3vfgtvgda.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3chqcpfsq.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3artyuzpi.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3epzuobbf.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3khjafexn.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3mvddzbks.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ylybcbiv.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dhnssgub.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3befbipui.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3qjklqzts.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3wrvrumxf.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ovbktzgc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jxsidarg.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3mzumgima.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3sdwcwsoe.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3mtyciahf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3unsdouzi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3kugulvpv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3uohsxsbv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hufeqbgg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3dceflopg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3bdaehtxw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3gvmlgdpi.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3cwlkrxkr.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3tlilbwsy.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ztjltapo.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3ktaguljl.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wvphyqzs.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3rqgnlraw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3vlciwtrx.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yxfqcihs.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3hevfrhhl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3wxjcxixc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3bcxhpdyw.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3iajwninr.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3pfdqgsyq.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kmgvegel.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3aqapbygv.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3exwoqsgz.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fhboyqxl.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3mkwomiji.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3pbcxeose.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3pfbpuuxw.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3cjpzwnjp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3cqhdrksz.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ohyuqkmj.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3eopqifhi.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3igvdtzaj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3azgjaodr.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3semjtitn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3avxgigim.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3dbsnymkk.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3rzpvyssm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3tirgnqui.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ajzhyciv.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3mvxlqssz.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3nzoiqosq.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3nkghgykt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3soktzppg.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3iqzmryzd.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3fpzhkokr.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3ixepaybn.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3mkrwksia.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3xcjtgrtu.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3qjmmrmlt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3fvcxctdc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3ehatocwe.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3rauvvoqz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3jligboyj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cbmzbwkf.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3yxzoecbz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ivyypynl.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3zpcrehyf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yiqpraqn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3kfuzqpru.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qybexqtb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mkaihtau.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3aofeaqle.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fkmdyigd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3tbzfiknu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ltebspfj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3rtprttax.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3bfbtwpoh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3eluzmhpo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3slpjehbu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xikldfep.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3gcixstyy.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3boqukiil.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3jpqnfrew.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3alzjofxg.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3urduaedk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3kljqnxgl.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3xmmvdedy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3fyuqzxiv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3bbjkvnub.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ubopbczv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3gxojpxde.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3pojirumq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3eimniclu.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3sthpcozh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3pghafjzn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3enbatgea.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uwwanrhz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3xrlszqrp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3yswzztzy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3oanontjg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3owzfpype.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3enfcvodp.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3xbqkshgl.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vucsoglv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3cxkrsyuf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3liwpjmsw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zurkqvoc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3xpafgyrw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3qcywoxxn.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3dqyijekx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3qmtvftlg.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3yrvxwplq.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3hdbzyvvz.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3lrrtdtuu.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jpiirdmr.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3obljtcoo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3epygiljr.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3dcmevapj.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3krhtuovs.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3htfjtzje.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ybjoyobk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ajrgiuep.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3sjinlviy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3xinfiadg.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3eabjfofp.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3sgooifmz.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3jluhttqx.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3vriugejp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3ydckehha.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3rpflrhxx.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3niapkhou.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3lfwzzctg.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dosdbyof.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ujnfvglk.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3sumpekae.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hrwrjgtw.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3hsklcocp.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zkkoszsu.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3rmvpeekh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3fuasbjwc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3mcaekaqc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ivaatfvi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3oewemsdi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3yqqoclvs.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3vnhxyqih.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fvyyyyor.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3hhrrscwc.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3ilspshmt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3pdnolvvi.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3nrrcdcuf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qhlspgxq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3dmofexea.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ieenjgti.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3xahjewtq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3aizyomhx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwidqmom.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xvuvsidh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3sekejmag.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3krrgeeed.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3zxnjhmsf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3qgpazswx.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3sgzztvbg.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ukimhkuv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3fjqluejg.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3bkdrqcrc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3boxiuids.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3swmyrhfy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3mflgawxy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3omojgbpl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3lsmoaxjq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3jfbvbucy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3atgblhij.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3xjfdpwny.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3unsvcgxw.html


<!-- 参考信息 -->