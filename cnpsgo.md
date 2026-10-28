代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhaomingkeji.xyz/gtqjfmmhfs.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hnqzz.top/gthreboune.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.vqdsnc.cn/gtgbetrfna.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.chenlongwang.top/gthonzwaab.html

[K06] 解析 URL 查询串
来源：http://hz.gzhubu.top/gtnskjvqzo.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.andypj.xyz/gtfhshcfta.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.fzhhl.top/gtdpjbwurz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yvedp.cn/gtoroygekh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.aizwys.cn/gtctmpwnqe.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yanxiufei.cn/gtxsgcsgcd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zycfv.cn/gtofwithyt.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yongpay.top/gtwdibokmw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.hywenlv.cn/gtjxforjba.html

[K07] 进制转换
来源：http://hz.jqgfzy.top/gtaqiqvxad.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.nanxuanxn.top/gtezkrpudj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.guowangkeji.top/gthwvuwcvn.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.sysykeji.top/gtyewraowf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.chenzaomai.com/gtycwjokbw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.nanxuanxn.top/gttmwrqbaz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hfpthk.cn/gtniticukt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.gaohongyu789.top/gtwopiyxtj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhengqikj.top/gtnnuprqsj.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jinqigfzy.top/gthuexvmie.html

Py:   pickle.dumps(obj)
来源：http://hz.c1oappe.top/gtmlcadnry.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hongshengwenyu.top/gtwsvjwwki.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shanyushiyangtech.top/gtymmrjntz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jinghuilouyu.cn/gttjbqrwph.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.9152youxi.cn/gtnaucjdhw.html

Go:   encoding/gob
来源：http://hz.yuxming.cn/gtuasezpbx.html

Ruby: Marshal.dump(obj)
来源：http://hz.wangshuangyany.cn/gtxnbgegos.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.fengsongda.top/gtbmhsbcsy.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtifhtoqvl.html

L. 网络请求
来源：http://hz.sufxvd.cn/gtfnfubjiz.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtcimvymhb.html

[L01] 发送 GET 请求
来源：http://hz.ehwqpu.com/gtdndopjod.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.sweek.top/gtaagbsllg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.cashguo.top/gtmlzjzsnk.html

JS:   await fetch(url)
来源：http://hz.sxryk.cn/gtvcdskuab.html

TS:   await fetch(url)
来源：http://hz.zhongyouzk.top/gthnyeyabc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.snrcjt.cn/gtpmthkkrc.html

Go:   resp, err := http.Get(url)
来源：http://hz.ywan-chungtsiang.top/gttlorhxmw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.shanyushiyangtech.top/gtpibypmzs.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.bjfxy.top/gtofgvqwgt.html

[L02] 发送 POST JSON
来源：http://hz.cheryme.top/gtlblypjfi.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hongshengwenyu.top/gtjscjcpcv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hammf.cn/gtcnicxccv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.c1oappe.top/gtpyersplw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yanxiufei.cn/gtbpuneufg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhixingplan.top/gtvirgvpmt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.guowangkeji.top/gtokfplnwj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.gotoacloud.top/gtojwsfkrm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.wangdashe.top/gtxziqenam.html

[L03] 设置自定义请求头
来源：http://hz.mhx1999.top/gtdzzdaxus.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.svipenyu.cn/gtkeojwgrg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.nwbrower.top/gtqjwvrnda.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yuanzhike.top/gtuvjcazhn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cucudq.cn/gthmqmavws.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.andypj.xyz/gtyaghlpvy.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhijiandao.cn/gtkkbidgbc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.mhx1999.top/gtveevuybr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.sweek.top/gtifwobhwv.html

[L04] 设置超时
来源：http://hz.hnqzz.top/gtqcapdtei.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xuetiantiany.cn/gtqonxkxeh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.cheryme.top/gtqsnmdhje.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ywan-chungtsiang.top/gtpqyjrtsc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.fengsongda.top/gttrezyfyf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hnqzz.top/gtwvvttzle.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.gaohongyu789.top/gtimkykgvb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hysaishi.cn/gtjjebfdjr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.meibo888.top/gtgyrswdmy.html

[L05] 上传文件（multipart）
来源：http://hz.jinqigufen.top/gtfgkzncow.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.316326.xyz/gtrbpmmfkf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.c1oappe.top/gtvvrnwcos.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.vqdsnc.cn/gtwbjndkyv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhengqikj.top/gtdsfpetho.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jiagoushi.top/gtrhrqiayt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhaomingkeji.xyz/gtkwnndsum.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.daxiang520.top/gtabrbpjqq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.daria6918.cn/gtdmpxmuxm.html

[L06] 解析响应为 JSON
来源：http://hz.shzxlz.cn/gtsciigqvk.html

Py:   resp.json()
来源：http://hz.shzxlz.cn/gtmwylcfru.html

PHP:  json_decode($body, true);
来源：http://hz.shzxlz.cn/gtpgsmvoej.html

JS:   await resp.json()
来源：http://hz.ydzc1.top/gtynjydmqj.html

TS:   await resp.json()
来源：http://hz.yueranfly.top/gtzfcoitoo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.shuidangran.top/gtdbsueckb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.smart0.xyz/gtzirlhidp.html

Ruby: JSON.parse(resp.body)
来源：http://hz.c1oappe.top/gtngmhgmgq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.0kj1m.cn/gtjndspebs.html

[L07] 处理 HTTP 状态码
来源：http://hz.pycfn.com/gtheudvtyp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xylfe.cn/gtndslmsvi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yonumen.top/gtxwugyrfs.html

JS:   resp.ok;  resp.status
来源：http://hz.tianlin.xyz/gtzjtrlens.html

TS:   resp.ok;  resp.status
来源：http://hz.hywenlv.cn/gtuhebmizr.html

Java: resp.statusCode()
来源：http://hz.daria6918.cn/gtocqayfgc.html

Go:   resp.StatusCode
来源：http://hz.ppjwa.cn/gtdqwhtctb.html

Ruby: resp.code.to_i
来源：http://hz.316326.xyz/gttvjrljvu.html

C#:   (int)resp.StatusCode
来源：http://hz.zdqjudy.top/gthjacxuit.html

[L08] 并发请求多个地址
来源：http://hz.ywan-chungtsiang.top/gtpzaqcfpx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.aibaodan.cn/gtmmvwwyjy.html

PHP:  curl_multi_init() 系列
来源：http://hz.yj20258.top/gtroiczfdu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ydjk.org.cn/gtcnexaxjp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xingfuxueyuan.xyz/gtbusptmko.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.wangshuangyany.cn/gtaahfsqin.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jinghuilouyu.cn/gtpxawygdh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.cqqwz.cn/gtzwtghrzg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.shzxlz.cn/gthxisflhf.html

================================================================================
来源：http://hz.snrcjt.cn/gtmfpsxeur.html

M. 命令行 / 进程 / 环境
来源：http://hz.chenjidiqi.icu/gtekntsohk.html

================================================================================
来源：http://hz.havefunace.top/gtwibfmyee.html

[M01] 读取命令行参数
来源：http://hz.havefunace.top/gtdzrimqfy.html

Py:   sys.argv[1:]
来源：http://hz.sxryk.cn/gtmeswjjur.html

PHP:  $argv;  $argc;
来源：http://hz.yj20258.top/gtnikqavpp.html

JS:   process.argv.slice(2)
来源：http://hz.xuetiantiany.cn/gtaknkeujo.html

TS:   process.argv.slice(2)
来源：http://hz.guannengcc.top/gtnmganpdm.html

Java: args 数组（main 方法参数）
来源：http://hz.yuanzhike.top/gttupqicfj.html

Go:   os.Args[1:]
来源：http://hz.fengsongda.top/gtxwrdmkdz.html

Ruby: ARGV
来源：http://hz.yuanzhike.top/gtzolmfgse.html

C#:   args 数组（Main 方法参数）
来源：http://hz.tanke756.top/gtwcwxmepe.html

[M02] 读取环境变量
来源：http://hz.bjfxy.top/gtcwpiawub.html

Py:   os.environ.get("HOME")
来源：http://hz.shangyingyoupin.top/gtrnpurfmm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.gotoacloud.top/gtstkefzst.html

JS:   process.env.HOME
来源：http://hz.fengsongda.top/gtmyvlhkvj.html

TS:   process.env.HOME
来源：http://hz.sysykeji.top/gtqquufpqp.html

Java: System.getenv("HOME")
来源：http://hz.birdmap.top/gtodgwmdnz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.sweek.top/gthnknzwrh.html

Ruby: ENV["HOME"]
来源：http://hz.xingfuxueyuan.xyz/gtwnhtsflz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.cdnleiting.top/gtetqbuhth.html

[M03] 执行外部命令
来源：http://hz.sysykeji.top/gtfxdryabx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yuanzhike.top/gtxopppalc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yvedp.cn/gtojxlkrpi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xuanzx.com/gttvzueexy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.tanke756.top/gtjelzoxhz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.iojbl.cn/gtdnieuenx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.xuanzx.com/gtbdprwquo.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.gotoacloud.top/gtuavhhcmv.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jqgufenzy.top/gtladrybab.html

[M04] 获取当前工作目录
来源：http://hz.tian-w.cn/gtkuuzqcmd.html

Py:   os.getcwd()
来源：http://hz.316326.xyz/gtayshmpgh.html

PHP:  getcwd();
来源：http://hz.nanxuanxn.top/gtfvedkmvo.html

JS:   process.cwd()
来源：http://hz.dianchejie.cn/gtqlwydqle.html

TS:   process.cwd()
来源：http://hz.ydzc1.top/gtxyyeooyv.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.havefunace.top/gtrevpewlf.html

Go:   os.Getwd()
来源：http://hz.sxryk.cn/gtfbcjggoq.html

Ruby: Dir.pwd
来源：http://hz.fzhhl.top/gtgcbnrnjx.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.tianlin.xyz/gtgzcyjtvq.html

[M05] 设置退出码
来源：http://hz.shanyushiyangtech.top/gtkfaknnxy.html

Py:   sys.exit(1)
来源：http://hz.yueranfly.top/gtfsxcjyit.html

PHP:  exit(1);
来源：http://hz.shanyushiyangtech.top/gtcdwpnqjv.html

JS:   process.exit(1)
来源：http://hz.cucudq.cn/gtqsagancg.html

TS:   process.exit(1)
来源：http://hz.hammf.cn/gtfyckimcl.html

Java: System.exit(1)
来源：http://hz.pycfn.com/gtfaptxgug.html

Go:   os.Exit(1)
来源：http://hz.bjfxy.top/gtbkxbcyyf.html

Ruby: exit 1
来源：http://hz.shanyushiyangtech.top/gtnoiovpti.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.mhx1999.top/gtsvyahilw.html

[M06] 向标准错误输出
来源：http://hz.ybcxt.top/gtmdyrvflb.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hysaishi.cn/gtbshkbwwd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.pycfn.com/gtkpntchdj.html

JS:   console.error("err")
来源：http://hz.zycfv.cn/gtqwfxvefa.html

TS:   console.error("err")
来源：http://hz.zycfv.cn/gtoiyxllcx.html

Java: System.err.println("err")
来源：http://hz.sysykeji.top/gtxgsxpxxw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.feifeiyinyue.top/gtpkxrdbac.html

Ruby: warn "err"
来源：http://hz.jinqigfzy.top/gtvpwlchkv.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zycfv.cn/gtgohjtcsl.html

[M07] 判断是否为主入口
来源：http://hz.yj20258.top/gthkwebutz.html

Py:   if __name__ == "__main__":
来源：http://hz.wangshuangyany.cn/gttslepdeb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.fzhhl.top/gtzxtudmjc.html

JS:   require.main === module
来源：http://hz.shuidangran.top/gtkqutffxo.html

TS:   require.main === module
来源：http://hz.zhijiandao.cn/gtxgncvwxh.html

Java: public static void main(String[] args)
来源：http://hz.tian-w.cn/gtdaguncde.html

Go:   func main()
来源：http://hz.birdmap.top/gtapspwsif.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.hnqzz.top/gtpsifypml.html

C#:   static void Main(string[] args)
来源：http://hz.mhx1999.top/gtruakqnwr.html

[M08] 获取系统与运行时信息
来源：http://hz.guowangkeji.top/gtuofvrwsv.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yonumen.top/gtlmxythmp.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhoulong.xyz/gtghhndcgc.html

JS:   process.platform;  process.version
来源：http://hz.dianchejie.cn/gtgptwkcht.html

TS:   process.platform;  process.version
来源：http://hz.hnxiangtu.top/gtnjazunmf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hammf.cn/gtrawmsgbx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yj20258888.top/gtxalqgbyu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhiwuduotai.top/gtzsafybye.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.cucudq.cn/gtrslxzhwa.html

================================================================================
来源：http://hz.dianchejie.cn/gthuphtjao.html

N. 数据结构与算法
来源：http://hz.pengpengdd.cyou/gtwocifggc.html

================================================================================
来源：http://hz.aibaodan.cn/gtybjasoup.html

[N01] 二分查找（有序数组）
来源：http://hz.jyoumei.cn/gtyesuxfhx.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.9152youxi.cn/gtijeedbuk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.gzhubu.top/gtpcrpauuh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhongyouzk.top/gtbrxcpooy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yueranfly.top/gtwmcmseru.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.xuetiantiany.cn/gtatlzqsch.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.shuidangran.top/gtfinmdcht.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.haohaochexian.top/gtazylqowf.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.hywenlv.cn/gtwanvcxfa.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.hongshengwenyu.top/gtfxgbmiuf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.svipenyu.cn/gtuiftjhiv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.quarkkingdee.top/gtytuzsjxs.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.aibaodan.cn/gtlexajswf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ehwqpu.com/gtjseqjzsw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.tian-w.cn/gtzbruhegi.html

Go:   slices.Sort(arr)
来源：http://hz.cheryme.top/gtvoedaayv.html

Ruby: arr.sort
来源：http://hz.iojbl.cn/gtuahwrocr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.shzxlz.cn/gtkfgqgonh.html

[N03] 快速排序（分治示例）
来源：http://hz.bjfxy.top/gtlfhalvah.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jinqigfzy.top/gtuaaxjvrr.html

PHP:  // 递归实现，或用 usort
来源：http://hz.hammf.cn/gtltvwqkim.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xziqi.cn/gtfwaueywq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yongpay.top/gtwgypkaok.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.svipenyu.cn/gtlrjpgmns.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.cdnleiting.top/gtuqupmraa.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.0kj1m.cn/gtgdntrerb.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.cdnleiting.top/gtqykreoun.html

[N04] 斐波那契数列
来源：http://hz.daxiang520.top/gtpzwgxnip.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.chenzaomai.com/gtyuhkotgt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.shangyingyoupin.top/gtjuwjfwml.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yonumen.top/gtspsmzxlw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ydjk.org.cn/gtqxqaxspn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.bjfxy.top/gtjcriwltm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.chenzaomai.com/gtvfyfnfia.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hysaishi.cn/gteagumspg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jinqigfzy.top/gtmjghutls.html

[N05] 最大公约数
来源：http://hz.yuanzhike.top/gtbhwsxyhx.html

Py:   math.gcd(a, b)
来源：http://hz.yongpay.top/gtvvnftndi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shzxlz.cn/gtvxgbjroq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhijiandao.cn/gtojarbcko.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gotoacloud.top/gtijvucdwr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.bjfxy.top/gtqrgbrxnz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.pycfn.com/gtjbkesbny.html

Ruby: a.gcd(b)
来源：http://hz.sxryk.cn/gtijcaddof.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.aibaodan.cn/gtmdvnbqnv.html

[N06] 判断回文字符串
来源：http://hz.dianchejie.cn/gtjjfacfeh.html

Py:   s == s[::-1]
来源：http://hz.sufxvd.cn/gtqegimwkg.html

PHP:  $s === strrev($s);
来源：http://hz.pycfn.com/gteblqfajh.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zdqjudy.top/gtbiwiyahr.html

TS:   s === [...s].reverse().join("")
来源：http://hz.guowangkeji.top/gtvxomgwcc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.shanyushiyangtech.top/gtuzidmtwr.html

Go:   // 双指针从两端比较
来源：http://hz.gaohongyu789.top/gtgvnuucxo.html

Ruby: s == s.reverse
来源：http://hz.jinyuanbaomall.cn/gttfumsegf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.quarkkingdee.top/gtziydznxb.html

[N07] 两数之和（返回下标）
来源：http://hz.sysykeji.top/gtqsdxzjhb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zhaomingkeji.xyz/gtlsxnbtke.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.chenjidiqi.icu/gtzlvtezlx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jinghuilouyu.cn/gtfgqndtwt.html

TS:   // 手写 Map<string, number>
来源：http://hz.gogol.net.cn/gtunnfqhbp.html

Java: // 手写 HashMap
来源：http://hz.cqqwz.cn/gtzcpxnbba.html

Go:   // 手写 map[int]int
来源：http://hz.jianghu66.top/gtscnmxjon.html

Ruby: // 手写 Hash
来源：http://hz.nanxuanxn.top/gttuwatzsk.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hongshengwenyu.top/gtvstzewwo.html

[N08] 生成全排列
来源：http://hz.havefunace.top/gtvxmwhgua.html

Py:   itertools.permutations(arr)
来源：http://hz.daxiang520.top/gtbhmoduey.html

PHP:  // 手写递归交换
来源：http://hz.andypj.xyz/gtpbqdesot.html

JS:   // 手写回溯递归
来源：http://hz.havefunace.top/gtxzmqzynj.html

TS:   // 手写回溯递归
来源：http://hz.hfpthk.cn/gthmyjmlsa.html

Java: // 手写回溯递归
来源：http://hz.jlsjyb.cn/gtrfynrbne.html

Go:   // 手写回溯递归
来源：http://hz.jinghuilouyu.cn/gthodehprj.html

Ruby: arr.permutation.to_a
来源：http://hz.xylfe.cn/gtaobstotp.html

C#:   // 手写回溯递归
来源：http://hz.bjfxy.top/gteqdxbkwe.html

[N09] 栈与队列
来源：http://hz.zhaomingkeji.xyz/gtmhzsytce.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.haohaochexian.top/gtuakobcnz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.haohaochexian.top/gtdpjzwigz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhengqikj.top/gtbszxbnvr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.nanxuanxn.top/gtlrnhauhe.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jyoumei.cn/gtxdaupfli.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.svipenyu.cn/gtgpctplpt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.smart0.xyz/gtjhmixgyc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.nwbrower.top/gtyjapqoga.html

[N10] 链表节点定义
来源：http://hz.xziqi.cn/gtyomnrcup.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yj202588.top/gtnfubgnet.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.c1oappe.top/gtznckfxlr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.cdnleiting.top/gtyemjxbqb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.shanyushiyangtech.top/gtawstlgsn.html

Java: class Node { int v; Node next; }
来源：http://hz.fzhhl.top/gtalptfyxs.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jinqigfzy.top/gtdnchesut.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.dashuyun.cn/gtqnbojhrn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.andypj.xyz/gtpgfjkuei.html

[N11] 二叉树中序遍历
来源：http://hz.zhijiandao.cn/gtioqhvugm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.ehwqpu.com/gtkiikhwlt.html

PHP:  // 手写递归函数
来源：http://hz.xingfuxueyuan.xyz/gtxesxdcbb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sysykeji.top/gtmrqcqgng.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.havefunace.top/gtfrpjoowj.html

Java: // 手写递归
来源：http://hz.pycfn.com/gtdamulwyw.html

Go:   // 手写递归
来源：http://hz.gotoacloud.top/gthjwzhdti.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.pycfn.com/gtwgngfmhw.html

C#:   // 手写递归
来源：http://hz.cdnleiting.top/gtsqobdzjc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.cashguo.top/gtfdbfsvwq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yanxiufei.cn/gtmepvxmvg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hnqzz.top/gtsiozezwi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhijiandao.cn/gtbbdqhedp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ywan-chungtsiang.top/gttnintnxy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xingfuxueyuan.xyz/gtybljruxq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.316326.xyz/gtytwnubgl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.shangyingyoupin.top/gtbwknttty.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xuetiantiany.cn/gtjxsodvmn.html

================================================================================
来源：http://hz.gotoacloud.top/gtukipmwox.html

O. 并发与异步
来源：http://hz.ydjk.org.cn/gtmreioutd.html

================================================================================
来源：http://hz.cdnleiting.top/gtcnhbaztf.html

[O01] 启动一个线程
来源：http://hz.birdmap.top/gtahltribh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xuetiantiany.cn/gtpfhorufw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ivvv.top/gtqduegmai.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.0kj1m.cn/gttojzqnzg.html

TS:   // 同 JS
来源：http://hz.xingfuxueyuan.xyz/gteofxhcqn.html


<!-- 参考信息 -->