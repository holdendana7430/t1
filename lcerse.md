代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3pszlyweg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3scaxfzfi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3mpdrnjfh.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3outucuru.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3etwkvsgt.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3xrjulbfk.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3goefijcq.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ynnllqsa.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3jozmonyw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3suoscvok.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3chfjcjiz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3fqqduluf.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3iwiqhcas.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3wrspbhne.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3mfhrjglf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3cxzgaort.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3laeetvew.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ngxinufq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3uchfirto.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3kfuygemc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3thvdavid.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3fmqaazcy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3aqhqdwem.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3oqtmaceh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3inbjvpfj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3roisyzxw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fuqxbelm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3jyabeoid.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3uxqkbgjy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3nkywxcsm.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3gedbraaa.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3udykwzgj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3tfuxpvln.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3rxualwgj.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3mtjwpejd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3stadpoph.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3jgxhlgwl.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jswlaxpd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3qzojsxlr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hgklgyhn.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3zlmxnobv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tlrsyyze.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3ymjhyltj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3uhcydezf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3okgrmxof.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3mwbyhhwa.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3feziljnh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3jzorpbqx.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3fqrzakhs.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3toianrjf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3pvhowipi.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3lnfdjfjo.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3bsagregm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3ngfjtaze.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ufvomomi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3mvaxzlbl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3trlgdoak.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3wudqcnbl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3ctonreol.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3vrppgryu.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3rrgdlutf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3zxkckcvr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3tbzhtwba.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3eozkuhsi.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3fxthsrse.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3uwnnpdeh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ospbxfdr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3csuniafn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3kwwomgyn.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3wvhuspoa.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3dsdhpiuc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3spmqyntn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ogfacrpd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3llqfzyyo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3jhabzeww.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3hdjtvpzf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3qvvwalcz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3pttmfpdk.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3vrizizrq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3gfqhruhg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3oorumxwa.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3nvfqevxq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3chrcxaoq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3tkehmxau.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3dsyddnet.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3gutbjxuf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ulcwdfih.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3hfezkoaf.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3rhwaraml.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3aqhcvfam.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3esukyamd.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ebrbmvfw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3hwnrjygl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3qarzajoo.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3pfxfhcpu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3kbcywrun.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3rvincdeb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3ytuymuoi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3hvtdfheb.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3nogqicds.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3pxlcjthx.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3pvghzuyn.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3jakevvcp.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3ltzvewrj.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3rtyimbfo.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3pshpivvr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3kpycfsau.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3rosmkpta.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3prrnchii.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ygxmghlz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3nbqhdvwf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3ugxsefvb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3tdnuailq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3ohhpfzcs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fsdsyqcw.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3xjexyrun.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vlhkiwuk.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ynywucqf.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3vpugzpue.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3urrgakts.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xqkwccny.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3mjigdkbq.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3fpusxjus.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3dmrjwlty.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3cxpzvsem.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3lzkeqivt.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3uxmauzlo.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mdgqoqas.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3gigylelf.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3smkuwgwg.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3wsumvvyj.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kqqbpwsq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lkplktkv.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3dmwrruwz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ggrcnopk.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3whvsndof.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3cauylyrl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3xeoafvcs.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3mylfoxsd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wnjdgnqd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ccaxoaio.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3twvkflxa.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3afnktaaz.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3jrpmdcxm.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3qrnphpkd.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wyzjsnrj.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3ngzeodyx.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ryuuldgu.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ppnmymtz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3bsqjezup.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3mvpzqqgh.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ddpyjmxo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3xphcecxv.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3vyfcrnxp.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3svqehzcr.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3cjovwwgf.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hzxqtymb.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sfxwogkd.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ezxglvty.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3isolhbkm.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3ygrnubhs.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3qrzzyikp.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3vbsmbkqa.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3hzsaikqh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3dbpxmnym.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3eulfliux.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3kpvhwlmy.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ryrtvvmu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ckzbasup.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3qzntqjfa.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vyvhdfex.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3lrzyqint.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3frxuyxtf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3rhzktxzr.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3qnuimibk.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3gtkklopv.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3licznrkr.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3wycthyhk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3gacngfmp.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3qyrkdtmx.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3mjqavunj.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3gnjglobi.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3vkjmfnmn.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3dbjhnqll.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3yfasinyy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3sabtrvpu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3wwwdnwkn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3cuqknkyf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3zoxvyzcq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3urehswcg.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3akymcxrh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hbjcuewc.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3tifgayot.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rkknwzhh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3rhduqoxd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zgtmzxck.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3fyvxlkkh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kgqzmmnw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tcvhmnvn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3qbrnglaw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qgyleeyx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3mnduuefa.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3pfdutbzp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3hvckwlul.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3oneqzzwp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3lqhovbos.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3jvafnfxf.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tuxqqgqc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3vleffauf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3mkbchemu.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3mvzupjlv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3ytxghazu.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3ahmxecqf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3dlzijgix.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3puunqqhj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3dzmvcjzc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3crnuvslm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3brytnzpm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3hdardyja.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3ygnemrul.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3iqedkwkl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3gvhoixuu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jaejeltb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3agzundlp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3huwzqcfc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3ceanvnpc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qwgkcyzn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zffdorgw.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3vdwpbdou.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3qnxdhdos.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3zcywlwnu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3xxcqokvd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3uekhogff.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3bjbhjdje.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3oczslbsf.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kkuhldmk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3xigxahko.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hphoivcx.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3pgdnpfmf.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cvbzcsze.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mrjevlgq.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3yinzkdcz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3wzrjegjm.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3dskybkpd.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3bbttpbwq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3laksoxtv.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3dvgokzhp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3cshsihdl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3xpctgcxi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3ogrdbejf.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3anlibkrg.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3armwzzhf.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3nbzmijoe.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3uwbsuxnm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3thmdyurd.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3sazmgqad.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3loqxynyp.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ursborsn.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bburfkyy.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jrspdyfl.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gqgafjxv.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kowssoxt.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3riurxewk.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nnzzqsex.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3lmdwzivo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3jpxvotdz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3uwhbuizu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3yjueshmw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3xzbofpms.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3euzsnydz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3knrwaezs.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3sakmmztn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3xnigpboh.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3xreblsmo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3qjxhafvo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvsfvkgn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3sputwlid.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3oaosvkhf.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3lgxgtodq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3gkslkfuq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3jtttsrqp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3wqecxfdp.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bkartjad.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3lmkezrka.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3khrggodx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3nbiggpud.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3zdykucue.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3iznwuvag.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3movbjima.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3eiocizfq.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3tdbjclar.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3pojbsktk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3gjwdsnfg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3fxpgkgad.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3qmjxbtbw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3cwormybp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3gecpvkpw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3clquupdu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ilqbbilw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3jondwlwi.html


<!-- 参考信息 -->