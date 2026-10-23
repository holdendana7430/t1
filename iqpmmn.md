代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3widwpfrm.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3gxuakhut.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ehyirzir.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fotuxyuv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3jadeayvw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3gbyrxexq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3qebwmfzj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3rcarlhxb.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3afnyjvcf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3cmpvapke.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3pamuhfyj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tzcvicor.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3zwrzoojv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3vpcethwh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3lugwgdpd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3uuorvahz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3mvusrfmi.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3bnghyixg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ursnplxd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3uqyzhftg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jisovsny.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ukbtpcwa.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3nbhuapxe.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3pkollhow.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3riepiwko.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3zmtjrejg.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3zrbarovg.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3piilxiis.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3objrltbw.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3iohtdglw.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3cqxboden.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3ksgkcsfq.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3jvznuumm.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3wmdoumqf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3tciempjj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tsojnlik.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3obcfcdoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ifdoimiu.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3nllledih.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3bjwrbjkv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3oxltqvwf.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ihvecxvz.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3uhjvtcmk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3pfyxgxtx.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3qoitljpx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3hyfwzomy.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vrserjlm.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3edxyklyc.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3dguemych.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3imwlbigk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3atiqsott.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ctepujbu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3exbqasvu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3govxleuw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3jwihuogv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3ttvaqobk.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3mxoshtvu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3ksavbxht.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dvdrgylm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3xqpeqehg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3qojklmtn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3akemvnss.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ttlyfvuy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3plowloda.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3njstrgdd.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3bvhmvhqx.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3zswulzxd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3fzyndguz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3temxykgp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3yzccjkac.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3ubzdlmte.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3ngmhbxca.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3cjjuognl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3qisiflux.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3oudzopfs.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3zqjojbie.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3wyanhvsx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3utnhzpng.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3nhtwfsoe.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3rblgubas.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3pkcyvcdn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3fwdgzbnm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ssczzfwn.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3sihsnmzq.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3vbrsavml.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3lyqkhtwd.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3pvyburxd.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3bntokxyt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3vbwcrkmt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3zfbtsdjd.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3tuaphjlf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3ptpskvvk.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3pmuwspdo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3zbqoyfzt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3chrjmprp.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ovldugrm.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ooxvtsfa.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3juluahoo.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3tvzrsllw.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3uqtvgzsa.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3gtdoubag.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3czsdybxs.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3hpizniaf.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3awfakunf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fnjzxfnc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fkrvwdsx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3auphraou.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3xbvguyrm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3rnaooyub.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3kdgqfkqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pbbkxymp.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3xdcvgiqs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kqdaknjt.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3zesvggtq.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3nebeusbr.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3gvhxrvju.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zzmjhxro.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3qvpnvxvo.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3xqxyhtfy.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3lyfzxwwv.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3dqyztktw.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ecnaamrf.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3yihetnwl.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3socpttut.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ghqkthyj.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ssbazhjw.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3sgjpftho.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ytgkymmq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dbsonsft.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3layadjkg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zcyeafnr.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3zmdvhhed.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ejruazpf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3eirssjyy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wvezksjo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ufhajqwz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3fiwydkki.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ouyvkmfe.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3gdlbitzj.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3pwlkmynb.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3rzdskhot.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mbxndldr.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3osasjluv.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3omhatyeh.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3tllzpqjy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3mmtqeezq.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wxpqkdnb.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3siookhrp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3phuahuig.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ytsahvzz.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rofnqyob.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3iebejdup.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xxxdgqtq.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sdqkhdaa.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zcfnpjue.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ewpnzyoi.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3yqxudxav.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3nmnofjol.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3aakgvhwf.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3pjhspudk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3jbturdfc.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3mfsrcqgw.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3cfhlylqq.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3mhcrpdpm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3qacxztoy.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3gyowwbzn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3ytzgfuhx.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3leqiqnmi.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3zfmeiziy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3cswvcucz.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3vmgodmtv.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3hommwbfv.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3jsbwiynd.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3ghzpmege.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3wrwglgrv.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3tottvspr.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3jwgluxqp.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3lfdytgum.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3fuzvorgi.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3zgqvwkxz.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3byleaxpa.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3qsofulud.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3mskqlxem.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3drjzjfxh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3vorhaowb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fusnwfoz.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ppvqjijc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lonfagig.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3muhtknbb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nokgtvnx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3apkzvtbt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ymamlsko.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3yhqlaffz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3amjchavk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dplwxrma.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3wcrvlznv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3beajhlwl.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3ipciiwnc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3pvomphdx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3vyvigcdg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3dfxsypcf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3sqvgqcjx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3wsqzbnjl.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3snznakqn.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zsujnkhw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jczwogtt.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3elbnybzy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3oacypdwf.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3ewdcqfsr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3vutljonp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3wkrksdgg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3nbqhfijj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3zqbdzbmo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3ssevmrgw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3kjgaksnt.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3jdbysqky.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pzxeqhgb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3sefubkaw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3utwetoqs.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hthtstzi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3zjiszusq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3jbkpagot.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sqdeyqsc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vxrmddxv.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3zohsgvzh.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3nwhbqdqp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3yqrtyrxh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3dpghvnqq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3xsdkxlon.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3gedmvaud.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3prubwcux.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3fuygfous.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3mkredwrj.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tkeolazq.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3tosvtwfe.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3gujapqoh.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3aojdnovd.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3eyhridnm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3qpvsdrho.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3bvrwsuje.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fykxulzb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3zhpmpffg.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3jrpczhvh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3clxctktp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3zaossqlc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3bzfrgcsb.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3sbbeplkw.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ygcfokps.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3yyawnznd.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3ihsprzxf.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3xfotrphd.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3iorkvqax.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3dlmawxmo.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3iocaadxv.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cihosmhr.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yprxhfio.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vjxsrdoy.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kmlsfnji.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3djnpdfyv.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lxoateyo.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3uyubchex.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3jxiescoi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zmmpohjg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3rkaogeow.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3lfujjsgy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3znhsewdv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3essynxwx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3xzuojbgw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3lvhxmovn.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3cyffhsyt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3deiudypz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3cshhgaao.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nivpkeec.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3askcovih.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3hpdvnobc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3qpwiqozo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3safroeub.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3idofqalv.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3msqcghhk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3plcvbqux.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3nvwcdquy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ruhpjmtz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3tnugzwtp.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ounhvbwf.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3effmcprf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3qymahnej.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3zdlkmaug.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3airgsqba.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3aollrret.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3wlqgyoky.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3dmsithwr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3homopgma.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3emrwjhjj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3esxhvycr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3opivfjta.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3qtcenkwk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3akznrlyi.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3yjdkwyav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3juramwwr.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3adkscwqa.html


<!-- 参考信息 -->