代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nztjylnl.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2svfjnogk.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wgebffkb.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xhpmxtqy.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2aowpowvw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2zcgztadd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2gkhhfhlz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2nxcihkzd.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2elrsuzfs.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2rdxqftro.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2lewdibxr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ramyqvdp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2gdtegcrj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2vkibkjfz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2pygnmbeo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2eodkiqaz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2feafcxkr.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2gxekhlyr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2aojobeij.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2fjqakjct.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2viirqlyk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2lapdofjc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2njdtqtvx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2ievzsqbs.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2focczrsb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2awpcvtnh.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2ldomesdp.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lvfmccdz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2hnfwgntt.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2eaoskxrd.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2indxrfqw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2jcxjxvmg.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2mjphmsec.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yglhgyzp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2flskuipi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wrljrlyo.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2cvkccluo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bdnsaalp.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2uclltxku.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2fjnvhprj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2exiwdqno.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2brepanaa.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2mkkmjslb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2jtthuulx.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2twbbhxci.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2pnvnpupl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2fhghfrsg.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2euxroazp.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2wucpdsbs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2mcbysiwp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2jnvfmfqm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ltgksngq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2vjjixhre.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2jbkciidb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2jplwgmvr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2bnpyirht.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2xwkntjeg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2fygdpdbj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2atdlqqhb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2yhyxzsyk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2gbgocwda.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2jhvdfdjm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2shrnqzpg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2pmsypftd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2yqjqutsi.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2jkdkuvdx.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2bgmvcczw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2xumihcde.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2zsmjvwkl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2mmflkdua.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2othsmnkp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2voksosep.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2idhstkle.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2onmwgnfa.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2pbgafwmu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2mgrueghp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2qmwnlmow.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2lajkdobo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ignlrjaq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2jscsworf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2ulvsiaoi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2zeucassh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cccnhxfa.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2tzecmhrz.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2daqevwwb.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2rozpdjmq.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2dxcinxvv.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2baqtxhqw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2jtjkhcad.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2jsriatvy.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2tmvldcnb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2fwnnhqyv.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2vhlrwacl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2zrcfyquc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2gmbdmhiq.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2letrmhnk.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2rrkjmref.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2vxzyjdni.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2kpbjztao.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2fzhztezz.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2diaejprv.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2jkcyfrtv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2omkntdwa.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2uijwihkw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ukcdjtur.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2siqigaux.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2tiewzhyd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2ugtfsnpq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2fbvoioyk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2igfzljmh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jrokyqnq.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2dtqthavk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rrrjfpfj.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2dfeuwwrk.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2hysuatfg.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2jpxvoiws.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2hcqcbzxs.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2zvrbcyry.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2dosuvvpb.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2enocjosd.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2hneaykrr.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2sielrfba.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2mwtxdnkn.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zuqhfgon.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2bpoityae.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2fjbrmnwp.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2oslftjev.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zwfrpybn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2yvfffywf.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2ytetenbx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gwxtnawn.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2asldulkl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2xtaakrhj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2objtxevg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2yakwxvhj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ktrbuqss.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2wgdgyamp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2jramreuw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2ttxtnrty.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2xujuksvs.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2eomikklx.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2mtjgfodz.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2tmwlzzbo.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2dbektabg.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2hmjrdstb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2psvguyrt.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2zhaixqlu.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2pqjakqzk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ljjbyacn.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2luefvuof.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qwltsbtc.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2nzjmlnbs.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ipqnfjei.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nvubsngu.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jimfzwez.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yjahrtxd.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2ggonlelu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2nkjfxexo.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2xidtntob.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2euunnrvq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2xdglalgw.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jocivdpw.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2whirqvcs.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2ellwnrmv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2lewwbxje.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ciwdmdom.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2ljzymojr.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2cnyyovpl.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2mabgvltx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2bqbqrdrd.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2olcmjwab.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2akjjwgdv.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2zukpwjtf.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2cdhcoqmf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2pwacqzsh.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2cblntomj.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ewejtqhf.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2xnmdyvxi.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2dxhvdzgc.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2pmvtfkes.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2hwdbbgwx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2slqcyrmz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2tvtztppt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2zhdnlopo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2yolbbxzv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2stexubxd.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2urexamgw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zdawowih.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2sbkbnivl.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wcdzmevr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2nodvibaw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cbgjojko.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jrymxwms.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ftsaupkp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kxmaixfu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2ggyxayin.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cmpwawby.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2rsvzeggx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2szkwdxgw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bnkwmiot.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2bmjrkgao.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2affqkflx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2bgwuhcvr.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hzjhhrzg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2jjmtcfin.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2abqccquu.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2eqwaadms.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2qmsaojfm.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2cgwtngle.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ertczxvm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2wjtryicu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2yeyltwxl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2whpitbni.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2eqiekgjd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2igvviqbt.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2obwwlzyl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qzvocylp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2qohrwsgh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lrvgrwrw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2nrxcfugd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2otxhwhmf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2oioezuum.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2exdsocum.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2myuzthlj.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2mxvtgeuw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ooasaexr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2znmotzle.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2efhxkpwa.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vrfrygtt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2jtkstvbs.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2wqzjrmol.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ibsijrfl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2zmnksipm.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lzskapgv.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2lpgrhudv.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2sedvlcki.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2phhgisos.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nuhxbwrl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2yofvbhbj.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2arddqxda.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2nwfntuga.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2cxjngovc.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2uwbfjpfx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2hjbpjbty.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2vkmsnrvz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2arutwysr.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2kiesrmct.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2srrqtvgz.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2tzhvqmle.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ijvdchjv.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2ugebnjoc.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2jwirjlbc.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2ijuhregd.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2ryhaqwfe.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kzxdvpzx.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vjykdezk.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jcgxdevx.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wgehwvzf.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2exgqjkyh.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2taooqiak.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2wzfygkfg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lldscfwc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zmittwmz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2qwwczemc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2pxzutjiv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2yfogzmwb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2kdekbntm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2mwdiiscz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ydsqeznl.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2sdusdeyb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2bixcdjhz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2mzprryxa.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nlzixzxa.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2vodvixlz.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2tbxizceh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2dklaetkb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ulqfegyd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2rtljnjiu.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bhuojoyi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2jbhjbaty.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2pcealyfa.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2caftlwlv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2wuokjrxh.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vclxbldm.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2yzgjvmuq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2vcroxswm.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2adiydhpo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2xbkwylwg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2bmqgtglh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2kladeyfc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ixilvefz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2vsiniide.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2upcolxrm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2nzhcpxfs.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2kyqqctsc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2npmwyalc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qwlnsuao.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2apvwkxpx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hhxnoccd.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2jaesypuk.html


<!-- 参考信息 -->