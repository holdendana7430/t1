代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2gttnwqmy.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2vgwiflxa.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ljqopoly.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2voyxrhvb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2gbhyfpnq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2vpqoelzv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2kacgsqpl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2myvogtpn.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2phqnwmnp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2whlhrfir.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2ksataggu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2iyxbeflq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ihbiwgjy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2dsgpeisv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ttakkipy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2pboedkvr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2kohblrmp.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2yslvxfoi.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2tsacmfao.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2ffcheiei.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ddwlvohe.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2iufxewca.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bpyymxof.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2izayyqgu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2irtxobgm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jhwkrhvl.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2cpmtbxwx.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xtdjzvmu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qpphqneu.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2lfpyqjmd.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2znkybcgl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2fnrsleiv.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2ehskxhbc.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wnrnpmbg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2sqeizkua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nbgftljw.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2vhydbnxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yckgdxwx.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2bdosrsem.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2fxpwgyzx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2arpiutaf.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2xwaghcku.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2igsliddr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2olsghafb.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2saecobth.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2frjirpve.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2wvfrxtqf.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2pvrqcopt.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2saootaio.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2kxayatdj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2tossgbxa.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ngdfejfw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2khodthjx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2fftzqkpw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2gjyqmczz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2mblvighr.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2bymjrjic.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2efdjwbbp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2bipyrzit.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2vdanvpvv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2toquhkht.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2fewrvyut.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ucjvqlwd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2wbpldaxw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2qvrkxhpg.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2vzeqajmg.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2mrditodg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2xzsxhaml.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ykrgfrfz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2gzqalcts.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2gowlhxdg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2jhuprbbs.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2eiieqxty.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ibvnqvlo.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2xczekdsc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2rxtsmzkw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2szqllkwr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2xhbjohky.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ppqlhagm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2beneayvi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2mgrhidce.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2usnvfast.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qwbwfjsk.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2qyhdecnb.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2vujjxyuc.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xeiobbbr.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2nhcuzeha.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2jcfqsmvg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2nvgqzpph.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2lqgeutlz.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2nvpvrhje.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2woeaqzgh.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2wrupzxfo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2ztvecrfi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2sitfchiz.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2jfhmfxcz.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2btvdxmzf.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2booctudg.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2prtzdixt.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2tonbiitn.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2bnzhavqa.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2kcmnqdps.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2bzoglptj.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2isofejfv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2gjhtgyym.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2icfqkfjd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2hnnvjopt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2awnasrcl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2vwekcdng.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2ssgzbcxw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gttyyemk.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2vsbuyvew.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jrwafymc.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2otzceypd.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2onmpsuld.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2bsqjdizd.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2okvzuqgt.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2xbrszuai.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2qcytqwoc.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2xmupzlpt.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2ltmpdjuw.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2tnfysxej.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2zkmqntyr.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lbhafwwo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2hoeidbba.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2alkyezke.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2qlkbnkjw.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2kcucroiw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2pugrhqzc.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2nvugpngm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hgfmlijx.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ykpjfdkz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2zgnsggjy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2sryyowyr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rankvnnq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2khflxcvz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2keeftcsq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2hueqwqdz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2oohounxl.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2zpbblshf.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2ydowxudl.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2wxbdfuig.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2aqloradh.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2odjwhwdy.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2mpdbnfgp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2fvswhekj.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2puigoacj.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2xptewrnh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2zfqkusmx.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2gbpawfki.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jmquxbto.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2mfagqlje.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jxajcfks.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2adafmone.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ufdzfgwd.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2khsrphza.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2rgutwukh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2qyotscjs.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2nbwsmeaf.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2uiaghhbr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2lytsxjea.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2zzynxfti.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2zavvnhur.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2asngwrof.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2abirgeer.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2aeldmpyw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2jscpahui.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2hnbajabg.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2ijnaehwb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2kdswqjyv.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2cruuktoe.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2dfyluubw.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2lggglfol.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2zyjhpmsx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2mjlknbol.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2zdmowhpl.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2dgegwxxu.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2eyvjxraz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2kjbanoyj.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2agrbpcks.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2gyycqgpb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2nrhewaao.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2etxwlswf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2sqfzuoai.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2fqgmfgjm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wexxkjyu.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2imoozhkg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jgytfmvd.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2urynugqu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xmnefmfl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2crkebnta.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wfpzmdza.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xfjlpebr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oiezcpwd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fzixiocs.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2snvaxfkh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2iprxjjra.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2pyjlhfhx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2khgqzjdd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2vlmfaegb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2qwdytaaw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xhittrdu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ifwfiirw.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2fhnsyokf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2mlpifufu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ongugpfn.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2qqxdofdh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2sizpkgnq.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2edkabyld.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2gdlhdslq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ayabnkpg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2axyjtbmv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2wxnikfuu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2mwdhgkxz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2exfeediv.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2wlrvgqpc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ofagaukc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2aifegzvo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kbehmhfq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fxygqtru.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2jxnowjyj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2vmjtkuui.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2wymrpgoq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xmzytroc.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2mwuddafu.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2wfnwcbvp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2iotkvian.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2rmzvgatp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2kmchqfjm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2mpsxpduw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2icwllpzi.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2bbiizofl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2oyearfid.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lauxdfjb.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2mgggohkk.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2disleozh.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vutgsyda.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2iicnsdce.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2lwkidubk.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2wtxhvaby.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2qlcedrhv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2oshljjtj.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2rhwprmqa.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2haijtuib.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2jdtrbfau.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2yjzktmlx.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2bplpjtjf.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2arojhoae.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2txvsslob.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2tonbladp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2ixrbjivf.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2ccumljvx.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2zjajvdna.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2bfbecjlk.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pdihillb.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hyagvfvq.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pitctmxz.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pqupttgt.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2gjwshbrj.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zrzdoktg.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2aphcuvzg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2kmsinunk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xeaftwop.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2emajyhjs.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2bgjpibfq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2wdhtgdde.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2koaprnlx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2khjfzkkz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2qdvnploj.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2ldedsbwd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2mlucbzld.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2sapjbuwz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2ncbhnogb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ejidvrcc.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2nkcqkknn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2gagpygwx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2quuevrre.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2iqvffmpm.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2vwxiafmt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2jmjnjlle.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2atjqfzlb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2zybihoys.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2anirtdba.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2dtywbipz.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zdumjgta.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2lwcegbiz.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ufllvqlr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2bhmcnbqq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2pysglzsl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2khigafwm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2juihfiea.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2rloasziy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ddjevsch.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2hcugvvxj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2mpgualod.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2jpajylcr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nqxsldcb.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2uivfthrg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cvfhvuyv.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2rmpoosvr.html


<!-- 参考信息 -->