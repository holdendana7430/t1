代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.aizwys.cn/gtollqzply.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.sufxvd.cn/gtfzvjnaqv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.tian-w.cn/gthxumpejv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.shuidangran.top/gtivkqyqni.html

[K06] 解析 URL 查询串
来源：http://hz.nanxuanxn.top/gtipjptulw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.pycfn.com/gtmpoqiarz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhongyouzk.top/gtnomgmrgk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.chenjidiqi.icu/gthsplgrah.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sufxvd.cn/gtmiexajip.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhengqikj.top/gtycmdeayr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.pycfn.com/gtoxlgfqcl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.wangshuangyany.cn/gtpfmwongn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yueranfly.top/gtuuauscmi.html

[K07] 进制转换
来源：http://hz.shanyushiyangtech.top/gtzdgdzeiy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ehwqpu.com/gtvvjbwhzi.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.fzhhl.top/gtmzkorlng.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.bjfxy.top/gtbslucpnm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jlsjyb.cn/gtofqrjfrg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xylfe.cn/gtzqanzhol.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hysaishi.cn/gtxjqhhvmx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.gzhubu.top/gtggwqctmy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.gogol.net.cn/gtntcqoajm.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zdqjudy.top/gtvoozstel.html

Py:   pickle.dumps(obj)
来源：http://hz.hysaishi.cn/gtzhueydms.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.shangyingyoupin.top/gtlixigqma.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.sweek.top/gtnfkpusbj.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhiwuduotai.top/gtqpdbmkqy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ehwqpu.com/gtziemomui.html

Go:   encoding/gob
来源：http://hz.cqqwz.cn/gtgoydszau.html

Ruby: Marshal.dump(obj)
来源：http://hz.jinqigfzy.top/gtsarqgaxb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jinyuanbaomall.cn/gtiuqjgbon.html

================================================================================
来源：http://hz.zhijiandao.cn/gtbomrghtu.html

L. 网络请求
来源：http://hz.shanyushiyangkeji.top/gtxczmbvhg.html

================================================================================
来源：http://hz.sxryk.cn/gtfmsqucvi.html

[L01] 发送 GET 请求
来源：http://hz.mhx1999.top/gtttfcnejm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jlsjyb.cn/gtqkvdkidz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.dashuyun.cn/gtqnfhydtr.html

JS:   await fetch(url)
来源：http://hz.jqgufenzy.top/gtsxlfanbf.html

TS:   await fetch(url)
来源：http://hz.ivvv.top/gthuxqlnwn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hfpthk.cn/gtzlormoqp.html

Go:   resp, err := http.Get(url)
来源：http://hz.ivvv.top/gtvdqlofco.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yangfankeji.com/gtkrxgmqaj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ivvv.top/gtykqibxrb.html

[L02] 发送 POST JSON
来源：http://hz.daxiang520.top/gtvnqhmkpt.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zycfv.cn/gtnhqaujhx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.snrcjt.cn/gtkopjuxgo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.iojbl.cn/gtyynpqouh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xinyue.icu/gtsrtltrxi.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.chenlongwang.top/gteigqluqp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhijiandao.cn/gtyufdttxr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yj20258888.top/gtmfoqcdwq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.cucudq.cn/gtokbknnsq.html

[L03] 设置自定义请求头
来源：http://hz.hywenlv.cn/gtwtarelqk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yanxiufei.cn/gtoghgmfkc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.guowangkeji.top/gtnhqlueds.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hongshengwenyu.top/gtegbwmgnh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hysaishi.cn/gtuagfsrge.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.daxiang520.top/gtpkstjrih.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.shzxlz.cn/gtmdgabdak.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.haohaochexian.top/gtgrkjvszc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.xziqi.cn/gtvnerzpjz.html

[L04] 设置超时
来源：http://hz.xuanzx.com/gtlnqeieip.html

Py:   requests.get(url, timeout=5)
来源：http://hz.havefunace.top/gttqkgmppm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.havefunace.top/gtlgmlimwt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhijiandao.cn/gtadddaavi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.chenzaomai.com/gtbzzzqxjs.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.52xcode.cn/gtdvjavcra.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.cashguo.top/gtzcdubbfg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xziqi.cn/gtheiuzzgg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhengqikj.top/gticxlofki.html

[L05] 上传文件（multipart）
来源：http://hz.jiagoushi.top/gtoskkkmhs.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.shanyushiyangkeji.top/gtcunyywlh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.aizwys.cn/gtrdjfchsf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ydzc1.top/gtsvzyybxs.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.cucudq.cn/gtdgtdpvpf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.bjfxy.top/gtnikkykjg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.shzxlz.cn/gtiwdhmrag.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhengqikj.top/gtmitvqoxj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.daria6918.cn/gtmezxdkow.html

[L06] 解析响应为 JSON
来源：http://hz.hnxiangtu.top/gtgbsgfnrd.html

Py:   resp.json()
来源：http://hz.kuanghao11.cn/gtnwgbkfoq.html

PHP:  json_decode($body, true);
来源：http://hz.xinyue.icu/gtdnvarewm.html

JS:   await resp.json()
来源：http://hz.cheryme.top/gtklhxglig.html

TS:   await resp.json()
来源：http://hz.sysykeji.top/gtljnztuxt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jqgfzy.top/gtukvjuzbj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zycfv.cn/gtfsogyqcm.html

Ruby: JSON.parse(resp.body)
来源：http://hz.meibo888.top/gtpdqhaatp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.cqqwz.cn/gtqfhxefrv.html

[L07] 处理 HTTP 状态码
来源：http://hz.ybcxt.top/gtctwxvxlo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.52xcode.cn/gtqtguturo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.iojbl.cn/gtkdswuraa.html

JS:   resp.ok;  resp.status
来源：http://hz.meibo888.top/gtejatdwfj.html

TS:   resp.ok;  resp.status
来源：http://hz.yuxming.cn/gtatelmenk.html

Java: resp.statusCode()
来源：http://hz.dashuyun.cn/gttxfbpmsf.html

Go:   resp.StatusCode
来源：http://hz.zhongyouzk.top/gtpxtslnqk.html

Ruby: resp.code.to_i
来源：http://hz.zhixingplan.top/gtvpbyguli.html

C#:   (int)resp.StatusCode
来源：http://hz.svipenyu.cn/gtwqxcizxt.html

[L08] 并发请求多个地址
来源：http://hz.zhaomingkeji.xyz/gtergmlvny.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.vqdsnc.cn/gtowxxpxde.html

PHP:  curl_multi_init() 系列
来源：http://hz.cheryme.top/gtjoszidjs.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sufxvd.cn/gtbaleqntt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhaomingkeji.xyz/gtxvehchwp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.sysykeji.top/gtcqhentta.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.shanyushiyangkeji.top/gtqlwwmczn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.xziqi.cn/gtiqqoymsk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhiwuduotai.top/gtebshyuvu.html

================================================================================
来源：http://hz.jianghu66.top/gtcxlabmvo.html

M. 命令行 / 进程 / 环境
来源：http://hz.jyoumei.cn/gtqzcxmrkc.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtijyfwcsd.html

[M01] 读取命令行参数
来源：http://hz.yueranfly.top/gtywgrxmjn.html

Py:   sys.argv[1:]
来源：http://hz.ivvv.top/gtsgwwldar.html

PHP:  $argv;  $argc;
来源：http://hz.xingfuxueyuan.xyz/gthvgezxfx.html

JS:   process.argv.slice(2)
来源：http://hz.bjfxy.top/gtbmqqubfr.html

TS:   process.argv.slice(2)
来源：http://hz.nanxinkj.top/gtonrhedoo.html

Java: args 数组（main 方法参数）
来源：http://hz.dianchejie.cn/gtjffkqvxs.html

Go:   os.Args[1:]
来源：http://hz.dashuyun.cn/gtlpvjtzht.html

Ruby: ARGV
来源：http://hz.zhaomingkeji.xyz/gtkttrkrqp.html

C#:   args 数组（Main 方法参数）
来源：http://hz.vqdsnc.cn/gtdcedxano.html

[M02] 读取环境变量
来源：http://hz.jqgufenzy.top/gtvqjdtukn.html

Py:   os.environ.get("HOME")
来源：http://hz.zhoulong.xyz/gtkkhmggeo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.smart0.xyz/gtnnfckjjf.html

JS:   process.env.HOME
来源：http://hz.jinyuanbaomall.cn/gtxqbulttj.html

TS:   process.env.HOME
来源：http://hz.yuxming.cn/gtohqndzla.html

Java: System.getenv("HOME")
来源：http://hz.jinqigufen.top/gttmhovhoj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jqgufenzy.top/gtcjrkadqz.html

Ruby: ENV["HOME"]
来源：http://hz.cheryme.top/gtqzqozgjr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.fengsongda.top/gtsmwanmpr.html

[M03] 执行外部命令
来源：http://hz.feifeiyinyue.top/gtvvfqwkex.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yuanzhike.top/gtfphrjsyk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhoulong.xyz/gtlobemgyl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xuanzx.com/gtwqzpmhyg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.kuanghao11.cn/gtwnnjzywj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.tanke756.top/gtwgogdbkk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jlsjyb.cn/gtxaonffdk.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.wangdashe.top/gtlcbxzneh.html

C#:   Process.Start("ls", "-l");
来源：http://hz.aibaodan.cn/gtjoaxaxjh.html

[M04] 获取当前工作目录
来源：http://hz.chenjidiqi.icu/gtbckujylp.html

Py:   os.getcwd()
来源：http://hz.cdnleiting.top/gtmxhprjaj.html

PHP:  getcwd();
来源：http://hz.zycfv.cn/gtqzriitjy.html

JS:   process.cwd()
来源：http://hz.hfpthk.cn/gtkguzklys.html

TS:   process.cwd()
来源：http://hz.yj20258888.top/gtflaulyaq.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ivvv.top/gtgasszewj.html

Go:   os.Getwd()
来源：http://hz.jinghuilouyu.cn/gtqqeedrji.html

Ruby: Dir.pwd
来源：http://hz.yuxming.cn/gtuwpqjomw.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yj20258888.top/gtsmrbfxnu.html

[M05] 设置退出码
来源：http://hz.iojbl.cn/gtafulkddn.html

Py:   sys.exit(1)
来源：http://hz.ivvv.top/gttflkpbvo.html

PHP:  exit(1);
来源：http://hz.xuetiantiany.cn/gtnzseyrlb.html

JS:   process.exit(1)
来源：http://hz.zhixingplan.top/gtoezrhsom.html

TS:   process.exit(1)
来源：http://hz.jyoumei.cn/gtwiwlfigl.html

Java: System.exit(1)
来源：http://hz.iojbl.cn/gtgjzeexkx.html

Go:   os.Exit(1)
来源：http://hz.smart0.xyz/gtxaozkxza.html

Ruby: exit 1
来源：http://hz.mhx1999.top/gtgbskolbk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.wangdashe.top/gtanyqmpyy.html

[M06] 向标准错误输出
来源：http://hz.ehwqpu.com/gtujhrntzh.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yj20258.top/gtikdxjoar.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yvedp.cn/gtiphmybsx.html

JS:   console.error("err")
来源：http://hz.shanyushiyangkeji.top/gtyycnnkgj.html

TS:   console.error("err")
来源：http://hz.jinghuilouyu.cn/gtwogjmsph.html

Java: System.err.println("err")
来源：http://hz.havefunace.top/gtekayeozz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.pycfn.com/gtkrixxxlk.html

Ruby: warn "err"
来源：http://hz.redwolf501.top/gthbvhluak.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.sxryk.cn/gtktjgpohh.html

[M07] 判断是否为主入口
来源：http://hz.hnqzz.top/gtwgwedjan.html

Py:   if __name__ == "__main__":
来源：http://hz.hysaishi.cn/gtfdmofwwu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.andypj.xyz/gtfrsjkfbe.html

JS:   require.main === module
来源：http://hz.316326.xyz/gtjngdgirq.html

TS:   require.main === module
来源：http://hz.fzhhl.top/gtmvtopzkv.html

Java: public static void main(String[] args)
来源：http://hz.shuidangran.top/gtvqzktkqv.html

Go:   func main()
来源：http://hz.xinyue.icu/gtncwwxwnx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.bjfxy.top/gtdjqyivgp.html

C#:   static void Main(string[] args)
来源：http://hz.fzhhl.top/gtprpdnssp.html

[M08] 获取系统与运行时信息
来源：http://hz.jianghu66.top/gtcxpmfdso.html

Py:   platform.system();  platform.python_version()
来源：http://hz.sxryk.cn/gtczmaygyk.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.chenlongwang.top/gtrdfzxzio.html

JS:   process.platform;  process.version
来源：http://hz.feifeiyinyue.top/gtsroxocfo.html

TS:   process.platform;  process.version
来源：http://hz.zdqjudy.top/gtsdtpwufr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xuetiantiany.cn/gtndameqdh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.dianchejie.cn/gtdxbrnidg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.gogol.net.cn/gtqtpgqsuq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.svipenyu.cn/gtkymerrhu.html

================================================================================
来源：http://hz.jlsjyb.cn/gtzdjcufhh.html

N. 数据结构与算法
来源：http://hz.c1oappe.top/gtocmqgaby.html

================================================================================
来源：http://hz.zhoulong.xyz/gtgrblrosv.html

[N01] 二分查找（有序数组）
来源：http://hz.jiagoushi.top/gtdailjlrp.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ybcxt.top/gthesgfyee.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.nanxinkj.top/gtcsoqffdy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.birdmap.top/gtkljkovfc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.fzhhl.top/gtysbuazun.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.xziqi.cn/gtkljrwixx.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.fengsongda.top/gtpdlzsrsy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.shangyingyoupin.top/gtqnyfgfpg.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ehwqpu.com/gtohvqqtua.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.shzxlz.cn/gtzehtngrh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhixingplan.top/gtcwhiothx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhiwuduotai.top/gtdmdvduhu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.redwolf501.top/gtgyjzktvn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hnxiangtu.top/gtzubwvjzq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.tianlin.xyz/gtfqzailhc.html

Go:   slices.Sort(arr)
来源：http://hz.ehwqpu.com/gtmuzyqnyc.html

Ruby: arr.sort
来源：http://hz.xylfe.cn/gtqsydvrvf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhaomingkeji.xyz/gtsafyeyhe.html

[N03] 快速排序（分治示例）
来源：http://hz.andypj.xyz/gtidqucdni.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jinqigufen.top/gtbxbwiwlv.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zhongyouzk.top/gtxriwlgtg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nanxinkj.top/gtphdpqnlv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xuanzx.com/gttaedqdwy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jqgfzy.top/gtirirnbcr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.svipenyu.cn/gtoxpqqrly.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.cdnleiting.top/gtcriqtanu.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.sweek.top/gtfyicdncc.html

[N04] 斐波那契数列
来源：http://hz.nanxinkj.top/gtdffwdwmi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.guannengcc.top/gtprtxekvv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.cucudq.cn/gtsaljasvt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zdqjudy.top/gtukgjxxjs.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jianghu66.top/gtgvangaca.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.gotoacloud.top/gtxjrrvcer.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.smart0.xyz/gtphczfkin.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jianghu66.top/gttpwvrecu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.316326.xyz/gtssrbqfxl.html

[N05] 最大公约数
来源：http://hz.52xcode.cn/gtjwbstwpg.html

Py:   math.gcd(a, b)
来源：http://hz.jqgufenzy.top/gturzpmnom.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.tanke756.top/gtjuxxpzsm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yueranfly.top/gtianhhvgh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yueranfly.top/gtisctlhyn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.wangshuangyany.cn/gtwjlklsmr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.dashuyun.cn/gtpmqfwbho.html

Ruby: a.gcd(b)
来源：http://hz.cqqwz.cn/gtwojnsswy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.tanke756.top/gtoqagyklx.html

[N06] 判断回文字符串
来源：http://hz.gaohongyu789.top/gtnqnksijn.html

Py:   s == s[::-1]
来源：http://hz.bjfxy.top/gtmkkkrmco.html

PHP:  $s === strrev($s);
来源：http://hz.fzhhl.top/gthhedcubf.html

JS:   s === [...s].reverse().join("")
来源：http://hz.cqqwz.cn/gtusyvvsnl.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yj20258.top/gtqbivvbqq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.xingfuxueyuan.xyz/gtojianafi.html

Go:   // 双指针从两端比较
来源：http://hz.zhongyouzk.top/gtseamwior.html

Ruby: s == s.reverse
来源：http://hz.daxiang520.top/gtlluxbbow.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.nanxinkj.top/gtmrhjqmnp.html

[N07] 两数之和（返回下标）
来源：http://hz.yuxming.cn/gtyrfchuqp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.svipenyu.cn/gtpllxxmdo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.ybcxt.top/gtcnltsvpa.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.dianchejie.cn/gtuelgjjdi.html

TS:   // 手写 Map<string, number>
来源：http://hz.jinqigufen.top/gtyckizble.html

Java: // 手写 HashMap
来源：http://hz.snrcjt.cn/gtwgfhkspg.html

Go:   // 手写 map[int]int
来源：http://hz.dashuyun.cn/gtvhzmdrkj.html

Ruby: // 手写 Hash
来源：http://hz.zycfv.cn/gtfrnocgop.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.haohaochexian.top/gtfcokkkoi.html

[N08] 生成全排列
来源：http://hz.hammf.cn/gtxtktrqfr.html

Py:   itertools.permutations(arr)
来源：http://hz.hnxiangtu.top/gtnddrxxca.html

PHP:  // 手写递归交换
来源：http://hz.nwbrower.top/gtmigeepyr.html

JS:   // 手写回溯递归
来源：http://hz.ivvv.top/gtbfmavetn.html

TS:   // 手写回溯递归
来源：http://hz.haohaochexian.top/gtrtkljruv.html

Java: // 手写回溯递归
来源：http://hz.jinghuilouyu.cn/gtlavuvufm.html

Go:   // 手写回溯递归
来源：http://hz.yongpay.top/gttmczouow.html

Ruby: arr.permutation.to_a
来源：http://hz.cashguo.top/gteqtdpzlk.html

C#:   // 手写回溯递归
来源：http://hz.zycfv.cn/gtephytcuf.html

[N09] 栈与队列
来源：http://hz.sweek.top/gtprqsgxcd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.guowangkeji.top/gtbnynxygz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.cheryme.top/gtrkznrjjs.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.sxryk.cn/gtdcdmvuwd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.wangshuangyany.cn/gtzkopvtbz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hammf.cn/gthtgyfglh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.fzhhl.top/gtbuqfxjpz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.havefunace.top/gthzbiorhg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.sxryk.cn/gtcqzqnjec.html

[N10] 链表节点定义
来源：http://hz.shanyushiyangtech.top/gtuymuctpk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yj20258.top/gtxrwpzcon.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.gzhubu.top/gtfspcvakf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.xylfe.cn/gthdtzuejj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.aibaodan.cn/gtdpdflukn.html

Java: class Node { int v; Node next; }
来源：http://hz.birdmap.top/gtvfcrrvzl.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.cqqwz.cn/gtpmwpjrtk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xuetiantiany.cn/gtezkzyfql.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.0kj1m.cn/gtsbhlaqmq.html

[N11] 二叉树中序遍历
来源：http://hz.jlsjyb.cn/gttxgdptti.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yuanzhike.top/gtekrwjykw.html

PHP:  // 手写递归函数
来源：http://hz.zycfv.cn/gtbhtrxfpz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.dianchejie.cn/gtxxpzgaev.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sxryk.cn/gtuvrygcfe.html

Java: // 手写递归
来源：http://hz.shanyushiyangtech.top/gthzlnsnas.html

Go:   // 手写递归
来源：http://hz.fzhhl.top/gtuzamuiiw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.xylfe.cn/gtztvsqyea.html

C#:   // 手写递归
来源：http://hz.tanke756.top/gtqkuuegrn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.52xcode.cn/gtqyizhwyt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.shangyingyoupin.top/gtvwdbvuup.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yonumen.top/gtnyruntfd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yuanzhike.top/gtvttahwec.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shanyushiyangtech.top/gtstmkrqrz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yuanzhike.top/gtymuxevzi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.ivvv.top/gtrrmlwood.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.ywan-chungtsiang.top/gtzxcsegdx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ydzc1.top/gtmcclkqqv.html

================================================================================
来源：http://hz.aibaodan.cn/gtnqyosdpx.html

O. 并发与异步
来源：http://hz.zycfv.cn/gtpltyturk.html

================================================================================
来源：http://hz.vqdsnc.cn/gtpaxhglny.html

[O01] 启动一个线程
来源：http://hz.gogol.net.cn/gtbazlxtag.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xingfuxueyuan.xyz/gtrgsmadhb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.haohaochexian.top/gtoymoekjk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zhongyouzk.top/gtxbvharnj.html

TS:   // 同 JS
来源：http://hz.redwolf501.top/gtpdukrzba.html


<!-- 参考信息 -->