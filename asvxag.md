代发 wailian999

[E14] URL 编码与 Base64
来源：http://hz.ehwqpu.com/gtbfgesiza.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhoulong.xyz/gtwoydymbr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.ydzc1.top/gttryigtwm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.daxiang520.top/gtyjgdctpn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.aibaodan.cn/gtxvsbywxs.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.meibo888.top/gtcgpolopx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhengqikj.top/gtkkunswki.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jinqigufen.top/gtlynrslml.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.shzxlz.cn/gtbghpyttw.html

[E15] HTML 转义 / 反转义
来源：http://hz.tanke756.top/gtdvzkniqh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.meibo888.top/gtvvzdrwjs.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jyoumei.cn/gtanvyeram.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zhongyouzk.top/gtiodncews.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zdqjudy.top/gtawrsqsah.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.shangyingyoupin.top/gtbwqvlihv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.fzhhl.top/gtraejhfji.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yj20258888.top/gtfjfiwjvi.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.hfpthk.cn/gtqjoavzvu.html

[E16] 数字千分位
来源：http://hz.9152youxi.cn/gtosyfjvav.html

Py:   f"{1234567:,}"
来源：http://hz.shangyingyoupin.top/gtupyacxbq.html

PHP:  number_format(1234567);
来源：http://hz.snrcjt.cn/gtxhhjhtix.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.sufxvd.cn/gtkybqwjic.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.cqqwz.cn/gtsqwgxhfu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.birdmap.top/gtdatrpptj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.tanke756.top/gterqzkxpz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.hnxiangtu.top/gtsttfmker.html

C#:   1234567.ToString("N0")
来源：http://hz.jinqigfzy.top/gtjkgcvdhd.html

[E17] 首字母大写
来源：http://hz.mhx1999.top/gtjwdqxclu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zhiwuduotai.top/gtczvasyst.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.kuanghao11.cn/gtllruxmbo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gzhubu.top/gttsyhpbyj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.nanxuanxn.top/gthgwozlhv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ivvv.top/gtzqbkwuuj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.daxiang520.top/gtzimjhgvv.html

Ruby: s.capitalize
来源：http://hz.zhixingplan.top/gtcnvjrare.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.sufxvd.cn/gtoivwhbth.html

[E18] 模板占位符替换
来源：http://hz.zhengqikj.top/gtezaatiep.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hysaishi.cn/gtjcgiaimg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.nanxinkj.top/gtzqwfjnin.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.ydjk.org.cn/gtxvttjjxe.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yj202588.top/gtotveqnym.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jiagoushi.top/gtdaxrvkdv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yj20258888.top/gtzprgqqzp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hongshengwenyu.top/gtonuwroms.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.sufxvd.cn/gtgbpvoije.html

[E19] 多行文本按行拆分
来源：http://hz.iojbl.cn/gtnhnghudj.html

Py:   s.splitlines()
来源：http://hz.gaohongyu789.top/gtbknljpia.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.shuidangran.top/gtkrhblyjf.html

JS:   s.split(/\r?\n/)
来源：http://hz.quarkkingdee.top/gtbzziljta.html

TS:   s.split(/\r?\n/)
来源：http://hz.andypj.xyz/gtgmdkvmcz.html

Java: s.lines().toList()
来源：http://hz.shangyingyoupin.top/gtziqoezyf.html

Go:   strings.Split(s, "\n")
来源：http://hz.ppjwa.cn/gtrguwvjwg.html

Ruby: s.lines
来源：http://hz.shanyushiyangkeji.top/gtjbzsikfn.html

C#:   s.Split('\n')
来源：http://hz.yueranfly.top/gtvohzoady.html

[E20] 判断字符串是否为空
来源：http://hz.9152youxi.cn/gtxbiiwyyt.html

Py:   if not s:
来源：http://hz.vqdsnc.cn/gtvieycxoo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yvedp.cn/gtrcctunyo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jinqigfzy.top/gtacrscyxz.html

TS:   if (s === "") {}
来源：http://hz.zdqjudy.top/gtxsesaczn.html

Java: if (s.isEmpty()) {}
来源：http://hz.hammf.cn/gtculrnxar.html

Go:   if s == "" {}
来源：http://hz.zhengqikj.top/gtavrlhdqh.html

Ruby: if s.empty?
来源：http://hz.birdmap.top/gtdwwwxzyo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.redwolf501.top/gtaubzcide.html

[E21] 超长截断加省略号
来源：http://hz.yj20258.top/gtdchqoyiv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.redwolf501.top/gtedduikav.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.xinyue.icu/gtvubdfuhp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhoulong.xyz/gtuieuttye.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.9152youxi.cn/gtvdljvgan.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yanxiufei.cn/gthmxvytnz.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.daria6918.cn/gtiziukaab.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.nanxinkj.top/gtmgrxmfcl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yj202588.top/gtenruoifk.html

[E22] 字节长度与字符长度
来源：http://hz.andypj.xyz/gtsbpnznlr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.fengsongda.top/gtevgsuyob.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shuidangran.top/gtiqtgykst.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hywenlv.cn/gtejkxtzkk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cheryme.top/gtigtzvjmy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.hnxiangtu.top/gtqtwmcujt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.nanxuanxn.top/gtogatunbc.html

Ruby: s.bytesize;  s.length
来源：http://hz.pycfn.com/gtfrxpxjii.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jinqigfzy.top/gtxtjbvbio.html

================================================================================
来源：http://hz.ybcxt.top/gtthqrnapa.html

F. 文件与目录
来源：http://hz.xuanzx.com/gtwyeyfgbi.html

================================================================================
来源：http://hz.jyoumei.cn/gtiuzwptxr.html

[F01] 读取整个文件
来源：http://hz.xuetiantiany.cn/gthcvpggoh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.nwbrower.top/gtjtbaggvm.html

PHP:  file_get_contents("a.txt");
来源：http://hz.ydjk.org.cn/gtjinvpefu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.aizwys.cn/gtfcjuitng.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hongshengwenyu.top/gtinozvlgt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.xinyue.icu/gtzihluvet.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.gotoacloud.top/gtudmhcklt.html

Ruby: File.read("a.txt")
来源：http://hz.vqdsnc.cn/gtskqyxpws.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jyoumei.cn/gtioxrkxej.html

[F02] 逐行读取文件
来源：http://hz.yonumen.top/gtlvbmoqyy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.c1oappe.top/gtllnluayh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ywan-chungtsiang.top/gtzryunsjt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ywan-chungtsiang.top/gtggtgbfzn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zycfv.cn/gtvczpavfw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yangfankeji.com/gtqfjxktpj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhijiandao.cn/gtiseparcc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zhongyouzk.top/gtiezsijvs.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.wangdashe.top/gtfthwiuqy.html

[F03] 写入文件（覆盖）
来源：http://hz.guannengcc.top/gtuxlrjabb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.haohaochexian.top/gtzcytveqn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.kuanghao11.cn/gtibvtmdvh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhengqikj.top/gthahauvcq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhengqikj.top/gtfkmlwsmp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.bjfxy.top/gtsdjsdiwi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.chenjidiqi.icu/gtvptigleo.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yongpay.top/gtimblyxct.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.gogol.net.cn/gtxgsecsco.html

[F04] 追加写入文件
来源：http://hz.shzxlz.cn/gtakeaxdtq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yj20258.top/gtvjfvgcyg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.ehwqpu.com/gtdjxfeaxk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yuxming.cn/gtzbzyuoru.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ivvv.top/gtemigynpm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.havefunace.top/gtowklcpbk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.hfpthk.cn/gttpjbqhid.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.meibo888.top/gtseetgdfe.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zhixingplan.top/gtinifriad.html

[F05] 判断文件或目录是否存在
来源：http://hz.bjfxy.top/gtfslqxhac.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.hysaishi.cn/gtjgyskjzs.html

PHP:  file_exists("a.txt");
来源：http://hz.ydjk.org.cn/gtfiszfknd.html

JS:   fs.existsSync("a.txt")
来源：http://hz.wangshuangyany.cn/gtzumybijp.html

TS:   fs.existsSync("a.txt")
来源：http://hz.0kj1m.cn/gtllhzelva.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jqgfzy.top/gteppznrss.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ydzc1.top/gtdkvxaeyz.html

Ruby: File.exist?("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtjdovnyai.html

C#:   File.Exists("a.txt")
来源：http://hz.jiagoushi.top/gttphyuvrn.html

[F06] 删除文件
来源：http://hz.cheryme.top/gtcbbbmeaw.html

Py:   os.remove("a.txt")
来源：http://hz.yj202588.top/gtbsemrpwv.html

PHP:  unlink("a.txt");
来源：http://hz.jiagoushi.top/gtgmetoeef.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.chenlongwang.top/gtnzdbwbhp.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jinghuilouyu.cn/gteilrkvcp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.cdnleiting.top/gtxuksusin.html

Go:   os.Remove("a.txt")
来源：http://hz.hnqzz.top/gtczogunkt.html

Ruby: File.delete("a.txt")
来源：http://hz.cdnleiting.top/gtkodkrgpp.html

C#:   File.Delete("a.txt");
来源：http://hz.yvedp.cn/gtbvckvzcn.html

[F07] 创建目录（含多级）
来源：http://hz.gotoacloud.top/gtqahqcykp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jinqigufen.top/gteudidsap.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.gotoacloud.top/gtinwecucj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.chenjidiqi.icu/gtqhpgkdyc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.havefunace.top/gtxeizyxsf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hnqzz.top/gtcizocstb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.guowangkeji.top/gtpqsklqzk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yuxming.cn/gtugawutqa.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.xingfuxueyuan.xyz/gtpagognfs.html

[F08] 遍历目录
来源：http://hz.jinqigufen.top/gtxmquowre.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.sxryk.cn/gthdaasgsw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.quarkkingdee.top/gtqoejodyz.html

JS:   fs.readdirSync("dir")
来源：http://hz.chenjidiqi.icu/gtzbzhclpx.html

TS:   fs.readdirSync("dir")
来源：http://hz.jinghuilouyu.cn/gthldgakte.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.shzxlz.cn/gtxzcuaerj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.mhx1999.top/gtpydoyoya.html

Ruby: Dir.children("dir")
来源：http://hz.gzhubu.top/gttnnyyyss.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jianghu66.top/gtptsdchbt.html

[F09] 获取文件大小
来源：http://hz.yj20258888.top/gtwtceoycg.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yj20258888.top/gtxtdinpjf.html

PHP:  filesize("a.txt");
来源：http://hz.ywan-chungtsiang.top/gtkvkbqtsx.html

JS:   fs.statSync("a.txt").size
来源：http://hz.daria6918.cn/gthgpaydvl.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hnqzz.top/gtmezvqtep.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.daxiang520.top/gtbkhnxhup.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhoulong.xyz/gtlslxiyha.html

Ruby: File.size("a.txt")
来源：http://hz.jqgfzy.top/gtnvturcob.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yj202588.top/gtautddpyd.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ybcxt.top/gttrjlihtn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.daxiang520.top/gteehxaxrf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.chenjidiqi.icu/gttlorsauv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtpcnfudvl.html

TS:   path.extname("a.txt")
来源：http://hz.shuidangran.top/gtpldyblny.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ywan-chungtsiang.top/gthcvgcsog.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hnqzz.top/gtxoxveqdc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.52xcode.cn/gtwjocexkj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.xziqi.cn/gtdjpvvgdd.html

[F11] 复制与移动文件
来源：http://hz.havefunace.top/gtniklvxmb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.xuetiantiany.cn/gtgdeavunl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.daria6918.cn/gtzxdancri.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hongshengwenyu.top/gtkhesxmkt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gzhubu.top/gtihbqilbv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ppjwa.cn/gtigtbxefo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.0kj1m.cn/gtoudzqbwm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ybcxt.top/gtqwyoxdiu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.tanke756.top/gtkheyrpgj.html

[F12] CSV 读写
来源：http://hz.jinqigufen.top/gtwrwefhwi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.andypj.xyz/gtdbkjvjct.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.smart0.xyz/gtmnfrjate.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.meibo888.top/gtctarfnvc.html

TS:   // 同上
来源：http://hz.ppjwa.cn/gtkbchkfnm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.bjfxy.top/gtpkwwifux.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ehwqpu.com/gtcvzxwddn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.316326.xyz/gtmxsouylt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.havefunace.top/gtcohgkjqh.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtwionwzqq.html

G. 面向对象
来源：http://hz.dianchejie.cn/gtksoaxpgb.html

================================================================================
来源：http://hz.yangfankeji.com/gthdhgigyj.html

[G01] 定义类
来源：http://hz.316326.xyz/gtmvonrbmc.html

Py:   class User: pass
来源：http://hz.fengsongda.top/gtmgekejya.html

PHP:  class User {}
来源：http://hz.wangshuangyany.cn/gtrughsuik.html

JS:   class User {}
来源：http://hz.zhiwuduotai.top/gtxmsikuwg.html

TS:   class User { name: string = ""; }
来源：http://hz.cheryme.top/gttrnkbyly.html

Java: class User {}
来源：http://hz.fengsongda.top/gtzakakrbw.html

Go:   type User struct { Name string }
来源：http://hz.hongshengwenyu.top/gtssztqaeq.html

Ruby: class User; end
来源：http://hz.tianlin.xyz/gtmexssbtj.html

C#:   class User {}
来源：http://hz.gotoacloud.top/gtxdumuxia.html

[G02] 构造函数
来源：http://hz.tianlin.xyz/gtzituuhjv.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.pengpengdd.cyou/gtwdwtdzyp.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.pycfn.com/gtpxvwollz.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yanxiufei.cn/gtkesxkwrq.html

TS:   constructor(public name: string) {}
来源：http://hz.9152youxi.cn/gtvqczojxy.html

Java: User(String name) { this.name = name; }
来源：http://hz.cqqwz.cn/gtuzpwweez.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shangyingyoupin.top/gtkpofisuc.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.sysykeji.top/gterkztlxr.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ydjk.org.cn/gtwwrrlsck.html

[G03] 实例属性
来源：http://hz.aibaodan.cn/gtnksryknn.html

Py:   self.name = "x"
来源：http://hz.yvedp.cn/gtsscozcla.html

PHP:  public string $name = "x";
来源：http://hz.iojbl.cn/gtsuwmcwhr.html

JS:   this.name = "x";
来源：http://hz.jqgfzy.top/gtfvuuawkl.html

TS:   name: string = "x";
来源：http://hz.zhijiandao.cn/gtstxordab.html

Java: private String name;
来源：http://hz.aibaodan.cn/gtgjhiqgio.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jinghuilouyu.cn/gtdobzsofn.html

Ruby: @name = "x"
来源：http://hz.aibaodan.cn/gtccdqjwdh.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jianghu66.top/gtjmrortrj.html

[G04] 定义方法
来源：http://hz.ywan-chungtsiang.top/gtjygnrfgs.html

Py:   def greet(self): return self.name
来源：http://hz.andypj.xyz/gthdgyptze.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.xuanzx.com/gtbrfflnsy.html

JS:   greet() { return this.name; }
来源：http://hz.pengpengdd.cyou/gtwmzhcslg.html

TS:   greet(): string { return this.name; }
来源：http://hz.xuanzx.com/gtwmdezuzj.html

Java: String greet() { return name; }
来源：http://hz.yueranfly.top/gtgxfbdbrs.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.gaohongyu789.top/gtxlvpbyww.html

Ruby: def greet; @name; end
来源：http://hz.tanke756.top/gttqxttfwk.html

C#:   public string Greet() => Name;
来源：http://hz.zdqjudy.top/gtaabsntgr.html

[G05] 继承
来源：http://hz.dianchejie.cn/gtwbbznbtl.html

Py:   class Admin(User): pass
来源：http://hz.ehwqpu.com/gtvskcrync.html

PHP:  class Admin extends User {}
来源：http://hz.shanyushiyangkeji.top/gtgbchnowa.html

JS:   class Admin extends User {}
来源：http://hz.sweek.top/gtvbqjdrad.html

TS:   class Admin extends User {}
来源：http://hz.yongpay.top/gtqrctsbcw.html

Java: class Admin extends User {}
来源：http://hz.andypj.xyz/gtfwqzttgh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.chenzaomai.com/gtejwkzrie.html

Ruby: class Admin < User; end
来源：http://hz.ywan-chungtsiang.top/gtjwwlbzhr.html

C#:   class Admin : User {}
来源：http://hz.aizwys.cn/gtdoifkuqz.html

[G06] 重写方法
来源：http://hz.sxryk.cn/gtrrwehwpu.html

Py:   def greet(self): return "admin"
来源：http://hz.chenlongwang.top/gtrjqkhrgw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhiwuduotai.top/gtjzjcsjke.html

JS:   greet() { return "admin"; }
来源：http://hz.pengpengdd.cyou/gtdzxcoqcn.html

TS:   greet(): string { return "admin"; }
来源：http://hz.daria6918.cn/gtetrfvlpd.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xziqi.cn/gtzgeajxpy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.bjfxy.top/gtporugaty.html

Ruby: def greet; "admin"; end
来源：http://hz.yj20258888.top/gtoszaqfrk.html

C#:   public override string Greet() => "admin";
来源：http://hz.quarkkingdee.top/gttcmmqjgb.html

[G07] 调用父类方法
来源：http://hz.smart0.xyz/gtvfwlxmce.html

Py:   super().greet()
来源：http://hz.sweek.top/gtmsusqbyv.html

PHP:  parent::greet();
来源：http://hz.daria6918.cn/gtcycbwwau.html

JS:   super.greet();
来源：http://hz.pengpengdd.cyou/gtpnzylqfq.html

TS:   super.greet();
来源：http://hz.xuanzx.com/gtqyraoeva.html

Java: super.greet();
来源：http://hz.chenzaomai.com/gtgrjixott.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.feifeiyinyue.top/gtlxcyvmhd.html

Ruby: super
来源：http://hz.iojbl.cn/gtwpzvteuc.html

C#:   base.Greet();
来源：http://hz.gotoacloud.top/gthrrgnlee.html

[G08] 静态方法与属性
来源：http://hz.ydjk.org.cn/gtlusdiqnu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hysaishi.cn/gtiafnqwrq.html

PHP:  public static function f() {}
来源：http://hz.shanyushiyangtech.top/gtdwfbzeft.html

JS:   static f() {}
来源：http://hz.tanke756.top/gtezbmtfvt.html

TS:   static f(): void {}
来源：http://hz.smart0.xyz/gtopfcctew.html

Java: static void f() {}
来源：http://hz.c1oappe.top/gtfqotynht.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhixingplan.top/gteqoeubll.html

Ruby: def self.f; end
来源：http://hz.c1oappe.top/gthczdupuw.html

C#:   public static void F() {}
来源：http://hz.zhongyouzk.top/gtqogxagds.html

[G09] 接口 / 抽象类
来源：http://hz.ydjk.org.cn/gtcyfbzzya.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.iojbl.cn/gthuntmdbz.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.316326.xyz/gtvnwyixbt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.nanxinkj.top/gtrtgpbxnv.html

TS:   interface Shape { area(): number; }
来源：http://hz.sweek.top/gtnwjjhjsm.html

Java: interface Shape { double area(); }
来源：http://hz.pengpengdd.cyou/gtfixkynlm.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.chenzaomai.com/gtxjmtkllv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.nanxuanxn.top/gtlmlpgual.html

C#:   interface IShape { double Area(); }
来源：http://hz.jqgufenzy.top/gtmfuvqhul.html

[G10] 访问控制
来源：http://hz.andypj.xyz/gtmhqbficb.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jinqigufen.top/gtaxtjkqwj.html

PHP:  public / protected / private
来源：http://hz.hongshengwenyu.top/gtfucovrjb.html

JS:   #private 字段；其余公开
来源：http://hz.chenlongwang.top/gtrtmkgskh.html

TS:   public / protected / private
来源：http://hz.jqgufenzy.top/gtzfmcrswq.html

Java: public / protected / private / 默认包级
来源：http://hz.guowangkeji.top/gtzybgsnta.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jinqigufen.top/gtadmikoyz.html

Ruby: public / protected / private
来源：http://hz.dashuyun.cn/gtmryrqdtw.html

C#:   public / protected / private / internal
来源：http://hz.yonumen.top/gthdnepord.html

[G11] getter / setter
来源：http://hz.xinyue.icu/gtwxesjupo.html

Py:   @property 与 @x.setter
来源：http://hz.zhiwuduotai.top/gtljcopujv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.cashguo.top/gttyltwzkn.html

JS:   get name() { return this._name; }
来源：http://hz.zdqjudy.top/gtqnjdmyzt.html

TS:   get name(): string { return this._name; }
来源：http://hz.yj202588.top/gtoxchqyro.html

Java: public String getName() { return name; }
来源：http://hz.yanxiufei.cn/gtuuxmfivi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.dianchejie.cn/gtzutxkkew.html

Ruby: attr_accessor :name
来源：http://hz.yangfankeji.com/gtpwkkxtps.html

C#:   public string Name { get; set; }
来源：http://hz.kuanghao11.cn/gtyuntjscp.html

[G12] 对象转字符串
来源：http://hz.zhoulong.xyz/gtjtnkzzaf.html

Py:   def __str__(self): return self.name
来源：http://hz.hfpthk.cn/gteplsgusq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.redwolf501.top/gtjxnnjcoa.html

JS:   toString() { return this.name; }
来源：http://hz.jinyuanbaomall.cn/gtafsanmkw.html

TS:   toString(): string { return this.name; }
来源：http://hz.sysykeji.top/gtogrusdve.html

Java: @Override public String toString() { return name; }
来源：http://hz.316326.xyz/gtldgzkbmx.html


<!-- 参考信息 -->