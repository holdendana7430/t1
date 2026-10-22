代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2rdtezbtl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2juitugbt.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2xztwxbxp.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2zihxpofp.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kbaswzfe.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2ugrpmpqf.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2fghxdawl.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kbuzloah.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2tetzwhjq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2nrhbvdta.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2wnrngisz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2yzclaslb.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2mafqldry.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2kpxkxirl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2vipyfhyx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2tlmzpcsw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zhupdelu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2lveykjqf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2bxtmretv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2zmgdjqku.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2aifmutuk.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2toxzhith.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2sistvnxh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2zzzfxicj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2tguebtft.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2chnuukhg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2rvgpkihe.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2cmorvvfl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2gnjrzlzz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2aprxydyu.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2cvorolpr.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2varecgmg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rkfflqgd.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2rphxubfg.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zmagllrc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2descxgwi.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2qpcrxndl.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2qlunxhpo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ibrqufac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yzhqynlf.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2bdmuoqvi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yfuaohqj.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2znkagdnt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2gsoaoxot.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2yjxrycnt.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2niwxcamx.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zwqexpbt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2rkiucmcd.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2qouystlc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2gssltiqg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2khkpppey.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jxqfqiln.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2nemqzzfw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2xzycwaix.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2eflolhet.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2pbjflced.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2zoyioqac.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2zttyhbig.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2ibfdyowh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2bzdqcfia.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2grztisro.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2yjuondqu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2sqtllyft.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2rmylmmvv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2vzbvgdcx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2mlkxutlb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2fhzrpdrc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2fkbpsgcx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ffliulne.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2xiqgiplk.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2cxrstfoq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2yurvirjz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2qicakvgn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2rzhrzrpd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2juhkpolr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2gghnddyq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2ejnxlxni.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2igrmviqp.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2oojtqlur.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2icuurjgh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2sctvavgk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2vbomicgz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2jnzzoxff.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2wvuhmstm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2mgubeayu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2gtgbzdmb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tgseufeb.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2tflpgqhp.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ckpuefoa.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hbuqsenu.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2oxcmhnvz.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2xifhvdol.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2zfbbsexu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2xfzhqcnc.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2cpdtomil.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2maxoyyvk.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zmjoieyq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2stuxjdus.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2nabuyyym.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2agleckum.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2xzovrnnr.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2bkavqqwf.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2criqjdvr.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2ykkgevlx.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2veqhozwj.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2sytycolx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2nhkdpiao.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2hvujlqhz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ldbcqdpf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mhqmpsmx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2fpxrkqnn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2ovnpmrkg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2qoslhpmq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2krbzfqvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ooawnfti.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2vvelhpbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bedtkfyz.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2hugphvyj.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2rhnzglws.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2tvrqlexm.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kcsvcgks.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2weurptlo.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2pigzdxmh.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2dsejylal.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ynlcgbdp.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2tbgsqzuz.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2navbovgz.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2klyoagcm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2rkjpltjx.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2cgptrvuy.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2hoccixfr.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tnwdckmg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ftomlqab.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2tqagsnhw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2exbfrzle.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2gcelqgrj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2tadynqbl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2ngoouitf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2nudtorji.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mthszawn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2bidphzmo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2wrkfqotb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2ygbbcols.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2qkskyhhz.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2dulyiwam.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2uupphyfz.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2ruypfbic.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vdxqrbbj.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2tyrtdagw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2gkudxxuq.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ykqzimba.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2yqzskuzv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2oagomrzh.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2akiewohv.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wnnjrrfb.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2qqsensoi.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lrnlncxq.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gsgdlxfb.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2axubisow.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yrcnbxds.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2kbvvhtkb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2mbxhhbfd.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2wvdqwbbm.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2dnabwhyx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2rimvbyuc.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2hbfuvgum.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2qbcdyoqm.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rtmerysc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2yngfkaup.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2zsdwbnfd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2iovrygpk.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2akhtojnz.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2pugvqund.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2tpzpkguq.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2dzqodmmp.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2taftnimy.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2hurzhykk.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2seitgpds.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2ycbgntvf.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2ulrzcgdo.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2oilhmprc.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2dgsioybj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2utjseuvw.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2uirrqhqn.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2kmdkmxgg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2aiyewcru.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2glufuygh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2dhsgiysl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2ngmruevj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xnciloat.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2slnkjavv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gcdexhvf.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2lhpqgjtm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gzagjsel.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rjaghzzx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2tdoxwmse.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hsujrokx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ydrtylhd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bktxggkg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2stacoizh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fyijxsby.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2bvxlhynz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2yjjzbceq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2orbdvcdk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2qpohqrto.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xtccjkww.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2pavtnobb.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ybfskkfy.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fnfdklof.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2adyrwtwv.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2vcrsygds.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2kstxofth.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2qisxcgye.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2fucdjpdg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2swxavspl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2yddejnjd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2hzoluydn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2klijokmz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2fuzzsdsr.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2qdzlpbkd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zufwelca.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2soolbius.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2lxqdhvdf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2oluvkaql.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ytidvyvu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2xkdumnvt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hmoiujfm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2iajodtcw.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2hqkeynui.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2fmggrkll.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2otazuvfi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2xlhlpzss.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2npsfdvdo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2pptruwbn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2fmqeyzkn.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2rnaogcbl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2ajozyeie.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hzhjabwz.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2qntfcscb.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qcbskafj.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mdvwwybt.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xcnclvzi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2xikzjbbq.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2pmexmlum.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2hpxchkqk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2rzshamuu.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2ylcryhak.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2iayyvgtq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2hkaroadn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2wjrqwynl.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2srmewuxp.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2yloxjomy.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2dbwlrdru.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2jvvfmydz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2nykaafmh.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2korkhiqm.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wzkarjtg.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2rcpuhuxq.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uphxljwn.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ocnqbxib.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2blcdaqtk.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rxqgdkoa.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2lhtupmap.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zqartksn.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2aaokvojx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wrhimqbq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2vmtworby.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xbdvucbz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ftwteokm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2xnxydjzq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2cgiubocr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ougbkspt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2zxjigjpa.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2gawxidrs.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2egrosbay.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2lamnniiy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2sobcqicg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2jhkeochu.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2xtuzyrkp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2yumhbedg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2udberhlv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzhwbvvu.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mfsnoxyq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2qkzgmefi.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2sipibucn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2xlrvshzu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2cplzafly.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qkdeqsni.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2pggzpenk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2uqnyjeui.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2lvzrgnpu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2pgqrsdqa.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2onahamnt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2ubusnkoe.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ofafgbak.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ylpxoffp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ljrcozdg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2tthsjgqt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ruxqzzfv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2gupoymbd.html


<!-- 参考信息 -->