代发 wailian999

[K06] 解析 URL 查询串
来源：http://hz.zhaomingkeji.xyz/gttmbexxdk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.guowangkeji.top/gtugmzccuk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.ppjwa.cn/gtfajedmyl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.chenlongwang.top/gtueazmuaf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hysaishi.cn/gtyvvklayx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.pycfn.com/gtaclpbtew.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.aizwys.cn/gtpyaraikq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.9152youxi.cn/gtthmakurn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.tian-w.cn/gttlihfybd.html

[K07] 进制转换
来源：http://hz.shanyushiyangkeji.top/gtbzqbcxwc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.haohaochexian.top/gtqhjxgaae.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.wangdashe.top/gtzkfrhmpz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shanyushiyangkeji.top/gtnqjnglve.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.nanxuanxn.top/gtjtyqkgxh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ydjk.org.cn/gtxojkxveh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.316326.xyz/gtqewvhaem.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.0kj1m.cn/gtkhszodiu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhongyouzk.top/gtvxxaynvx.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhoulong.xyz/gtnshghizx.html

Py:   pickle.dumps(obj)
来源：http://hz.shzxlz.cn/gtsuzvfgdq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.guowangkeji.top/gtvzhnaprt.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.gogol.net.cn/gtooiiobxh.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ydzc1.top/gtwwromjkv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.shanyushiyangtech.top/gtbaymjusp.html

Go:   encoding/gob
来源：http://hz.zhaomingkeji.xyz/gtnjbjhxzx.html

Ruby: Marshal.dump(obj)
来源：http://hz.gaohongyu789.top/gtyyqlkmun.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.chenzaomai.com/gtqzylqqrz.html

================================================================================
来源：http://hz.mhx1999.top/gtbzpdlvii.html

L. 网络请求
来源：http://hz.vqdsnc.cn/gtvirbhejf.html

================================================================================
来源：http://hz.hysaishi.cn/gtmwdoqbur.html

[L01] 发送 GET 请求
来源：http://hz.cucudq.cn/gtdgajeceb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.snrcjt.cn/gtfhpndysa.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.mhx1999.top/gtvkbgrtih.html

JS:   await fetch(url)
来源：http://hz.jqgufenzy.top/gtyqixwbno.html

TS:   await fetch(url)
来源：http://hz.zhoulong.xyz/gtaylkwgjg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yj202588.top/gtteuvyoqv.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhijiandao.cn/gtfnbosulh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.aibaodan.cn/gtrhvzskhq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zycfv.cn/gttzslursl.html

[L02] 发送 POST JSON
来源：http://hz.redwolf501.top/gtxfngtsil.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.cdnleiting.top/gtqlcllcwv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jinyuanbaomall.cn/gtynfqbqvi.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cucudq.cn/gtwdcxygab.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yj20258888.top/gtrxsfyanp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.cheryme.top/gtoikvgqxz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jiagoushi.top/gtdnnhwaaw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yj20258888.top/gtgnopgfve.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yonumen.top/gtwmrqbsoz.html

[L03] 设置自定义请求头
来源：http://hz.cheryme.top/gtypzkjjhh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.pycfn.com/gtkfybtuvd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.nanxuanxn.top/gtiphtjobh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.pycfn.com/gtlgccrapr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jyoumei.cn/gtepigkwnn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jyoumei.cn/gtozafnvzw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.gotoacloud.top/gtbhuduxls.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yonumen.top/gtdiltnpwu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jinghuilouyu.cn/gtslyjxsln.html

[L04] 设置超时
来源：http://hz.ywan-chungtsiang.top/gtcbjebdaf.html

Py:   requests.get(url, timeout=5)
来源：http://hz.wangshuangyany.cn/gtlyyrjzkd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.aibaodan.cn/gtzivfkkoq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.52xcode.cn/gtxqgklyqg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cashguo.top/gtorkpobtw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jianghu66.top/gtfriojwsy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yj20258.top/gthllqqfkb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ywan-chungtsiang.top/gtygywhnva.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yj202588.top/gtumkxbcto.html

[L05] 上传文件（multipart）
来源：http://hz.daria6918.cn/gtfglxzobv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jlsjyb.cn/gtemscxjis.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.vqdsnc.cn/gtvkjvhxjd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.316326.xyz/gtmqdbwtgr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yangfankeji.com/gtaqwemoix.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xuanzx.com/gtrpfnnmoy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.meibo888.top/gtsrorgawq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yj20258888.top/gtnnstromw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.sysykeji.top/gtvebvmcoi.html

[L06] 解析响应为 JSON
来源：http://hz.yj20258888.top/gtraskabkd.html

Py:   resp.json()
来源：http://hz.shanyushiyangkeji.top/gtvabbpdeg.html

PHP:  json_decode($body, true);
来源：http://hz.yj202588.top/gtxysabdua.html

JS:   await resp.json()
来源：http://hz.birdmap.top/gtwfizxntm.html

TS:   await resp.json()
来源：http://hz.yj20258.top/gthnuoiufn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.xinyue.icu/gtdwnclcrm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.kuanghao11.cn/gtuadyxlia.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yuanzhike.top/gtjystkcqq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.52xcode.cn/gtxhjycnrw.html

[L07] 处理 HTTP 状态码
来源：http://hz.shanyushiyangtech.top/gtmcyxmozf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.haohaochexian.top/gttzeqowaa.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ehwqpu.com/gtbtswvzew.html

JS:   resp.ok;  resp.status
来源：http://hz.yueranfly.top/gtrgodizxb.html

TS:   resp.ok;  resp.status
来源：http://hz.fengsongda.top/gtnrnfpzga.html

Java: resp.statusCode()
来源：http://hz.cqqwz.cn/gtrkhbhvzq.html

Go:   resp.StatusCode
来源：http://hz.hywenlv.cn/gtmjtifeyw.html

Ruby: resp.code.to_i
来源：http://hz.nanxuanxn.top/gtawjjejir.html

C#:   (int)resp.StatusCode
来源：http://hz.hongshengwenyu.top/gtbhvzqouh.html

[L08] 并发请求多个地址
来源：http://hz.gzhubu.top/gtiifvrsps.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hfpthk.cn/gtilpdaqzi.html

PHP:  curl_multi_init() 系列
来源：http://hz.daxiang520.top/gtomguvwzm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cqqwz.cn/gttwsxhafz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nanxinkj.top/gtvtywhgpu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yangfankeji.com/gtllhqtanu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xylfe.cn/gtpmpkzznz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.c1oappe.top/gtriuvrmrq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zdqjudy.top/gtjefqpaev.html

================================================================================
来源：http://hz.jinqigufen.top/gtgalhgdva.html

M. 命令行 / 进程 / 环境
来源：http://hz.chenzaomai.com/gtezrlskbw.html

================================================================================
来源：http://hz.yj20258888.top/gtxsjbtcdz.html

[M01] 读取命令行参数
来源：http://hz.gzhubu.top/gtqcjmilus.html

Py:   sys.argv[1:]
来源：http://hz.yj202588.top/gtxttahymf.html

PHP:  $argv;  $argc;
来源：http://hz.xinyue.icu/gtunnjsdfv.html

JS:   process.argv.slice(2)
来源：http://hz.bjfxy.top/gtlsmmnacr.html

TS:   process.argv.slice(2)
来源：http://hz.snrcjt.cn/gtegbrblho.html

Java: args 数组（main 方法参数）
来源：http://hz.xuanzx.com/gtvfbikugx.html

Go:   os.Args[1:]
来源：http://hz.zhaomingkeji.xyz/gtsvsnbxdo.html

Ruby: ARGV
来源：http://hz.vqdsnc.cn/gtiocsgvuq.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yj20258888.top/gtiqxopljf.html

[M02] 读取环境变量
来源：http://hz.jqgfzy.top/gttewusnnc.html

Py:   os.environ.get("HOME")
来源：http://hz.jyoumei.cn/gtjshccfds.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.nwbrower.top/gtkrkppbgn.html

JS:   process.env.HOME
来源：http://hz.tian-w.cn/gthhfaiyml.html

TS:   process.env.HOME
来源：http://hz.zdqjudy.top/gtthjyffdt.html

Java: System.getenv("HOME")
来源：http://hz.hammf.cn/gtqxwybeib.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.ybcxt.top/gtnucltzbx.html

Ruby: ENV["HOME"]
来源：http://hz.yangfankeji.com/gtdguhvxht.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yanxiufei.cn/gtqhqtituz.html

[M03] 执行外部命令
来源：http://hz.yj20258888.top/gtutrsimql.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.cqqwz.cn/gtwrvwmmmp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.guannengcc.top/gteqqupkci.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yuanzhike.top/gtzfwakslw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.wangshuangyany.cn/gtphdbksew.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ywan-chungtsiang.top/gtdmhaaejd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zycfv.cn/gtvpijzdif.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.cheryme.top/gtxxlpakzh.html

C#:   Process.Start("ls", "-l");
来源：http://hz.316326.xyz/gtyntaicmf.html

[M04] 获取当前工作目录
来源：http://hz.yvedp.cn/gtmdnxifmp.html

Py:   os.getcwd()
来源：http://hz.tanke756.top/gttwasaxwk.html

PHP:  getcwd();
来源：http://hz.chenlongwang.top/gtirrrwvkt.html

JS:   process.cwd()
来源：http://hz.ywan-chungtsiang.top/gtwotrlbii.html

TS:   process.cwd()
来源：http://hz.jyoumei.cn/gthytbjzgd.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhijiandao.cn/gtidbkztsr.html

Go:   os.Getwd()
来源：http://hz.birdmap.top/gtdgnggrwg.html

Ruby: Dir.pwd
来源：http://hz.jiagoushi.top/gtwbwdtqky.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.shuidangran.top/gtrxetucsj.html

[M05] 设置退出码
来源：http://hz.jinghuilouyu.cn/gtzkdywpwn.html

Py:   sys.exit(1)
来源：http://hz.hfpthk.cn/gtxexjeemz.html

PHP:  exit(1);
来源：http://hz.zhaomingkeji.xyz/gtmxunafjc.html

JS:   process.exit(1)
来源：http://hz.xziqi.cn/gtidreriub.html

TS:   process.exit(1)
来源：http://hz.nwbrower.top/gtebziwvjx.html

Java: System.exit(1)
来源：http://hz.tian-w.cn/gtmkpijiax.html

Go:   os.Exit(1)
来源：http://hz.shzxlz.cn/gtblsqzymm.html

Ruby: exit 1
来源：http://hz.meibo888.top/gthusjufpq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jyoumei.cn/gtwfwawzkc.html

[M06] 向标准错误输出
来源：http://hz.hongshengwenyu.top/gthoxvtjqm.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jyoumei.cn/gtuxosxtyq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xinyue.icu/gtsbmbbulc.html

JS:   console.error("err")
来源：http://hz.mhx1999.top/gtwkbxvnqr.html

TS:   console.error("err")
来源：http://hz.xuanzx.com/gtadubmjfx.html

Java: System.err.println("err")
来源：http://hz.yvedp.cn/gtwpwaqfdg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhengqikj.top/gtaxuajlng.html

Ruby: warn "err"
来源：http://hz.aizwys.cn/gtfaxgylve.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ywan-chungtsiang.top/gtteanidmg.html

[M07] 判断是否为主入口
来源：http://hz.chenjidiqi.icu/gttbveszmn.html

Py:   if __name__ == "__main__":
来源：http://hz.cashguo.top/gtpknzjxpe.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ydzc1.top/gtnpnpbsys.html

JS:   require.main === module
来源：http://hz.yangfankeji.com/gtkbqbyojo.html

TS:   require.main === module
来源：http://hz.xuetiantiany.cn/gtfdoqwzkr.html

Java: public static void main(String[] args)
来源：http://hz.bjfxy.top/gtqcbwbsst.html

Go:   func main()
来源：http://hz.jqgufenzy.top/gtggsghiwz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.feifeiyinyue.top/gtfospxbvk.html

C#:   static void Main(string[] args)
来源：http://hz.svipenyu.cn/gtrjrptwvh.html

[M08] 获取系统与运行时信息
来源：http://hz.meibo888.top/gtghknwkcu.html

Py:   platform.system();  platform.python_version()
来源：http://hz.redwolf501.top/gtjlucgixf.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jinqigufen.top/gtonxzwslm.html

JS:   process.platform;  process.version
来源：http://hz.sxryk.cn/gttkqclycu.html

TS:   process.platform;  process.version
来源：http://hz.birdmap.top/gtsqzmuwrj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.0kj1m.cn/gtirtzbpaj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.c1oappe.top/gtdqicsyvt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.xuetiantiany.cn/gtdqdhlxpd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hnxiangtu.top/gtqmnhqtur.html

================================================================================
来源：http://hz.yj20258.top/gtalfxavoh.html

N. 数据结构与算法
来源：http://hz.yj20258888.top/gtdgmcxkdd.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtdzjhmovi.html

[N01] 二分查找（有序数组）
来源：http://hz.chenzaomai.com/gtwxsmqnjd.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.sxryk.cn/gtdqgtpqcf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hywenlv.cn/gtqfvyatao.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hammf.cn/gtjmwnzyww.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hfpthk.cn/gtpgokhdtg.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jianghu66.top/gtlqkxszff.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yj20258.top/gtvdorjqyj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.quarkkingdee.top/gtfvyswwqg.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yj202588.top/gthubzbaeo.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jianghu66.top/gtlrdxakbu.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.fzhhl.top/gtocukonxj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.daxiang520.top/gtdbrpwmfs.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.snrcjt.cn/gtmockvtqd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ydjk.org.cn/gtxweutxwr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.meibo888.top/gtkiksogom.html

Go:   slices.Sort(arr)
来源：http://hz.yongpay.top/gtxwafcojb.html

Ruby: arr.sort
来源：http://hz.hysaishi.cn/gtgaaadwbh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhijiandao.cn/gtzickgcju.html

[N03] 快速排序（分治示例）
来源：http://hz.yuxming.cn/gtyzkazdip.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.chenzaomai.com/gtkjxwyyrx.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zhixingplan.top/gtcnkkoiru.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.chenjidiqi.icu/gtshyvpkvo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinghuilouyu.cn/gtpaidaxec.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.chenzaomai.com/gtqxpnqjha.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yonumen.top/gtkkaqfygs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zycfv.cn/gtdawoovop.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jyoumei.cn/gtrpkdupgf.html

[N04] 斐波那契数列
来源：http://hz.zhixingplan.top/gtywbogcft.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.shangyingyoupin.top/gtceqxoruj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhongyouzk.top/gtksaqipzt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.dianchejie.cn/gtgafyqucz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.pengpengdd.cyou/gtvjjrnvdd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jinqigfzy.top/gtjpsjmgyj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.tian-w.cn/gtkpbuowug.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hfpthk.cn/gtntpjvgae.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.shanyushiyangtech.top/gtzebheymz.html

[N05] 最大公约数
来源：http://hz.cheryme.top/gtocgltaft.html

Py:   math.gcd(a, b)
来源：http://hz.zhijiandao.cn/gtnmkxatnx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.quarkkingdee.top/gtpsuyqflo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.fzhhl.top/gtaxikdwgs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hnxiangtu.top/gtenvxbeip.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.cqqwz.cn/gtjhuhdqfe.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hywenlv.cn/gtjcuwgkhf.html

Ruby: a.gcd(b)
来源：http://hz.jqgufenzy.top/gtkgbrzcop.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhijiandao.cn/gtuldncoeh.html

[N06] 判断回文字符串
来源：http://hz.jiagoushi.top/gtilobcobu.html

Py:   s == s[::-1]
来源：http://hz.pengpengdd.cyou/gtkvwxnbil.html

PHP:  $s === strrev($s);
来源：http://hz.dianchejie.cn/gtdtbtplbv.html

JS:   s === [...s].reverse().join("")
来源：http://hz.dashuyun.cn/gtiwtmxvqg.html

TS:   s === [...s].reverse().join("")
来源：http://hz.xingfuxueyuan.xyz/gttslpyefx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yj20258888.top/gtqylmqzib.html

Go:   // 双指针从两端比较
来源：http://hz.yongpay.top/gtfsyytzgk.html

Ruby: s == s.reverse
来源：http://hz.snrcjt.cn/gtuhipgqjt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.chenzaomai.com/gtmuleovzy.html

[N07] 两数之和（返回下标）
来源：http://hz.yongpay.top/gtabauznvn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.tanke756.top/gthijesqtb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.52xcode.cn/gtqjisqatb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.gogol.net.cn/gtobmzfklw.html

TS:   // 手写 Map<string, number>
来源：http://hz.52xcode.cn/gthmejwdzh.html

Java: // 手写 HashMap
来源：http://hz.cucudq.cn/gtrcznpaua.html

Go:   // 手写 map[int]int
来源：http://hz.fengsongda.top/gtpsgzywkr.html

Ruby: // 手写 Hash
来源：http://hz.c1oappe.top/gtwadsksdz.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.dashuyun.cn/gtirjmkgyn.html

[N08] 生成全排列
来源：http://hz.zhongyouzk.top/gtlvwoyapj.html

Py:   itertools.permutations(arr)
来源：http://hz.feifeiyinyue.top/gtvainuwkd.html

PHP:  // 手写递归交换
来源：http://hz.kuanghao11.cn/gthgbjyxma.html

JS:   // 手写回溯递归
来源：http://hz.zhaomingkeji.xyz/gtzgrlwuxx.html

TS:   // 手写回溯递归
来源：http://hz.svipenyu.cn/gtfywkllst.html

Java: // 手写回溯递归
来源：http://hz.ydjk.org.cn/gttklweiat.html

Go:   // 手写回溯递归
来源：http://hz.smart0.xyz/gtmowtlyjw.html

Ruby: arr.permutation.to_a
来源：http://hz.nanxuanxn.top/gtgycxxmfw.html

C#:   // 手写回溯递归
来源：http://hz.zdqjudy.top/gtuiqnttdp.html

[N09] 栈与队列
来源：http://hz.shzxlz.cn/gtczcyiisb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jqgfzy.top/gtajiuszza.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.guowangkeji.top/gtmayzomqe.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.iojbl.cn/gtbmazilny.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.nwbrower.top/gterfsldlb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.smart0.xyz/gtampevvkp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.fzhhl.top/gtavorxjwx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.316326.xyz/gtczldulni.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yj20258.top/gtssxvzvwj.html

[N10] 链表节点定义
来源：http://hz.ywan-chungtsiang.top/gtudvjhsor.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.nanxinkj.top/gtibiwhice.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jiagoushi.top/gtbfltyyaf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.chenzaomai.com/gtoilzzvvj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.ivvv.top/gtzhiifvsw.html

Java: class Node { int v; Node next; }
来源：http://hz.yuxming.cn/gtkdfpsock.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yj20258888.top/gthbabegmq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.ydzc1.top/gtmgbnkfmb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.chenjidiqi.icu/gtswtipxpy.html

[N11] 二叉树中序遍历
来源：http://hz.zdqjudy.top/gthxehskxf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jyoumei.cn/gtwyeiutnt.html

PHP:  // 手写递归函数
来源：http://hz.yueranfly.top/gtibieytto.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhaomingkeji.xyz/gtnxfpswso.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.haohaochexian.top/gtfxsdmgzf.html

Java: // 手写递归
来源：http://hz.0kj1m.cn/gtxsqyoctc.html

Go:   // 手写递归
来源：http://hz.zhoulong.xyz/gthamqraqw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.redwolf501.top/gtzryomgks.html

C#:   // 手写递归
来源：http://hz.sweek.top/gtdwotabog.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.shuidangran.top/gtwlbttisv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.chenzaomai.com/gtomoaokxh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.cdnleiting.top/gtzlracqnu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yanxiufei.cn/gtgamvgthx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.iojbl.cn/gtcxykyvdx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.vqdsnc.cn/gtqckllsba.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yueranfly.top/gtolyweejm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yvedp.cn/gtbsprmldt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jqgfzy.top/gtxaelaked.html

================================================================================
来源：http://hz.xinyue.icu/gtcjcglnic.html

O. 并发与异步
来源：http://hz.shanyushiyangkeji.top/gtfkjiuazr.html

================================================================================
来源：http://hz.shzxlz.cn/gtjdokunnd.html

[O01] 启动一个线程
来源：http://hz.tanke756.top/gtqduomeoi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.fzhhl.top/gtehtntzeq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.guowangkeji.top/gtexhiztsv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.guowangkeji.top/gtxhtsgqzq.html

TS:   // 同 JS
来源：http://hz.xylfe.cn/gtmizhxyic.html

Java: new Thread(() -> f()).start()
来源：http://hz.yuxming.cn/gtxjrtrvgc.html

Go:   go f()
来源：http://hz.quarkkingdee.top/gtbodtholo.html

Ruby: Thread.new { f }
来源：http://hz.aizwys.cn/gtscaqciks.html

C#:   Task.Run(() => F());
来源：http://hz.nanxuanxn.top/gtwtwztrvs.html


<!-- 参考信息 -->