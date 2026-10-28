代发 wailian999

[E14] URL 编码与 Base64
来源：http://hz.316326.xyz/gtyhjnnvij.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.sxryk.cn/gtqqpxiyrt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yonumen.top/gtyvyeqaax.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.guowangkeji.top/gtpqnrjgtt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jqgfzy.top/gtuysykaaj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.sysykeji.top/gtdzyalwxo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jiagoushi.top/gtotzbssiq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yj20258888.top/gtxocinhrv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.tian-w.cn/gtmfbzhhbq.html

[E15] HTML 转义 / 反转义
来源：http://hz.nanxuanxn.top/gttigrqfww.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.nwbrower.top/gtnyopxoyo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zhongyouzk.top/gtcmjkquzw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.guannengcc.top/gtncczptvl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.haohaochexian.top/gtculjtrbk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zhaomingkeji.xyz/gtugbjmzqr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hywenlv.cn/gtseytjqrp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.cashguo.top/gtqhqjusto.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yonumen.top/gthyvvuanz.html

[E16] 数字千分位
来源：http://hz.nanxuanxn.top/gteozpmqbc.html

Py:   f"{1234567:,}"
来源：http://hz.9152youxi.cn/gtwoxnrajl.html

PHP:  number_format(1234567);
来源：http://hz.xuanzx.com/gtjevuxqpv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.snrcjt.cn/gtrwqdqgtl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.snrcjt.cn/gtfuzicuip.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.quarkkingdee.top/gtjnuzvcre.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.xingfuxueyuan.xyz/gtikpyndxb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zycfv.cn/gtjjiepfim.html

C#:   1234567.ToString("N0")
来源：http://hz.jqgufenzy.top/gtiuvneidb.html

[E17] 首字母大写
来源：http://hz.gotoacloud.top/gtclmmjptu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.tianlin.xyz/gtlalpycsy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.tianlin.xyz/gtavgzyvzi.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yj20258.top/gtwckcyluq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jiagoushi.top/gtnwvbulnr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jqgfzy.top/gtradfluhd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yuanzhike.top/gtjmqimjsd.html

Ruby: s.capitalize
来源：http://hz.jiagoushi.top/gtfbbadnfq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.xinyue.icu/gtrpvucgzu.html

[E18] 模板占位符替换
来源：http://hz.yj202588.top/gtsrdksssg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jqgufenzy.top/gtplwdibkd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.wangdashe.top/gtpyladoqs.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hnqzz.top/gtfuwudhih.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.ivvv.top/gtbcrukqyo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jiagoushi.top/gtbpnxtxvd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zdqjudy.top/gtixvduzoe.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yuanzhike.top/gtqxseqdgm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.xinyue.icu/gtcxjahvro.html

[E19] 多行文本按行拆分
来源：http://hz.zhengqikj.top/gtlkjltilt.html

Py:   s.splitlines()
来源：http://hz.shanyushiyangkeji.top/gtfbsdsnjf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zhiwuduotai.top/gtzkjkgtol.html

JS:   s.split(/\r?\n/)
来源：http://hz.bjfxy.top/gtjuybepau.html

TS:   s.split(/\r?\n/)
来源：http://hz.havefunace.top/gtdxukborj.html

Java: s.lines().toList()
来源：http://hz.gzhubu.top/gtuqrrwnip.html

Go:   strings.Split(s, "\n")
来源：http://hz.cdnleiting.top/gtvrbudnkp.html

Ruby: s.lines
来源：http://hz.dashuyun.cn/gtzldikhsu.html

C#:   s.Split('\n')
来源：http://hz.ydjk.org.cn/gtpsgndzoj.html

[E20] 判断字符串是否为空
来源：http://hz.shangyingyoupin.top/gtzyothccw.html

Py:   if not s:
来源：http://hz.hysaishi.cn/gtjxagqrnd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.tian-w.cn/gtpqscjmtm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jinghuilouyu.cn/gtcgbthdpl.html

TS:   if (s === "") {}
来源：http://hz.yuxming.cn/gtqdzbytpj.html

Java: if (s.isEmpty()) {}
来源：http://hz.snrcjt.cn/gtojfadpla.html

Go:   if s == "" {}
来源：http://hz.aibaodan.cn/gtxaihlsil.html

Ruby: if s.empty?
来源：http://hz.nanxuanxn.top/gtlymcffwk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ydjk.org.cn/gthznfjaus.html

[E21] 超长截断加省略号
来源：http://hz.shanyushiyangtech.top/gtnitljxzq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jiagoushi.top/gtkxewwkqt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.daria6918.cn/gtdckepwml.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jiagoushi.top/gthkjuqddq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yonumen.top/gtlohqwiao.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zhongyouzk.top/gtbehpicdm.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.shuidangran.top/gtoxvzzxkj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.pengpengdd.cyou/gtjytlnpbn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ppjwa.cn/gtvkpkthxu.html

[E22] 字节长度与字符长度
来源：http://hz.9152youxi.cn/gtyaabjvaa.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ybcxt.top/gtuveirvkq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.bjfxy.top/gtpgivmyak.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yangfankeji.com/gtilejcdlp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.snrcjt.cn/gtanhxxlnh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.gogol.net.cn/gtkmckeeke.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.nanxinkj.top/gtxficxvzm.html

Ruby: s.bytesize;  s.length
来源：http://hz.dashuyun.cn/gtkwcabtsu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.chenzaomai.com/gtgopgwcll.html

================================================================================
来源：http://hz.ybcxt.top/gtpanhizhf.html

F. 文件与目录
来源：http://hz.kuanghao11.cn/gteogibtbn.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtjiutltyv.html

[F01] 读取整个文件
来源：http://hz.jqgufenzy.top/gtcpugqqsn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zhijiandao.cn/gtitmdsydy.html

PHP:  file_get_contents("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtlmiufvsu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.shzxlz.cn/gtfbvpsrpj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.shzxlz.cn/gtsfofutzf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhijiandao.cn/gtjrgbozov.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.pycfn.com/gtrhprniuo.html

Ruby: File.read("a.txt")
来源：http://hz.daria6918.cn/gtqrzhqbxr.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.birdmap.top/gtyaufbaos.html

[F02] 逐行读取文件
来源：http://hz.shzxlz.cn/gtqtatthvc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jlsjyb.cn/gtthqzohym.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.fzhhl.top/gtnfaqpuhu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhongyouzk.top/gtlyyovsqp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xuetiantiany.cn/gthnqmtqdn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yonumen.top/gtgunqoiap.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhengqikj.top/gtbgonhboq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.9152youxi.cn/gtjeteddvp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yongpay.top/gtbkwebhli.html

[F03] 写入文件（覆盖）
来源：http://hz.meibo888.top/gtgpxeygta.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.xylfe.cn/gtwljqpawl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.nwbrower.top/gtyrqecnhx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.redwolf501.top/gtifagvznu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xuetiantiany.cn/gtqjkqplyi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.meibo888.top/gtxjcwscmx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.vqdsnc.cn/gtsglisjdu.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jqgufenzy.top/gtoxjhftnp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.wangshuangyany.cn/gtwklitmmh.html

[F04] 追加写入文件
来源：http://hz.redwolf501.top/gtxmysnnul.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.wangshuangyany.cn/gtcgtshfzq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.iojbl.cn/gtgsudnzmv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.wangshuangyany.cn/gtoitwuumu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xinyue.icu/gtltbtlnxo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.cheryme.top/gtvpafgtad.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yj20258888.top/gtcrthzovs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jqgfzy.top/gtjpaicrmh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.shangyingyoupin.top/gtkgamlxxb.html

[F05] 判断文件或目录是否存在
来源：http://hz.guowangkeji.top/gtrpgzeoan.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zhongyouzk.top/gtfzlqfrcm.html

PHP:  file_exists("a.txt");
来源：http://hz.tian-w.cn/gtbzlhbbvi.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hnqzz.top/gtauykgakb.html

TS:   fs.existsSync("a.txt")
来源：http://hz.aibaodan.cn/gtbcpplpbp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.chenjidiqi.icu/gtqcdpnshd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.shanyushiyangtech.top/gtavmcgnjy.html

Ruby: File.exist?("a.txt")
来源：http://hz.hammf.cn/gtqtpgklxf.html

C#:   File.Exists("a.txt")
来源：http://hz.yonumen.top/gtteyzlgxp.html

[F06] 删除文件
来源：http://hz.daxiang520.top/gtjhcfuvhk.html

Py:   os.remove("a.txt")
来源：http://hz.tanke756.top/gtgfcfnwri.html

PHP:  unlink("a.txt");
来源：http://hz.shzxlz.cn/gtrbknxonu.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ppjwa.cn/gtdrowsshd.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hongshengwenyu.top/gtycobivgr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xuetiantiany.cn/gtkaupvqsv.html

Go:   os.Remove("a.txt")
来源：http://hz.yuxming.cn/gtrzqjurjf.html

Ruby: File.delete("a.txt")
来源：http://hz.andypj.xyz/gtfewbecjt.html

C#:   File.Delete("a.txt");
来源：http://hz.sysykeji.top/gtodzmyczh.html

[F07] 创建目录（含多级）
来源：http://hz.hysaishi.cn/gtdvopmdow.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.cashguo.top/gtbvfqnnxi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.gotoacloud.top/gtskgtpmto.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.kuanghao11.cn/gtqqqzmksp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.tianlin.xyz/gtagzbeyoq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jinghuilouyu.cn/gtqhbihtwc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yvedp.cn/gtgemahier.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.haohaochexian.top/gthsduqkdz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jqgufenzy.top/gtjddxxtxy.html

[F08] 遍历目录
来源：http://hz.cdnleiting.top/gtmgcottkn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.snrcjt.cn/gtvlxmebps.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.sweek.top/gtnrftjqdk.html

JS:   fs.readdirSync("dir")
来源：http://hz.ywan-chungtsiang.top/gtcdphwfws.html

TS:   fs.readdirSync("dir")
来源：http://hz.gzhubu.top/gtjllypnby.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.smart0.xyz/gtkdrhnvif.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.shangyingyoupin.top/gtqaunconx.html

Ruby: Dir.children("dir")
来源：http://hz.feifeiyinyue.top/gtqadirryq.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yangfankeji.com/gtwarykhpq.html

[F09] 获取文件大小
来源：http://hz.yongpay.top/gtmdfbtgec.html

Py:   os.path.getsize("a.txt")
来源：http://hz.nwbrower.top/gtgthotbsa.html

PHP:  filesize("a.txt");
来源：http://hz.0kj1m.cn/gtghgivmph.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xylfe.cn/gthvftbddt.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xylfe.cn/gthznsygqs.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.sufxvd.cn/gtyqoqsuiv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ydzc1.top/gtoayicyfi.html

Ruby: File.size("a.txt")
来源：http://hz.nwbrower.top/gtsqpuesbw.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.316326.xyz/gtbjlnaurs.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.chenzaomai.com/gtqlcqyujt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jyoumei.cn/gticltfiyx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.hammf.cn/gtmwxonqqd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.quarkkingdee.top/gttpgomujp.html

TS:   path.extname("a.txt")
来源：http://hz.shzxlz.cn/gtphqztflx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yj20258888.top/gtpqfpxoru.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.bjfxy.top/gtemwlidez.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.xylfe.cn/gtwgfabvby.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yanxiufei.cn/gtquhtvjog.html

[F11] 复制与移动文件
来源：http://hz.yvedp.cn/gtpnuagank.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.svipenyu.cn/gtoutwodyz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.nanxuanxn.top/gtmrkfsvii.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yj202588.top/gtgvasviio.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sweek.top/gtbnihhshw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ydzc1.top/gthzinunvp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xziqi.cn/gtafsremrq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ivvv.top/gtxapqvtxd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.chenzaomai.com/gtjnluskxu.html

[F12] CSV 读写
来源：http://hz.vqdsnc.cn/gtnefuiynu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hongshengwenyu.top/gtkwbvbnzi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.shanyushiyangkeji.top/gtdhkvblup.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.tanke756.top/gtepznfvhk.html

TS:   // 同上
来源：http://hz.jyoumei.cn/gtqlmlmjli.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.cdnleiting.top/gtebpovddu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.xinyue.icu/gtuhydyykd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yj20258.top/gthvwicret.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yonumen.top/gtqpykkdby.html

================================================================================
来源：http://hz.mhx1999.top/gtfiiooyde.html

G. 面向对象
来源：http://hz.kuanghao11.cn/gtbxkwjiee.html

================================================================================
来源：http://hz.ivvv.top/gtnlsvngol.html

[G01] 定义类
来源：http://hz.gzhubu.top/gtssfslgje.html

Py:   class User: pass
来源：http://hz.svipenyu.cn/gtucmxxpjt.html

PHP:  class User {}
来源：http://hz.cqqwz.cn/gtoncbmfqm.html

JS:   class User {}
来源：http://hz.daxiang520.top/gtgypbtxtl.html

TS:   class User { name: string = ""; }
来源：http://hz.hammf.cn/gtygjzadvs.html

Java: class User {}
来源：http://hz.hongshengwenyu.top/gtzfhgudaa.html

Go:   type User struct { Name string }
来源：http://hz.hnqzz.top/gtkzrccqed.html

Ruby: class User; end
来源：http://hz.jiagoushi.top/gthlzvouhp.html

C#:   class User {}
来源：http://hz.shzxlz.cn/gtxrteqpph.html

[G02] 构造函数
来源：http://hz.dashuyun.cn/gtljtcbuaq.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhaomingkeji.xyz/gtiyhvmqsb.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.wangshuangyany.cn/gtsedznpxt.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.nanxuanxn.top/gtrkdelsyq.html

TS:   constructor(public name: string) {}
来源：http://hz.ehwqpu.com/gtuszbpmyn.html

Java: User(String name) { this.name = name; }
来源：http://hz.daria6918.cn/gtpfizpnvo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.snrcjt.cn/gtvrnbktdl.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.svipenyu.cn/gtuyigsayw.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hongshengwenyu.top/gtusllhyrh.html

[G03] 实例属性
来源：http://hz.xylfe.cn/gtqvlxeumr.html

Py:   self.name = "x"
来源：http://hz.zhiwuduotai.top/gtommoztpp.html

PHP:  public string $name = "x";
来源：http://hz.ivvv.top/gtikrkkjvb.html

JS:   this.name = "x";
来源：http://hz.meibo888.top/gtavyalflf.html

TS:   name: string = "x";
来源：http://hz.jinyuanbaomall.cn/gtatrmrbje.html

Java: private String name;
来源：http://hz.bjfxy.top/gtwgfoixhb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.svipenyu.cn/gtnuechepa.html

Ruby: @name = "x"
来源：http://hz.yueranfly.top/gtyssrmdcm.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jinyuanbaomall.cn/gtlkzavnuf.html

[G04] 定义方法
来源：http://hz.dashuyun.cn/gtsspcgfzj.html

Py:   def greet(self): return self.name
来源：http://hz.hongshengwenyu.top/gtosgbieuz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jinqigfzy.top/gtgzdpfuds.html

JS:   greet() { return this.name; }
来源：http://hz.quarkkingdee.top/gteotpfdqg.html

TS:   greet(): string { return this.name; }
来源：http://hz.ybcxt.top/gtnchxzxda.html

Java: String greet() { return name; }
来源：http://hz.yonumen.top/gtsqtnlppq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ppjwa.cn/gtuiveoqyz.html

Ruby: def greet; @name; end
来源：http://hz.zhengqikj.top/gtlgwssvei.html

C#:   public string Greet() => Name;
来源：http://hz.wangshuangyany.cn/gtmmgssfeu.html

[G05] 继承
来源：http://hz.hnqzz.top/gtiqumpohu.html

Py:   class Admin(User): pass
来源：http://hz.chenjidiqi.icu/gtlxyloqmd.html

PHP:  class Admin extends User {}
来源：http://hz.xziqi.cn/gtvjctmxft.html

JS:   class Admin extends User {}
来源：http://hz.yongpay.top/gtfjjvrtcm.html

TS:   class Admin extends User {}
来源：http://hz.yj20258888.top/gthwrrycgu.html

Java: class Admin extends User {}
来源：http://hz.pycfn.com/gtzxqjkawz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.xylfe.cn/gtmotologw.html

Ruby: class Admin < User; end
来源：http://hz.shzxlz.cn/gtfnhwtbzg.html

C#:   class Admin : User {}
来源：http://hz.nanxuanxn.top/gtvggyyrcp.html

[G06] 重写方法
来源：http://hz.quarkkingdee.top/gtdlfltdrp.html

Py:   def greet(self): return "admin"
来源：http://hz.daria6918.cn/gtixpdbdxy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.shanyushiyangtech.top/gtsyqftggp.html

JS:   greet() { return "admin"; }
来源：http://hz.ybcxt.top/gtvbcrynux.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhaomingkeji.xyz/gtzrmgxdtk.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.vqdsnc.cn/gtpwvrxcnl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.hammf.cn/gtkwlmejyw.html

Ruby: def greet; "admin"; end
来源：http://hz.ydzc1.top/gtjyfmwsxd.html

C#:   public override string Greet() => "admin";
来源：http://hz.xingfuxueyuan.xyz/gtanznwwtz.html

[G07] 调用父类方法
来源：http://hz.guannengcc.top/gtwqsomgxe.html

Py:   super().greet()
来源：http://hz.hfpthk.cn/gtoqmrzgdq.html

PHP:  parent::greet();
来源：http://hz.chenlongwang.top/gtupleopsv.html

JS:   super.greet();
来源：http://hz.andypj.xyz/gtftewjpsq.html

TS:   super.greet();
来源：http://hz.mhx1999.top/gtrsjswjla.html

Java: super.greet();
来源：http://hz.yuxming.cn/gtmsygvzuz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.gotoacloud.top/gtjplpkjju.html

Ruby: super
来源：http://hz.hywenlv.cn/gtlhznocfc.html

C#:   base.Greet();
来源：http://hz.ybcxt.top/gtfnwzckjt.html

[G08] 静态方法与属性
来源：http://hz.snrcjt.cn/gtollorxeb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.shuidangran.top/gtevhtphpk.html

PHP:  public static function f() {}
来源：http://hz.cqqwz.cn/gtwvkylbvs.html

JS:   static f() {}
来源：http://hz.meibo888.top/gtqhhwwruv.html

TS:   static f(): void {}
来源：http://hz.chenlongwang.top/gthuhbrhqj.html

Java: static void f() {}
来源：http://hz.jiagoushi.top/gtzshvhrro.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yueranfly.top/gtnwupbvhw.html

Ruby: def self.f; end
来源：http://hz.zdqjudy.top/gtmhvidspj.html

C#:   public static void F() {}
来源：http://hz.tanke756.top/gttgmvjiql.html

[G09] 接口 / 抽象类
来源：http://hz.yvedp.cn/gtmeggutiw.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.meibo888.top/gtzqkulmgu.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.pycfn.com/gtiloxbfwp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.sufxvd.cn/gtvyrsgcwe.html

TS:   interface Shape { area(): number; }
来源：http://hz.jinghuilouyu.cn/gtivgibjjm.html

Java: interface Shape { double area(); }
来源：http://hz.snrcjt.cn/gtzqvzyiwm.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.cucudq.cn/gttcbvamtt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zdqjudy.top/gttgwdeuzq.html

C#:   interface IShape { double Area(); }
来源：http://hz.mhx1999.top/gtnuwgziaj.html

[G10] 访问控制
来源：http://hz.shanyushiyangkeji.top/gtjefcitbw.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hnqzz.top/gttwdroizz.html

PHP:  public / protected / private
来源：http://hz.cqqwz.cn/gtlzitmqmo.html

JS:   #private 字段；其余公开
来源：http://hz.hammf.cn/gtjrzbugez.html

TS:   public / protected / private
来源：http://hz.0kj1m.cn/gtfzppcgtb.html

Java: public / protected / private / 默认包级
来源：http://hz.jqgufenzy.top/gtngiforrt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.hongshengwenyu.top/gtcumhhkmu.html

Ruby: public / protected / private
来源：http://hz.hfpthk.cn/gtafwbsgho.html

C#:   public / protected / private / internal
来源：http://hz.guowangkeji.top/gtrrlqzxen.html

[G11] getter / setter
来源：http://hz.yuxming.cn/gteytyilmj.html

Py:   @property 与 @x.setter
来源：http://hz.sxryk.cn/gtvnzbayaq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hysaishi.cn/gtvddeotto.html

JS:   get name() { return this._name; }
来源：http://hz.52xcode.cn/gtsxngfzbu.html

TS:   get name(): string { return this._name; }
来源：http://hz.yongpay.top/gttylbjetn.html

Java: public String getName() { return name; }
来源：http://hz.cqqwz.cn/gtfxwzwyij.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.sweek.top/gtensgbwya.html

Ruby: attr_accessor :name
来源：http://hz.zdqjudy.top/gtjdhvdddc.html

C#:   public string Name { get; set; }
来源：http://hz.ywan-chungtsiang.top/gtuiklpxfd.html

[G12] 对象转字符串
来源：http://hz.yj202588.top/gtiwyubnml.html

Py:   def __str__(self): return self.name
来源：http://hz.shzxlz.cn/gtfjuqlqux.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yvedp.cn/gtwjvaokqg.html

JS:   toString() { return this.name; }
来源：http://hz.sysykeji.top/gtsczszdpv.html

TS:   toString(): string { return this.name; }
来源：http://hz.cheryme.top/gtyeacmmin.html

Java: @Override public String toString() { return name; }
来源：http://hz.shzxlz.cn/gtyelxizhh.html


<!-- 参考信息 -->