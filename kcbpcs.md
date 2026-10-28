代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.wangdashe.top/gtgbsjbcjw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jyoumei.cn/gtilffdnhq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.guannengcc.top/gtzcefmuov.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.gogol.net.cn/gtexldaarb.html

[K06] 解析 URL 查询串
来源：http://hz.hnxiangtu.top/gtzkyhmfcx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hongshengwenyu.top/gtgoqogfnp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.cheryme.top/gtalkzpgsk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shanyushiyangtech.top/gtlviwvzie.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ydjk.org.cn/gtzubxjywz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.bjfxy.top/gtylehxwxe.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jyoumei.cn/gtgpkmyrii.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yj20258888.top/gtkorsnogx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jianghu66.top/gtuxiderzb.html

[K07] 进制转换
来源：http://hz.pengpengdd.cyou/gtgptauucy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.sufxvd.cn/gthgozidri.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.shuidangran.top/gtdnseuvpb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xinyue.icu/gtdxmkzwnd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ivvv.top/gtfaizrfea.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hammf.cn/gtbfluaehn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jqgfzy.top/gtgbodtocv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zhixingplan.top/gtxouoqtml.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.sysykeji.top/gtpwydtlow.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.redwolf501.top/gtttpshrkd.html

Py:   pickle.dumps(obj)
来源：http://hz.hywenlv.cn/gtilyqdxot.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.meibo888.top/gtfsekjgug.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.cashguo.top/gtejtgoucl.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.wangshuangyany.cn/gtcxejjsyq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jinqigufen.top/gtzcpjzjtr.html

Go:   encoding/gob
来源：http://hz.jlsjyb.cn/gtqrkpdpjv.html

Ruby: Marshal.dump(obj)
来源：http://hz.gaohongyu789.top/gtswekxhsc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ydzc1.top/gtxuboocmz.html

================================================================================
来源：http://hz.guowangkeji.top/gthrsqscvb.html

L. 网络请求
来源：http://hz.nanxuanxn.top/gtoiaandix.html

================================================================================
来源：http://hz.gogol.net.cn/gtyayjmczt.html

[L01] 发送 GET 请求
来源：http://hz.cheryme.top/gtcwgqydoh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yueranfly.top/gtdbgcmelg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.andypj.xyz/gttknuabxs.html

JS:   await fetch(url)
来源：http://hz.yongpay.top/gtkxlznuxb.html

TS:   await fetch(url)
来源：http://hz.hongshengwenyu.top/gtdculfoqx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.vqdsnc.cn/gtugnhyoip.html

Go:   resp, err := http.Get(url)
来源：http://hz.chenjidiqi.icu/gtpekfqflw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.tianlin.xyz/gtpubmvzye.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.fzhhl.top/gtkqsoutzo.html

[L02] 发送 POST JSON
来源：http://hz.gzhubu.top/gtvglumbui.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jqgufenzy.top/gtypewjnjf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yueranfly.top/gtudlvroke.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.9152youxi.cn/gthinkhvan.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tianlin.xyz/gtavdghcal.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jyoumei.cn/gtnkltczvt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ybcxt.top/gtgxsgywhc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.hnqzz.top/gtoiplgnob.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.dianchejie.cn/gttoofqyng.html

[L03] 设置自定义请求头
来源：http://hz.tian-w.cn/gtgykpcfkn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ehwqpu.com/gtcsqubvkk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.shuidangran.top/gthjcdosgb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhongyouzk.top/gtnyinxhvc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hongshengwenyu.top/gtcszucemo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.daxiang520.top/gtnjumvozz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.guannengcc.top/gtmlvzkgvb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.pengpengdd.cyou/gticnvhnot.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ppjwa.cn/gtqtgorios.html

[L04] 设置超时
来源：http://hz.aibaodan.cn/gthzoyvnas.html

Py:   requests.get(url, timeout=5)
来源：http://hz.gzhubu.top/gtjrnebgwb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yj20258888.top/gtovafnckr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.tianlin.xyz/gtckitxkdy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.birdmap.top/gtpoeecpbt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yvedp.cn/gtpaxanapk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.snrcjt.cn/gtawikgdfy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zhengqikj.top/gtjgbkoxav.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.aibaodan.cn/gtrpzcauay.html

[L05] 上传文件（multipart）
来源：http://hz.zhaomingkeji.xyz/gtmhcgunpp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.havefunace.top/gthkbkxrxr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.cashguo.top/gtlpraeupg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.shangyingyoupin.top/gtyrzaabcb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ydjk.org.cn/gtyyryfcvh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yanxiufei.cn/gtdbfkdxdz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xingfuxueyuan.xyz/gtwvmqrdys.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.cqqwz.cn/gtpxlmeqys.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.andypj.xyz/gtcebxlcqx.html

[L06] 解析响应为 JSON
来源：http://hz.sweek.top/gtpnbdnwil.html

Py:   resp.json()
来源：http://hz.hywenlv.cn/gtlgcykocq.html

PHP:  json_decode($body, true);
来源：http://hz.9152youxi.cn/gtxbivmzha.html

JS:   await resp.json()
来源：http://hz.yvedp.cn/gtcbobkciy.html

TS:   await resp.json()
来源：http://hz.hammf.cn/gtlwmcwvqf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.andypj.xyz/gthhvnlpiv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yuanzhike.top/gtlwcmjbvl.html

Ruby: JSON.parse(resp.body)
来源：http://hz.kuanghao11.cn/gtpjmhmvcl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhoulong.xyz/gtuumqdowk.html

[L07] 处理 HTTP 状态码
来源：http://hz.hfpthk.cn/gtmdyfpwav.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.shanyushiyangkeji.top/gthpnepnyw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.birdmap.top/gtcusgavwj.html

JS:   resp.ok;  resp.status
来源：http://hz.shuidangran.top/gtntvpjnxw.html

TS:   resp.ok;  resp.status
来源：http://hz.birdmap.top/gtoobtqnpo.html

Java: resp.statusCode()
来源：http://hz.sysykeji.top/gtthgyhxdv.html

Go:   resp.StatusCode
来源：http://hz.shangyingyoupin.top/gtbxveddnq.html

Ruby: resp.code.to_i
来源：http://hz.daria6918.cn/gthlruiabv.html

C#:   (int)resp.StatusCode
来源：http://hz.xuetiantiany.cn/gtuldadpvq.html

[L08] 并发请求多个地址
来源：http://hz.gaohongyu789.top/gtmxiyrxqg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yonumen.top/gtdmcyuifr.html

PHP:  curl_multi_init() 系列
来源：http://hz.quarkkingdee.top/gtmmcqhrvs.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shanyushiyangkeji.top/gtbexbovxt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xuanzx.com/gtsjcfjxci.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.chenjidiqi.icu/gtppehisbj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhengqikj.top/gtoixubwsv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.52xcode.cn/gttcagmogd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.iojbl.cn/gtmstdyecw.html

================================================================================
来源：http://hz.sxryk.cn/gtectqztli.html

M. 命令行 / 进程 / 环境
来源：http://hz.c1oappe.top/gtopkbcoup.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtkjprtwwk.html

[M01] 读取命令行参数
来源：http://hz.zhijiandao.cn/gtexpcvctk.html

Py:   sys.argv[1:]
来源：http://hz.quarkkingdee.top/gtjcrqgypj.html

PHP:  $argv;  $argc;
来源：http://hz.xziqi.cn/gtrwwxnqaf.html

JS:   process.argv.slice(2)
来源：http://hz.iojbl.cn/gtrwewvsbp.html

TS:   process.argv.slice(2)
来源：http://hz.gotoacloud.top/gthqyitkul.html

Java: args 数组（main 方法参数）
来源：http://hz.feifeiyinyue.top/gthvwhprap.html

Go:   os.Args[1:]
来源：http://hz.sweek.top/gtwyoimccx.html

Ruby: ARGV
来源：http://hz.c1oappe.top/gtkmqlmqed.html

C#:   args 数组（Main 方法参数）
来源：http://hz.xylfe.cn/gtfhjiedqt.html

[M02] 读取环境变量
来源：http://hz.ydjk.org.cn/gtlnzuluin.html

Py:   os.environ.get("HOME")
来源：http://hz.jyoumei.cn/gtzkoeoogw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zhixingplan.top/gtinzmediu.html

JS:   process.env.HOME
来源：http://hz.yj202588.top/gtzrknybzm.html

TS:   process.env.HOME
来源：http://hz.yj202588.top/gtkshmfkfx.html

Java: System.getenv("HOME")
来源：http://hz.jyoumei.cn/gtyznxwjwp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.tianlin.xyz/gtxkzduunn.html

Ruby: ENV["HOME"]
来源：http://hz.tanke756.top/gtjaevorxj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhiwuduotai.top/gthbajbdmw.html

[M03] 执行外部命令
来源：http://hz.haohaochexian.top/gtwjmiqnqv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.52xcode.cn/gtstybwrbc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.havefunace.top/gtxteblewh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hysaishi.cn/gtrwxpjwul.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.dianchejie.cn/gtpijtehov.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.xuetiantiany.cn/gtrsnaxxuw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.wangshuangyany.cn/gtdhbdcldo.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yueranfly.top/gtijkswixd.html

C#:   Process.Start("ls", "-l");
来源：http://hz.dashuyun.cn/gtphzknmyp.html

[M04] 获取当前工作目录
来源：http://hz.zhiwuduotai.top/gtsyycfaii.html

Py:   os.getcwd()
来源：http://hz.guannengcc.top/gtmdaylwfl.html

PHP:  getcwd();
来源：http://hz.hysaishi.cn/gtiuwhknxk.html

JS:   process.cwd()
来源：http://hz.hysaishi.cn/gtktqtpmse.html

TS:   process.cwd()
来源：http://hz.jinqigufen.top/gtzbunduzy.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jianghu66.top/gtffsyidqf.html

Go:   os.Getwd()
来源：http://hz.cdnleiting.top/gtdonwzisr.html

Ruby: Dir.pwd
来源：http://hz.xingfuxueyuan.xyz/gtjfdzghei.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jinqigufen.top/gtuyofdlwf.html

[M05] 设置退出码
来源：http://hz.svipenyu.cn/gtncsbupum.html

Py:   sys.exit(1)
来源：http://hz.ppjwa.cn/gtrltgasde.html

PHP:  exit(1);
来源：http://hz.zhongyouzk.top/gtrafuhpbb.html

JS:   process.exit(1)
来源：http://hz.jlsjyb.cn/gtuwwbblex.html

TS:   process.exit(1)
来源：http://hz.bjfxy.top/gtuigjxpxv.html

Java: System.exit(1)
来源：http://hz.zdqjudy.top/gtfolxhnyv.html

Go:   os.Exit(1)
来源：http://hz.ivvv.top/gtctlgsjjb.html

Ruby: exit 1
来源：http://hz.zhixingplan.top/gtriwlwgfu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jianghu66.top/gtnjvleakk.html

[M06] 向标准错误输出
来源：http://hz.zhiwuduotai.top/gtgoapnqbw.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yvedp.cn/gtvqcevgaz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.vqdsnc.cn/gtvydpxxdz.html

JS:   console.error("err")
来源：http://hz.meibo888.top/gtsiqhfxvx.html

TS:   console.error("err")
来源：http://hz.meibo888.top/gtslnizchg.html

Java: System.err.println("err")
来源：http://hz.zdqjudy.top/gtwlpgompf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xylfe.cn/gtfvwqcjfc.html

Ruby: warn "err"
来源：http://hz.xuanzx.com/gtovmejlbp.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yuxming.cn/gtkpgguvkl.html

[M07] 判断是否为主入口
来源：http://hz.ywan-chungtsiang.top/gtmkgfdhqf.html

Py:   if __name__ == "__main__":
来源：http://hz.mhx1999.top/gtjzlbdfcl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.sxryk.cn/gtrqpewlwm.html

JS:   require.main === module
来源：http://hz.yueranfly.top/gticlzruxl.html

TS:   require.main === module
来源：http://hz.aibaodan.cn/gtjtisxorf.html

Java: public static void main(String[] args)
来源：http://hz.havefunace.top/gtotrolxnd.html

Go:   func main()
来源：http://hz.vqdsnc.cn/gtucvmonbw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zycfv.cn/gtosdkgkur.html

C#:   static void Main(string[] args)
来源：http://hz.yanxiufei.cn/gtncxbksul.html

[M08] 获取系统与运行时信息
来源：http://hz.fzhhl.top/gtowilshzv.html

Py:   platform.system();  platform.python_version()
来源：http://hz.sxryk.cn/gtzmbevvye.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.chenlongwang.top/gtbrurdbow.html

JS:   process.platform;  process.version
来源：http://hz.birdmap.top/gtklfgztbf.html

TS:   process.platform;  process.version
来源：http://hz.316326.xyz/gtveqzgipe.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.bjfxy.top/gtlvowovep.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.sxryk.cn/gttkqucgne.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yonumen.top/gtgkbzaheu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yonumen.top/gtqzlwmohm.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtqxswcixy.html

N. 数据结构与算法
来源：http://hz.xingfuxueyuan.xyz/gtburoshta.html

================================================================================
来源：http://hz.fzhhl.top/gtludmsczi.html

[N01] 二分查找（有序数组）
来源：http://hz.ppjwa.cn/gtsrnqraeq.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.gaohongyu789.top/gtttnqansx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.haohaochexian.top/gtvdzzyrck.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.chenjidiqi.icu/gtcudrfzzs.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yanxiufei.cn/gteqhvnvob.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.gaohongyu789.top/gtbeqlawjp.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ydzc1.top/gttvozysvk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hysaishi.cn/gtcuosmgds.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jyoumei.cn/gtuaxlxmjw.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.kuanghao11.cn/gtnjxijwhx.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jianghu66.top/gtuuvwmahq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hnxiangtu.top/gtoraliplf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.meibo888.top/gtemonoaiv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinghuilouyu.cn/gtmxlwrefu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hysaishi.cn/gtsemiiimo.html

Go:   slices.Sort(arr)
来源：http://hz.daxiang520.top/gtqwfwowba.html

Ruby: arr.sort
来源：http://hz.hongshengwenyu.top/gtxsfhohxx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.shuidangran.top/gtihyvuxgi.html

[N03] 快速排序（分治示例）
来源：http://hz.cashguo.top/gtuphuuxos.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ybcxt.top/gtuilvqrme.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yueranfly.top/gtrzbfedfx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nwbrower.top/gttvggkkld.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.iojbl.cn/gtmeejlkro.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yonumen.top/gtaqwtvewj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jiagoushi.top/gtjxkakgbl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ybcxt.top/gtesolfijt.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhijiandao.cn/gtfoydoeei.html

[N04] 斐波那契数列
来源：http://hz.quarkkingdee.top/gtsbckjygk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.kuanghao11.cn/gtrynzbmcj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yongpay.top/gtriqrufin.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hfpthk.cn/gtjfmrvcos.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.tian-w.cn/gtyonabmcf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.fengsongda.top/gtzucesrbr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.shuidangran.top/gtodkqhaoz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yj202588.top/gtghsphpmp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yj202588.top/gttjmdmxqv.html

[N05] 最大公约数
来源：http://hz.xuanzx.com/gtbnfgwcus.html

Py:   math.gcd(a, b)
来源：http://hz.hnxiangtu.top/gtxbugvhgk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zdqjudy.top/gtqzzfmwtk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.nanxuanxn.top/gtjwevwsff.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hongshengwenyu.top/gtljomjqlv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.chenlongwang.top/gtasqvvezv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.aizwys.cn/gtunekeuuu.html

Ruby: a.gcd(b)
来源：http://hz.yj20258888.top/gtmdyoxhvi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhiwuduotai.top/gtaogcdrqg.html

[N06] 判断回文字符串
来源：http://hz.ywan-chungtsiang.top/gtgqddlehe.html

Py:   s == s[::-1]
来源：http://hz.hongshengwenyu.top/gtnkgqbfsz.html

PHP:  $s === strrev($s);
来源：http://hz.ydzc1.top/gtttphrjmx.html

JS:   s === [...s].reverse().join("")
来源：http://hz.xziqi.cn/gtnjshkucu.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hammf.cn/gtpjnqsjcb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.9152youxi.cn/gtvstdutbg.html

Go:   // 双指针从两端比较
来源：http://hz.guannengcc.top/gtpjnkrioh.html

Ruby: s == s.reverse
来源：http://hz.xinyue.icu/gtynwbdpiu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hammf.cn/gtdvmhxoxt.html

[N07] 两数之和（返回下标）
来源：http://hz.pycfn.com/gtrpvzegwe.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.shanyushiyangtech.top/gtayqdanxj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.shangyingyoupin.top/gtphjgedju.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.sxryk.cn/gtqkhgrxja.html

TS:   // 手写 Map<string, number>
来源：http://hz.cashguo.top/gtioudidiv.html

Java: // 手写 HashMap
来源：http://hz.gzhubu.top/gtueyqdpzt.html

Go:   // 手写 map[int]int
来源：http://hz.hammf.cn/gtwipjyeka.html

Ruby: // 手写 Hash
来源：http://hz.chenjidiqi.icu/gtrndevsej.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.shuidangran.top/gtfqmagmuz.html

[N08] 生成全排列
来源：http://hz.iojbl.cn/gtbshwvulk.html

Py:   itertools.permutations(arr)
来源：http://hz.xuanzx.com/gtrqewsrzo.html

PHP:  // 手写递归交换
来源：http://hz.yj20258888.top/gtzcsuvlub.html

JS:   // 手写回溯递归
来源：http://hz.yongpay.top/gtdlznzlcq.html

TS:   // 手写回溯递归
来源：http://hz.sysykeji.top/gtkyzgevvh.html

Java: // 手写回溯递归
来源：http://hz.bjfxy.top/gtxagbewug.html

Go:   // 手写回溯递归
来源：http://hz.cqqwz.cn/gtwwiggpda.html

Ruby: arr.permutation.to_a
来源：http://hz.ydzc1.top/gtkjboiknk.html

C#:   // 手写回溯递归
来源：http://hz.52xcode.cn/gtibunidun.html

[N09] 栈与队列
来源：http://hz.yj20258888.top/gthqavobkz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yj20258.top/gtyjbdhzwn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.gaohongyu789.top/gtonymkiuz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.andypj.xyz/gtrhknyczp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.dianchejie.cn/gtpasjvltc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.dashuyun.cn/gtvoisjlok.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhixingplan.top/gtnyeizwyd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.gogol.net.cn/gtkjefccpv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yuanzhike.top/gtiziesnoh.html

[N10] 链表节点定义
来源：http://hz.zhengqikj.top/gtkyrccsxp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.nanxinkj.top/gtremrcjtu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.snrcjt.cn/gtaolifgkp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.aizwys.cn/gthfefdsql.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hfpthk.cn/gtctpufruz.html

Java: class Node { int v; Node next; }
来源：http://hz.ydzc1.top/gthutfqfzo.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yongpay.top/gtnucjqbok.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.dianchejie.cn/gtxeqeeqqb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.ppjwa.cn/gtehzxgqgi.html

[N11] 二叉树中序遍历
来源：http://hz.hnxiangtu.top/gtrqbvdzzp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.0kj1m.cn/gtuigxwzpv.html

PHP:  // 手写递归函数
来源：http://hz.havefunace.top/gtvkycugtj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.tian-w.cn/gtneviitvl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gogol.net.cn/gtidputyee.html

Java: // 手写递归
来源：http://hz.jinqigfzy.top/gtaesztpmm.html

Go:   // 手写递归
来源：http://hz.zhixingplan.top/gtlcxtmzim.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.daria6918.cn/gtpfkgijim.html

C#:   // 手写递归
来源：http://hz.xuetiantiany.cn/gtttrwwvqr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.c1oappe.top/gtcbwbvhqm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.xinyue.icu/gtgtmkqbek.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhoulong.xyz/gtzlrzfivq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.aibaodan.cn/gtdbgdytgq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ydjk.org.cn/gttnedceyt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shanyushiyangkeji.top/gtyjjlxqyu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.wangdashe.top/gtcjbvutvv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.smart0.xyz/gtowdywbti.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhongyouzk.top/gteuxntxez.html

================================================================================
来源：http://hz.gogol.net.cn/gtkkmlwrdz.html

O. 并发与异步
来源：http://hz.fzhhl.top/gtzriaibwf.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtoxihbwfg.html

[O01] 启动一个线程
来源：http://hz.aizwys.cn/gtekwqnaof.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jinqigfzy.top/gtbsaejzth.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.jqgfzy.top/gtpipbaibq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jiagoushi.top/gtpqgbqmnh.html

TS:   // 同 JS
来源：http://hz.yj20258888.top/gtsvuooafp.html


<!-- 参考信息 -->