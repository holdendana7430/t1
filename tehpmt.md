代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2zzhxfcxw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xswfjtsb.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2lklbrzlh.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2zvfedafb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2jmiicuru.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2vcjkqsud.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2iejnrsbj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2sessauxz.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2ufnsbwow.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2skwtjxux.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2dkcvqzjz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zaktxxsu.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2jifaqsyd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uujmxgjs.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2bjhcchzd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2eyvalsrw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2cpkeoncc.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2rxoblvuj.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2kkyrpfgb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2dytjvtmf.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2lvdcyqyu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2mgoieopf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2pdwmzkdk.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2mzgxrabq.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2mqnqlpkj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2zcsamzxh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2xqjudxff.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2wgilhvrv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2wdiougvs.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2hzhofwbb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2ocwjufaw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2eggulznn.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2iutwnsdm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2xubxjvjm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2iqmiisku.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ropjewit.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2fvyamuow.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2xfrsaytx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2zqrkoycz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2gmtaljwk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2rgwkzyky.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2lmlrmfmu.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2dmindqnd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2wsfulqih.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2mjdqbyhj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2byyszkwx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2cxfheupq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2pjqikosc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2yobrxdst.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2irlkbedi.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2cwfndvgy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2xgosqksn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2lwrfpvmz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2yqnwvdht.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ehxcctab.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2enplowpe.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2mydqozde.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2eitmbtjv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mtpqlbmp.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2xqoitirs.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2epvjuyhz.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dalmfgfh.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2bpznmtfr.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2oxpblvzu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2wjodahyn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2xhgezfab.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2opauznyr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2byycuycl.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xpkoheaw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2qarqaenk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ndgplhqa.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2qcwxnbct.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2urgkbyvr.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2aajnczfk.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2aqydtqrj.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2sqxnelag.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2qmxwpsuu.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2cwdzwmyf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2iidoiqly.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2ejumizqx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2lxwbqlce.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xnzqztnz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2vgtjjgua.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2orhmlrxw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2pumaoext.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2utqumgap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qdzenxvu.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2afgudfpk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xiftnwds.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2dulyqyin.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ieyjkzmt.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2kjivoena.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2xrykjdfc.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ohxxvmln.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ffxlkshv.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2rptrpirw.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2nuetdmdg.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2iuqxpwvf.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2yrasbpbi.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2foluxjdk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ycsdeqzn.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2lzkudgjw.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2wjpmpcim.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tkufimya.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2uztspxqq.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2couriofl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kqalqyyp.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2jhzioesz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2dbgddmpg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2tazgbuqh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cvehayzg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2htpjlfeh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2wybcmmmz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2azwwnckh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2luzyqudb.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2cfaoxmbl.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2rbxurbik.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2usyppegd.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2qbwixkxo.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ucdntmlr.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wyvajxrg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2bhqukgcn.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2qkollwvd.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2niqjyqma.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2mkwoyvvb.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2dkrnnabx.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ugwlzerm.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ozsozpuf.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fqrhkqvx.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ifkadlha.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nnyutlho.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2inqxyrwl.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2gwbvovzc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2zdmsftre.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2dktfjgrv.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2nnadlwny.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2atrzxvjg.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hfslkoog.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xtuarqfa.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kasyifjt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2phwaimdf.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2inmxxqtv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2tqeywmjj.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2wbeucugt.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ymdnddie.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ewrvbmao.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ljcakhar.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2bzhczsqm.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2fvbfgsvk.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2ifpotjxm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2xqzrhmgc.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2hvxwbedf.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ydexyixs.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2tyqslmas.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2lozjtjqj.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2wvbciovi.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2rskwetqf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2eatbzisf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2aeestizj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2wlorgstj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2qekxyghc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ondnuoyz.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2serspkxf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ffqnpzus.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2kadqwklj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gicrbcpo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2rgwehwbx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2uchgbmrm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2hyqyzzav.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uqjuujak.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vqyxvoul.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2kupsvhmh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kritmkdr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2nqtwttgh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ismhclgd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2vgghvsoy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2gxgyqhkp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2tqwmkosx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2jmqgyqam.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2arowgyyk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2hvhvzuuz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2stnncbcs.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2eurdbntg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2iyfxikzs.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2qzagbfyu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2hseqkeww.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2rvpybubx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2uhtqroab.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2jpheqrny.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2zaxafgxs.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2hqgcbkkf.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2dcyutipx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2kgzstugy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2gehausdb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ufhoraag.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zolrxrst.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2yikkdahn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2lcidzhsd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2qcreetmo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2egytawcl.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2nfqfkejd.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2karygjbh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmvclbux.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjmtrkuy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2yjsaweix.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2lmkeehxm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2vraifnzx.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2clipicdj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2xliuljcb.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qyjwrbtr.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2sfpcotgz.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wvlnlqoe.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2slnydssd.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xwrievwg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2jobefmql.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ssyllleu.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2sszqcqnu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2tisdjwgh.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2fmdoiwot.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2weyxmeao.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2fqyyxazc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2kovmetqp.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2zkzbxsjn.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2zjqarqmq.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2nxpphrmn.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2mgvaspco.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2czyizlzo.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2powasfwf.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ighezidq.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2fksguozg.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xmhgbbnv.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kfiraefw.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ljzemhil.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zavthetq.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2usvhmmwc.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pcluktxb.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2pjgoxhnw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2yxkhhvzr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2skjybdtl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mnbpzqou.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2htqyptww.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2lelndwne.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2bmrbwnnp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2lmrmdiut.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2cciwrcdf.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2cillgnik.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2typhdgtt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2srieqqiw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2oqqrjrkp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2byegjgaf.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrbuwbep.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2nsjbujea.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2rysuemcd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2fjyndwxx.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fhskhnmq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2ozurcald.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2uzjhdvqf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2brlqpuoa.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2hhwetwih.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2gikkzbyf.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ebcqhbdg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2tmxrsspl.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2kzjxwazi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2ykqimuwv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2slwpegfs.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2rnmfbepf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2jkjxpisn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2jdmiykqn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2poluvxza.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2npyyqcvt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2gbgzyybb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2omrqgaed.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2powandew.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2jzzdljeh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fzgrbuqw.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2qesocwwc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2fwytcyfr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2nwpnmkeu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2mtubukjg.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hkngsvkb.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2pvxcintg.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2cqgveuhi.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2jwvyrfif.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2qnrellrc.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2mxagjcpa.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2ofbcnuph.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2ednajcrp.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rqeetyhp.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2dfjvkfhc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ioahkuur.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2inppyavd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2grwuhqex.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2hftorgcq.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2gztzuinf.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ipbloccu.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2rjaretys.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2votqjwnd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2olblqbko.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhtnqytd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2qtvwctwz.html


<!-- 参考信息 -->