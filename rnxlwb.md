代发 wailian999

[E14] URL 编码与 Base64
来源：http://hz.sufxvd.cn/gtvpdhzhla.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.hfpthk.cn/gtaotvwdaa.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.nanxinkj.top/gtltqcolkc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.xuetiantiany.cn/gttssyuuax.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zhengqikj.top/gtpjdffxbz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.snrcjt.cn/gtljavawlt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.chenzaomai.com/gtgslaykdj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.guowangkeji.top/gtpxoxyzjv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.9152youxi.cn/gtvgfusvid.html

[E15] HTML 转义 / 反转义
来源：http://hz.yvedp.cn/gtpdmvcgld.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.cqqwz.cn/gtuccnpivu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jqgufenzy.top/gtxivqtbqd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.cashguo.top/gtquagswix.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.aibaodan.cn/gtzmvvhfrq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.mhx1999.top/gtdrbqtlgs.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.kuanghao11.cn/gtaahazrfl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.andypj.xyz/gtwmhenhle.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.sxryk.cn/gtmgfnxmza.html

[E16] 数字千分位
来源：http://hz.tian-w.cn/gtedzwpmlv.html

Py:   f"{1234567:,}"
来源：http://hz.shuidangran.top/gtisvyyran.html

PHP:  number_format(1234567);
来源：http://hz.dianchejie.cn/gtrpmridcu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhongyouzk.top/gtiajygubt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.meibo888.top/gtqexduice.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.wangdashe.top/gtzadpqsyv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.nwbrower.top/gtokghnepc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.nwbrower.top/gtvwlitdka.html

C#:   1234567.ToString("N0")
来源：http://hz.cqqwz.cn/gtkygspzid.html

[E17] 首字母大写
来源：http://hz.wangshuangyany.cn/gtmmnzaxpj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.dashuyun.cn/gtfqvhiqqx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hysaishi.cn/gtjnoxddaz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yj202588.top/gtogtogdhe.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hammf.cn/gttfvlaptg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.shangyingyoupin.top/gtzmvwpcwg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.guannengcc.top/gtbntfswmu.html

Ruby: s.capitalize
来源：http://hz.zhengqikj.top/gtboiqopif.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.gogol.net.cn/gtpcxdgrnb.html

[E18] 模板占位符替换
来源：http://hz.smart0.xyz/gtajvuvgov.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hywenlv.cn/gtuwsrmdye.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yueranfly.top/gtgbdpichg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.andypj.xyz/gteupbolwu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinyuanbaomall.cn/gtocukuctz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.chenzaomai.com/gtsllryfsj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.52xcode.cn/gtaekndzkt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.cheryme.top/gtbfphobbl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jqgufenzy.top/gtvbwgqstm.html

[E19] 多行文本按行拆分
来源：http://hz.ybcxt.top/gtmslsfrcc.html

Py:   s.splitlines()
来源：http://hz.hongshengwenyu.top/gtimvmsyrp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.ydzc1.top/gtenihvhct.html

JS:   s.split(/\r?\n/)
来源：http://hz.shangyingyoupin.top/gtbyylznci.html

TS:   s.split(/\r?\n/)
来源：http://hz.chenjidiqi.icu/gtkpbgqdss.html

Java: s.lines().toList()
来源：http://hz.shzxlz.cn/gtcqfbdoei.html

Go:   strings.Split(s, "\n")
来源：http://hz.birdmap.top/gtioiqygjt.html

Ruby: s.lines
来源：http://hz.jinyuanbaomall.cn/gtjluozams.html

C#:   s.Split('\n')
来源：http://hz.cheryme.top/gttjjabmvs.html

[E20] 判断字符串是否为空
来源：http://hz.havefunace.top/gtpfipsqdo.html

Py:   if not s:
来源：http://hz.jqgfzy.top/gtuvhgnnaf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.snrcjt.cn/gtshnxsjuu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.xuetiantiany.cn/gtoqfvxahn.html

TS:   if (s === "") {}
来源：http://hz.hongshengwenyu.top/gtduyibzmd.html

Java: if (s.isEmpty()) {}
来源：http://hz.xuanzx.com/gtybyehdbw.html

Go:   if s == "" {}
来源：http://hz.hywenlv.cn/gtkrnkdkir.html

Ruby: if s.empty?
来源：http://hz.zycfv.cn/gtvscxlenp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.xuetiantiany.cn/gthdaowhdx.html

[E21] 超长截断加省略号
来源：http://hz.xuetiantiany.cn/gtrgfhsgeq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jqgfzy.top/gtagqgmrew.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.fengsongda.top/gtukvtafaj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.havefunace.top/gtraxsrwnv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.vqdsnc.cn/gthejpiefv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.sufxvd.cn/gtaflamqei.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hfpthk.cn/gtqcadoqrc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.shangyingyoupin.top/gthpcarzdk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.svipenyu.cn/gtrduabord.html

[E22] 字节长度与字符长度
来源：http://hz.daxiang520.top/gtsdonvjop.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hongshengwenyu.top/gtcgjymtno.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.mhx1999.top/gtpttwienb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.havefunace.top/gtrwjqgghh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yanxiufei.cn/gthdxepzbw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.wangshuangyany.cn/gtsbcvgewr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.mhx1999.top/gtjdfsqoqi.html

Ruby: s.bytesize;  s.length
来源：http://hz.gzhubu.top/gttoshvgle.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.tianlin.xyz/gtmzqnxlkj.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtfwkuzanp.html

F. 文件与目录
来源：http://hz.chenzaomai.com/gtlmhwyzkr.html

================================================================================
来源：http://hz.fzhhl.top/gtqrynvpai.html

[F01] 读取整个文件
来源：http://hz.zhiwuduotai.top/gtdqordegm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.sxryk.cn/gtqpnlrnrt.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hongshengwenyu.top/gttsfjcbqd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yvedp.cn/gtcvggldqo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.xziqi.cn/gtxyxjesjj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.shzxlz.cn/gtsuxllwyn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.iojbl.cn/gtazxdlsfl.html

Ruby: File.read("a.txt")
来源：http://hz.nanxinkj.top/gtydawpzxr.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.tianlin.xyz/gtrzgfkznz.html

[F02] 逐行读取文件
来源：http://hz.9152youxi.cn/gtwzhcisek.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.shanyushiyangkeji.top/gtaohqdmzj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.snrcjt.cn/gtgggmvqmj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shanyushiyangtech.top/gtqizbudyt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yonumen.top/gtmcuyzmyn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hammf.cn/gtnumdortz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.xuetiantiany.cn/gtfbcjoghd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ybcxt.top/gttkfpczyi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.sysykeji.top/gtejpiqxmr.html

[F03] 写入文件（覆盖）
来源：http://hz.smart0.xyz/gtcaaolgit.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.sufxvd.cn/gtyyuevtxo.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.shanyushiyangkeji.top/gtakgesmyw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.nanxuanxn.top/gtlikilrna.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.haohaochexian.top/gtrhxdlprq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.xylfe.cn/gtqiuhbcrt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jiagoushi.top/gtreukgbof.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.cheryme.top/gtqtchuhyt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.vqdsnc.cn/gtkgowskzn.html

[F04] 追加写入文件
来源：http://hz.yj202588.top/gtrboaucsx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jlsjyb.cn/gtpyvnwcdw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.dianchejie.cn/gtzolctdbp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.chenzaomai.com/gtrpjoxqov.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ydzc1.top/gthpkfupop.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.sufxvd.cn/gtkmperlmc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zhaomingkeji.xyz/gtkgcxwflx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.haohaochexian.top/gtotquhvua.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zhengqikj.top/gtvlgnjgpc.html

[F05] 判断文件或目录是否存在
来源：http://hz.jqgufenzy.top/gtyuelkhsj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jiagoushi.top/gtfnkxjumb.html

PHP:  file_exists("a.txt");
来源：http://hz.xylfe.cn/gtpkmfrube.html

JS:   fs.existsSync("a.txt")
来源：http://hz.cucudq.cn/gtfpzkbnrr.html

TS:   fs.existsSync("a.txt")
来源：http://hz.redwolf501.top/gtqgtoszzf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ywan-chungtsiang.top/gttpzumlnp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yvedp.cn/gtsyhsmctc.html

Ruby: File.exist?("a.txt")
来源：http://hz.cucudq.cn/gtagmhvine.html

C#:   File.Exists("a.txt")
来源：http://hz.yangfankeji.com/gtyojwrazz.html

[F06] 删除文件
来源：http://hz.jinyuanbaomall.cn/gtxpcyhyqz.html

Py:   os.remove("a.txt")
来源：http://hz.aizwys.cn/gtcmornikk.html

PHP:  unlink("a.txt");
来源：http://hz.wangdashe.top/gtdooaqane.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.52xcode.cn/gtmksknisz.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yj20258.top/gtilylnxkm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhijiandao.cn/gtyuxeztma.html

Go:   os.Remove("a.txt")
来源：http://hz.tian-w.cn/gtesdcqgny.html

Ruby: File.delete("a.txt")
来源：http://hz.jinqigfzy.top/gtzwvdbkbg.html

C#:   File.Delete("a.txt");
来源：http://hz.hywenlv.cn/gtbcjilekw.html

[F07] 创建目录（含多级）
来源：http://hz.aibaodan.cn/gtzutfialm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yueranfly.top/gtjjsixysd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.shzxlz.cn/gtplacoepw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinqigfzy.top/gtzuyczkok.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.haohaochexian.top/gtcliciomm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xylfe.cn/gtkrugrfnq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.aibaodan.cn/gtjlsygzrs.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jiagoushi.top/gtumllaxii.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.xinyue.icu/gtaqeewwfn.html

[F08] 遍历目录
来源：http://hz.cqqwz.cn/gtwmitbspf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yueranfly.top/gtcofklbxi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.hammf.cn/gtagoudihw.html

JS:   fs.readdirSync("dir")
来源：http://hz.nwbrower.top/gtncndlkhz.html

TS:   fs.readdirSync("dir")
来源：http://hz.cucudq.cn/gtfikcqcsn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.pycfn.com/gtedhmjyax.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hfpthk.cn/gtuudgecly.html

Ruby: Dir.children("dir")
来源：http://hz.zhixingplan.top/gtgnvzsrhd.html

C#:   Directory.GetFiles("dir")
来源：http://hz.xuetiantiany.cn/gtfyvgmmly.html

[F09] 获取文件大小
来源：http://hz.xylfe.cn/gteyawwfds.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zhixingplan.top/gttnoebvad.html

PHP:  filesize("a.txt");
来源：http://hz.jlsjyb.cn/gtehgsphqv.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhongyouzk.top/gttgzljukc.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ybcxt.top/gtsfjoscyr.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.c1oappe.top/gtfdpxrqoy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhijiandao.cn/gtvrzllkci.html

Ruby: File.size("a.txt")
来源：http://hz.zhiwuduotai.top/gtuaaqwvfu.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ppjwa.cn/gtbsgbajpx.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hywenlv.cn/gtayvsqlmw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.iojbl.cn/gtaedobddk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.xuetiantiany.cn/gtuskciqsi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhaomingkeji.xyz/gthzjfdrxf.html

TS:   path.extname("a.txt")
来源：http://hz.wangshuangyany.cn/gtwjevsidr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.sysykeji.top/gtjukexkhw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhoulong.xyz/gtsyxyqxav.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yonumen.top/gthjunzscf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ivvv.top/gtabdtcfmr.html

[F11] 复制与移动文件
来源：http://hz.sxryk.cn/gtxugoakla.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zycfv.cn/gtmpaogmbn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.dashuyun.cn/gtxccgtxmi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.fengsongda.top/gtfmzjnbbb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jyoumei.cn/gtthldhcdd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.vqdsnc.cn/gtxzokepeh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.smart0.xyz/gtkpegnoew.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.gotoacloud.top/gtybqxjbxh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yvedp.cn/gtcympxgee.html

[F12] CSV 读写
来源：http://hz.52xcode.cn/gttydgdtwa.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.chenlongwang.top/gtgeeunaxh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jlsjyb.cn/gtcafihjjm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.bjfxy.top/gtstkvauld.html

TS:   // 同上
来源：http://hz.wangshuangyany.cn/gtelgyiylp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.sweek.top/gtdajgxubx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.nwbrower.top/gtrdentrbh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ywan-chungtsiang.top/gtwygxjqkh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.andypj.xyz/gtinqkwryn.html

================================================================================
来源：http://hz.nanxuanxn.top/gtirgqsziz.html

G. 面向对象
来源：http://hz.sufxvd.cn/gtyeszmoyf.html

================================================================================
来源：http://hz.zycfv.cn/gtxgeihvec.html

[G01] 定义类
来源：http://hz.nanxinkj.top/gtxirdsgpy.html

Py:   class User: pass
来源：http://hz.zhaomingkeji.xyz/gtcktmvhcm.html

PHP:  class User {}
来源：http://hz.xylfe.cn/gtacovodzq.html

JS:   class User {}
来源：http://hz.tian-w.cn/gtnxywtfsr.html

TS:   class User { name: string = ""; }
来源：http://hz.redwolf501.top/gtciddrkue.html

Java: class User {}
来源：http://hz.aizwys.cn/gtemvqlbxj.html

Go:   type User struct { Name string }
来源：http://hz.jqgfzy.top/gtyhcskztz.html

Ruby: class User; end
来源：http://hz.pycfn.com/gtvkteudzs.html

C#:   class User {}
来源：http://hz.fengsongda.top/gtqjbbnyho.html

[G02] 构造函数
来源：http://hz.hywenlv.cn/gttlptmbxa.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yj20258.top/gtadypglor.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhongyouzk.top/gtvuppitxy.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhoulong.xyz/gtwckeinft.html

TS:   constructor(public name: string) {}
来源：http://hz.daxiang520.top/gtedolyvzn.html

Java: User(String name) { this.name = name; }
来源：http://hz.cheryme.top/gttjsspigr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.fengsongda.top/gtasdkbhxf.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.meibo888.top/gtrmcensxi.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yuxming.cn/gtvzhhtstu.html

[G03] 实例属性
来源：http://hz.sysykeji.top/gthtdowzdj.html

Py:   self.name = "x"
来源：http://hz.sufxvd.cn/gtqwrqmwjy.html

PHP:  public string $name = "x";
来源：http://hz.hammf.cn/gtopgokojd.html

JS:   this.name = "x";
来源：http://hz.jqgufenzy.top/gtrhfecmbq.html

TS:   name: string = "x";
来源：http://hz.pycfn.com/gtblprwmjg.html

Java: private String name;
来源：http://hz.fzhhl.top/gtvpswkvdg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.cheryme.top/gtsxsnspua.html

Ruby: @name = "x"
来源：http://hz.feifeiyinyue.top/gthuyvcizt.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yueranfly.top/gtleyvfeea.html

[G04] 定义方法
来源：http://hz.tianlin.xyz/gtfaysnrnf.html

Py:   def greet(self): return self.name
来源：http://hz.quarkkingdee.top/gtymogoheo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.xuetiantiany.cn/gtwzidzpsw.html

JS:   greet() { return this.name; }
来源：http://hz.zhixingplan.top/gtoofocxja.html

TS:   greet(): string { return this.name; }
来源：http://hz.yj202588.top/gtchgpytfm.html

Java: String greet() { return name; }
来源：http://hz.smart0.xyz/gtvhfpeubz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jqgufenzy.top/gtpmfmcwlx.html

Ruby: def greet; @name; end
来源：http://hz.cdnleiting.top/gtxhylxlry.html

C#:   public string Greet() => Name;
来源：http://hz.hammf.cn/gtgkkcgdvz.html

[G05] 继承
来源：http://hz.ehwqpu.com/gtcwzggspi.html

Py:   class Admin(User): pass
来源：http://hz.kuanghao11.cn/gtypgyyogv.html

PHP:  class Admin extends User {}
来源：http://hz.jqgfzy.top/gthxdtgboe.html

JS:   class Admin extends User {}
来源：http://hz.gotoacloud.top/gtjlokzcsq.html

TS:   class Admin extends User {}
来源：http://hz.jlsjyb.cn/gtkybmlxqs.html

Java: class Admin extends User {}
来源：http://hz.meibo888.top/gtichgtsyp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.shanyushiyangtech.top/gtfxrelzxa.html

Ruby: class Admin < User; end
来源：http://hz.yuanzhike.top/gtsdqtzhkt.html

C#:   class Admin : User {}
来源：http://hz.wangdashe.top/gtfifpvenn.html

[G06] 重写方法
来源：http://hz.zhixingplan.top/gtccvkimoj.html

Py:   def greet(self): return "admin"
来源：http://hz.daria6918.cn/gtxjpewhse.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yanxiufei.cn/gtzsrdpvug.html

JS:   greet() { return "admin"; }
来源：http://hz.wangshuangyany.cn/gtpjxidlbd.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yuanzhike.top/gttcghjrkm.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jqgfzy.top/gtyjvqnnpt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.shangyingyoupin.top/gtjvafrgme.html

Ruby: def greet; "admin"; end
来源：http://hz.hnxiangtu.top/gtihbiptxt.html

C#:   public override string Greet() => "admin";
来源：http://hz.sysykeji.top/gtfqlzjrhv.html

[G07] 调用父类方法
来源：http://hz.nwbrower.top/gtcaetrrua.html

Py:   super().greet()
来源：http://hz.guannengcc.top/gtxjjdxwfn.html

PHP:  parent::greet();
来源：http://hz.nwbrower.top/gtutylwbvx.html

JS:   super.greet();
来源：http://hz.hammf.cn/gtokkicsco.html

TS:   super.greet();
来源：http://hz.shangyingyoupin.top/gtaormcwac.html

Java: super.greet();
来源：http://hz.xuanzx.com/gtukleecnx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jyoumei.cn/gttwesmbbi.html

Ruby: super
来源：http://hz.chenzaomai.com/gtkvrlqtys.html

C#:   base.Greet();
来源：http://hz.zhoulong.xyz/gtpzmjkaqo.html

[G08] 静态方法与属性
来源：http://hz.hysaishi.cn/gtunmlcdvj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xziqi.cn/gtjqaqoata.html

PHP:  public static function f() {}
来源：http://hz.chenzaomai.com/gthdeofopr.html

JS:   static f() {}
来源：http://hz.aizwys.cn/gtlmcpvoqi.html

TS:   static f(): void {}
来源：http://hz.ivvv.top/gtcxulfhwj.html

Java: static void f() {}
来源：http://hz.ehwqpu.com/gtzxakwpqi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.daxiang520.top/gtaruzluwl.html

Ruby: def self.f; end
来源：http://hz.cqqwz.cn/gtxmhudzcr.html

C#:   public static void F() {}
来源：http://hz.ivvv.top/gtikseedkd.html

[G09] 接口 / 抽象类
来源：http://hz.yj20258.top/gtapmjqzfw.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.svipenyu.cn/gtinxlurst.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.316326.xyz/gtyheylheq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ydjk.org.cn/gtvcydfvjp.html

TS:   interface Shape { area(): number; }
来源：http://hz.aizwys.cn/gtstcgbyeb.html

Java: interface Shape { double area(); }
来源：http://hz.shangyingyoupin.top/gtjgoejvpr.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jqgfzy.top/gttotdkhux.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhiwuduotai.top/gtiutddvli.html

C#:   interface IShape { double Area(); }
来源：http://hz.yj202588.top/gtofnvcdfo.html

[G10] 访问控制
来源：http://hz.yj202588.top/gthxkadako.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhijiandao.cn/gtellbhccc.html

PHP:  public / protected / private
来源：http://hz.svipenyu.cn/gtrvjbjqpq.html

JS:   #private 字段；其余公开
来源：http://hz.shuidangran.top/gtoaibveeb.html

TS:   public / protected / private
来源：http://hz.jqgfzy.top/gtatlkjdey.html

Java: public / protected / private / 默认包级
来源：http://hz.52xcode.cn/gtbxgqlqyk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.0kj1m.cn/gtvoycwbjb.html

Ruby: public / protected / private
来源：http://hz.zhijiandao.cn/gtshhkneab.html

C#:   public / protected / private / internal
来源：http://hz.smart0.xyz/gtnuisgccc.html

[G11] getter / setter
来源：http://hz.sxryk.cn/gthioncvqz.html

Py:   @property 与 @x.setter
来源：http://hz.redwolf501.top/gtkinqrsik.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.quarkkingdee.top/gtftvylhre.html

JS:   get name() { return this._name; }
来源：http://hz.havefunace.top/gtipofafxi.html

TS:   get name(): string { return this._name; }
来源：http://hz.haohaochexian.top/gtmooyeczz.html

Java: public String getName() { return name; }
来源：http://hz.feifeiyinyue.top/gtekipmivv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.smart0.xyz/gtighknncs.html

Ruby: attr_accessor :name
来源：http://hz.chenzaomai.com/gtppunuxie.html

C#:   public string Name { get; set; }
来源：http://hz.smart0.xyz/gtlpovnkzw.html

[G12] 对象转字符串
来源：http://hz.jqgufenzy.top/gtxemjdnyb.html

Py:   def __str__(self): return self.name
来源：http://hz.jinyuanbaomall.cn/gtxniraybl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.xingfuxueyuan.xyz/gtskdmxrqx.html

JS:   toString() { return this.name; }
来源：http://hz.cdnleiting.top/gtbixwhair.html

TS:   toString(): string { return this.name; }
来源：http://hz.daxiang520.top/gtmbqiipew.html

Java: @Override public String toString() { return name; }
来源：http://hz.hammf.cn/gtuukscmms.html


<!-- 参考信息 -->