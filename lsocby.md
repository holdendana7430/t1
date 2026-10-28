代发 wailian999

Go:   strings.Count(s, "a")
来源：http://hz.jinqigufen.top/gtcrfubjum.html

Ruby: s.count("a")
来源：http://hz.xuanzx.com/gtkseuxyqw.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zhengqikj.top/gtuzcgnyxp.html

[E13] 逐字符遍历
来源：http://hz.daria6918.cn/gtygxldfrs.html

Py:   for ch in s: print(ch)
来源：http://hz.jqgfzy.top/gtugishydm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.hnqzz.top/gtmumjynpg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gogol.net.cn/gtbfhbtijy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shanyushiyangtech.top/gtcthappuv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.pengpengdd.cyou/gtrejjvsch.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.sufxvd.cn/gtqqfaliqj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.quarkkingdee.top/gtpccyxink.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jqgfzy.top/gtultsmekm.html

[E14] URL 编码与 Base64
来源：http://hz.wangshuangyany.cn/gtotbwtvmq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.xylfe.cn/gtkqmtkjrt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.sufxvd.cn/gtuenrtppk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yueranfly.top/gtfindkujv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.tian-w.cn/gtyvdzlzxb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.guowangkeji.top/gteybrtdrj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yj20258888.top/gtiltgmtgy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.sweek.top/gtihkhfihj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.cashguo.top/gtpvwsgehv.html

[E15] HTML 转义 / 反转义
来源：http://hz.xziqi.cn/gtzdsbgmfr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.cqqwz.cn/gtofkhltiu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.sweek.top/gtgzwfbuvh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jqgfzy.top/gtetbfuaga.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jianghu66.top/gtbpkuikse.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.daria6918.cn/gtpcjyeokz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.c1oappe.top/gtmsunqmmc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.daxiang520.top/gtplbrxpyf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.ybcxt.top/gtmdvczbef.html

[E16] 数字千分位
来源：http://hz.hammf.cn/gtklkukylz.html

Py:   f"{1234567:,}"
来源：http://hz.smart0.xyz/gtlcwvymdv.html

PHP:  number_format(1234567);
来源：http://hz.havefunace.top/gtuopdttbt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.andypj.xyz/gtnojsrwno.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.gogol.net.cn/gtbtezbxco.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.wangdashe.top/gtreoacsuc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.quarkkingdee.top/gtxfbvgrxg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.pycfn.com/gtcjavkjyv.html

C#:   1234567.ToString("N0")
来源：http://hz.chenlongwang.top/gtdnyrbgmz.html

[E17] 首字母大写
来源：http://hz.hnxiangtu.top/gtjviwmdvv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zhixingplan.top/gthgtfwawz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zhengqikj.top/gtoowgcmfc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.daxiang520.top/gtkxvrvzjf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.iojbl.cn/gtyoffzzzk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.52xcode.cn/gtnipqhhro.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.fengsongda.top/gtqodluoyl.html

Ruby: s.capitalize
来源：http://hz.yvedp.cn/gtmplolamz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.feifeiyinyue.top/gtkdybjwif.html

[E18] 模板占位符替换
来源：http://hz.iojbl.cn/gthwjvaajj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yuxming.cn/gtpefjawcy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zdqjudy.top/gtbbrvlwai.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.iojbl.cn/gtvnatyfjf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.meibo888.top/gtwvgwybzd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.ivvv.top/gtxgzycdug.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.snrcjt.cn/gtlvaekvdk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.vqdsnc.cn/gtaweyyuiw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yanxiufei.cn/gttddigcca.html

[E19] 多行文本按行拆分
来源：http://hz.zhongyouzk.top/gtuokgirsa.html

Py:   s.splitlines()
来源：http://hz.sweek.top/gtrmjjgiiy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.redwolf501.top/gtjecxcqtt.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhiwuduotai.top/gtmbfxaqsw.html

TS:   s.split(/\r?\n/)
来源：http://hz.gzhubu.top/gtqrwaqlkd.html

Java: s.lines().toList()
来源：http://hz.jinqigfzy.top/gthxmhothj.html

Go:   strings.Split(s, "\n")
来源：http://hz.sufxvd.cn/gtdicxksuq.html

Ruby: s.lines
来源：http://hz.pengpengdd.cyou/gtnmeddybu.html

C#:   s.Split('\n')
来源：http://hz.pycfn.com/gtoxtswhko.html

[E20] 判断字符串是否为空
来源：http://hz.chenlongwang.top/gtcuriicso.html

Py:   if not s:
来源：http://hz.shanyushiyangkeji.top/gtjpjbidtp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.fzhhl.top/gtxyjnhwdo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hysaishi.cn/gtseltqlou.html

TS:   if (s === "") {}
来源：http://hz.andypj.xyz/gtrnqvasdb.html

Java: if (s.isEmpty()) {}
来源：http://hz.quarkkingdee.top/gtjixpasyf.html

Go:   if s == "" {}
来源：http://hz.smart0.xyz/gtsnfmnmgs.html

Ruby: if s.empty?
来源：http://hz.daxiang520.top/gtyisdqafz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jqgufenzy.top/gtgmqtbipq.html

[E21] 超长截断加省略号
来源：http://hz.cqqwz.cn/gtkgrwwjgm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zhijiandao.cn/gtpslaywfc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.kuanghao11.cn/gtfeccbzac.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.dashuyun.cn/gtqawdfbxk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.nanxuanxn.top/gtdhzdtnvg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ydjk.org.cn/gtbyjtlzho.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.9152youxi.cn/gteuqitxpy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.shuidangran.top/gtjjngbavx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.gotoacloud.top/gtssihekkt.html

[E22] 字节长度与字符长度
来源：http://hz.zhijiandao.cn/gteslmqlsx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jinyuanbaomall.cn/gtahlhibvo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jinqigfzy.top/gtmsxctrfi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.quarkkingdee.top/gtifwqekhy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinghuilouyu.cn/gtcygitlie.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zdqjudy.top/gthlttcbmi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.chenzaomai.com/gttrkxksal.html

Ruby: s.bytesize;  s.length
来源：http://hz.andypj.xyz/gtjzdtucsp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.wangshuangyany.cn/gtlzdyoboa.html

================================================================================
来源：http://hz.hywenlv.cn/gtvfpztjrt.html

F. 文件与目录
来源：http://hz.nanxinkj.top/gtgfspikec.html

================================================================================
来源：http://hz.zdqjudy.top/gtkhetqcmi.html

[F01] 读取整个文件
来源：http://hz.yj20258888.top/gtzgstwkuj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hysaishi.cn/gtdzyjytxt.html

PHP:  file_get_contents("a.txt");
来源：http://hz.vqdsnc.cn/gtwwrmlrrj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.birdmap.top/gthnzizlmf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.andypj.xyz/gtchqjjqxu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jyoumei.cn/gthhmhrxyn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhoulong.xyz/gtmtsjgoui.html

Ruby: File.read("a.txt")
来源：http://hz.wangshuangyany.cn/gtuihvvoxn.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.gogol.net.cn/gtnocpgkcq.html

[F02] 逐行读取文件
来源：http://hz.yueranfly.top/gttivbycwd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.cdnleiting.top/gtorqcplbv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ppjwa.cn/gtrpacebzh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ywan-chungtsiang.top/gtadgmtzhc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yj202588.top/gtbycoasmd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.xuanzx.com/gtegaqfjzc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.snrcjt.cn/gtmifqxevz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.cucudq.cn/gtbvlqclex.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.ydjk.org.cn/gtoptgfypi.html

[F03] 写入文件（覆盖）
来源：http://hz.vqdsnc.cn/gtygrzsraq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.gzhubu.top/gtgipbrvrg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.gotoacloud.top/gtiokiqrva.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.guowangkeji.top/gtoxkajdhw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shanyushiyangtech.top/gtexvhmcpf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.iojbl.cn/gtspbtbanr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.gaohongyu789.top/gtdzimbkxi.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yonumen.top/gtgphetlcl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.shanyushiyangtech.top/gtnkcwsbta.html

[F04] 追加写入文件
来源：http://hz.hfpthk.cn/gtwatvipii.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hysaishi.cn/gtygtpqjxh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.vqdsnc.cn/gtdkwzogpm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.guowangkeji.top/gtnigjwdde.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.pengpengdd.cyou/gtzhermqnw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.bjfxy.top/gtqverfcys.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.shanyushiyangkeji.top/gtapxcuipi.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ehwqpu.com/gtjdpnzjdy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.tianlin.xyz/gtpmhiodtv.html

[F05] 判断文件或目录是否存在
来源：http://hz.pengpengdd.cyou/gtxaevvbxs.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.xuanzx.com/gtmcwyqybr.html

PHP:  file_exists("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtnzgcunhs.html

JS:   fs.existsSync("a.txt")
来源：http://hz.dashuyun.cn/gtcoetantl.html

TS:   fs.existsSync("a.txt")
来源：http://hz.feifeiyinyue.top/gtopheyobt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.chenlongwang.top/gtqadlonwv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.gotoacloud.top/gtpiabumyi.html

Ruby: File.exist?("a.txt")
来源：http://hz.xylfe.cn/gtjlpgfxho.html

C#:   File.Exists("a.txt")
来源：http://hz.shzxlz.cn/gthtntymcl.html

[F06] 删除文件
来源：http://hz.yueranfly.top/gtvtsduhef.html

Py:   os.remove("a.txt")
来源：http://hz.fzhhl.top/gtxtuseted.html

PHP:  unlink("a.txt");
来源：http://hz.jinqigufen.top/gtdqearxhv.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.daria6918.cn/gtnbqeoaht.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.daria6918.cn/gtkkgxwdvl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.aizwys.cn/gtlrrttcqv.html

Go:   os.Remove("a.txt")
来源：http://hz.shuidangran.top/gtfvitgqeg.html

Ruby: File.delete("a.txt")
来源：http://hz.yongpay.top/gtjgodfbtd.html

C#:   File.Delete("a.txt");
来源：http://hz.hfpthk.cn/gtlkiternr.html

[F07] 创建目录（含多级）
来源：http://hz.zycfv.cn/gtqfollagu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.guannengcc.top/gtpgyupgcg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhiwuduotai.top/gtlqagnxyj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shanyushiyangtech.top/gtpbayjisy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.guowangkeji.top/gtbrbfvrwb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jqgufenzy.top/gtfzptxzhl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yj20258888.top/gtlwskdjbn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jqgfzy.top/gtyhrwrvwl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yj20258888.top/gttqcdnufd.html

[F08] 遍历目录
来源：http://hz.aibaodan.cn/gtolsiawpp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.havefunace.top/gtattiiary.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.vqdsnc.cn/gtjtdpbtuk.html

JS:   fs.readdirSync("dir")
来源：http://hz.hnqzz.top/gtpqgynslw.html

TS:   fs.readdirSync("dir")
来源：http://hz.hfpthk.cn/gtlksjtuft.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zhongyouzk.top/gtpmvwhtme.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.pengpengdd.cyou/gtymdrrndc.html

Ruby: Dir.children("dir")
来源：http://hz.jinghuilouyu.cn/gtbrocvpfm.html

C#:   Directory.GetFiles("dir")
来源：http://hz.0kj1m.cn/gtedtwijsc.html

[F09] 获取文件大小
来源：http://hz.gotoacloud.top/gtatzanteq.html

Py:   os.path.getsize("a.txt")
来源：http://hz.havefunace.top/gtrzrfiacv.html

PHP:  filesize("a.txt");
来源：http://hz.sweek.top/gtogretcgl.html

JS:   fs.statSync("a.txt").size
来源：http://hz.wangdashe.top/gthpfgpnrm.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yongpay.top/gtkipmgvai.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.daxiang520.top/gtsofnocbq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yj202588.top/gtiejggpkg.html

Ruby: File.size("a.txt")
来源：http://hz.dashuyun.cn/gtcrpwwgvc.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.shzxlz.cn/gtgjatorbt.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.c1oappe.top/gtkriwohvr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.aizwys.cn/gtkgqbuciz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jlsjyb.cn/gtpxhapabw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.birdmap.top/gtxsakwpej.html

TS:   path.extname("a.txt")
来源：http://hz.snrcjt.cn/gtwfbipaeh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.vqdsnc.cn/gtkahcwqpw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jinyuanbaomall.cn/gtwynblqzb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ybcxt.top/gtyqvsrpef.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jianghu66.top/gtlmysmaum.html

[F11] 复制与移动文件
来源：http://hz.c1oappe.top/gtulwajnsb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.xziqi.cn/gtlejguuke.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.ydzc1.top/gtmfqzwfvx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.vqdsnc.cn/gtutkfqrbn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.guannengcc.top/gtggtkxqjw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.sysykeji.top/gtohaulibl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yongpay.top/gtyivblgve.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.0kj1m.cn/gtegvkwkcr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.xziqi.cn/gtfmkkkbqi.html

[F12] CSV 读写
来源：http://hz.zhongyouzk.top/gtgadryqmi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xuetiantiany.cn/gtfvbmsfuy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.daxiang520.top/gtkwafgwwv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.guannengcc.top/gtbmfixias.html

TS:   // 同上
来源：http://hz.nwbrower.top/gtzqgkihru.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zdqjudy.top/gtptalrais.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ydzc1.top/gtdmjfllsn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.c1oappe.top/gtclnkpbdn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.snrcjt.cn/gtxpgdebrw.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtrrlqyffo.html

G. 面向对象
来源：http://hz.c1oappe.top/gtfpuyvori.html

================================================================================
来源：http://hz.yanxiufei.cn/gtvolnazcu.html

[G01] 定义类
来源：http://hz.chenzaomai.com/gtlubzmoix.html

Py:   class User: pass
来源：http://hz.jqgfzy.top/gtlasvgzcp.html

PHP:  class User {}
来源：http://hz.ydjk.org.cn/gtzdxuieoh.html

JS:   class User {}
来源：http://hz.vqdsnc.cn/gtqcawgxwy.html

TS:   class User { name: string = ""; }
来源：http://hz.hnqzz.top/gtbmjlteai.html

Java: class User {}
来源：http://hz.yanxiufei.cn/gtivifvrmo.html

Go:   type User struct { Name string }
来源：http://hz.zhijiandao.cn/gtdmpnuejc.html

Ruby: class User; end
来源：http://hz.dashuyun.cn/gtmkgtghnj.html

C#:   class User {}
来源：http://hz.gaohongyu789.top/gtimychjdm.html

[G02] 构造函数
来源：http://hz.yvedp.cn/gthoyiuful.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.guowangkeji.top/gtlohhpxub.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.daxiang520.top/gtrhsdhhco.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.iojbl.cn/gtojggedgm.html

TS:   constructor(public name: string) {}
来源：http://hz.pengpengdd.cyou/gtqjhgikbh.html

Java: User(String name) { this.name = name; }
来源：http://hz.jiagoushi.top/gtavpobasz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jqgfzy.top/gtdzubreif.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.aizwys.cn/gtkyfrwvey.html

C#:   public User(string name) { Name = name; }
来源：http://hz.9152youxi.cn/gtskrgjrrb.html

[G03] 实例属性
来源：http://hz.zhongyouzk.top/gtficjueai.html

Py:   self.name = "x"
来源：http://hz.hnqzz.top/gtxkepqhbf.html

PHP:  public string $name = "x";
来源：http://hz.shuidangran.top/gtjtrldpfn.html

JS:   this.name = "x";
来源：http://hz.feifeiyinyue.top/gthqpmhzms.html

TS:   name: string = "x";
来源：http://hz.jinghuilouyu.cn/gtubtrkehp.html

Java: private String name;
来源：http://hz.zhoulong.xyz/gtealtzhye.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yuanzhike.top/gtqstelxkt.html

Ruby: @name = "x"
来源：http://hz.xingfuxueyuan.xyz/gtxglwksiz.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.gotoacloud.top/gtreomzrpe.html

[G04] 定义方法
来源：http://hz.kuanghao11.cn/gtyuejxwnw.html

Py:   def greet(self): return self.name
来源：http://hz.vqdsnc.cn/gtwanlvinp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.tianlin.xyz/gtavvqnxee.html

JS:   greet() { return this.name; }
来源：http://hz.shanyushiyangkeji.top/gtggecnhlm.html

TS:   greet(): string { return this.name; }
来源：http://hz.yueranfly.top/gtyuprhxgq.html

Java: String greet() { return name; }
来源：http://hz.zhaomingkeji.xyz/gtynftbxet.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.mhx1999.top/gtrlthvvnz.html

Ruby: def greet; @name; end
来源：http://hz.svipenyu.cn/gtxknxbafn.html

C#:   public string Greet() => Name;
来源：http://hz.ydjk.org.cn/gtzafptpkq.html

[G05] 继承
来源：http://hz.gaohongyu789.top/gtsmwiafnc.html

Py:   class Admin(User): pass
来源：http://hz.shzxlz.cn/gtypnrnnnj.html

PHP:  class Admin extends User {}
来源：http://hz.jinghuilouyu.cn/gtofmcfvxq.html

JS:   class Admin extends User {}
来源：http://hz.ybcxt.top/gtikohxqlc.html

TS:   class Admin extends User {}
来源：http://hz.birdmap.top/gtlysboert.html

Java: class Admin extends User {}
来源：http://hz.ehwqpu.com/gtvfgqiond.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yj202588.top/gtxknoksbi.html

Ruby: class Admin < User; end
来源：http://hz.daria6918.cn/gttjnmzfoj.html

C#:   class Admin : User {}
来源：http://hz.gogol.net.cn/gtbtcgdqpy.html

[G06] 重写方法
来源：http://hz.nwbrower.top/gtsscfvauj.html

Py:   def greet(self): return "admin"
来源：http://hz.gzhubu.top/gtanhlwbqd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.tanke756.top/gtrxmbmcdx.html

JS:   greet() { return "admin"; }
来源：http://hz.guowangkeji.top/gthdpbygzl.html

TS:   greet(): string { return "admin"; }
来源：http://hz.9152youxi.cn/gtybmymgeb.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.nanxinkj.top/gtvxsqilwy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jinqigufen.top/gtopatziib.html

Ruby: def greet; "admin"; end
来源：http://hz.yongpay.top/gtgnvintel.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhaomingkeji.xyz/gteihccthd.html

[G07] 调用父类方法
来源：http://hz.jqgfzy.top/gtxqeumzqf.html

Py:   super().greet()
来源：http://hz.bjfxy.top/gtzgozygir.html

PHP:  parent::greet();
来源：http://hz.pycfn.com/gtkjlwnbwp.html

JS:   super.greet();
来源：http://hz.xziqi.cn/gtphwgovgt.html

TS:   super.greet();
来源：http://hz.nanxinkj.top/gtxseomyev.html

Java: super.greet();
来源：http://hz.fengsongda.top/gtixaxnonn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.xingfuxueyuan.xyz/gtawlsppsk.html

Ruby: super
来源：http://hz.yueranfly.top/gtqnriarzy.html

C#:   base.Greet();
来源：http://hz.zycfv.cn/gtkznqokfm.html

[G08] 静态方法与属性
来源：http://hz.ppjwa.cn/gtrgavwnfo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.gzhubu.top/gtyujkqblu.html

PHP:  public static function f() {}
来源：http://hz.ydjk.org.cn/gtslhvunvb.html

JS:   static f() {}
来源：http://hz.ywan-chungtsiang.top/gtkqjspshy.html

TS:   static f(): void {}
来源：http://hz.daxiang520.top/gtdhbroter.html

Java: static void f() {}
来源：http://hz.wangdashe.top/gtmwgjomic.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hnxiangtu.top/gteixtxwlo.html

Ruby: def self.f; end
来源：http://hz.aizwys.cn/gttsbufkhx.html

C#:   public static void F() {}
来源：http://hz.nanxinkj.top/gtouxfneln.html

[G09] 接口 / 抽象类
来源：http://hz.gaohongyu789.top/gtmseiecjl.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jinqigfzy.top/gtvmelphwt.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.0kj1m.cn/gtagiywkoi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zhaomingkeji.xyz/gtnbuvphdb.html

TS:   interface Shape { area(): number; }
来源：http://hz.gaohongyu789.top/gtmfxkftsu.html

Java: interface Shape { double area(); }
来源：http://hz.wangshuangyany.cn/gtzxsigddp.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.pycfn.com/gttbesefpo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.fzhhl.top/gtpdmasrij.html

C#:   interface IShape { double Area(); }
来源：http://hz.yongpay.top/gthurmfoyc.html

[G10] 访问控制
来源：http://hz.gotoacloud.top/gtdwjdxvsw.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.shangyingyoupin.top/gtwkkiqpvz.html

PHP:  public / protected / private
来源：http://hz.yangfankeji.com/gteqxyhmrq.html

JS:   #private 字段；其余公开
来源：http://hz.cashguo.top/gtevcrkrau.html

TS:   public / protected / private
来源：http://hz.shangyingyoupin.top/gtrnptlaag.html

Java: public / protected / private / 默认包级
来源：http://hz.jianghu66.top/gtysidovdv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.quarkkingdee.top/gtirqkmglf.html

Ruby: public / protected / private
来源：http://hz.yj20258888.top/gtytayumnx.html

C#:   public / protected / private / internal
来源：http://hz.zhixingplan.top/gtxmleimri.html

[G11] getter / setter
来源：http://hz.jqgfzy.top/gtbcmevram.html

Py:   @property 与 @x.setter
来源：http://hz.cqqwz.cn/gtpikvnxju.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.pengpengdd.cyou/gtoqophqbb.html


<!-- 参考信息 -->