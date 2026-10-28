代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://hz.guowangkeji.top/gtyaugcixd.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yueranfly.top/gtkiuproci.html

JS:   structuredClone(obj)
来源：http://hz.xinyue.icu/gtitcqqjfg.html

TS:   structuredClone(obj)
来源：http://hz.chenzaomai.com/gtfbzplfoq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zycfv.cn/gtknaoupko.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jinghuilouyu.cn/gtrtafoonk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yueranfly.top/gtsitutmhw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.shuidangran.top/gtywilrvhy.html

[K06] 解析 URL 查询串
来源：http://hz.ybcxt.top/gterfduzjh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ydjk.org.cn/gtbdsgwgas.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zycfv.cn/gthjmehcbt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xinyue.icu/gtzzayktgj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ivvv.top/gtcgzmnvrm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.bjfxy.top/gtxaowcxdb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.daxiang520.top/gtfnpswhlm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.nanxuanxn.top/gtlfewagzk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jiagoushi.top/gttzgundnh.html

[K07] 进制转换
来源：http://hz.sxryk.cn/gtlbesbery.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ppjwa.cn/gtivbwxuwz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jinqigufen.top/gtaxzguhdg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.guannengcc.top/gttmkrjuou.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.redwolf501.top/gtxxavcovo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.haohaochexian.top/gtrpuhgvgl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhoulong.xyz/gttgjfhkfb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.cheryme.top/gtqihmvbth.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.52xcode.cn/gtgivyitrx.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.pycfn.com/gtablxhwno.html

Py:   pickle.dumps(obj)
来源：http://hz.xingfuxueyuan.xyz/gtbkhplfyf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.fzhhl.top/gtpuqgizos.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.gotoacloud.top/gtbmdhgbdx.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yj20258888.top/gtckmpvsfy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.gotoacloud.top/gtytgznpco.html

Go:   encoding/gob
来源：http://hz.aizwys.cn/gtwoaqtrmq.html

Ruby: Marshal.dump(obj)
来源：http://hz.jinqigufen.top/gtawycnisa.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ydjk.org.cn/gtdydcwusa.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtrcgycipt.html

L. 网络请求
来源：http://hz.svipenyu.cn/gtuygayqbn.html

================================================================================
来源：http://hz.sweek.top/gtsjigoisr.html

[L01] 发送 GET 请求
来源：http://hz.quarkkingdee.top/gtlquxvgwt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.daria6918.cn/gtqhyzdpqq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.xuetiantiany.cn/gtkcbztltr.html

JS:   await fetch(url)
来源：http://hz.fengsongda.top/gtdmythqox.html

TS:   await fetch(url)
来源：http://hz.jqgfzy.top/gtyxevaccu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.chenjidiqi.icu/gthoplmuqb.html

Go:   resp, err := http.Get(url)
来源：http://hz.gzhubu.top/gtnxuekscq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.gzhubu.top/gtvpvlpbsy.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ywan-chungtsiang.top/gtylvjolmv.html

[L02] 发送 POST JSON
来源：http://hz.kuanghao11.cn/gtimofderr.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.meibo888.top/gttysyawbc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.316326.xyz/gtdltqfumx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gzhubu.top/gtthuovcui.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jianghu66.top/gtqzmhlxtk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ivvv.top/gttrnuaose.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yj202588.top/gtldhmdlem.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.wangdashe.top/gtxxvkvhem.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.shangyingyoupin.top/gtjcchhgpw.html

[L03] 设置自定义请求头
来源：http://hz.jinqigufen.top/gtovykmhag.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hysaishi.cn/gtgipaekmq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.chenzaomai.com/gtvvaymuvj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.daxiang520.top/gtllstbkei.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yanxiufei.cn/gtoqncjvlj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.snrcjt.cn/gthorvqxql.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jianghu66.top/gtpquntnoi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.tian-w.cn/gtnxryesqt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.xuetiantiany.cn/gtyuousolq.html

[L04] 设置超时
来源：http://hz.xuanzx.com/gtswyqmhkq.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cdnleiting.top/gtkayvzjkf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.cdnleiting.top/gtqqhpkmde.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hywenlv.cn/gtqahojscn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hnqzz.top/gtbtnqjriy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.daria6918.cn/gtjhmvhypi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.redwolf501.top/gtwwobovor.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.guannengcc.top/gteffotcjd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.kuanghao11.cn/gtplzlcxbj.html

[L05] 上传文件（multipart）
来源：http://hz.shzxlz.cn/gtarcwzqdq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.ehwqpu.com/gtdjckdomk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.meibo888.top/gtnyeylnky.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.xinyue.icu/gtdsablyzt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.feifeiyinyue.top/gtiybjydrd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.shanyushiyangtech.top/gtzdinmwok.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.snrcjt.cn/gtdtfwjymu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.hammf.cn/gtuzzzlrnx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.shanyushiyangkeji.top/gtddifyxfi.html

[L06] 解析响应为 JSON
来源：http://hz.jqgfzy.top/gthtnrmuzj.html

Py:   resp.json()
来源：http://hz.xylfe.cn/gtbexjtbcz.html

PHP:  json_decode($body, true);
来源：http://hz.gotoacloud.top/gtjivltqnw.html

JS:   await resp.json()
来源：http://hz.jinyuanbaomall.cn/gtjfymheqi.html

TS:   await resp.json()
来源：http://hz.ivvv.top/gtpyihfbqx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.cucudq.cn/gtbhtdfjdk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.52xcode.cn/gtemdxqxxa.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhengqikj.top/gtojpkmupw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.aizwys.cn/gtkdavhdqd.html

[L07] 处理 HTTP 状态码
来源：http://hz.yongpay.top/gtugdlqvxh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.ybcxt.top/gtzufrheie.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.haohaochexian.top/gtbrjcqynb.html

JS:   resp.ok;  resp.status
来源：http://hz.ivvv.top/gtqpzuvjkh.html

TS:   resp.ok;  resp.status
来源：http://hz.chenlongwang.top/gtvcpcmswz.html

Java: resp.statusCode()
来源：http://hz.dashuyun.cn/gtbtebxyui.html

Go:   resp.StatusCode
来源：http://hz.guannengcc.top/gtqdrcnrmy.html

Ruby: resp.code.to_i
来源：http://hz.xuanzx.com/gtpvmzgpto.html

C#:   (int)resp.StatusCode
来源：http://hz.jqgufenzy.top/gtaagmqikn.html

[L08] 并发请求多个地址
来源：http://hz.havefunace.top/gthmdgyjqj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.daxiang520.top/gtaiirsurl.html

PHP:  curl_multi_init() 系列
来源：http://hz.hywenlv.cn/gthetsssqj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xuanzx.com/gtjiwncbrm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xuetiantiany.cn/gtmpghjatn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.daxiang520.top/gtjthcvzpj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.316326.xyz/gtqevyesai.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.birdmap.top/gtrzvfteja.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.shuidangran.top/gtltoldzbd.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtlrcdpthd.html

M. 命令行 / 进程 / 环境
来源：http://hz.nwbrower.top/gtqrylmoug.html

================================================================================
来源：http://hz.yj202588.top/gtqsdzoowr.html

[M01] 读取命令行参数
来源：http://hz.daria6918.cn/gthxpdemxl.html

Py:   sys.argv[1:]
来源：http://hz.cqqwz.cn/gtrmtfpiud.html

PHP:  $argv;  $argc;
来源：http://hz.smart0.xyz/gtihtwhycs.html

JS:   process.argv.slice(2)
来源：http://hz.mhx1999.top/gtjyqyicsc.html

TS:   process.argv.slice(2)
来源：http://hz.sweek.top/gtxorqoodf.html

Java: args 数组（main 方法参数）
来源：http://hz.gotoacloud.top/gtkerydhhb.html

Go:   os.Args[1:]
来源：http://hz.chenlongwang.top/gtztxynudo.html

Ruby: ARGV
来源：http://hz.yongpay.top/gtqgwtnppm.html

C#:   args 数组（Main 方法参数）
来源：http://hz.mhx1999.top/gtgqkdadem.html

[M02] 读取环境变量
来源：http://hz.wangdashe.top/gtjqyxqgrt.html

Py:   os.environ.get("HOME")
来源：http://hz.cqqwz.cn/gtduvpguxo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.9152youxi.cn/gtvndrlyzm.html

JS:   process.env.HOME
来源：http://hz.yueranfly.top/gtnhflcspu.html

TS:   process.env.HOME
来源：http://hz.zhongyouzk.top/gtjidyqoxp.html

Java: System.getenv("HOME")
来源：http://hz.meibo888.top/gtyynpvfzo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yongpay.top/gtfseoqhcv.html

Ruby: ENV["HOME"]
来源：http://hz.jyoumei.cn/gtspmlobhq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hammf.cn/gtsmeebipn.html

[M03] 执行外部命令
来源：http://hz.yonumen.top/gtfpzdsioz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xuanzx.com/gtotnzaduj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.chenlongwang.top/gtogqabfui.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.havefunace.top/gtvlwuayen.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xziqi.cn/gtlnekoyry.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.tanke756.top/gtoibssmhz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hywenlv.cn/gtbikvasnk.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jinqigfzy.top/gtwxfloyjv.html

C#:   Process.Start("ls", "-l");
来源：http://hz.fzhhl.top/gtscimbnsl.html

[M04] 获取当前工作目录
来源：http://hz.jinqigfzy.top/gtgntkocjf.html

Py:   os.getcwd()
来源：http://hz.ivvv.top/gtudyawwes.html

PHP:  getcwd();
来源：http://hz.tanke756.top/gtkjtvbywk.html

JS:   process.cwd()
来源：http://hz.yueranfly.top/gtynxropbi.html

TS:   process.cwd()
来源：http://hz.shuidangran.top/gtpvxvwejw.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yuxming.cn/gtqbmxcofm.html

Go:   os.Getwd()
来源：http://hz.tian-w.cn/gtpucfsqnc.html

Ruby: Dir.pwd
来源：http://hz.zhoulong.xyz/gtbhiffmzk.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.smart0.xyz/gtmbiqguku.html

[M05] 设置退出码
来源：http://hz.gzhubu.top/gtuvhetpyc.html

Py:   sys.exit(1)
来源：http://hz.tanke756.top/gtttkpycbf.html

PHP:  exit(1);
来源：http://hz.gzhubu.top/gtaqauwdac.html

JS:   process.exit(1)
来源：http://hz.yj202588.top/gtcapofodp.html

TS:   process.exit(1)
来源：http://hz.cucudq.cn/gtgxqrbace.html

Java: System.exit(1)
来源：http://hz.ybcxt.top/gtizzzuxbj.html

Go:   os.Exit(1)
来源：http://hz.52xcode.cn/gtndiaouye.html

Ruby: exit 1
来源：http://hz.ehwqpu.com/gtdbbsrimm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.haohaochexian.top/gteqhvzlqs.html

[M06] 向标准错误输出
来源：http://hz.gaohongyu789.top/gtqzxxwirt.html

Py:   print("err", file=sys.stderr)
来源：http://hz.nanxinkj.top/gtjlhfvplh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.nanxuanxn.top/gtsoxfidzk.html

JS:   console.error("err")
来源：http://hz.dashuyun.cn/gtiuntuduo.html

TS:   console.error("err")
来源：http://hz.birdmap.top/gticfgcuow.html

Java: System.err.println("err")
来源：http://hz.yj20258888.top/gtyqqelkyp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.gogol.net.cn/gtjdhkdpqv.html

Ruby: warn "err"
来源：http://hz.ydzc1.top/gtdksljgyp.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.wangdashe.top/gtwqjdzdrj.html

[M07] 判断是否为主入口
来源：http://hz.jqgfzy.top/gtqwowywhw.html

Py:   if __name__ == "__main__":
来源：http://hz.nanxinkj.top/gtnyskndsm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.chenlongwang.top/gtytjutitp.html

JS:   require.main === module
来源：http://hz.birdmap.top/gtakgmbdmw.html

TS:   require.main === module
来源：http://hz.xingfuxueyuan.xyz/gtnhjfmqye.html

Java: public static void main(String[] args)
来源：http://hz.smart0.xyz/gtxlegqwga.html

Go:   func main()
来源：http://hz.jyoumei.cn/gtfcurkojf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.tanke756.top/gtcbfhxtuh.html

C#:   static void Main(string[] args)
来源：http://hz.birdmap.top/gtniwqjywe.html

[M08] 获取系统与运行时信息
来源：http://hz.52xcode.cn/gtkyrzplxo.html

Py:   platform.system();  platform.python_version()
来源：http://hz.daxiang520.top/gtycakvejb.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.shangyingyoupin.top/gtaaslqyaa.html

JS:   process.platform;  process.version
来源：http://hz.hnxiangtu.top/gtcxcozmnf.html

TS:   process.platform;  process.version
来源：http://hz.wangdashe.top/gtmawyfqlg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.ehwqpu.com/gtzqopehxl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.gogol.net.cn/gtaaxkqdmt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.gaohongyu789.top/gtckxfeuea.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.andypj.xyz/gtidqymltu.html

================================================================================
来源：http://hz.sysykeji.top/gtprnqltte.html

N. 数据结构与算法
来源：http://hz.jinyuanbaomall.cn/gtxuoloklw.html

================================================================================
来源：http://hz.zycfv.cn/gtxdzrdevd.html

[N01] 二分查找（有序数组）
来源：http://hz.vqdsnc.cn/gtdiatuccq.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ydzc1.top/gtdztvmoaq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhiwuduotai.top/gtuqeowpnn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gotoacloud.top/gtmizmptvd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hongshengwenyu.top/gtbvnyuaea.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.ehwqpu.com/gtdudyubjc.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.gogol.net.cn/gtjquwbndg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jiagoushi.top/gtjkiutqfa.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.svipenyu.cn/gtcgxdvkxr.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.tianlin.xyz/gtptbctkmy.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.nanxuanxn.top/gtokaantvf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.sufxvd.cn/gtgdrfcpls.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ehwqpu.com/gtkznlogar.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.snrcjt.cn/gtlopfwdow.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.svipenyu.cn/gtxokezrrj.html

Go:   slices.Sort(arr)
来源：http://hz.nanxuanxn.top/gtiwrsxiui.html

Ruby: arr.sort
来源：http://hz.yangfankeji.com/gtkacrfezl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.sysykeji.top/gtmxvfzgts.html

[N03] 快速排序（分治示例）
来源：http://hz.jqgufenzy.top/gtiqwtgstt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.cucudq.cn/gtwpxftmps.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yvedp.cn/gtetdyezuo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nwbrower.top/gtzrwqvhky.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shuidangran.top/gtjxakkdhh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhoulong.xyz/gtjnbgdkpn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.gaohongyu789.top/gtthddhpxy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hongshengwenyu.top/gtddqnhdbh.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.snrcjt.cn/gtgpnksavo.html

[N04] 斐波那契数列
来源：http://hz.shzxlz.cn/gtcxzfikuj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.shzxlz.cn/gtufkroqrp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhaomingkeji.xyz/gtskrjaijk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ehwqpu.com/gtafgjcocu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yonumen.top/gttinkfugd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.fzhhl.top/gtjfhtojdv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.dianchejie.cn/gtmjxhwafx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.cqqwz.cn/gtvgyrfano.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.svipenyu.cn/gtxdzbohal.html

[N05] 最大公约数
来源：http://hz.daxiang520.top/gttnjjcejl.html

Py:   math.gcd(a, b)
来源：http://hz.xuanzx.com/gtudqerzdn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.havefunace.top/gtfregkbky.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.52xcode.cn/gtdttzmpuu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yj20258888.top/gtqdmoeuls.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.nanxinkj.top/gtgavsyjjy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.xinyue.icu/gtcrvwqeqn.html

Ruby: a.gcd(b)
来源：http://hz.svipenyu.cn/gtknwkmeqv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.cdnleiting.top/gtadqtrdtl.html

[N06] 判断回文字符串
来源：http://hz.nanxinkj.top/gtpewtdfgy.html

Py:   s == s[::-1]
来源：http://hz.vqdsnc.cn/gtvgrrljjn.html

PHP:  $s === strrev($s);
来源：http://hz.daria6918.cn/gtusllmcfp.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jqgufenzy.top/gtgqbojqea.html

TS:   s === [...s].reverse().join("")
来源：http://hz.tanke756.top/gttygdnkwd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ehwqpu.com/gthaoddfxb.html

Go:   // 双指针从两端比较
来源：http://hz.sufxvd.cn/gtwnwexztq.html

Ruby: s == s.reverse
来源：http://hz.yvedp.cn/gtnhwlfdxn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.birdmap.top/gtzwkwfplp.html

[N07] 两数之和（返回下标）
来源：http://hz.hywenlv.cn/gtouawgidp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhoulong.xyz/gtqkrqhvux.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.aizwys.cn/gtysctfwmp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jinqigfzy.top/gtqohzvpup.html

TS:   // 手写 Map<string, number>
来源：http://hz.9152youxi.cn/gtfguyngci.html

Java: // 手写 HashMap
来源：http://hz.gzhubu.top/gtiqxkblmo.html

Go:   // 手写 map[int]int
来源：http://hz.cucudq.cn/gtlvsvxtom.html

Ruby: // 手写 Hash
来源：http://hz.mhx1999.top/gtskvdxgej.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.smart0.xyz/gthrvnovig.html

[N08] 生成全排列
来源：http://hz.dashuyun.cn/gthekjpwfa.html

Py:   itertools.permutations(arr)
来源：http://hz.yangfankeji.com/gthkonswqd.html

PHP:  // 手写递归交换
来源：http://hz.9152youxi.cn/gtrvbpzcck.html

JS:   // 手写回溯递归
来源：http://hz.tian-w.cn/gtwdqmxshr.html

TS:   // 手写回溯递归
来源：http://hz.xuanzx.com/gtybkgrvtz.html

Java: // 手写回溯递归
来源：http://hz.tianlin.xyz/gtsnwatmtk.html

Go:   // 手写回溯递归
来源：http://hz.yangfankeji.com/gtregmdlty.html

Ruby: arr.permutation.to_a
来源：http://hz.tanke756.top/gtatjatnkr.html

C#:   // 手写回溯递归
来源：http://hz.gzhubu.top/gtllbcdwfw.html

[N09] 栈与队列
来源：http://hz.cashguo.top/gtmjvmdmcx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yanxiufei.cn/gtanbavrrp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.nwbrower.top/gtbxzzmdgz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhijiandao.cn/gtzuupvvwr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.andypj.xyz/gtoozqvjvt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhoulong.xyz/gthqeeplqp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.smart0.xyz/gtnnasyutr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hnqzz.top/gtcwyxzzkx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.tian-w.cn/gtfkeleuae.html

[N10] 链表节点定义
来源：http://hz.fengsongda.top/gtqdgzsonq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.316326.xyz/gtyfekgywc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.andypj.xyz/gtuncpwnbh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhijiandao.cn/gtnvrqbnjj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhixingplan.top/gtwgzcabnz.html

Java: class Node { int v; Node next; }
来源：http://hz.ybcxt.top/gttjfzhjtk.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.cucudq.cn/gtcoqmfefu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.cheryme.top/gtvlltglwc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.nanxinkj.top/gtoakcmene.html

[N11] 二叉树中序遍历
来源：http://hz.zhiwuduotai.top/gthbtzjvxg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.mhx1999.top/gtkzzobohn.html

PHP:  // 手写递归函数
来源：http://hz.yongpay.top/gttznjbdfq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zdqjudy.top/gtxeryqodh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.birdmap.top/gtjdqaixyi.html

Java: // 手写递归
来源：http://hz.yongpay.top/gtkiklpaup.html

Go:   // 手写递归
来源：http://hz.cucudq.cn/gtqafexuse.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhaomingkeji.xyz/gtwijkxpeb.html

C#:   // 手写递归
来源：http://hz.yuanzhike.top/gtbvgpguaq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.aizwys.cn/gtxiqzpbab.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yj20258888.top/gtxbithklh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.0kj1m.cn/gtgoniqeab.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.nanxuanxn.top/gtqyqhheds.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.nanxinkj.top/gtfgreorup.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yanxiufei.cn/gtuwousptd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.dashuyun.cn/gtpvireert.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.aibaodan.cn/gtfmsabbwe.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shangyingyoupin.top/gtgdxqyloh.html

================================================================================
来源：http://hz.iojbl.cn/gtpttpvbbm.html

O. 并发与异步
来源：http://hz.9152youxi.cn/gtzyhpnvnk.html

================================================================================
来源：http://hz.9152youxi.cn/gtacznsnes.html

[O01] 启动一个线程
来源：http://hz.gzhubu.top/gtrmhwlvca.html


<!-- 参考信息 -->