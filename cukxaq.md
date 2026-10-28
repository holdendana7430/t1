代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.daxiang520.top/gtqmtixxyi.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yj202588.top/gtaazdcgos.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.pycfn.com/gtdvxnzoqv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ywan-chungtsiang.top/gtsmdnisnm.html

[K06] 解析 URL 查询串
来源：http://hz.cqqwz.cn/gthmzbzvtb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.tian-w.cn/gtghvjewyq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhongyouzk.top/gtqiyimglr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.quarkkingdee.top/gtaqctndcc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.aibaodan.cn/gtnrbyuytz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.meibo888.top/gtpspdtyoj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.iojbl.cn/gtcjrfjbgp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.gotoacloud.top/gtdiuxegqb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jinqigfzy.top/gtxhmalkxb.html

[K07] 进制转换
来源：http://hz.zhijiandao.cn/gtuycgdhng.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.feifeiyinyue.top/gtyrhlqjft.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hnqzz.top/gtcbtopirx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhijiandao.cn/gtttzjyldq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.wangshuangyany.cn/gtxsfnfohy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.snrcjt.cn/gtjwdacnyn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhiwuduotai.top/gtbxejfnli.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jinghuilouyu.cn/gtbimoaanb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hywenlv.cn/gtmjbmsqgb.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.gaohongyu789.top/gtefvwryuy.html

Py:   pickle.dumps(obj)
来源：http://hz.ivvv.top/gtfgljagos.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.cqqwz.cn/gtipvggbkt.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.sweek.top/gtamjwvovq.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.fengsongda.top/gtxkxdktud.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.cashguo.top/gtkxuktkuw.html

Go:   encoding/gob
来源：http://hz.xuanzx.com/gtmgsmnflv.html

Ruby: Marshal.dump(obj)
来源：http://hz.jyoumei.cn/gtfvbxvwjr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ydzc1.top/gtunqorcqw.html

================================================================================
来源：http://hz.yuanzhike.top/gtyzyoabhw.html

L. 网络请求
来源：http://hz.yj202588.top/gtnpltesuh.html

================================================================================
来源：http://hz.jqgfzy.top/gtkxwvgpzl.html

[L01] 发送 GET 请求
来源：http://hz.ydzc1.top/gtlbpjnzwk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hywenlv.cn/gthemuuvhm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.gzhubu.top/gtdkzpaxhf.html

JS:   await fetch(url)
来源：http://hz.pycfn.com/gtewovhhoy.html

TS:   await fetch(url)
来源：http://hz.zhengqikj.top/gtigbyayot.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yangfankeji.com/gtxlnlnqxh.html

Go:   resp, err := http.Get(url)
来源：http://hz.shanyushiyangkeji.top/gtungljkvc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.ywan-chungtsiang.top/gtksozarhp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.9152youxi.cn/gtrmszakau.html

[L02] 发送 POST JSON
来源：http://hz.pengpengdd.cyou/gtjqkjyomq.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.andypj.xyz/gtjdsvcucn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.chenzaomai.com/gtjxpacexz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.chenzaomai.com/gtbdbcrwqp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.birdmap.top/gtfucpcndg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.redwolf501.top/gtclqykumb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.sysykeji.top/gtoqbyjkjl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jinyuanbaomall.cn/gtczwzukqq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.birdmap.top/gtmmkbjdtd.html

[L03] 设置自定义请求头
来源：http://hz.jqgufenzy.top/gtgnkfazdx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhongyouzk.top/gteoohpraz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.wangshuangyany.cn/gthkjstukv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ydzc1.top/gtgrkklctm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yongpay.top/gtmplxzzjt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.andypj.xyz/gtzlyhtyox.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.tian-w.cn/gtsitimdyf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.shuidangran.top/gtdzhhxopc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.quarkkingdee.top/gtgcyanmro.html

[L04] 设置超时
来源：http://hz.nanxinkj.top/gtteybiyje.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jqgfzy.top/gtpyrlbylr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.guowangkeji.top/gtjzfhpqdz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.9152youxi.cn/gtxpeuingr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ywan-chungtsiang.top/gtvewslavm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.wangshuangyany.cn/gtdxzbjpmk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hfpthk.cn/gtpvjfdewx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.tanke756.top/gtgimkohrc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.gzhubu.top/gthitsrbec.html

[L05] 上传文件（multipart）
来源：http://hz.yangfankeji.com/gtgoanyzuk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.pycfn.com/gtgnmxbmnb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.gzhubu.top/gtrptlkpue.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hnxiangtu.top/gtyzcltksn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.meibo888.top/gtvgviwvkf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.snrcjt.cn/gthgcltloi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zycfv.cn/gthrknrasn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shanyushiyangtech.top/gtnjloalif.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.sufxvd.cn/gtysegfyyw.html

[L06] 解析响应为 JSON
来源：http://hz.yvedp.cn/gtjzudjxwj.html

Py:   resp.json()
来源：http://hz.xziqi.cn/gtqtmwngof.html

PHP:  json_decode($body, true);
来源：http://hz.hywenlv.cn/gtqtmvlnbb.html

JS:   await resp.json()
来源：http://hz.yueranfly.top/gtxqawhjdj.html

TS:   await resp.json()
来源：http://hz.xziqi.cn/gtwyzmjzkv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.aizwys.cn/gttskklfny.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.nwbrower.top/gtbhuorvdv.html

Ruby: JSON.parse(resp.body)
来源：http://hz.chenlongwang.top/gtwvklucbz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ivvv.top/gtqdpfixeh.html

[L07] 处理 HTTP 状态码
来源：http://hz.yuanzhike.top/gtugslombx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hysaishi.cn/gtavwkouth.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.aibaodan.cn/gtlwvpsojy.html

JS:   resp.ok;  resp.status
来源：http://hz.zhiwuduotai.top/gtqxunuetg.html

TS:   resp.ok;  resp.status
来源：http://hz.cheryme.top/gtwnuvonel.html

Java: resp.statusCode()
来源：http://hz.jlsjyb.cn/gttaxgqltn.html

Go:   resp.StatusCode
来源：http://hz.birdmap.top/gtxiixyntz.html

Ruby: resp.code.to_i
来源：http://hz.smart0.xyz/gtidcohlwp.html

C#:   (int)resp.StatusCode
来源：http://hz.dianchejie.cn/gtbnuhavsg.html

[L08] 并发请求多个地址
来源：http://hz.ydzc1.top/gtwvmzwivm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.shuidangran.top/gtkmhgzpcv.html

PHP:  curl_multi_init() 系列
来源：http://hz.pycfn.com/gtfgpcpmkx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hfpthk.cn/gtfzldwnqn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhiwuduotai.top/gtsvcjsaym.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhixingplan.top/gtbhebfwty.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhengqikj.top/gtknupccvw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.xinyue.icu/gttvvyxgzg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ybcxt.top/gttnxkdpud.html

================================================================================
来源：http://hz.guannengcc.top/gtrrcwwbtb.html

M. 命令行 / 进程 / 环境
来源：http://hz.yj20258.top/gttmnsrgzg.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtqnwohrkw.html

[M01] 读取命令行参数
来源：http://hz.ppjwa.cn/gthcorzivn.html

Py:   sys.argv[1:]
来源：http://hz.snrcjt.cn/gtwjlwtvyt.html

PHP:  $argv;  $argc;
来源：http://hz.gzhubu.top/gtrjtaehly.html

JS:   process.argv.slice(2)
来源：http://hz.feifeiyinyue.top/gtsaikpvrm.html

TS:   process.argv.slice(2)
来源：http://hz.svipenyu.cn/gtcewksyzw.html

Java: args 数组（main 方法参数）
来源：http://hz.9152youxi.cn/gtbbdvydgu.html

Go:   os.Args[1:]
来源：http://hz.guannengcc.top/gtfoouspvs.html

Ruby: ARGV
来源：http://hz.ybcxt.top/gtedywxxqv.html

C#:   args 数组（Main 方法参数）
来源：http://hz.shanyushiyangtech.top/gtomkdeiaj.html

[M02] 读取环境变量
来源：http://hz.mhx1999.top/gtltxlzrgv.html

Py:   os.environ.get("HOME")
来源：http://hz.ybcxt.top/gtqtozgcdn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zhijiandao.cn/gtpmaeeacz.html

JS:   process.env.HOME
来源：http://hz.zhaomingkeji.xyz/gttpdogklx.html

TS:   process.env.HOME
来源：http://hz.zdqjudy.top/gthhcuxguo.html

Java: System.getenv("HOME")
来源：http://hz.dashuyun.cn/gtfdxhukoj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.pycfn.com/gtrjasqklx.html

Ruby: ENV["HOME"]
来源：http://hz.xingfuxueyuan.xyz/gtenwoenpz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhiwuduotai.top/gtyoahpcyk.html

[M03] 执行外部命令
来源：http://hz.yanxiufei.cn/gtfcsqugru.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.dashuyun.cn/gtngwoavql.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.tanke756.top/gtmcoickah.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.52xcode.cn/gtczdjmkxj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.meibo888.top/gthjxdmsuz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jianghu66.top/gtcjowibmm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yonumen.top/gtdkxcelyl.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.redwolf501.top/gtgxzjfgrt.html

C#:   Process.Start("ls", "-l");
来源：http://hz.sweek.top/gtbxyapiqb.html

[M04] 获取当前工作目录
来源：http://hz.hammf.cn/gtubwlyvrz.html

Py:   os.getcwd()
来源：http://hz.yuxming.cn/gtyicuavio.html

PHP:  getcwd();
来源：http://hz.cqqwz.cn/gtefvoliga.html

JS:   process.cwd()
来源：http://hz.nanxinkj.top/gtcnyoheoh.html

TS:   process.cwd()
来源：http://hz.zhiwuduotai.top/gtgtqoboyn.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yj202588.top/gtdozwfldv.html

Go:   os.Getwd()
来源：http://hz.guowangkeji.top/gtvkymymct.html

Ruby: Dir.pwd
来源：http://hz.316326.xyz/gtessutvlj.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.c1oappe.top/gtukmbhxjk.html

[M05] 设置退出码
来源：http://hz.havefunace.top/gtbycmdgay.html

Py:   sys.exit(1)
来源：http://hz.xuetiantiany.cn/gtehquqges.html

PHP:  exit(1);
来源：http://hz.guannengcc.top/gtpmyrxfqz.html

JS:   process.exit(1)
来源：http://hz.xinyue.icu/gtqueuiwcg.html

TS:   process.exit(1)
来源：http://hz.ydzc1.top/gtkuclldjv.html

Java: System.exit(1)
来源：http://hz.guowangkeji.top/gtkvikgkcj.html

Go:   os.Exit(1)
来源：http://hz.jqgfzy.top/gtffsfuqiq.html

Ruby: exit 1
来源：http://hz.pengpengdd.cyou/gtofvgwtxb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jqgfzy.top/gtguugpady.html

[M06] 向标准错误输出
来源：http://hz.ehwqpu.com/gtqjgsbgmj.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hongshengwenyu.top/gtlkdpwwyt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yvedp.cn/gtzfwdnrki.html

JS:   console.error("err")
来源：http://hz.pycfn.com/gtbhmdrifg.html

TS:   console.error("err")
来源：http://hz.nanxinkj.top/gthjmsaxgr.html

Java: System.err.println("err")
来源：http://hz.yangfankeji.com/gthfethvnh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhiwuduotai.top/gtrwshqbwz.html

Ruby: warn "err"
来源：http://hz.0kj1m.cn/gtifnsigtj.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.0kj1m.cn/gttqqjhlas.html

[M07] 判断是否为主入口
来源：http://hz.gzhubu.top/gtembhpfun.html

Py:   if __name__ == "__main__":
来源：http://hz.zhoulong.xyz/gtxovbvgnj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cucudq.cn/gtwfysncfo.html

JS:   require.main === module
来源：http://hz.dashuyun.cn/gtrokwpnlj.html

TS:   require.main === module
来源：http://hz.guowangkeji.top/gtrwhpskmi.html

Java: public static void main(String[] args)
来源：http://hz.fengsongda.top/gtknepstax.html

Go:   func main()
来源：http://hz.zhaomingkeji.xyz/gtulzzeuwl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yonumen.top/gtsgreohlf.html

C#:   static void Main(string[] args)
来源：http://hz.zhongyouzk.top/gtjnqtgfqz.html

[M08] 获取系统与运行时信息
来源：http://hz.xylfe.cn/gtoxcmmfmx.html

Py:   platform.system();  platform.python_version()
来源：http://hz.iojbl.cn/gtplzhidis.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yuxming.cn/gteapgoapd.html

JS:   process.platform;  process.version
来源：http://hz.cashguo.top/gthjmmgmcc.html

TS:   process.platform;  process.version
来源：http://hz.cheryme.top/gtchngxvzp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.ybcxt.top/gtvyrtdfqt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.nanxinkj.top/gtzxfrxjdx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.c1oappe.top/gtgninxehf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.wangdashe.top/gtwbuaezos.html

================================================================================
来源：http://hz.gaohongyu789.top/gtmcwhbcdf.html

N. 数据结构与算法
来源：http://hz.yangfankeji.com/gtlsiwnugc.html

================================================================================
来源：http://hz.jinqigfzy.top/gtjmkznral.html

[N01] 二分查找（有序数组）
来源：http://hz.ywan-chungtsiang.top/gttbxrqrrx.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.birdmap.top/gtaoqkdqmm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jinqigfzy.top/gtfxtizmey.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sweek.top/gtptzopxtj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hnqzz.top/gtukfsqygp.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jianghu66.top/gtfrecamgu.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.vqdsnc.cn/gtsesoeofs.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhaomingkeji.xyz/gtcnmrrbyv.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ehwqpu.com/gtaaowerue.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yvedp.cn/gtecjexhtp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenlongwang.top/gtxecozhph.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hammf.cn/gtjmpctibu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gogol.net.cn/gtpwkaoagx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hfpthk.cn/gtbxfnrhti.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hywenlv.cn/gtuvlkqfvk.html

Go:   slices.Sort(arr)
来源：http://hz.xylfe.cn/gtjgvprimz.html

Ruby: arr.sort
来源：http://hz.yj202588.top/gtuhniqfoj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.sysykeji.top/gtioacocrv.html

[N03] 快速排序（分治示例）
来源：http://hz.smart0.xyz/gtubmwehuz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.shanyushiyangtech.top/gtmxlpcnax.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zycfv.cn/gtzpyhpybi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hammf.cn/gtubittymc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.andypj.xyz/gtxqlrpxka.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhiwuduotai.top/gtkfkbazbn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.cqqwz.cn/gtljlbatlw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.0kj1m.cn/gtclfwistg.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.havefunace.top/gttmihsiuc.html

[N04] 斐波那契数列
来源：http://hz.smart0.xyz/gtmrejybil.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ydzc1.top/gtzyulmobx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jinqigfzy.top/gtvovkadvh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.haohaochexian.top/gtqaalmcca.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hnxiangtu.top/gtvlhsagas.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.cucudq.cn/gtkpelehiz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.nanxuanxn.top/gtwctfquch.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.dashuyun.cn/gtyhqqiigu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.andypj.xyz/gtbhdobfqe.html

[N05] 最大公约数
来源：http://hz.gogol.net.cn/gtesfhtumz.html

Py:   math.gcd(a, b)
来源：http://hz.wangdashe.top/gtxfymhoir.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.pycfn.com/gtssbgfqvv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.fengsongda.top/gtclpawrng.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hysaishi.cn/gtfkzrrrzj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yongpay.top/gtwvvjppnz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jyoumei.cn/gtagankhhl.html

Ruby: a.gcd(b)
来源：http://hz.guowangkeji.top/gtpqjlkkwx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.pycfn.com/gtbxforqbk.html

[N06] 判断回文字符串
来源：http://hz.9152youxi.cn/gtwvneqkul.html

Py:   s == s[::-1]
来源：http://hz.chenjidiqi.icu/gtzigyljba.html

PHP:  $s === strrev($s);
来源：http://hz.havefunace.top/gtmqieshut.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zdqjudy.top/gtugdzqxct.html

TS:   s === [...s].reverse().join("")
来源：http://hz.pengpengdd.cyou/gtzjpjhpvk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.hfpthk.cn/gtucroapoy.html

Go:   // 双指针从两端比较
来源：http://hz.xylfe.cn/gtatmtpxbu.html

Ruby: s == s.reverse
来源：http://hz.dashuyun.cn/gtdcnearpd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhixingplan.top/gtwskdsfbv.html

[N07] 两数之和（返回下标）
来源：http://hz.jianghu66.top/gtkhcikraw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ehwqpu.com/gtkgczuzzg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.chenlongwang.top/gtpnplavzl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.sweek.top/gtmjbpjnsk.html

TS:   // 手写 Map<string, number>
来源：http://hz.zhongyouzk.top/gtmyasbrhc.html

Java: // 手写 HashMap
来源：http://hz.zhengqikj.top/gtcqvmmpmu.html

Go:   // 手写 map[int]int
来源：http://hz.yuanzhike.top/gtmgdbziar.html

Ruby: // 手写 Hash
来源：http://hz.hnxiangtu.top/gtetisusau.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jianghu66.top/gtplioujah.html

[N08] 生成全排列
来源：http://hz.svipenyu.cn/gtwqzuwrky.html

Py:   itertools.permutations(arr)
来源：http://hz.bjfxy.top/gtsrmcaudw.html

PHP:  // 手写递归交换
来源：http://hz.yvedp.cn/gtyfajpkcn.html

JS:   // 手写回溯递归
来源：http://hz.yueranfly.top/gtkyscprfn.html

TS:   // 手写回溯递归
来源：http://hz.chenlongwang.top/gtybcvtlke.html

Java: // 手写回溯递归
来源：http://hz.chenjidiqi.icu/gttlvapjyt.html

Go:   // 手写回溯递归
来源：http://hz.nanxinkj.top/gtheopvizb.html

Ruby: arr.permutation.to_a
来源：http://hz.hysaishi.cn/gtjwkzhork.html

C#:   // 手写回溯递归
来源：http://hz.wangshuangyany.cn/gtmnaqvvjg.html

[N09] 栈与队列
来源：http://hz.yuanzhike.top/gtobutlxkg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jinqigufen.top/gtnzbrtyzp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zdqjudy.top/gtucijxffc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.bjfxy.top/gtblthoepo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.smart0.xyz/gtelsqidaw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hywenlv.cn/gtasscyrbx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.pengpengdd.cyou/gtyhusvbec.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.shzxlz.cn/gtlgetkxyi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.mhx1999.top/gtertvwoud.html

[N10] 链表节点定义
来源：http://hz.jqgfzy.top/gtarccmwid.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.guannengcc.top/gtaxdnzkbd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.c1oappe.top/gteyigdhdk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.gaohongyu789.top/gtfccfzzeb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.ydjk.org.cn/gtgfmtovji.html

Java: class Node { int v; Node next; }
来源：http://hz.yangfankeji.com/gtckabflab.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.316326.xyz/gttleilykj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jlsjyb.cn/gtvewgquug.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jqgufenzy.top/gtwygwastg.html

[N11] 二叉树中序遍历
来源：http://hz.jiagoushi.top/gttwknhvgr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.cheryme.top/gtvwlgdudf.html

PHP:  // 手写递归函数
来源：http://hz.quarkkingdee.top/gtuxgieqga.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jqgufenzy.top/gtbgunrcqb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.birdmap.top/gtwknsnmyx.html

Java: // 手写递归
来源：http://hz.nanxuanxn.top/gtgpjbsspm.html

Go:   // 手写递归
来源：http://hz.xuetiantiany.cn/gtqkkgssgc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.shzxlz.cn/gtqzvlzmrl.html

C#:   // 手写递归
来源：http://hz.nanxuanxn.top/gthllzhwee.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yuxming.cn/gtrkzucotf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.hammf.cn/gtcsvwnrko.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jianghu66.top/gterwhkfff.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xuetiantiany.cn/gtbommqqlz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cashguo.top/gtpcslinuv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.guowangkeji.top/gtqvoxjbxy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jqgufenzy.top/gtwasnzhfu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.ehwqpu.com/gtmdvzlntk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hammf.cn/gtjlvhnkxs.html

================================================================================
来源：http://hz.shzxlz.cn/gtpntksszr.html

O. 并发与异步
来源：http://hz.ydjk.org.cn/gtqzhsyhip.html

================================================================================
来源：http://hz.redwolf501.top/gtqbfbpozk.html

[O01] 启动一个线程
来源：http://hz.tanke756.top/gtyalafrky.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yj20258.top/gtkuluvxdv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.gaohongyu789.top/gtrdkrkmfx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.xingfuxueyuan.xyz/gthlhsvwgv.html

TS:   // 同 JS
来源：http://hz.pengpengdd.cyou/gtmgyscojf.html


<!-- 参考信息 -->