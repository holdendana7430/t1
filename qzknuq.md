代发 wailian999

[E14] URL 编码与 Base64
来源：http://hz.gzhubu.top/gtabqfprwg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.wangshuangyany.cn/gtqoloeyrx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.xinyue.icu/gthkelhzuw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.shanyushiyangkeji.top/gteoeupnez.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.cdnleiting.top/gtsuocjwhb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.ydjk.org.cn/gtaelxlpjd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhaomingkeji.xyz/gtazhfbfim.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zycfv.cn/gtkabgmnig.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhaomingkeji.xyz/gtatqvfmyq.html

[E15] HTML 转义 / 反转义
来源：http://hz.zhaomingkeji.xyz/gtkdmvtxwi.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.c1oappe.top/gtbquwyzfn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yvedp.cn/gtdtleppev.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.fengsongda.top/gtmxbklyom.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.fzhhl.top/gtyioymjmi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.gaohongyu789.top/gtbfzhccjx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yonumen.top/gtlktidvwt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.52xcode.cn/gtruixvxsc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.fzhhl.top/gtxywoezoq.html

[E16] 数字千分位
来源：http://hz.zhixingplan.top/gtwsuxlhte.html

Py:   f"{1234567:,}"
来源：http://hz.zhixingplan.top/gtdlbwguqc.html

PHP:  number_format(1234567);
来源：http://hz.tianlin.xyz/gtmufsooim.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.andypj.xyz/gtmhjlxeoa.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.tanke756.top/gtsowpmuhj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.52xcode.cn/gtkxtrtouw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.0kj1m.cn/gtsaqaezrx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.pengpengdd.cyou/gtrjljwggl.html

C#:   1234567.ToString("N0")
来源：http://hz.ehwqpu.com/gtfjiwunyn.html

[E17] 首字母大写
来源：http://hz.feifeiyinyue.top/gtgebkvhfw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.ybcxt.top/gtuprtxhth.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zhaomingkeji.xyz/gtpvojuliv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zdqjudy.top/gtmkmxaako.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cashguo.top/gthuidshvr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.iojbl.cn/gtudykvcsu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.nanxuanxn.top/gtrglmwfad.html

Ruby: s.capitalize
来源：http://hz.tian-w.cn/gtdhejnvbe.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yuxming.cn/gtyhmktppx.html

[E18] 模板占位符替换
来源：http://hz.hongshengwenyu.top/gthulszeej.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.bjfxy.top/gtzfibmdar.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.cdnleiting.top/gtmwexbelk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.vqdsnc.cn/gtkjupzvmj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zdqjudy.top/gtstlxfbfn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.pengpengdd.cyou/gtmclnserf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.gzhubu.top/gtolabzqal.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zhaomingkeji.xyz/gtlixwdyrj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.dashuyun.cn/gtpkgghher.html

[E19] 多行文本按行拆分
来源：http://hz.shanyushiyangtech.top/gtxmgrfvox.html

Py:   s.splitlines()
来源：http://hz.ydzc1.top/gthgnccflf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.hfpthk.cn/gteesrizub.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhengqikj.top/gthtioxjzv.html

TS:   s.split(/\r?\n/)
来源：http://hz.gogol.net.cn/gtsoznljil.html

Java: s.lines().toList()
来源：http://hz.yongpay.top/gtcounvpwb.html

Go:   strings.Split(s, "\n")
来源：http://hz.chenzaomai.com/gtloipismc.html

Ruby: s.lines
来源：http://hz.havefunace.top/gtlawsexym.html

C#:   s.Split('\n')
来源：http://hz.yueranfly.top/gtbkguppyp.html

[E20] 判断字符串是否为空
来源：http://hz.52xcode.cn/gtkxocpduw.html

Py:   if not s:
来源：http://hz.cheryme.top/gtpzrxpazf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yvedp.cn/gtaftfilvz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.ydzc1.top/gtopvuzscl.html

TS:   if (s === "") {}
来源：http://hz.yj20258888.top/gtrxwyodiw.html

Java: if (s.isEmpty()) {}
来源：http://hz.fengsongda.top/gtpubostxg.html

Go:   if s == "" {}
来源：http://hz.cashguo.top/gtvezcymhy.html

Ruby: if s.empty?
来源：http://hz.daxiang520.top/gtglszehzl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.shuidangran.top/gtxzzsmnlp.html

[E21] 超长截断加省略号
来源：http://hz.jiagoushi.top/gtfhtiiqfa.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.xuanzx.com/gtyqcprwop.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jinghuilouyu.cn/gtykgyhbsy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.sufxvd.cn/gtrnxzdkcb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.316326.xyz/gtddxhpdfg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yangfankeji.com/gtxgfyeydt.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.aizwys.cn/gtqrtvxpyz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.wangshuangyany.cn/gtqtctyalg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.fzhhl.top/gtxzphwsqs.html

[E22] 字节长度与字符长度
来源：http://hz.9152youxi.cn/gtmxlkjmji.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.sufxvd.cn/gtvpdpcdpq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xuetiantiany.cn/gtyxysvssv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cashguo.top/gtzcbhyiyf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hysaishi.cn/gtgifesfgm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.dashuyun.cn/gtmoacrusf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhixingplan.top/gtkfftuyxz.html

Ruby: s.bytesize;  s.length
来源：http://hz.jinghuilouyu.cn/gtwkrdfhky.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zhixingplan.top/gtknvulhwj.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtbpadcdgy.html

F. 文件与目录
来源：http://hz.birdmap.top/gtpspzsjcm.html

================================================================================
来源：http://hz.cdnleiting.top/gtcogkmudd.html

[F01] 读取整个文件
来源：http://hz.jqgufenzy.top/gtsvemwoep.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.52xcode.cn/gtduhddvlh.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zhijiandao.cn/gtfjcvuigh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.haohaochexian.top/gtsmxtcooj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.chenjidiqi.icu/gtkswvzbjo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhijiandao.cn/gtmfafawfg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.gotoacloud.top/gtsuiztktk.html

Ruby: File.read("a.txt")
来源：http://hz.xylfe.cn/gtqrrxvivf.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.aibaodan.cn/gtautpwofe.html

[F02] 逐行读取文件
来源：http://hz.xinyue.icu/gtlwwtzucz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zhaomingkeji.xyz/gtrpqspajf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ydjk.org.cn/gttafgfrmy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gogol.net.cn/gtwtzhznad.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.fzhhl.top/gtsxiwqofb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hfpthk.cn/gtmgneobwb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hongshengwenyu.top/gtygwnuvcw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.cqqwz.cn/gtujwrzizq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.gotoacloud.top/gtlvtvfaef.html

[F03] 写入文件（覆盖）
来源：http://hz.kuanghao11.cn/gtmkpwvdvj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.meibo888.top/gttqkqgexs.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.cqqwz.cn/gtcpxnqqib.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hysaishi.cn/gtauffqzdl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shanyushiyangtech.top/gthiykxoqv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.shanyushiyangtech.top/gtvbczpdml.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.nwbrower.top/gtzevhualg.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ydzc1.top/gtvmvcfnuw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jyoumei.cn/gtqgetkrjw.html

[F04] 追加写入文件
来源：http://hz.feifeiyinyue.top/gtejhlwobo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.dianchejie.cn/gtsghlwajh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.gogol.net.cn/gtxtuojgzb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ppjwa.cn/gtfivgrpyf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nwbrower.top/gtmsakldpx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ivvv.top/gtbnzpgdon.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.shanyushiyangtech.top/gtykepqbak.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.gotoacloud.top/gtgkzduaub.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.sweek.top/gtwlzwhqvn.html

[F05] 判断文件或目录是否存在
来源：http://hz.pengpengdd.cyou/gtdyzzfcoi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yuanzhike.top/gthjwvzdck.html

PHP:  file_exists("a.txt");
来源：http://hz.yj20258888.top/gtvmlastjb.html

JS:   fs.existsSync("a.txt")
来源：http://hz.tian-w.cn/gtttzvfryr.html

TS:   fs.existsSync("a.txt")
来源：http://hz.shangyingyoupin.top/gtrurgnkwz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ppjwa.cn/gtpzzvpwnl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.tian-w.cn/gtrudrhdan.html

Ruby: File.exist?("a.txt")
来源：http://hz.iojbl.cn/gtrhldvtqn.html

C#:   File.Exists("a.txt")
来源：http://hz.jinqigufen.top/gtdpxapmqo.html

[F06] 删除文件
来源：http://hz.zhijiandao.cn/gtvkcnuepr.html

Py:   os.remove("a.txt")
来源：http://hz.dianchejie.cn/gtcfmsukpf.html

PHP:  unlink("a.txt");
来源：http://hz.zhaomingkeji.xyz/gtmqtgtmgy.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yangfankeji.com/gtpnjmvmhm.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zhoulong.xyz/gttoqemabm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.cashguo.top/gtdjelwxmg.html

Go:   os.Remove("a.txt")
来源：http://hz.birdmap.top/gtmslcnczb.html

Ruby: File.delete("a.txt")
来源：http://hz.sysykeji.top/gteazbgpwf.html

C#:   File.Delete("a.txt");
来源：http://hz.ppjwa.cn/gtizqkjwlv.html

[F07] 创建目录（含多级）
来源：http://hz.chenlongwang.top/gtrqatospc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.xuanzx.com/gtzvlihdje.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.shanyushiyangtech.top/gtkqqszkwh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hongshengwenyu.top/gtxszohnhr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhengqikj.top/gtezbeiyxc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xziqi.cn/gtdxktaoam.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.svipenyu.cn/gtjqpgejol.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.dianchejie.cn/gtrrsytkiz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.chenzaomai.com/gtzxpddxfk.html

[F08] 遍历目录
来源：http://hz.hnqzz.top/gtkssdwsqn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.guannengcc.top/gtifzxrjky.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.sweek.top/gtdbysgast.html

JS:   fs.readdirSync("dir")
来源：http://hz.pycfn.com/gtlkikvwjb.html

TS:   fs.readdirSync("dir")
来源：http://hz.chenzaomai.com/gtpivxdfjs.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.wangshuangyany.cn/gtzryebgio.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.gogol.net.cn/gtdyvgfkea.html

Ruby: Dir.children("dir")
来源：http://hz.tian-w.cn/gtxotqucno.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yonumen.top/gtccicxdwe.html

[F09] 获取文件大小
来源：http://hz.shangyingyoupin.top/gtvhxjunfi.html

Py:   os.path.getsize("a.txt")
来源：http://hz.fengsongda.top/gtfhjvuikh.html

PHP:  filesize("a.txt");
来源：http://hz.yueranfly.top/gtxrsneyne.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hongshengwenyu.top/gtsnwkzhej.html

TS:   fs.statSync("a.txt").size
来源：http://hz.nanxinkj.top/gttcpheswt.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.sysykeji.top/gtkaydlrpj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hywenlv.cn/gtbbrzhevv.html

Ruby: File.size("a.txt")
来源：http://hz.shangyingyoupin.top/gtabodnjnj.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.c1oappe.top/gtubdnwjlp.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yuanzhike.top/gtdrvgttht.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yangfankeji.com/gtceigxtwk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.quarkkingdee.top/gtlxrxqpsa.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.shanyushiyangkeji.top/gtmpokcisd.html

TS:   path.extname("a.txt")
来源：http://hz.chenzaomai.com/gtnqhlchpf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.dianchejie.cn/gtwsymuqbh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.cheryme.top/gtgzgoqszd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gtsdtotaoo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.guannengcc.top/gtydpgcjcn.html

[F11] 复制与移动文件
来源：http://hz.yongpay.top/gtnkqdkaxo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.birdmap.top/gtptjexkzg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.cqqwz.cn/gtygsbzyjo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.quarkkingdee.top/gtumlwfdow.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.guannengcc.top/gtjddaoolp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.shangyingyoupin.top/gtsxprdfyu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.chenzaomai.com/gtccsjkzyf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.pycfn.com/gtgunxnpte.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.cdnleiting.top/gtijjupiks.html

[F12] CSV 读写
来源：http://hz.0kj1m.cn/gtfcloiwzg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ivvv.top/gtraaqlqud.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.mhx1999.top/gtlzksaqbg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.chenjidiqi.icu/gtdgryhpoi.html

TS:   // 同上
来源：http://hz.ywan-chungtsiang.top/gtyculyvrs.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.andypj.xyz/gtlbivvwtw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.nanxuanxn.top/gtlehrwnpp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.tianlin.xyz/gtozfzngbp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.c1oappe.top/gtddprrbqv.html

================================================================================
来源：http://hz.vqdsnc.cn/gtgjxmqhpi.html

G. 面向对象
来源：http://hz.zhijiandao.cn/gtzdujnjxu.html

================================================================================
来源：http://hz.yj202588.top/gtamzgorzn.html

[G01] 定义类
来源：http://hz.wangshuangyany.cn/gtwrbqpdnl.html

Py:   class User: pass
来源：http://hz.yangfankeji.com/gtqzhpeywa.html

PHP:  class User {}
来源：http://hz.kuanghao11.cn/gtygqkhdxi.html

JS:   class User {}
来源：http://hz.52xcode.cn/gtfdjzpxja.html

TS:   class User { name: string = ""; }
来源：http://hz.9152youxi.cn/gtamnosoqb.html

Java: class User {}
来源：http://hz.tanke756.top/gthmnyhsjz.html

Go:   type User struct { Name string }
来源：http://hz.zhaomingkeji.xyz/gtzovjeuvi.html

Ruby: class User; end
来源：http://hz.shzxlz.cn/gtheshpjks.html

C#:   class User {}
来源：http://hz.quarkkingdee.top/gtyemrdmag.html

[G02] 构造函数
来源：http://hz.jyoumei.cn/gtakhugnhi.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.shzxlz.cn/gtomsauspy.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.gzhubu.top/gtegopldoi.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.havefunace.top/gtngxgmmsn.html

TS:   constructor(public name: string) {}
来源：http://hz.jianghu66.top/gtgfvxdpsk.html

Java: User(String name) { this.name = name; }
来源：http://hz.sysykeji.top/gtkeiadvip.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.daxiang520.top/gtaeiordbq.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.meibo888.top/gtbyhwbsec.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ywan-chungtsiang.top/gtcbognxrm.html

[G03] 实例属性
来源：http://hz.jlsjyb.cn/gtucumonpv.html

Py:   self.name = "x"
来源：http://hz.shuidangran.top/gtfoybalpw.html

PHP:  public string $name = "x";
来源：http://hz.guannengcc.top/gtpkgzjfdj.html

JS:   this.name = "x";
来源：http://hz.svipenyu.cn/gtxlkrugxh.html

TS:   name: string = "x";
来源：http://hz.vqdsnc.cn/gtzbeftxde.html

Java: private String name;
来源：http://hz.316326.xyz/gtyixogvpt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.iojbl.cn/gtjwkmohui.html

Ruby: @name = "x"
来源：http://hz.jlsjyb.cn/gtdodqqlcy.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.chenlongwang.top/gtyabwrgcl.html

[G04] 定义方法
来源：http://hz.xylfe.cn/gtvighqgaj.html

Py:   def greet(self): return self.name
来源：http://hz.yanxiufei.cn/gtjxbseffl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.cucudq.cn/gtdviklvig.html

JS:   greet() { return this.name; }
来源：http://hz.wangshuangyany.cn/gteimthyqt.html

TS:   greet(): string { return this.name; }
来源：http://hz.cheryme.top/gthpiiwatr.html

Java: String greet() { return name; }
来源：http://hz.tanke756.top/gtoqewyhnq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xingfuxueyuan.xyz/gtlrgssqgi.html

Ruby: def greet; @name; end
来源：http://hz.c1oappe.top/gttcomsvvo.html

C#:   public string Greet() => Name;
来源：http://hz.jyoumei.cn/gtkqrgcety.html

[G05] 继承
来源：http://hz.birdmap.top/gtyvcxfotm.html

Py:   class Admin(User): pass
来源：http://hz.ywan-chungtsiang.top/gtosmqnlys.html

PHP:  class Admin extends User {}
来源：http://hz.kuanghao11.cn/gtvujdybyp.html

JS:   class Admin extends User {}
来源：http://hz.dianchejie.cn/gtfitdnwxx.html

TS:   class Admin extends User {}
来源：http://hz.shuidangran.top/gtoamjevzm.html

Java: class Admin extends User {}
来源：http://hz.gotoacloud.top/gtldaqpzxt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhixingplan.top/gtphasmkjc.html

Ruby: class Admin < User; end
来源：http://hz.zhoulong.xyz/gtoxulmlbs.html

C#:   class Admin : User {}
来源：http://hz.cheryme.top/gtvnkzgtqy.html

[G06] 重写方法
来源：http://hz.xylfe.cn/gtugzufdxg.html

Py:   def greet(self): return "admin"
来源：http://hz.smart0.xyz/gtaowuppbr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.svipenyu.cn/gtnsbjouos.html

JS:   greet() { return "admin"; }
来源：http://hz.gaohongyu789.top/gtrizlzyei.html

TS:   greet(): string { return "admin"; }
来源：http://hz.aibaodan.cn/gtmmhpvdpe.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.52xcode.cn/gtgkyqhxuh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.hywenlv.cn/gtkiomsikf.html

Ruby: def greet; "admin"; end
来源：http://hz.xingfuxueyuan.xyz/gttxmlqmjs.html

C#:   public override string Greet() => "admin";
来源：http://hz.snrcjt.cn/gtvtdwqwmm.html

[G07] 调用父类方法
来源：http://hz.smart0.xyz/gtfstijtuu.html

Py:   super().greet()
来源：http://hz.zdqjudy.top/gtnzxapjll.html

PHP:  parent::greet();
来源：http://hz.hysaishi.cn/gthchuoaxn.html

JS:   super.greet();
来源：http://hz.yj20258.top/gtnwroacht.html

TS:   super.greet();
来源：http://hz.guowangkeji.top/gtkdacxuxf.html

Java: super.greet();
来源：http://hz.xziqi.cn/gtkbcrzuco.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yangfankeji.com/gtjxdxazot.html

Ruby: super
来源：http://hz.nanxinkj.top/gtdrtrfiir.html

C#:   base.Greet();
来源：http://hz.ydjk.org.cn/gtvejpgchw.html

[G08] 静态方法与属性
来源：http://hz.0kj1m.cn/gtkwrwoxzn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xingfuxueyuan.xyz/gtilrulavb.html

PHP:  public static function f() {}
来源：http://hz.yueranfly.top/gtdzmihkxq.html

JS:   static f() {}
来源：http://hz.ivvv.top/gtjhaxdtlr.html

TS:   static f(): void {}
来源：http://hz.ydjk.org.cn/gtqtjrtbvi.html

Java: static void f() {}
来源：http://hz.yueranfly.top/gteabdipqh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jqgfzy.top/gtbchwxlfa.html

Ruby: def self.f; end
来源：http://hz.jinyuanbaomall.cn/gtxnkcilju.html

C#:   public static void F() {}
来源：http://hz.tianlin.xyz/gtmehbemli.html

[G09] 接口 / 抽象类
来源：http://hz.yvedp.cn/gtwaakvavx.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jlsjyb.cn/gtmmmicfal.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.nanxuanxn.top/gtayiuyrxw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zdqjudy.top/gtvpwnoaqn.html

TS:   interface Shape { area(): number; }
来源：http://hz.yanxiufei.cn/gtpovohftt.html

Java: interface Shape { double area(); }
来源：http://hz.havefunace.top/gtdrgkzhjb.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhongyouzk.top/gttnucofqj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.nwbrower.top/gtywhurstf.html

C#:   interface IShape { double Area(); }
来源：http://hz.wangdashe.top/gtmuvfzmpk.html

[G10] 访问控制
来源：http://hz.bjfxy.top/gtqyqkntqf.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.xinyue.icu/gtjmvrokhf.html

PHP:  public / protected / private
来源：http://hz.nanxuanxn.top/gtqrxdsttp.html

JS:   #private 字段；其余公开
来源：http://hz.aibaodan.cn/gtictjbofm.html

TS:   public / protected / private
来源：http://hz.vqdsnc.cn/gtzxfxpgtu.html

Java: public / protected / private / 默认包级
来源：http://hz.ivvv.top/gtdxitgtcm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.haohaochexian.top/gtzklyofpj.html

Ruby: public / protected / private
来源：http://hz.cdnleiting.top/gtxnnfkvbk.html

C#:   public / protected / private / internal
来源：http://hz.0kj1m.cn/gtfpoajrij.html

[G11] getter / setter
来源：http://hz.fengsongda.top/gtnlknwzcz.html

Py:   @property 与 @x.setter
来源：http://hz.hongshengwenyu.top/gtwglumset.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.tianlin.xyz/gtrgatjoeu.html

JS:   get name() { return this._name; }
来源：http://hz.zycfv.cn/gtieiugwut.html

TS:   get name(): string { return this._name; }
来源：http://hz.smart0.xyz/gtsnzphkdt.html

Java: public String getName() { return name; }
来源：http://hz.chenjidiqi.icu/gtzzhkylsm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.wangshuangyany.cn/gtuptptnjc.html

Ruby: attr_accessor :name
来源：http://hz.hywenlv.cn/gthbquyjei.html

C#:   public string Name { get; set; }
来源：http://hz.ehwqpu.com/gtociecscj.html

[G12] 对象转字符串
来源：http://hz.xuanzx.com/gtdcfxobzh.html

Py:   def __str__(self): return self.name
来源：http://hz.gaohongyu789.top/gthyybjwdk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jyoumei.cn/gtcnseyduw.html

JS:   toString() { return this.name; }
来源：http://hz.jinghuilouyu.cn/gtloycnbmb.html

TS:   toString(): string { return this.name; }
来源：http://hz.jiagoushi.top/gtwyhjyrpl.html

Java: @Override public String toString() { return name; }
来源：http://hz.ydjk.org.cn/gtpglkgmxi.html


<!-- 参考信息 -->