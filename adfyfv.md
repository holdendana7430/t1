代发 wailian999

[E14] URL 编码与 Base64
来源：http://hz.jlsjyb.cn/gtmkvdlpsw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.aibaodan.cn/gtrecbhqoz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hfpthk.cn/gttxrltzla.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.xylfe.cn/gtbhjcmrhc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.vqdsnc.cn/gtdqgahwtc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zycfv.cn/gtaluiglpi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yj202588.top/gtyorqlvsz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yj20258.top/gtaqlnutlo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.hysaishi.cn/gtqsuowwnl.html

[E15] HTML 转义 / 反转义
来源：http://hz.hysaishi.cn/gtlfpmdohs.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.quarkkingdee.top/gtohbzkhpf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.chenzaomai.com/gtfojoxmrs.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.fzhhl.top/gtxwgmafnu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.guannengcc.top/gtjyzemrun.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.sysykeji.top/gtjmoodnjq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.cheryme.top/gtrimgwbdl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.shuidangran.top/gtnntiniva.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.316326.xyz/gtloowefij.html

[E16] 数字千分位
来源：http://hz.nanxuanxn.top/gtzzfwowao.html

Py:   f"{1234567:,}"
来源：http://hz.hnqzz.top/gtcivifwls.html

PHP:  number_format(1234567);
来源：http://hz.jqgfzy.top/gthsopkkca.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.fzhhl.top/gtoplhwrmm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.meibo888.top/gtuhzmfikf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.sysykeji.top/gtnmzmdhup.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.kuanghao11.cn/gtjpxiktgj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.hammf.cn/gthklprzoi.html

C#:   1234567.ToString("N0")
来源：http://hz.hywenlv.cn/gtlmwtdxtv.html

[E17] 首字母大写
来源：http://hz.feifeiyinyue.top/gtnlgfqjle.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.hysaishi.cn/gtqppwluwi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.aizwys.cn/gtjidwfldr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinqigufen.top/gteiopllba.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.iojbl.cn/gthqzrwpil.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zhaomingkeji.xyz/gthwmdzumt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yj20258888.top/gtsepjjasc.html

Ruby: s.capitalize
来源：http://hz.xinyue.icu/gtdmfaupzv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.ehwqpu.com/gtdyvmexgw.html

[E18] 模板占位符替换
来源：http://hz.yanxiufei.cn/gttphzkdkq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.shuidangran.top/gtfirueftk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.snrcjt.cn/gtypcxxabs.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yj20258.top/gtbvjzdnbe.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.smart0.xyz/gtyxcfvbnw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.daxiang520.top/gtcghziljq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.xinyue.icu/gtuubeuyyw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.fengsongda.top/gtturugvsp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.shuidangran.top/gtlxogklpi.html

[E19] 多行文本按行拆分
来源：http://hz.wangshuangyany.cn/gtdncpgxfh.html

Py:   s.splitlines()
来源：http://hz.shuidangran.top/gtywdctewg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.0kj1m.cn/gtzmyjwyhh.html

JS:   s.split(/\r?\n/)
来源：http://hz.yueranfly.top/gtzazkohgd.html

TS:   s.split(/\r?\n/)
来源：http://hz.9152youxi.cn/gtpoigijjb.html

Java: s.lines().toList()
来源：http://hz.chenlongwang.top/gtskrzdaqb.html

Go:   strings.Split(s, "\n")
来源：http://hz.bjfxy.top/gtgsdaxjkd.html

Ruby: s.lines
来源：http://hz.kuanghao11.cn/gtuggmwwjn.html

C#:   s.Split('\n')
来源：http://hz.jlsjyb.cn/gtdlnjubno.html

[E20] 判断字符串是否为空
来源：http://hz.xuanzx.com/gtutuzldmn.html

Py:   if not s:
来源：http://hz.zhixingplan.top/gtwdclgfag.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.shanyushiyangtech.top/gtwwwpphme.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.0kj1m.cn/gtuadfuanz.html

TS:   if (s === "") {}
来源：http://hz.shzxlz.cn/gtkhhojxob.html

Java: if (s.isEmpty()) {}
来源：http://hz.gaohongyu789.top/gtovcppstt.html

Go:   if s == "" {}
来源：http://hz.svipenyu.cn/gttnevuvfj.html

Ruby: if s.empty?
来源：http://hz.jinqigufen.top/gtsoxdvmef.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.aizwys.cn/gtiblvlqzv.html

[E21] 超长截断加省略号
来源：http://hz.sufxvd.cn/gtvodglmys.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zhongyouzk.top/gtxybnmofq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.sxryk.cn/gtidcbzqjq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.wangdashe.top/gttfwassar.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.dashuyun.cn/gtxkxjfyyz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.guowangkeji.top/gtqjsfwkgu.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.0kj1m.cn/gtmimveiom.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.9152youxi.cn/gtvbsyefdb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.gotoacloud.top/gtlyrnpdpf.html

[E22] 字节长度与字符长度
来源：http://hz.9152youxi.cn/gthkykmpoa.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.smart0.xyz/gtdzdlmlxh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.52xcode.cn/gtorwpsgbo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yj20258888.top/gtalcfbdhu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jlsjyb.cn/gtpvugvmfp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.sysykeji.top/gtwspwexal.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.bjfxy.top/gtixmsccjj.html

Ruby: s.bytesize;  s.length
来源：http://hz.hysaishi.cn/gtznpugsbd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jyoumei.cn/gtgauumkmv.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtzagvpglu.html

F. 文件与目录
来源：http://hz.jqgfzy.top/gtrazorskf.html

================================================================================
来源：http://hz.svipenyu.cn/gtnoztvoff.html

[F01] 读取整个文件
来源：http://hz.shangyingyoupin.top/gtleeansat.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yueranfly.top/gtxhfouzxk.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yj202588.top/gtpkgnotav.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.cdnleiting.top/gtubqlqouq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhongyouzk.top/gtayruiysg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yongpay.top/gtrrxbiwjr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.quarkkingdee.top/gtsosxcfiv.html

Ruby: File.read("a.txt")
来源：http://hz.ydjk.org.cn/gtucklxcnb.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.dashuyun.cn/gttztfxhau.html

[F02] 逐行读取文件
来源：http://hz.mhx1999.top/gtavrgaajt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ywan-chungtsiang.top/gtzstoytvd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.chenzaomai.com/gtvhzminhv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhiwuduotai.top/gtybqdiiyb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhengqikj.top/gttmthhyhw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hywenlv.cn/gtqlmpczeg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.tanke756.top/gtxvhzydvi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.guannengcc.top/gtkuyloofj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.hongshengwenyu.top/gtrlcklioc.html

[F03] 写入文件（覆盖）
来源：http://hz.svipenyu.cn/gthyiqqeqz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.shzxlz.cn/gtkeveygiv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.shzxlz.cn/gtvrqllkco.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinqigfzy.top/gtyawyzarl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.daria6918.cn/gtqgzqwuiw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.yongpay.top/gtljpduebg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zycfv.cn/gtvzqnszgn.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.nanxuanxn.top/gtbteyywaj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.guowangkeji.top/gtlzdamuor.html

[F04] 追加写入文件
来源：http://hz.vqdsnc.cn/gtcjtowgyi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zhengqikj.top/gtchsbmgma.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.aibaodan.cn/gttzseqmwo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jianghu66.top/gtpmpnluuy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hammf.cn/gtwyrgtzyy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.gogol.net.cn/gtvwqazeje.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zhiwuduotai.top/gteqnpxbwx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.cqqwz.cn/gtrcleemji.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.chenlongwang.top/gtoxkufanc.html

[F05] 判断文件或目录是否存在
来源：http://hz.9152youxi.cn/gtrbmkyklx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.xuanzx.com/gtpmeyntqi.html

PHP:  file_exists("a.txt");
来源：http://hz.chenjidiqi.icu/gtfqvaxled.html

JS:   fs.existsSync("a.txt")
来源：http://hz.quarkkingdee.top/gtdbuudffq.html

TS:   fs.existsSync("a.txt")
来源：http://hz.hywenlv.cn/gttxspygzt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yonumen.top/gtdmafmrqm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.cheryme.top/gtgjdmiulp.html

Ruby: File.exist?("a.txt")
来源：http://hz.cqqwz.cn/gtdcwjttrp.html

C#:   File.Exists("a.txt")
来源：http://hz.feifeiyinyue.top/gtghdpyhpc.html

[F06] 删除文件
来源：http://hz.zhixingplan.top/gtpvzpuksf.html

Py:   os.remove("a.txt")
来源：http://hz.tanke756.top/gtvqckdhzq.html

PHP:  unlink("a.txt");
来源：http://hz.nanxuanxn.top/gttvtevtdr.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.daria6918.cn/gtowoptwxy.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hysaishi.cn/gtbjzolegz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xuanzx.com/gtrolchmij.html

Go:   os.Remove("a.txt")
来源：http://hz.bjfxy.top/gtkpwesuls.html

Ruby: File.delete("a.txt")
来源：http://hz.jianghu66.top/gtaxqcjgvr.html

C#:   File.Delete("a.txt");
来源：http://hz.xuanzx.com/gtycmyapqg.html

[F07] 创建目录（含多级）
来源：http://hz.dianchejie.cn/gtwtfxmgvs.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.cucudq.cn/gtqgzqcwbh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jqgufenzy.top/gtysqvpimc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinyuanbaomall.cn/gtbmvcvcur.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ybcxt.top/gtsbahibmr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.iojbl.cn/gtvrgismea.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jqgufenzy.top/gtxdtuddzm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.shanyushiyangtech.top/gteyhtcush.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.shuidangran.top/gtzuqtcvux.html

[F08] 遍历目录
来源：http://hz.nanxinkj.top/gtnrgkcoap.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhaomingkeji.xyz/gtacpsnyxk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.shuidangran.top/gteczffgkl.html

JS:   fs.readdirSync("dir")
来源：http://hz.gaohongyu789.top/gtfamchtta.html

TS:   fs.readdirSync("dir")
来源：http://hz.ehwqpu.com/gtnhqgmtdj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.wangshuangyany.cn/gtcmnjhbtj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.ydjk.org.cn/gtkrmttitl.html

Ruby: Dir.children("dir")
来源：http://hz.yj20258888.top/gtsmkmazeo.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yj202588.top/gtefombvro.html

[F09] 获取文件大小
来源：http://hz.sweek.top/gtsrmipjll.html

Py:   os.path.getsize("a.txt")
来源：http://hz.vqdsnc.cn/gtyhaammuk.html

PHP:  filesize("a.txt");
来源：http://hz.ivvv.top/gtlrytfjzw.html

JS:   fs.statSync("a.txt").size
来源：http://hz.haohaochexian.top/gtyumzlatg.html

TS:   fs.statSync("a.txt").size
来源：http://hz.guannengcc.top/gttpxybmfc.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.gzhubu.top/gtriyqnvct.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.pengpengdd.cyou/gtuhgjevzn.html

Ruby: File.size("a.txt")
来源：http://hz.quarkkingdee.top/gtlzzyblhv.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.smart0.xyz/gtnpvzofqz.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yj20258888.top/gtkcrhnsiu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jlsjyb.cn/gtzejxcuxn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jianghu66.top/gtvqegnzjs.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yanxiufei.cn/gtxxuehwkt.html

TS:   path.extname("a.txt")
来源：http://hz.hnxiangtu.top/gthpjjrpor.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yonumen.top/gtohwnxjtj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.dashuyun.cn/gtpxwnadhv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.meibo888.top/gtqubqutsb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.sysykeji.top/gtrvreajwp.html

[F11] 复制与移动文件
来源：http://hz.ydjk.org.cn/gtnryhaqbi.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.birdmap.top/gtbpcaifdw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.quarkkingdee.top/gtqkijtaoe.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hfpthk.cn/gtqgsqoivk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhaomingkeji.xyz/gtvirghnka.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hysaishi.cn/gtvqbmnxge.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.chenlongwang.top/gtxwgaidre.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.nwbrower.top/gthtzckouw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.havefunace.top/gtucwnzjwv.html

[F12] CSV 读写
来源：http://hz.hongshengwenyu.top/gtbfaeudph.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhaomingkeji.xyz/gtixahbkhw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yuanzhike.top/gtdkrknqtn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.birdmap.top/gtfpdfymmw.html

TS:   // 同上
来源：http://hz.jiagoushi.top/gtusobtash.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.cqqwz.cn/gtznyzbeum.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yuxming.cn/gtrryhzqax.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.cashguo.top/gtvugxuwqs.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.gogol.net.cn/gtitumbfhn.html

================================================================================
来源：http://hz.ppjwa.cn/gtzvhvzwwd.html

G. 面向对象
来源：http://hz.shanyushiyangtech.top/gtzepgeift.html

================================================================================
来源：http://hz.kuanghao11.cn/gtamvoexla.html

[G01] 定义类
来源：http://hz.hongshengwenyu.top/gtlfydmaae.html

Py:   class User: pass
来源：http://hz.kuanghao11.cn/gtotfgbloz.html

PHP:  class User {}
来源：http://hz.cqqwz.cn/gttxukhktu.html

JS:   class User {}
来源：http://hz.52xcode.cn/gtgelinkhd.html

TS:   class User { name: string = ""; }
来源：http://hz.ivvv.top/gtniwppazm.html

Java: class User {}
来源：http://hz.yangfankeji.com/gthutzkdvy.html

Go:   type User struct { Name string }
来源：http://hz.cheryme.top/gtgvbzvydo.html

Ruby: class User; end
来源：http://hz.yongpay.top/gtzhhhzlvf.html

C#:   class User {}
来源：http://hz.nanxuanxn.top/gtdlwegffh.html

[G02] 构造函数
来源：http://hz.chenzaomai.com/gthpcmsghx.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hnqzz.top/gtddjlrrgh.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.wangdashe.top/gtfkoqbckr.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.52xcode.cn/gtxhiqjqqv.html

TS:   constructor(public name: string) {}
来源：http://hz.chenlongwang.top/gtwhsdfmes.html

Java: User(String name) { this.name = name; }
来源：http://hz.snrcjt.cn/gtnaalnrym.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zhiwuduotai.top/gtuiswgpqt.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.sysykeji.top/gtkcndqkyu.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ivvv.top/gtwnvrooir.html

[G03] 实例属性
来源：http://hz.yj20258888.top/gtwvizltfm.html

Py:   self.name = "x"
来源：http://hz.ywan-chungtsiang.top/gtnuwamokg.html

PHP:  public string $name = "x";
来源：http://hz.pycfn.com/gtechvqkyz.html

JS:   this.name = "x";
来源：http://hz.xziqi.cn/gthwkentkq.html

TS:   name: string = "x";
来源：http://hz.sufxvd.cn/gtodhlwqvk.html

Java: private String name;
来源：http://hz.haohaochexian.top/gtwjbvftgd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yvedp.cn/gtaydqltea.html

Ruby: @name = "x"
来源：http://hz.yueranfly.top/gtujqyhqfa.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jqgufenzy.top/gtrurornbw.html

[G04] 定义方法
来源：http://hz.hysaishi.cn/gtmnjkfhkb.html

Py:   def greet(self): return self.name
来源：http://hz.nanxuanxn.top/gtbxbwdloj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yueranfly.top/gtqizmtsgo.html

JS:   greet() { return this.name; }
来源：http://hz.jinqigfzy.top/gtldrudxtz.html

TS:   greet(): string { return this.name; }
来源：http://hz.shuidangran.top/gtrisbvurl.html

Java: String greet() { return name; }
来源：http://hz.0kj1m.cn/gtbbijeyjg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.fengsongda.top/gterdjspld.html

Ruby: def greet; @name; end
来源：http://hz.shuidangran.top/gtmjjifkvh.html

C#:   public string Greet() => Name;
来源：http://hz.c1oappe.top/gtrjjpohpt.html

[G05] 继承
来源：http://hz.hysaishi.cn/gtubhyuvfe.html

Py:   class Admin(User): pass
来源：http://hz.xingfuxueyuan.xyz/gtrcooreal.html

PHP:  class Admin extends User {}
来源：http://hz.pengpengdd.cyou/gtmvicgskx.html

JS:   class Admin extends User {}
来源：http://hz.yvedp.cn/gtfcslywfn.html

TS:   class Admin extends User {}
来源：http://hz.yongpay.top/gtgvkjgave.html

Java: class Admin extends User {}
来源：http://hz.yanxiufei.cn/gtjhnbwqxv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.snrcjt.cn/gtjrmpfenb.html

Ruby: class Admin < User; end
来源：http://hz.c1oappe.top/gtsvzxxdwx.html

C#:   class Admin : User {}
来源：http://hz.chenlongwang.top/gtbgsnslxf.html

[G06] 重写方法
来源：http://hz.chenjidiqi.icu/gtflvpewam.html

Py:   def greet(self): return "admin"
来源：http://hz.snrcjt.cn/gtzgvlugyo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.sxryk.cn/gtznzsudhn.html

JS:   greet() { return "admin"; }
来源：http://hz.chenjidiqi.icu/gttctvinqt.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yuanzhike.top/gtaxnzuwlk.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.tian-w.cn/gtekmyrtvy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.316326.xyz/gtohfqewuj.html

Ruby: def greet; "admin"; end
来源：http://hz.ehwqpu.com/gtfbjmmjdc.html

C#:   public override string Greet() => "admin";
来源：http://hz.yueranfly.top/gtdbtwveiq.html

[G07] 调用父类方法
来源：http://hz.jlsjyb.cn/gtlrjjtimo.html

Py:   super().greet()
来源：http://hz.feifeiyinyue.top/gtfewfxdom.html

PHP:  parent::greet();
来源：http://hz.316326.xyz/gtgabflyqn.html

JS:   super.greet();
来源：http://hz.zhijiandao.cn/gtlctloldk.html

TS:   super.greet();
来源：http://hz.svipenyu.cn/gtwvudumsw.html

Java: super.greet();
来源：http://hz.jinqigufen.top/gtsonxtmjp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhoulong.xyz/gtfhisvego.html

Ruby: super
来源：http://hz.ppjwa.cn/gtrxzctatc.html

C#:   base.Greet();
来源：http://hz.xingfuxueyuan.xyz/gttmncpjty.html

[G08] 静态方法与属性
来源：http://hz.xingfuxueyuan.xyz/gtlmiohgce.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xziqi.cn/gtowhzmwqs.html

PHP:  public static function f() {}
来源：http://hz.yongpay.top/gtibdzvhkk.html

JS:   static f() {}
来源：http://hz.cucudq.cn/gtonvwajot.html

TS:   static f(): void {}
来源：http://hz.jinqigufen.top/gtymmvdtdt.html

Java: static void f() {}
来源：http://hz.hywenlv.cn/gtpbywcpsn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yvedp.cn/gtwdzuszhl.html

Ruby: def self.f; end
来源：http://hz.xuanzx.com/gtlaigvcen.html

C#:   public static void F() {}
来源：http://hz.yj202588.top/gtoaxhcpke.html

[G09] 接口 / 抽象类
来源：http://hz.smart0.xyz/gticloewce.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yuxming.cn/gtsjrgsmwp.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.gogol.net.cn/gtjtsjpsnj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ybcxt.top/gtwkucoyfk.html

TS:   interface Shape { area(): number; }
来源：http://hz.hnqzz.top/gtlgchbdor.html

Java: interface Shape { double area(); }
来源：http://hz.chenjidiqi.icu/gtfnkatyjz.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yj20258888.top/gtskzwmcmv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.smart0.xyz/gtgbjtiljt.html

C#:   interface IShape { double Area(); }
来源：http://hz.cashguo.top/gtujfcnlaf.html

[G10] 访问控制
来源：http://hz.xuetiantiany.cn/gtbgofmmub.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.redwolf501.top/gtdvpazfkm.html

PHP:  public / protected / private
来源：http://hz.316326.xyz/gtkswvzcjx.html

JS:   #private 字段；其余公开
来源：http://hz.yuxming.cn/gtgmmesxet.html

TS:   public / protected / private
来源：http://hz.jinqigufen.top/gtdlzhmoky.html

Java: public / protected / private / 默认包级
来源：http://hz.shanyushiyangtech.top/gtrxgvxrtf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.quarkkingdee.top/gttufvxfsd.html

Ruby: public / protected / private
来源：http://hz.yj20258.top/gtovgsobvv.html

C#:   public / protected / private / internal
来源：http://hz.xuanzx.com/gtfqubbguj.html

[G11] getter / setter
来源：http://hz.yonumen.top/gtrpwcjiwj.html

Py:   @property 与 @x.setter
来源：http://hz.feifeiyinyue.top/gtcppztkbk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.ydzc1.top/gtxfbeosmi.html

JS:   get name() { return this._name; }
来源：http://hz.quarkkingdee.top/gtdmqzrgza.html

TS:   get name(): string { return this._name; }
来源：http://hz.redwolf501.top/gtifuzzqyg.html

Java: public String getName() { return name; }
来源：http://hz.mhx1999.top/gtdmkyehgu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhixingplan.top/gtbmkgibac.html

Ruby: attr_accessor :name
来源：http://hz.shzxlz.cn/gtwtpvtdue.html

C#:   public string Name { get; set; }
来源：http://hz.mhx1999.top/gtsutypwfs.html

[G12] 对象转字符串
来源：http://hz.daxiang520.top/gtgegprzzn.html

Py:   def __str__(self): return self.name
来源：http://hz.ybcxt.top/gtbymklnjm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.gaohongyu789.top/gtlakpkgsk.html

JS:   toString() { return this.name; }
来源：http://hz.hongshengwenyu.top/gtajxfnllc.html

TS:   toString(): string { return this.name; }
来源：http://hz.sxryk.cn/gtlihjigfy.html

Java: @Override public String toString() { return name; }
来源：http://hz.ydjk.org.cn/gtxbiuuefx.html


<!-- 参考信息 -->