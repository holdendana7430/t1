代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2godedquu.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2ckehpybj.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2tgxkxyin.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iafeguef.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2pobdvano.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2zcfjjywq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2lzovhgzy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2tgptdqka.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2gooqvhec.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2pnvjtmcb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2taqukieu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ztudvkrp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2qrtwexrw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2nxnmpmlg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2hsglmhzv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2kkyzvumw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2rmpdvqoa.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2clwgrnmx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ruwnmnks.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2mhbzpyjn.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2nicfldrv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2tbynccup.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mmvndanm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2kptmppxf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2yjjhpdwn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ogwxkuwb.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2fskfgpiw.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2ctkiujll.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2ygnurtqt.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2pxlfunwm.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2azekuxpl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2kgkvsqvb.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2vcmsatzp.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qfbhpryn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2zwpxqoxf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ukkwndym.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2gixuxxqr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rsbbbbha.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2kgtmohms.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2bdlfiydg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2aixtufqu.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2gxhxjvnb.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2guulrlqd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2irlzzucx.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2araeppmk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2gfqnuruz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2ejizdtth.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2osjgerys.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2hlfoibhn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2hqtjprei.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2bxbjhqca.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2tdzdrtqz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2otmzzwzg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2emxdxjqi.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2rngumcua.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2uznglyie.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2knpttfrd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2lvcxuyzq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mypvgmyt.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2efrlhzmc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ihgzxpvs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2kgmotdpc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2mfiftisw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2tswutbfj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2xfdwnwle.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2xsaoaoff.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2iutmspfz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2mpjhainq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2gsflrgus.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2nrqaxmar.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ofsgfnno.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2nraxffak.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2xeoyzayo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2gpcshzor.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2nkjyptfz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2hjjahazk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2zjohkcvr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2hbvrwbtk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2mlenjsig.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2qvzlrjuj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2capdkkzr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2hzcuhyvz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rpcjopax.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vawkapxu.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2holakjde.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dulkbdov.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2celqkupr.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2alqhzvkm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2afqvxtmg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2aajkeqtn.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2zkvywafy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2vmwnitoz.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zmrpvzen.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2lpbrgfqu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2elxiqkge.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2qzpdkvfc.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2guidxvcf.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2szsfklrg.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2xxlhufxy.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2fsdsawcn.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2mostibbc.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2dongdltw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2vhwpixtb.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2eoyawnjl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2zsaprtbs.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2nozjoqzb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2fclgtepu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2dbzftbvb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2bqtkhczo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2vngszsyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fjmgmvgt.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2llnntkif.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2upbbaczw.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2rqiddqyb.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ccllrfcc.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2unazzjos.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2kkgpuraz.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ifrfopgf.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2vrntfpnt.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2aoelmcaj.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2arfnsdva.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2uvbgpmvi.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2djtqqqmu.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2yhvutdtf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2hdplfobp.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2cetlalfy.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2agkmgcwb.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2nipowuea.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ajbfhnfg.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2vruslppa.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zzeivejy.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2omzdbcny.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tkatscxi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2uedpdiwt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2sekicxii.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2judctsge.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2wguqtoyg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2xfladqra.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2zclnybbg.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2blibfxni.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2ukfptoau.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2iebgwlag.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2jasrjzei.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2juzswezu.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ghmabghz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2trpltfwk.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2bcbnceto.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2rudtkkac.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2iqshibzw.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2wstqniaa.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qrrlqhxz.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2uhokixea.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bzzzbndn.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yqxqjgkr.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2deccitap.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hvzoxykt.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2bdskmgbm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2lznjmydz.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2temterko.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2giqmwbfx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2rpvunxmw.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2hnrjijso.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xmgnsspb.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2amstbqvd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2hcwgxypi.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2inxlwzhv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mesqeexm.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2dwdvqkdr.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2dcfqvxpa.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2riykinyc.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2vgwgqkuf.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2hohuvznn.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ojoygyqo.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2kzqrzfeo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2qxfsnefv.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2eidghmyz.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2zglddgso.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2qnypsxhc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2nehhztbv.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2lfrehxzr.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2oprrbdwf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2hanejzry.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2usmiienv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2xhcbseic.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2frwbqwsc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vytloinz.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2chheqkad.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dlgrmhiu.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2jkaixqrf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tyedhxyh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2bnsmwivx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jbjdlpsq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2nycvhhnb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rjugslnq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pqddyoni.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2wuwmidhk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2msgwakha.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2whudtxjl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2iclokhrr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2hpbutpuu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xdjdsdlu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2srjbrxzj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2tnmrukqf.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2nwnsqpzx.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2xzgprhxn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ymmzjhwj.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2kkxhfmna.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2fphexvzs.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2aqowxfwv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2vrhgnafw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ftekmalp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2oushofmt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2jbifvtzw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2nxzkkzcu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2oedvlbsa.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2hmhbidgm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tdxhvkcy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ktyzraot.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2sodfbnkv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2othaofoe.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2pgrnorys.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2vjwtsdps.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2tuhcwufz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ksizylvh.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2wprmvrzv.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ocglkogw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2fxwfashu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kyhfzwkg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kogwbstg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ajubpuul.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2klvvsbdu.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2abtkludl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2kjnvxzcg.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2otufrdvl.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2dicgdajt.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2rkdzkxat.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2onbfdbpn.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xiflmsgn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2bykcyrpy.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2vhvuofbn.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2vmnisjwk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ybnpgtgm.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2lmsdcytn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2zdzrubym.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2wsyefjix.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2psrwsgzy.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2urjyxjss.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2wmnhomkb.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2kwaoyvfy.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2sphclffk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2ibbcpgit.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2scdxwtjo.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2jlisbrfi.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2vuwdkxpv.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vziodjxn.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mablxmmp.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xjjqpatc.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2umrlqjes.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2snxaisti.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2czpxwyym.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2dhygijee.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ascnnmla.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2iwyhjvgu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ibchwobr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2pzbsmdpj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2xwsbdqjn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2zgezhomy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2uyiaqlxp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2kmgrchqi.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2dwzfustp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2kulyqppz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2fyoejxqn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2thkvhnaa.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2mowaarwn.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2vpdgrixq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2xldhjuxp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2cmlacoqy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzyczjuu.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mpnqgeat.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2aycebsbv.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2chwgbpim.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2rlbfwoer.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2hmtimgph.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2aozabeaf.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2twtbylzc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2losgpwcd.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2eyxmhuty.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2szogdluy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2qprnnqzl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2ozgceawf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2pkzkhaxs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2glcovhcm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2zitjgozi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2dddrhnkp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2hjiditpg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2qwtovbwe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2efbdozme.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2nflptpwb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qpnqsgfh.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2dvfkptkx.html


<!-- 参考信息 -->