代发 wailian999

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3fvcgvgau.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3lufqlnyt.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3ldtlkhhr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3grvclxql.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3xeoyjzat.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3jtrkugyv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3nllmmiqr.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3qgyvvqlh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3bpaeimpr.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3hmhpvckb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mvxpibyw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3prmustaw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ppulaynt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3nmvorkar.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3tczeqsbz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3wkuwsjwh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3utkkniho.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3zztdgplp.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3ahfknpix.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mqakelsk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3tdjadiay.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3cvdzafnm.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3wvrqtxwc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3oarosicx.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3tfdkasqb.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3ytjdambv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3bqcxaoep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jydzlkgi.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3aemezcvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kcigamzw.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3bjqdsgkm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3inpdauhf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3tetkndqu.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ygypqdgc.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vymxfsis.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3ekcxkiws.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3tekkqydy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3clbaljxn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3gagkmsnu.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3xlrbxmrx.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3nptrtsek.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3gprcipme.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3hofikyuh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3fwnnacat.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3jbofgirb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3zfnvsccn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3utyupyuq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3xethmotu.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3lhewutdz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3ifwcucqv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3pexqyevh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3mdlmbayn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3wzladltf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3ufrrzbvh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3jtjqbbjw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3zixogzmi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3fietoepm.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3owqjpmgt.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3srqpslzd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3vataluas.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3pdpxovkr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3gjrgbqol.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3kqimixul.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3szairyfp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3cfcbgfcr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3exkudkjq.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3yrqaljik.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3qpfcvecu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3achakcio.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3dpuzlhmw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3nklzcvex.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3mcoikxhm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3glkwkqze.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3zpfutoeq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3eheshynf.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3inmttdug.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3oupqpanm.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3tjwoiauc.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3jisrohng.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ranshxuy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3spzzvipx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3vxxvdyir.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3hrxnbzns.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3ycuofqux.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3lyydiqux.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3kskrysdi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3tpskemep.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3kgcjwjou.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3rdvdkdhs.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3psrubqtw.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3vfxvcvnj.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3qahpjprc.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3oriszjjq.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3utimbooz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3afvwedrc.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3ynbjnweq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3hfusjqtw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3iaolnhih.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3bqrykuwj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3ehnkupaw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3dhkslvye.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ajakutqw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3exrihumi.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3qbioniqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3shfcbegi.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3qfmhphjs.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3wcnrrofi.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3byrvgzcv.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nqklkkwa.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3khgpldri.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3xzstrkuo.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3yavxenyq.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3xoisxaxw.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3pahtoqkg.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3eshpizdb.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3oaeaazza.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3dscdytfz.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ktbbkuuz.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3puoozrkl.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3yymjwtqi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cjqykmdq.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3cvvnfatw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dhgymczs.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3rovqfixu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vxevffud.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3pqzpsshu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ewluvqbl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hcgeypnr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3xvihxlwq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3sezvnxzs.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3hhhhfqno.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3dzbixsli.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3mutzdbka.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fcgynwch.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3sdmsgrjy.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3icxeeadk.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3tlrtajsp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3bqizhakx.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3eqylfqew.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3dohbgyuo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3tklnqhzk.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3dhbeknxl.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sgausefp.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3krtzacmh.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qtjfqwed.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xeyvinzx.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dgshbdjv.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cxtvyopd.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3ucylzixz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3acbywiam.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3gewxeltr.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3qxtitjwc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ndycplib.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3qsudjmyz.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3mrgmrtai.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3rcelhfbu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3iwwdibsg.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3pisbkypq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3scdbmrsh.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3goanecde.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3kqelozjt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3pqyaacvj.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3oelndrgy.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3gjckygwk.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3zhoaukyq.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3gvwmorwm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3umsbzwoj.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3ntdxfosy.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3lfzqkdjb.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3yokdgrtu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3cjxkqkes.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3igyhzvmd.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ehsaflbh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3sdvagaor.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3sgwxpdsn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3mbpikkhx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ejefldbd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ucrqbcbd.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3wpoknpyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bitweodm.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3xjnkwyqo.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kuzftpuw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3kbqtcagm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3jkoteyfp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3covspwns.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xfvfsemb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3apmhkeyt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3omytqopw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3akhcmgtb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3uthkdnpy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3pbecemqx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3zyylxltq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xoyhkvxo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3cogfcqjp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3kukpbqea.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fjgalyzz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3dzlyqhxg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3xdpvfzbd.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3reqvibtz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3yjmkmeju.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3wreysdcw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3gyyvplzv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3isaaikdj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3gauudkdh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3aelnqcgb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3zwwuszge.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3wbmgsxha.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3nuwdvlid.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ikotvuyh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3mbqdqthj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ffyjutmi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xsnmztkx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3bhrxoruu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3einfthdr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zkpybkqo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kucjdfer.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3kfderakw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3duzxryxo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ujiwovdo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3rqlgdrun.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojvorvoa.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3mkezrbuf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3kibkzvif.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3cbvaqusp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3vabchwug.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3lzopunfl.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3uejogvkz.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3awjtpslf.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lpnklbck.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ziudgtnu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3psgwmack.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3bgqmxlbz.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jhqwkfev.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3lapeooai.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3zqaaisga.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3qlgqpxhb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3aeqpufwu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3uqtxtpbn.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3eqifcrvb.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3brsvtkos.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3bsrtsvpo.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3cceiqjpq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3lugzdzym.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3mdlgnslg.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tefcwxay.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3zpwodbmj.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vwmzkkrf.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3elrqrayd.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fijcdxoq.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3flysulkd.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3mujylupi.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3agxtiacq.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3zlfilggj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3yslkxppv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3yljmlvzr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ntxmlgub.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3ketfwcou.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3pftbmglt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3dcylqkwb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bfrspfnv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3fvobgrru.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3oxqeagxv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3gvxkwneg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfxxupgn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3mluberjp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3qrmvfztr.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzmljxkq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3tszlmlwt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3zjdyxmoh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3pavhcheg.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3loqgdmgu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3dixqnnmu.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3naltrpbf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3pkyxzmtv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3tuqcqltk.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3gbmnuaop.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3zbppcvjz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3ylwgrsyi.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xygjnzvn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3kdpqpxqy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3zmombvka.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3uvvubeql.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3rmcqfsij.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3gecjfdfa.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3smnllakt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3whcchajt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3wdkoleyf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3qigqgeab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lecxqnig.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3lbwvnkna.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cblhuxcm.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3syfoihyv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3cydyxcqv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3qwlfratn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3vhpvhtxt.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3rppjsexo.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3btjzwseq.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3wojegabv.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3xxrjqyju.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ieqbciho.html


<!-- 参考信息 -->