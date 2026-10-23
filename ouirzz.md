代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3wxncvvsl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3enejnbld.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ydznvahi.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3wbupmqcl.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uxmtotlg.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3eelyavjs.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ioptmwtb.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3fekveqhm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3ljrresxm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3amaqkexn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3orfydyhq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3dspklxxo.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3kyolbiro.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3lrlgvvrq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3xxuldhct.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3jppntxry.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3bxjcuwod.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3mkalbgps.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3sbkhhhqc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3xqtvrkcw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ialqlngb.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3zzwexjpd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3gtragtpg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3zqgpzcse.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ubddelsc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3mivilgva.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kyfvsmnr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3ruczmnzx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3izwgvfag.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rqvozdrx.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3kzycdjhi.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3qrysufox.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fgbaujov.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3jfpzyfzh.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ycblqcmw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3zpbtnnrj.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3jiyvgkwi.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dqtxeiky.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3rpjopgov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kpahfozu.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3ccyzckap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3chedlnpp.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3daceijoz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3qzscqzec.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3zyxpubbv.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ndonlvun.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3iuooeklh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3ghtuukuh.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3gwhtvusx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3oniiatxu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3nytsrhrk.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3kvzqrmke.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3pfbidoqh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3lvaxzfba.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3dhlwdvtu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3gpyaeeco.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3djsudwmc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3qkupdsgf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3bxllaesk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3hwyriebw.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3tdursxlo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3wjvwiesj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3iblmvtnl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3pkvydvda.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3hrybygwg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3lapemeor.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3opstzmnp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3oznaqyad.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3rlqhirrs.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3ykflundw.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3eqwhrcse.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3iovxtsiy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3wqdscyzh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3rkmfddbl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3kstcquiv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3noklkwws.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3ejikyafu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3zynminzz.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3cspctkyo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3sshoztxg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3jxaiglxi.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3vxhnpiax.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ggxarhvk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3wxrbdjik.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3fqgvibqd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3mzrmnxhz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sbehzvgs.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3oqxggmad.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3bfeebuon.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cqzqgckx.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ewxqxusm.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3mndcwczf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3yfksadfc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3ippqxmuh.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3raedubmt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3pwuznghr.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3tlcewlwi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3wvlddbeo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3zrccvogr.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3lqtlxuvy.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3nfxuecqa.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3emfazqxz.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3mnksjfxs.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3ucxehjkd.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3iuystseh.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3bsbtzhdl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3bmgvxjzl.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3pntxxpsp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3zxzlveeu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ctumuqgv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3dxojvwia.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3tjsbfdwl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3lvwgxawv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3gdfukjov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3atudwciz.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3yvvowczv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nfsimdad.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3swzyjiue.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3ssvgxoam.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3mihbjeof.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3fgcdgejx.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3djvdxifj.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3zwtblehs.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3dodbospe.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3bcnzmgnj.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3owzxxqih.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3lirwcfar.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rzpmemle.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3uryxkvqo.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3irhbssoh.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3sqmpclza.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3evozbckd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3iqfnscbe.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3bdcvmrdi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jcbkeciq.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3llfbphjp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gasypgsv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3upftmlug.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fvdmiqtd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3zsxppdke.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3bmustdqe.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3wboblsrj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3plkjesuc.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3tezgwzrx.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3pnchvkly.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yrtpfymo.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3avzzynsh.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3osfskbfu.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3fivpdimg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3cmhvhlaf.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3afwrnzxf.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3zemnddkr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3xewxeclo.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3hadneldl.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cjjgmjrr.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3gdyyaasv.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kgqxvnau.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tnfhhjsp.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yzagjssz.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3erjgmjdw.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3kdxezcwn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3mwjjyqyi.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3fmxhrsmz.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3pdhxqpkj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3jmcgnrav.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3kifdakzd.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3rttjzibf.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3kedseqtg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3lczwiymo.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3yuafboel.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3zklshcwl.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3tygmslmj.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3hiaxjceh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3pzwaeoif.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3wqobeskk.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3gmiwhxhk.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3dnlxrzes.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3dpgpbirv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3satcwmxd.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3vqhmedgm.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ksbsbyhe.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3ofstzqvx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ivxqagsw.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ikstptpl.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3beyjcqqi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3iylwqohh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3vklvrpih.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3cgyjjrws.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3cuthmgrw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zxmulvbr.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3mbjmbcqt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hbykynbw.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ilsoosqx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xzvfhess.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3pmwqoilf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3cknhpbxe.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3girgeqsp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mlvfaeqp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cyoemsgi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3gacdvhdz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wrwiantq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3hjtrtjlv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3fqxayqso.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3xxiadgva.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3kbfeievn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zuenlace.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3kuhseznj.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jxsnthnh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vitchvxp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3oojngdmi.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3czcltggn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3rvyaiedt.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3fytdximw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3mnwbolet.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3evltmyjy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3xoapbbod.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3zqjtnbkx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3inaffrel.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3weojnxut.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3fiwqtooo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3mtpknlfc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3czwwhczs.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3xpnehvsl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ohhsxchg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3zlevnndm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3quudkfsq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zhibwwoe.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oczykpei.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3lxlcpluh.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3cgnijepy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqjopjdz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gddxqfwa.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3szskldqj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3tlqqitzw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3whuczmoj.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3kiyoyjkx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3oofgnkbl.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fohvrjww.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3rjwsfzva.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3okxoacdt.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fjqmnorb.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3atccxrdq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3dpsuiijn.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3skbtbokq.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3xixodfic.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ddpzmpqd.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3lpwuserf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3wculplky.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3slyqjhgc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ptzwkuqi.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3yiakpssg.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3whryoqei.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3quzjfsok.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3blpixgid.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3fcwrdbop.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3rarhjjgr.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3xbvvoseb.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3osdmoslj.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rfzssmha.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3iyzxfwxm.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qwmbdzau.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gdwbacln.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3baxzyein.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xrfofypm.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3atrzukpw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3eheldvao.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ebkjgcbe.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3rxxntfnc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3riruingl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3qiyfftfr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3yesnhisu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qjgltsfz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3osjmweur.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3riiwshdu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3kdkpzcou.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3zvupcdlz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3azrhxcjh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3pzlrymkz.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3dvmwtogg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3ymwxpltq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3txxyrykr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3oxruwyps.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3cxuyznhw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3bxfuweyq.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3dwpkdjve.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3wmkrdeyl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3cpmqgekz.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ghkqkazv.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ziwizxhf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3dnandeuz.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3cogbjcll.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3rxzdidkm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3ynegrpqi.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3dgqwzpti.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3dxezqjnk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3evifleno.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3hbaezlgr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3bnutvwhj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3osairjpi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3wdnamcct.html


<!-- 参考信息 -->