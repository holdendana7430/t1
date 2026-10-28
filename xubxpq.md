代发 wailian999

Go:   strings.Count(s, "a")
来源：http://hz.zhiwuduotai.top/gtbwtyxizp.html

Ruby: s.count("a")
来源：http://hz.yj202588.top/gtpqfouxka.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ivvv.top/gtovyrzgtn.html

[E13] 逐字符遍历
来源：http://hz.chenzaomai.com/gtenwaxodt.html

Py:   for ch in s: print(ch)
来源：http://hz.wangshuangyany.cn/gtcfvzxghn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.quarkkingdee.top/gtevnphzzo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.nanxuanxn.top/gtxbtgaqgp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shanyushiyangtech.top/gtpdlfveiy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.guannengcc.top/gtcplmatjg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.aizwys.cn/gtywvlmhse.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yuxming.cn/gtbvilouoc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.ppjwa.cn/gtiabyejuq.html

[E14] URL 编码与 Base64
来源：http://hz.jinqigfzy.top/gtgvmxkrdv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yuanzhike.top/gtdhwinqkt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.xuetiantiany.cn/gtzqssvmqf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yuanzhike.top/gtoifaswiz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.cdnleiting.top/gttcjppwfk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jqgufenzy.top/gtrkibvtsa.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.aizwys.cn/gtgnmdwjbn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.cheryme.top/gtlzroigst.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.daria6918.cn/gtjwmwwgnd.html

[E15] HTML 转义 / 反转义
来源：http://hz.chenlongwang.top/gtzpazsaxd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.vqdsnc.cn/gtifhvhjcj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.tian-w.cn/gtxsodlagg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yuxming.cn/gtzzuffiii.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.snrcjt.cn/gtfnkllaki.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hongshengwenyu.top/gtbmnpgjnk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hnxiangtu.top/gtwenffhlm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.sufxvd.cn/gtvkywbsvw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.ydjk.org.cn/gtoealnhwa.html

[E16] 数字千分位
来源：http://hz.sufxvd.cn/gtbbfuxjlw.html

Py:   f"{1234567:,}"
来源：http://hz.vqdsnc.cn/gtwoksoyii.html

PHP:  number_format(1234567);
来源：http://hz.yonumen.top/gtwvryzadg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.nanxuanxn.top/gtraxzccuy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hammf.cn/gtogespwbx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.shangyingyoupin.top/gtyhmlqwot.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.quarkkingdee.top/gtdpwearos.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.wangshuangyany.cn/gtgwbvcadq.html

C#:   1234567.ToString("N0")
来源：http://hz.sweek.top/gtliojkcuc.html

[E17] 首字母大写
来源：http://hz.yanxiufei.cn/gtdazryrzi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.sweek.top/gtcjvxswyu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.chenjidiqi.icu/gtttexbakz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cucudq.cn/gtsauejsmd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhijiandao.cn/gtumqsmwtg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ppjwa.cn/gtucusnccu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zdqjudy.top/gttgixdtgb.html

Ruby: s.capitalize
来源：http://hz.jyoumei.cn/gtrrgyiduu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.fengsongda.top/gtypcqqzke.html

[E18] 模板占位符替换
来源：http://hz.cucudq.cn/gtivrjqzlo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.vqdsnc.cn/gtosfhbgco.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.xziqi.cn/gtrrxfinzb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.gzhubu.top/gtmfaljakm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yueranfly.top/gtbkjqnpyu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yonumen.top/gtdpwllvcd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.xingfuxueyuan.xyz/gtbgcvuchb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.dashuyun.cn/gtloriswig.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.hongshengwenyu.top/gtcfnshete.html

[E19] 多行文本按行拆分
来源：http://hz.yangfankeji.com/gtvqyjnyaw.html

Py:   s.splitlines()
来源：http://hz.kuanghao11.cn/gtvrngrygn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jyoumei.cn/gtbpubousf.html

JS:   s.split(/\r?\n/)
来源：http://hz.hfpthk.cn/gtkwvmwdzr.html

TS:   s.split(/\r?\n/)
来源：http://hz.gotoacloud.top/gtbeqkfcyt.html

Java: s.lines().toList()
来源：http://hz.jqgfzy.top/gtbjlvtgnc.html

Go:   strings.Split(s, "\n")
来源：http://hz.cucudq.cn/gtarscgotw.html

Ruby: s.lines
来源：http://hz.jqgfzy.top/gtahdmrkju.html

C#:   s.Split('\n')
来源：http://hz.pengpengdd.cyou/gtkipsfqws.html

[E20] 判断字符串是否为空
来源：http://hz.xuanzx.com/gtxupsrtdz.html

Py:   if not s:
来源：http://hz.redwolf501.top/gtpiuodewc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.gaohongyu789.top/gtirebmhzq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.xingfuxueyuan.xyz/gttkgdgqtp.html

TS:   if (s === "") {}
来源：http://hz.jinghuilouyu.cn/gteuuqghbb.html

Java: if (s.isEmpty()) {}
来源：http://hz.nwbrower.top/gttotcvajh.html

Go:   if s == "" {}
来源：http://hz.cheryme.top/gtdmdcegbt.html

Ruby: if s.empty?
来源：http://hz.ehwqpu.com/gtdveycxjz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zycfv.cn/gtiuuypvfw.html

[E21] 超长截断加省略号
来源：http://hz.havefunace.top/gtahrkqvmq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yj20258.top/gtskiuyzym.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.gaohongyu789.top/gtncbwqmze.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jyoumei.cn/gtfrrjzjzc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gzhubu.top/gtphgiqjub.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.smart0.xyz/gtninldmfb.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ppjwa.cn/gteyvzdehr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jinghuilouyu.cn/gtrucucqtf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jinqigfzy.top/gtgyzxdjdy.html

[E22] 字节长度与字符长度
来源：http://hz.xuanzx.com/gtkjujdvet.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yvedp.cn/gtagpsafbp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.fengsongda.top/gtfpasaixj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yanxiufei.cn/gtfbdijrxl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.haohaochexian.top/gtqzomfyqi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.hysaishi.cn/gtvqzfhtke.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.meibo888.top/gtodxojsjw.html

Ruby: s.bytesize;  s.length
来源：http://hz.pengpengdd.cyou/gtomwjfdww.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zdqjudy.top/gtjmoerieu.html

================================================================================
来源：http://hz.gaohongyu789.top/gtfqfcuzsz.html

F. 文件与目录
来源：http://hz.chenzaomai.com/gtmiifvshi.html

================================================================================
来源：http://hz.ybcxt.top/gtclyubhwn.html

[F01] 读取整个文件
来源：http://hz.jinqigufen.top/gtrvfyeztj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.bjfxy.top/gtnpqcczdv.html

PHP:  file_get_contents("a.txt");
来源：http://hz.ydzc1.top/gtstntuqzm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.smart0.xyz/gtbxhsfrgs.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yongpay.top/gttdfmbdoh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.quarkkingdee.top/gtmbmvkgxs.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yj20258.top/gtpjvwlutn.html

Ruby: File.read("a.txt")
来源：http://hz.sxryk.cn/gttlpqsrkk.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.nanxuanxn.top/gtajvogolb.html

[F02] 逐行读取文件
来源：http://hz.jqgufenzy.top/gtgfvazutv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.xingfuxueyuan.xyz/gtfjsdkbqr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.gogol.net.cn/gtiibzqzmp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yueranfly.top/gtncfgqish.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.mhx1999.top/gtzwfbofcb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.dashuyun.cn/gtoxpxjeog.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.redwolf501.top/gtjkcdfxqm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.aizwys.cn/gtwwelglcp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.andypj.xyz/gtemquivlf.html

[F03] 写入文件（覆盖）
来源：http://hz.shuidangran.top/gtvcwmtvqs.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.xziqi.cn/gtrrqtqwwx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.havefunace.top/gtxjdwdxxn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhongyouzk.top/gtxhfegpmv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.tianlin.xyz/gtsnseqnli.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.gogol.net.cn/gtskvomgin.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.dashuyun.cn/gtczcmvqct.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.gotoacloud.top/gtgnjzcwoz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.kuanghao11.cn/gtwnptpean.html

[F04] 追加写入文件
来源：http://hz.9152youxi.cn/gtjdlgftzq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jinqigufen.top/gtppetpctr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hnqzz.top/gthacdcdky.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.daria6918.cn/gtjcdgqedj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cheryme.top/gtsiutbomh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zhongyouzk.top/gtlnklvzwj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.fengsongda.top/gtkhpotetm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhijiandao.cn/gtwpvmpago.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zhongyouzk.top/gtbswrlyyz.html

[F05] 判断文件或目录是否存在
来源：http://hz.yueranfly.top/gtyjccaefj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.haohaochexian.top/gtslcbkcpx.html

PHP:  file_exists("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtdprncgwn.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hnxiangtu.top/gtcjxicuig.html

TS:   fs.existsSync("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtiyxbrcxn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.daxiang520.top/gttuovuqkr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ydjk.org.cn/gtsoyljjbh.html

Ruby: File.exist?("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtlgyltcuc.html

C#:   File.Exists("a.txt")
来源：http://hz.sufxvd.cn/gtmdwnfbpp.html

[F06] 删除文件
来源：http://hz.jyoumei.cn/gtermdtxhd.html

Py:   os.remove("a.txt")
来源：http://hz.hywenlv.cn/gtfqrmshdj.html

PHP:  unlink("a.txt");
来源：http://hz.tianlin.xyz/gthzggikdb.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.c1oappe.top/gtbkmmqvko.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yongpay.top/gthmjgxdwt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhengqikj.top/gtujwisstn.html

Go:   os.Remove("a.txt")
来源：http://hz.316326.xyz/gthunsqazs.html

Ruby: File.delete("a.txt")
来源：http://hz.yuxming.cn/gtkdwepckp.html

C#:   File.Delete("a.txt");
来源：http://hz.yuxming.cn/gtzapzvdwn.html

[F07] 创建目录（含多级）
来源：http://hz.nanxinkj.top/gtpyugddhv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.quarkkingdee.top/gtwrumqfyn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.316326.xyz/gtynsuneft.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cheryme.top/gtekdntrwd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hnxiangtu.top/gtqymbzcmb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.dianchejie.cn/gtdmwdkhiq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.sweek.top/gtkdjalbzz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zhijiandao.cn/gtbwqrvqbq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.sxryk.cn/gteodhmdwt.html

[F08] 遍历目录
来源：http://hz.nanxinkj.top/gtvijlyeah.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.hnxiangtu.top/gtwitqjndu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.gaohongyu789.top/gtptxkroge.html

JS:   fs.readdirSync("dir")
来源：http://hz.shanyushiyangkeji.top/gtjvnrauqz.html

TS:   fs.readdirSync("dir")
来源：http://hz.yongpay.top/gtydmmybef.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.bjfxy.top/gtyalioiif.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.xuanzx.com/gthyaiespe.html

Ruby: Dir.children("dir")
来源：http://hz.gzhubu.top/gtsusxxzxk.html

C#:   Directory.GetFiles("dir")
来源：http://hz.cheryme.top/gtcbveqyqp.html

[F09] 获取文件大小
来源：http://hz.shzxlz.cn/gtioxsxxjs.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ydzc1.top/gtgjnmprps.html

PHP:  filesize("a.txt");
来源：http://hz.zhixingplan.top/gtyidwffyy.html

JS:   fs.statSync("a.txt").size
来源：http://hz.dashuyun.cn/gtuevlqxzj.html

TS:   fs.statSync("a.txt").size
来源：http://hz.cheryme.top/gtjnbwgkgc.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.xylfe.cn/gtdnbdfrnk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.iojbl.cn/gtniwwvthn.html

Ruby: File.size("a.txt")
来源：http://hz.cqqwz.cn/gtyzgtcish.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ydjk.org.cn/gtpankfwnl.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhixingplan.top/gtztxjifgw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yangfankeji.com/gtkjuxxxlu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.tianlin.xyz/gtrhcmakzg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hywenlv.cn/gtkrsgurfo.html

TS:   path.extname("a.txt")
来源：http://hz.yj20258888.top/gtjnlaybrd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.fzhhl.top/gtbkjtcrps.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.9152youxi.cn/gtgxgxylus.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gtewtqdhya.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jiagoushi.top/gtzhfppzpt.html

[F11] 复制与移动文件
来源：http://hz.xziqi.cn/gtgefcwphn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.havefunace.top/gtufgvroap.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.aibaodan.cn/gtzwjlmnnq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ehwqpu.com/gtvkaqadkp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shangyingyoupin.top/gtdkwbycdu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jianghu66.top/gtquirnazt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jqgfzy.top/gtgrqerexo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.chenjidiqi.icu/gtiwjvmutg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hfpthk.cn/gteymtwkhf.html

[F12] CSV 读写
来源：http://hz.tanke756.top/gtqzyjyfgl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.gaohongyu789.top/gtjyqxlaod.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.nanxuanxn.top/gtiukjiwsc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhoulong.xyz/gtcseqcqza.html

TS:   // 同上
来源：http://hz.9152youxi.cn/gtsiyjtwuv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jqgfzy.top/gtzcfvotgy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zycfv.cn/gtazkdhhgk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.sweek.top/gtcqalhjqa.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.quarkkingdee.top/gtddujzxsv.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtdnopymxd.html

G. 面向对象
来源：http://hz.chenlongwang.top/gtvwimzhqo.html

================================================================================
来源：http://hz.yvedp.cn/gttrajwdcr.html

[G01] 定义类
来源：http://hz.bjfxy.top/gthrmapdvb.html

Py:   class User: pass
来源：http://hz.yangfankeji.com/gtwmftnqpn.html

PHP:  class User {}
来源：http://hz.tianlin.xyz/gtfdlqpnvu.html

JS:   class User {}
来源：http://hz.ybcxt.top/gtywvgztkc.html

TS:   class User { name: string = ""; }
来源：http://hz.zhengqikj.top/gtdhnzlufg.html

Java: class User {}
来源：http://hz.cdnleiting.top/gtgnlcjheu.html

Go:   type User struct { Name string }
来源：http://hz.sxryk.cn/gtvrsuvgha.html

Ruby: class User; end
来源：http://hz.birdmap.top/gtyzquvyph.html

C#:   class User {}
来源：http://hz.xuanzx.com/gttawtrtoy.html

[G02] 构造函数
来源：http://hz.hongshengwenyu.top/gttqkemmvt.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.ydzc1.top/gtqlakveuu.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.sysykeji.top/gtlccznedg.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.svipenyu.cn/gtynpyoxbe.html

TS:   constructor(public name: string) {}
来源：http://hz.dashuyun.cn/gtxzdwolig.html

Java: User(String name) { this.name = name; }
来源：http://hz.jinqigufen.top/gtbwnlptdb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.chenjidiqi.icu/gtmtbvooyb.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.hongshengwenyu.top/gtwshktwuv.html

C#:   public User(string name) { Name = name; }
来源：http://hz.xylfe.cn/gtedpglbxt.html

[G03] 实例属性
来源：http://hz.cashguo.top/gtomtbxalt.html

Py:   self.name = "x"
来源：http://hz.yanxiufei.cn/gtguwbwgjo.html

PHP:  public string $name = "x";
来源：http://hz.mhx1999.top/gtfcktvfir.html

JS:   this.name = "x";
来源：http://hz.ydjk.org.cn/gtcqdnpkiq.html

TS:   name: string = "x";
来源：http://hz.dashuyun.cn/gtozwuplje.html

Java: private String name;
来源：http://hz.hywenlv.cn/gtpqrnjjky.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shuidangran.top/gtpbdxujzx.html

Ruby: @name = "x"
来源：http://hz.dashuyun.cn/gtetxpibiy.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ywan-chungtsiang.top/gtmpgbzmmi.html

[G04] 定义方法
来源：http://hz.shzxlz.cn/gtykdsdlsx.html

Py:   def greet(self): return self.name
来源：http://hz.sufxvd.cn/gtruujgkao.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yanxiufei.cn/gtymzqrlpz.html

JS:   greet() { return this.name; }
来源：http://hz.fzhhl.top/gtfoqgpdqf.html

TS:   greet(): string { return this.name; }
来源：http://hz.ybcxt.top/gturiqelfi.html

Java: String greet() { return name; }
来源：http://hz.jqgfzy.top/gtjutrxegl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yj202588.top/gtjievqmhb.html

Ruby: def greet; @name; end
来源：http://hz.ppjwa.cn/gtqavjtodx.html

C#:   public string Greet() => Name;
来源：http://hz.wangdashe.top/gtjnircazq.html

[G05] 继承
来源：http://hz.cqqwz.cn/gtnqeghmgl.html

Py:   class Admin(User): pass
来源：http://hz.jinqigfzy.top/gtikjrkmkx.html

PHP:  class Admin extends User {}
来源：http://hz.jinqigfzy.top/gtgbzusiwb.html

JS:   class Admin extends User {}
来源：http://hz.cheryme.top/gtegytrxhk.html

TS:   class Admin extends User {}
来源：http://hz.jiagoushi.top/gtzyeyaqan.html

Java: class Admin extends User {}
来源：http://hz.316326.xyz/gtimsldkdi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.kuanghao11.cn/gtbwvhtvsx.html

Ruby: class Admin < User; end
来源：http://hz.guowangkeji.top/gtgstzlhjl.html

C#:   class Admin : User {}
来源：http://hz.dianchejie.cn/gthsnpltbz.html

[G06] 重写方法
来源：http://hz.sysykeji.top/gtwfyofgzf.html

Py:   def greet(self): return "admin"
来源：http://hz.hywenlv.cn/gtbogovyzn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.redwolf501.top/gtcnxifyil.html

JS:   greet() { return "admin"; }
来源：http://hz.guannengcc.top/gtzdmpnazo.html

TS:   greet(): string { return "admin"; }
来源：http://hz.birdmap.top/gtinurbrir.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.tian-w.cn/gtmnjugjve.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.hnxiangtu.top/gtxmujrtbj.html

Ruby: def greet; "admin"; end
来源：http://hz.xingfuxueyuan.xyz/gtfcxmzvge.html

C#:   public override string Greet() => "admin";
来源：http://hz.guowangkeji.top/gtibebssbf.html

[G07] 调用父类方法
来源：http://hz.tanke756.top/gtlmxrnvgz.html

Py:   super().greet()
来源：http://hz.quarkkingdee.top/gtysvemaoi.html

PHP:  parent::greet();
来源：http://hz.ywan-chungtsiang.top/gtrhaudtxh.html

JS:   super.greet();
来源：http://hz.guannengcc.top/gtqjfiutft.html

TS:   super.greet();
来源：http://hz.smart0.xyz/gtouvtsblk.html

Java: super.greet();
来源：http://hz.hongshengwenyu.top/gtchyiduzs.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.daria6918.cn/gtzcgsndkh.html

Ruby: super
来源：http://hz.svipenyu.cn/gtkjouvsbo.html

C#:   base.Greet();
来源：http://hz.yuxming.cn/gtdvvfcmml.html

[G08] 静态方法与属性
来源：http://hz.chenjidiqi.icu/gtpripwpke.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.feifeiyinyue.top/gtxqtwqddg.html

PHP:  public static function f() {}
来源：http://hz.cashguo.top/gtivgllftc.html

JS:   static f() {}
来源：http://hz.hammf.cn/gtlhdukblg.html

TS:   static f(): void {}
来源：http://hz.gaohongyu789.top/gtuxlbepzg.html

Java: static void f() {}
来源：http://hz.ivvv.top/gtdyqqmjsh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.ybcxt.top/gtkslhnels.html

Ruby: def self.f; end
来源：http://hz.zhongyouzk.top/gtinswgaul.html

C#:   public static void F() {}
来源：http://hz.zhijiandao.cn/gtjubseaio.html

[G09] 接口 / 抽象类
来源：http://hz.guowangkeji.top/gtjemofeqx.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ywan-chungtsiang.top/gtmokspcsi.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hammf.cn/gtuyeqnmef.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.dianchejie.cn/gtqoiwljpa.html

TS:   interface Shape { area(): number; }
来源：http://hz.nwbrower.top/gtjhpbmezx.html

Java: interface Shape { double area(); }
来源：http://hz.sysykeji.top/gtbhsbewfj.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.sufxvd.cn/gtqrrcgnol.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.cdnleiting.top/gtgambezsp.html

C#:   interface IShape { double Area(); }
来源：http://hz.yangfankeji.com/gtpqidioic.html

[G10] 访问控制
来源：http://hz.tanke756.top/gtwhngnnvz.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.cheryme.top/gtasrtvovr.html

PHP:  public / protected / private
来源：http://hz.chenjidiqi.icu/gtvtjipaqk.html

JS:   #private 字段；其余公开
来源：http://hz.daxiang520.top/gtotwowwso.html

TS:   public / protected / private
来源：http://hz.fzhhl.top/gtmlmscuds.html

Java: public / protected / private / 默认包级
来源：http://hz.birdmap.top/gtbpfpibor.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.wangdashe.top/gtrbheezjg.html

Ruby: public / protected / private
来源：http://hz.quarkkingdee.top/gtcsduioka.html

C#:   public / protected / private / internal
来源：http://hz.yonumen.top/gtvsgtmiwl.html

[G11] getter / setter
来源：http://hz.mhx1999.top/gtawjqbwie.html

Py:   @property 与 @x.setter
来源：http://hz.ydzc1.top/gtwnnlrqsk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.kuanghao11.cn/gtcbtxdaoa.html


<!-- 参考信息 -->