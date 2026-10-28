代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.dianchejie.cn/gtotjecddz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.pengpengdd.cyou/gtezxsgazv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.svipenyu.cn/gtfnamdxnx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hysaishi.cn/gtmyvzducr.html

[K06] 解析 URL 查询串
来源：http://hz.hammf.cn/gtilfshbqx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hammf.cn/gtnchzeyze.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.gaohongyu789.top/gtzqunzlfx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj20258888.top/gtnlfkkwyt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj20258.top/gtsyfvfvro.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yvedp.cn/gthldxpsnb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhoulong.xyz/gtfcqknnav.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.sxryk.cn/gtnecuhzmt.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.bjfxy.top/gtjkuvlwyw.html

[K07] 进制转换
来源：http://hz.tianlin.xyz/gthtraqaib.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.nanxuanxn.top/gtmjrofweb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhijiandao.cn/gticibacjt.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.fzhhl.top/gtocfrbygw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.aibaodan.cn/gtjntlkmjw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ywan-chungtsiang.top/gtcxpiebiv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hysaishi.cn/gtkuqdifey.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.dianchejie.cn/gtxyfgiwmj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hammf.cn/gtnpyonzdz.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yj202588.top/gtzxzocpzk.html

Py:   pickle.dumps(obj)
来源：http://hz.shangyingyoupin.top/gtqsfmcpyi.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.sxryk.cn/gtexioqivg.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.meibo888.top/gtxlsiagit.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.tanke756.top/gterkeurvj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ppjwa.cn/gttjzeyhku.html

Go:   encoding/gob
来源：http://hz.chenzaomai.com/gtdayimhsd.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhongyouzk.top/gticwrisaf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xuetiantiany.cn/gtnhwztunk.html

================================================================================
来源：http://hz.fengsongda.top/gtlyupdbiu.html

L. 网络请求
来源：http://hz.jianghu66.top/gtazrsspwl.html

================================================================================
来源：http://hz.jyoumei.cn/gtiumbbcsd.html

[L01] 发送 GET 请求
来源：http://hz.zhengqikj.top/gtumzxphuc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.sweek.top/gtbvfbyuyh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yanxiufei.cn/gtfmeeqszq.html

JS:   await fetch(url)
来源：http://hz.hongshengwenyu.top/gthviudlhd.html

TS:   await fetch(url)
来源：http://hz.pengpengdd.cyou/gtgrmvensr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ydzc1.top/gtxzmmgtcz.html

Go:   resp, err := http.Get(url)
来源：http://hz.yj202588.top/gtxinhacph.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xuanzx.com/gtwckgpxdt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yuxming.cn/gtdhtqdyqs.html

[L02] 发送 POST JSON
来源：http://hz.yvedp.cn/gtjjokpixv.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhongyouzk.top/gtvgrpxqhn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.dashuyun.cn/gtrcefpiok.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhaomingkeji.xyz/gtyksaixqw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.fzhhl.top/gtymiomtiv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.chenlongwang.top/gtpklfmtxc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhoulong.xyz/gtpozbfrev.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.sxryk.cn/gtzpogbyko.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.andypj.xyz/gtzdawmvna.html

[L03] 设置自定义请求头
来源：http://hz.nwbrower.top/gtqlgddhoa.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.aibaodan.cn/gtsoakebsc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.wangshuangyany.cn/gtfhptrgpw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhixingplan.top/gtrwlirtgj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinyuanbaomall.cn/gtxbzyohsa.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hnxiangtu.top/gtcjzooekj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yuanzhike.top/gtsxtlvzwv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.quarkkingdee.top/gthfcqjokf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.0kj1m.cn/gtobsfxubf.html

[L04] 设置超时
来源：http://hz.jianghu66.top/gtnyahpgbm.html

Py:   requests.get(url, timeout=5)
来源：http://hz.dashuyun.cn/gtspqbacdy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.shanyushiyangkeji.top/gtijvjupbm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ydjk.org.cn/gtdfokbshg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.daria6918.cn/gtzddduktd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.guannengcc.top/gtkhjjzvhm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.xylfe.cn/gtvcgmisff.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zhijiandao.cn/gtcihsllvw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.nanxuanxn.top/gtqctuhebk.html

[L05] 上传文件（multipart）
来源：http://hz.c1oappe.top/gtbfmhctov.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yonumen.top/gtseqeesrf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jinyuanbaomall.cn/gtzugfhlcu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.fzhhl.top/gtkubvbvsz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.tian-w.cn/gtkseevlaj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xingfuxueyuan.xyz/gtawtabviu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yuxming.cn/gtpyxoqibb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ivvv.top/gtenhoavxx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.ybcxt.top/gtdygpatoq.html

[L06] 解析响应为 JSON
来源：http://hz.sufxvd.cn/gtpszyaodk.html

Py:   resp.json()
来源：http://hz.jqgfzy.top/gtcseadmns.html

PHP:  json_decode($body, true);
来源：http://hz.zhoulong.xyz/gtuogrxnqa.html

JS:   await resp.json()
来源：http://hz.hfpthk.cn/gtjogfysjl.html

TS:   await resp.json()
来源：http://hz.pycfn.com/gtdcnvirvq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yvedp.cn/gtdqrqhjtv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.sysykeji.top/gtbghewgyr.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ivvv.top/gtunugdjxq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.sysykeji.top/gtooxtbxhs.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhengqikj.top/gtommayxag.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.nwbrower.top/gtrxjzavor.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.chenjidiqi.icu/gtuqbltatj.html

JS:   resp.ok;  resp.status
来源：http://hz.yj202588.top/gtcvnuhrsv.html

TS:   resp.ok;  resp.status
来源：http://hz.jqgfzy.top/gtrvuxeipl.html

Java: resp.statusCode()
来源：http://hz.yueranfly.top/gtrzgpjslz.html

Go:   resp.StatusCode
来源：http://hz.pycfn.com/gtitgewpua.html

Ruby: resp.code.to_i
来源：http://hz.hywenlv.cn/gtbwdoezhd.html

C#:   (int)resp.StatusCode
来源：http://hz.guannengcc.top/gtnnyxcocp.html

[L08] 并发请求多个地址
来源：http://hz.yvedp.cn/gtrhvsdzww.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yangfankeji.com/gtxfjphcye.html

PHP:  curl_multi_init() 系列
来源：http://hz.ppjwa.cn/gteazlikcw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yuanzhike.top/gtbrzrjyhe.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinyuanbaomall.cn/gtrsouxivc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hammf.cn/gtohhwarcm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.shanyushiyangkeji.top/gtbegtcyoe.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.chenjidiqi.icu/gtjtgqsdnv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xingfuxueyuan.xyz/gtliekskaq.html

================================================================================
来源：http://hz.0kj1m.cn/gtshqpsbyg.html

M. 命令行 / 进程 / 环境
来源：http://hz.dianchejie.cn/gtbuauobrr.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtwjrkacot.html

[M01] 读取命令行参数
来源：http://hz.sxryk.cn/gtxonsglzo.html

Py:   sys.argv[1:]
来源：http://hz.hongshengwenyu.top/gtpqckirvq.html

PHP:  $argv;  $argc;
来源：http://hz.jinqigufen.top/gtwmnteyyv.html

JS:   process.argv.slice(2)
来源：http://hz.gaohongyu789.top/gtvuvibzrw.html

TS:   process.argv.slice(2)
来源：http://hz.ppjwa.cn/gttllkvkmz.html

Java: args 数组（main 方法参数）
来源：http://hz.zycfv.cn/gtbgxylpbr.html

Go:   os.Args[1:]
来源：http://hz.ehwqpu.com/gtjlpqqtud.html

Ruby: ARGV
来源：http://hz.birdmap.top/gtowtdvbks.html

C#:   args 数组（Main 方法参数）
来源：http://hz.haohaochexian.top/gtqlxafdle.html

[M02] 读取环境变量
来源：http://hz.yueranfly.top/gtppcjvsjl.html

Py:   os.environ.get("HOME")
来源：http://hz.sysykeji.top/gtbskusart.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jinqigufen.top/gtjzufuccz.html

JS:   process.env.HOME
来源：http://hz.xingfuxueyuan.xyz/gtfzfusixo.html

TS:   process.env.HOME
来源：http://hz.c1oappe.top/gtpfwgmjal.html

Java: System.getenv("HOME")
来源：http://hz.cheryme.top/gtwvwdwlbk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.nwbrower.top/gtpvzdsfna.html

Ruby: ENV["HOME"]
来源：http://hz.fengsongda.top/gtcfjooetx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.0kj1m.cn/gtkbvceyuq.html

[M03] 执行外部命令
来源：http://hz.xinyue.icu/gtjqibizjj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.9152youxi.cn/gtxqzdzeqt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.c1oappe.top/gttrjyqmqv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jyoumei.cn/gttzsysmje.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.svipenyu.cn/gtzbmlqxfg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.chenzaomai.com/gtdokdurnd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.feifeiyinyue.top/gtluauzimi.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.nwbrower.top/gtcfcjqbeh.html

C#:   Process.Start("ls", "-l");
来源：http://hz.havefunace.top/gtrjkfdktd.html

[M04] 获取当前工作目录
来源：http://hz.yvedp.cn/gtyzsjkpqv.html

Py:   os.getcwd()
来源：http://hz.pengpengdd.cyou/gtbsguorhv.html

PHP:  getcwd();
来源：http://hz.jinyuanbaomall.cn/gtgykyfhij.html

JS:   process.cwd()
来源：http://hz.hnxiangtu.top/gtwosajotk.html

TS:   process.cwd()
来源：http://hz.sweek.top/gtpkhmfqze.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.fzhhl.top/gtaqkfekqx.html

Go:   os.Getwd()
来源：http://hz.ehwqpu.com/gtcafhejjw.html

Ruby: Dir.pwd
来源：http://hz.daria6918.cn/gtxhlfohxn.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.chenlongwang.top/gtfxblqtmk.html

[M05] 设置退出码
来源：http://hz.iojbl.cn/gtolcucxfp.html

Py:   sys.exit(1)
来源：http://hz.xingfuxueyuan.xyz/gtaaovznws.html

PHP:  exit(1);
来源：http://hz.yvedp.cn/gtxtypzwjw.html

JS:   process.exit(1)
来源：http://hz.zhiwuduotai.top/gtedumijuk.html

TS:   process.exit(1)
来源：http://hz.c1oappe.top/gtnbchhjjm.html

Java: System.exit(1)
来源：http://hz.jyoumei.cn/gtopkxvdxd.html

Go:   os.Exit(1)
来源：http://hz.ehwqpu.com/gthgrtozbp.html

Ruby: exit 1
来源：http://hz.tian-w.cn/gtajvtezab.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.haohaochexian.top/gtzjjvenbe.html

[M06] 向标准错误输出
来源：http://hz.hongshengwenyu.top/gtsworgbcb.html

Py:   print("err", file=sys.stderr)
来源：http://hz.cqqwz.cn/gtuekjwfqz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.cucudq.cn/gtyhadxjla.html

JS:   console.error("err")
来源：http://hz.ppjwa.cn/gtesxjdpxd.html

TS:   console.error("err")
来源：http://hz.cucudq.cn/gtimvfowfa.html

Java: System.err.println("err")
来源：http://hz.aibaodan.cn/gtsnfbnseb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.sysykeji.top/gtmeojvqml.html

Ruby: warn "err"
来源：http://hz.hfpthk.cn/gtixnckoiq.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.wangshuangyany.cn/gthtljosfb.html

[M07] 判断是否为主入口
来源：http://hz.yangfankeji.com/gtalzfemon.html

Py:   if __name__ == "__main__":
来源：http://hz.yonumen.top/gtjumgzfob.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jqgufenzy.top/gtqkrnysji.html

JS:   require.main === module
来源：http://hz.pycfn.com/gtogpvmzml.html

TS:   require.main === module
来源：http://hz.zhongyouzk.top/gtjwfopdru.html

Java: public static void main(String[] args)
来源：http://hz.meibo888.top/gtqyhtdzlv.html

Go:   func main()
来源：http://hz.xingfuxueyuan.xyz/gtnaxgalby.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yj20258.top/gtgikfgdjp.html

C#:   static void Main(string[] args)
来源：http://hz.pengpengdd.cyou/gtwqobyuhe.html

[M08] 获取系统与运行时信息
来源：http://hz.jinyuanbaomall.cn/gtcxjhrvnk.html

Py:   platform.system();  platform.python_version()
来源：http://hz.tian-w.cn/gtdfwmeqto.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.c1oappe.top/gtywgdpuyq.html

JS:   process.platform;  process.version
来源：http://hz.daria6918.cn/gtnmudtlxb.html

TS:   process.platform;  process.version
来源：http://hz.tian-w.cn/gtrcfrnigq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.sysykeji.top/gtsxctbpqc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jinyuanbaomall.cn/gtaeknrcfm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yuanzhike.top/gtfyqvpsbu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jianghu66.top/gtguvdnuig.html

================================================================================
来源：http://hz.cheryme.top/gtvwaxbahb.html

N. 数据结构与算法
来源：http://hz.nanxuanxn.top/gtyygpgqzp.html

================================================================================
来源：http://hz.gaohongyu789.top/gtgcnxmikm.html

[N01] 二分查找（有序数组）
来源：http://hz.ehwqpu.com/gtmvgcygpv.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.sxryk.cn/gtfqzgukdp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.gogol.net.cn/gtrrltzlnp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.wangshuangyany.cn/gtjrmlkgow.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jqgfzy.top/gtadxieoop.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.tanke756.top/gtptzbtycp.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.sxryk.cn/gtydowcdkw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.tianlin.xyz/gtundwmiwl.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.hongshengwenyu.top/gtaibdbvsj.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.316326.xyz/gtmemvwbmz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ivvv.top/gtplswuqyp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.iojbl.cn/gtkmrtnupz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhijiandao.cn/gtgxibtjfw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinyuanbaomall.cn/gtdiqmgzsi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.vqdsnc.cn/gtkdzrxmxc.html

Go:   slices.Sort(arr)
来源：http://hz.chenlongwang.top/gtywduvgie.html

Ruby: arr.sort
来源：http://hz.snrcjt.cn/gtizhgzwnl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.andypj.xyz/gtsvjuvdoe.html

[N03] 快速排序（分治示例）
来源：http://hz.zhengqikj.top/gtyerzordx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.316326.xyz/gtwcvuuzsv.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jinyuanbaomall.cn/gtkoxtfelu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.dashuyun.cn/gtejddimlw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xuanzx.com/gtadgfwoqr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yangfankeji.com/gtzwctcugv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.sweek.top/gttmzsmpfs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.sxryk.cn/gtlixanead.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.vqdsnc.cn/gtjiyjxgtr.html

[N04] 斐波那契数列
来源：http://hz.hysaishi.cn/gtbtaaujjo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xingfuxueyuan.xyz/gtazpzkwnv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.quarkkingdee.top/gtkjrzweuv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yuanzhike.top/gtmroisacu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj20258888.top/gtimctyzzc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.aizwys.cn/gtlggrgpoh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.chenlongwang.top/gthpfqzany.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jinghuilouyu.cn/gtpqntwnma.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.iojbl.cn/gtgfxqvxik.html

[N05] 最大公约数
来源：http://hz.hysaishi.cn/gteukfuzho.html

Py:   math.gcd(a, b)
来源：http://hz.zhoulong.xyz/gthfjkbcfs.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jyoumei.cn/gtdxcapebb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.daria6918.cn/gtalumkkyd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xinyue.icu/gtvmzzurab.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yj202588.top/gtemvpxoan.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jqgfzy.top/gtejckufba.html

Ruby: a.gcd(b)
来源：http://hz.ehwqpu.com/gtcbrcxqha.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.vqdsnc.cn/gtozwqmqlq.html

[N06] 判断回文字符串
来源：http://hz.birdmap.top/gtillpabix.html

Py:   s == s[::-1]
来源：http://hz.jianghu66.top/gtndcezqzl.html

PHP:  $s === strrev($s);
来源：http://hz.nwbrower.top/gtbgrctflx.html

JS:   s === [...s].reverse().join("")
来源：http://hz.daria6918.cn/gtlbcmohvo.html

TS:   s === [...s].reverse().join("")
来源：http://hz.cashguo.top/gtegcsbhan.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jiagoushi.top/gtmpumnzui.html

Go:   // 双指针从两端比较
来源：http://hz.haohaochexian.top/gtqtxldzuk.html

Ruby: s == s.reverse
来源：http://hz.aizwys.cn/gtzrwfumjm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.feifeiyinyue.top/gtetyjhald.html

[N07] 两数之和（返回下标）
来源：http://hz.shanyushiyangtech.top/gtyfafbdyb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hnqzz.top/gtticirixk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hongshengwenyu.top/gtqgilidxv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xuetiantiany.cn/gtpgmaghzk.html

TS:   // 手写 Map<string, number>
来源：http://hz.chenjidiqi.icu/gtjejpcmlo.html

Java: // 手写 HashMap
来源：http://hz.xuetiantiany.cn/gtclcjaelz.html

Go:   // 手写 map[int]int
来源：http://hz.meibo888.top/gtobmbwxec.html

Ruby: // 手写 Hash
来源：http://hz.fzhhl.top/gtosrbxklr.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jqgufenzy.top/gtenwerocf.html

[N08] 生成全排列
来源：http://hz.ivvv.top/gtxicsrdvv.html

Py:   itertools.permutations(arr)
来源：http://hz.tian-w.cn/gtrrslgspf.html

PHP:  // 手写递归交换
来源：http://hz.jiagoushi.top/gttdfhycdz.html

JS:   // 手写回溯递归
来源：http://hz.yueranfly.top/gthhnuyxcb.html

TS:   // 手写回溯递归
来源：http://hz.cucudq.cn/gtuaguvhba.html

Java: // 手写回溯递归
来源：http://hz.jinyuanbaomall.cn/gtgqqkthio.html

Go:   // 手写回溯递归
来源：http://hz.snrcjt.cn/gtbcmwfdtf.html

Ruby: arr.permutation.to_a
来源：http://hz.yj202588.top/gtipythgho.html

C#:   // 手写回溯递归
来源：http://hz.nanxinkj.top/gttmizdrlm.html

[N09] 栈与队列
来源：http://hz.jinqigufen.top/gtojonwktk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.iojbl.cn/gtizwrnymd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.kuanghao11.cn/gtajfzesza.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.9152youxi.cn/gtupqwzqhb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ydjk.org.cn/gtaasxvnrs.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ppjwa.cn/gtxcmfulpa.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhixingplan.top/gtiiwsfjes.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.shzxlz.cn/gtdrynmxkq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.cdnleiting.top/gtnafmdcxz.html

[N10] 链表节点定义
来源：http://hz.ydjk.org.cn/gtwjcjxzbz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.daxiang520.top/gtekytgxjs.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.tian-w.cn/gtuxvwenrc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.chenjidiqi.icu/gtjpspfpjt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhaomingkeji.xyz/gtxenzjpva.html

Java: class Node { int v; Node next; }
来源：http://hz.yj20258.top/gtiupfvvmr.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yanxiufei.cn/gtxechhgpr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.ppjwa.cn/gtquxvmwat.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yanxiufei.cn/gtahfzbxxv.html

[N11] 二叉树中序遍历
来源：http://hz.smart0.xyz/gtfgdhegpe.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jyoumei.cn/gtchrsplgb.html

PHP:  // 手写递归函数
来源：http://hz.sufxvd.cn/gtemmqihrc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.birdmap.top/gtwqgxehjq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cheryme.top/gtzwzlpaci.html

Java: // 手写递归
来源：http://hz.yj20258.top/gtxrrzgfbf.html

Go:   // 手写递归
来源：http://hz.hnxiangtu.top/gtvmnoxbtr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.shanyushiyangkeji.top/gttvjldbkm.html

C#:   // 手写递归
来源：http://hz.aizwys.cn/gtdmnvdfmr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.gotoacloud.top/gtbpyotyew.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.meibo888.top/gtlqxcfbgr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yj20258.top/gtwkfkhwae.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.tian-w.cn/gtckllaide.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gotoacloud.top/gtgnbzzsof.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.xuanzx.com/gtzbtkakdl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.shzxlz.cn/gtvoasyzjc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.tanke756.top/gtxawkwjva.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.daxiang520.top/gtitzryqcd.html

================================================================================
来源：http://hz.ydjk.org.cn/gtukgfvzzs.html

O. 并发与异步
来源：http://hz.chenzaomai.com/gtjqhtpnxs.html

================================================================================
来源：http://hz.ppjwa.cn/gtzsounxir.html

[O01] 启动一个线程
来源：http://hz.sweek.top/gtjrwnonnw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.gotoacloud.top/gtzpiznemp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.meibo888.top/gtxffianjd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jqgfzy.top/gttbkxptsr.html

TS:   // 同 JS
来源：http://hz.vqdsnc.cn/gtyufjmpmt.html


<!-- 参考信息 -->