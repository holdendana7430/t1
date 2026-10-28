代发 wailian999

JS:   [...s].reverse().join("")
来源：http://hz.yanxiufei.cn/gtaisxicjs.html

TS:   [...s].reverse().join("")
来源：http://hz.xingfuxueyuan.xyz/gtsxhzemmq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.kuanghao11.cn/gtdwxpsbjx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yanxiufei.cn/gthqxsjuly.html

Ruby: s.reverse
来源：http://hz.gogol.net.cn/gtmxhihhfk.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hfpthk.cn/gtkpxjcqlg.html

[E12] 统计某字符出现次数
来源：http://hz.yueranfly.top/gtzfuxspsh.html

Py:   s.count("a")
来源：http://hz.jiagoushi.top/gtqpejslbg.html

PHP:  substr_count($s, "a");
来源：http://hz.jqgfzy.top/gtwqammcex.html

JS:   s.split("a").length - 1
来源：http://hz.yongpay.top/gtosdeokji.html

TS:   s.split("a").length - 1
来源：http://hz.shangyingyoupin.top/gtdrucvgqj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zhoulong.xyz/gtupuaqugu.html

Go:   strings.Count(s, "a")
来源：http://hz.xingfuxueyuan.xyz/gtizroglgg.html

Ruby: s.count("a")
来源：http://hz.smart0.xyz/gttfbxwibl.html

C#:   s.Count(c => c == 'a')
来源：http://hz.hywenlv.cn/gttwiagcja.html

[E13] 逐字符遍历
来源：http://hz.yj202588.top/gtkbbfulrx.html

Py:   for ch in s: print(ch)
来源：http://hz.quarkkingdee.top/gtdjdtlrbz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.cashguo.top/gtitopowyi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.tanke756.top/gtpmnmtbro.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jianghu66.top/gtbpyootyo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jlsjyb.cn/gtzgwjhrpa.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.cqqwz.cn/gtjempjygh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.kuanghao11.cn/gtolrptprv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.xuetiantiany.cn/gttmikmyaq.html

[E14] URL 编码与 Base64
来源：http://hz.zhongyouzk.top/gtfdrqqhmo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yj20258.top/gtqxsqqozh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.zhaomingkeji.xyz/gtlhmvzhjs.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.ybcxt.top/gtxopugwtt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.xziqi.cn/gthxxhvesb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zycfv.cn/gtpovibgod.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.guannengcc.top/gtjtuogcyu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.hywenlv.cn/gtwqhejhau.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.9152youxi.cn/gtuhpqxaro.html

[E15] HTML 转义 / 反转义
来源：http://hz.hammf.cn/gtyqzwbplm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.nanxuanxn.top/gtmlqvaohx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.tanke756.top/gtarioyboz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yongpay.top/gtfezlmfdf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.tanke756.top/gtczpjhxxc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.52xcode.cn/gthfbdbnhe.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zhoulong.xyz/gtoqzcciji.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.shanyushiyangtech.top/gtpgpiedui.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.andypj.xyz/gtkmbrqsuq.html

[E16] 数字千分位
来源：http://hz.ehwqpu.com/gttdnifzws.html

Py:   f"{1234567:,}"
来源：http://hz.shangyingyoupin.top/gtztsywbto.html

PHP:  number_format(1234567);
来源：http://hz.gzhubu.top/gtuvbuypxa.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ivvv.top/gtbbpkrnay.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yonumen.top/gtlcmbvvpq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.vqdsnc.cn/gtyhvssnsx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.chenzaomai.com/gtozcvxocp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.sysykeji.top/gtrwkfasqe.html

C#:   1234567.ToString("N0")
来源：http://hz.c1oappe.top/gtcfgjqxuz.html

[E17] 首字母大写
来源：http://hz.sxryk.cn/gtksztrgof.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.quarkkingdee.top/gtswbazfsa.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zhaomingkeji.xyz/gthiyuzdbj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.guowangkeji.top/gtgswphxqp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ydzc1.top/gtoscbuldg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yangfankeji.com/gtxdvxrnfq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yvedp.cn/gtvstqhdwx.html

Ruby: s.capitalize
来源：http://hz.fzhhl.top/gtgfazhhnt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yueranfly.top/gtqhkmzvwn.html

[E18] 模板占位符替换
来源：http://hz.zhiwuduotai.top/gtqjfinrtt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.guannengcc.top/gtyjkqihol.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.sweek.top/gtpedqmars.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.zycfv.cn/gtfvwpphwv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.chenjidiqi.icu/gtaftawjoa.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.shanyushiyangtech.top/gtlxqyqlml.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ydzc1.top/gthnbbdzzs.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yuxming.cn/gtayfxzelb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.aizwys.cn/gtyaifepmz.html

[E19] 多行文本按行拆分
来源：http://hz.yongpay.top/gtphztxbuj.html

Py:   s.splitlines()
来源：http://hz.sxryk.cn/gtsllugxat.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.birdmap.top/gtgwbzoyox.html

JS:   s.split(/\r?\n/)
来源：http://hz.daxiang520.top/gtvfhvyytl.html

TS:   s.split(/\r?\n/)
来源：http://hz.yj20258.top/gtqtekmucm.html

Java: s.lines().toList()
来源：http://hz.xylfe.cn/gtrkfujjpm.html

Go:   strings.Split(s, "\n")
来源：http://hz.jlsjyb.cn/gtfvuhpiso.html

Ruby: s.lines
来源：http://hz.snrcjt.cn/gtozffavar.html

C#:   s.Split('\n')
来源：http://hz.zycfv.cn/gtbmvgzrgu.html

[E20] 判断字符串是否为空
来源：http://hz.tianlin.xyz/gteqotcihw.html

Py:   if not s:
来源：http://hz.ivvv.top/gteoabhncs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.c1oappe.top/gtrehhkeyh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.cucudq.cn/gtptrosemc.html

TS:   if (s === "") {}
来源：http://hz.ehwqpu.com/gtifaejppi.html

Java: if (s.isEmpty()) {}
来源：http://hz.cucudq.cn/gtjoxumdcy.html

Go:   if s == "" {}
来源：http://hz.aibaodan.cn/gtydowktgr.html

Ruby: if s.empty?
来源：http://hz.316326.xyz/gtqbqwcbyy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.nanxinkj.top/gtqzvxhqte.html

[E21] 超长截断加省略号
来源：http://hz.hysaishi.cn/gtgrkfbcwb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.pengpengdd.cyou/gtelvicimx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jiagoushi.top/gtuhpwtjdg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.andypj.xyz/gtrgrbelub.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhijiandao.cn/gtemccbzza.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ydzc1.top/gtbirlsdpj.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.wangshuangyany.cn/gtvodmmhys.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jqgufenzy.top/gticoothnc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jyoumei.cn/gtuufapbjo.html

[E22] 字节长度与字符长度
来源：http://hz.redwolf501.top/gttucvmavp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zycfv.cn/gthbglmjou.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhongyouzk.top/gtftpcfdsy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhengqikj.top/gthmezgawi.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jqgufenzy.top/gtiegexadr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.daxiang520.top/gtetvfsmcw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.aibaodan.cn/gtktqecnfr.html

Ruby: s.bytesize;  s.length
来源：http://hz.yangfankeji.com/gtanvuatck.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.aizwys.cn/gtlywtxpal.html

================================================================================
来源：http://hz.xylfe.cn/gtwcqhudgf.html

F. 文件与目录
来源：http://hz.yangfankeji.com/gttwlietsg.html

================================================================================
来源：http://hz.fengsongda.top/gtcxgsvivl.html

[F01] 读取整个文件
来源：http://hz.jlsjyb.cn/gtuzmsmbsb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.xuetiantiany.cn/gtcpagehpk.html

PHP:  file_get_contents("a.txt");
来源：http://hz.ivvv.top/gtiptzfbul.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.9152youxi.cn/gtwxhvbrxt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.vqdsnc.cn/gtfzcafdtv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.cucudq.cn/gtkjcohorl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yongpay.top/gtchizoyza.html

Ruby: File.read("a.txt")
来源：http://hz.ehwqpu.com/gtkwoxgoni.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jqgufenzy.top/gtgtsiucaj.html

[F02] 逐行读取文件
来源：http://hz.redwolf501.top/gthlwucyim.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.tian-w.cn/gtnjhqqhau.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.gzhubu.top/gtrjurizkn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hongshengwenyu.top/gtowdrbiub.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hywenlv.cn/gtkpxagtbn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.redwolf501.top/gtcglvozom.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.fzhhl.top/gtlblxvmfx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.smart0.xyz/gtuuhhyvri.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.cdnleiting.top/gtyrgpgyim.html

[F03] 写入文件（覆盖）
来源：http://hz.hysaishi.cn/gtgediqzqn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.redwolf501.top/gttsnlzmfv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jqgfzy.top/gtzwotonhr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhiwuduotai.top/gtbylrjgoj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xinyue.icu/gtlwhkcuhy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.0kj1m.cn/gtnfddusxf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.nanxuanxn.top/gtmgfcmvjl.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.tianlin.xyz/gtkxpcnhwf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.guannengcc.top/gtykeegbvg.html

[F04] 追加写入文件
来源：http://hz.quarkkingdee.top/gtrxyzbaan.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.0kj1m.cn/gtlosjnlwh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.shuidangran.top/gtxywbscgh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gaohongyu789.top/gtxppmmxxz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.havefunace.top/gtqglqdkuo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.cucudq.cn/gtxhrkaxkp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.wangshuangyany.cn/gtxqcyitiw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.gzhubu.top/gthvmezjir.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.sysykeji.top/gtdpamgyrg.html

[F05] 判断文件或目录是否存在
来源：http://hz.jlsjyb.cn/gtiusmvxoi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.redwolf501.top/gtfknedpko.html

PHP:  file_exists("a.txt");
来源：http://hz.jinghuilouyu.cn/gthpkabxnt.html

JS:   fs.existsSync("a.txt")
来源：http://hz.gzhubu.top/gtjnpvjulj.html

TS:   fs.existsSync("a.txt")
来源：http://hz.wangshuangyany.cn/gtnvnltase.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.cucudq.cn/gtyszjjvbd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yvedp.cn/gtwloybyut.html

Ruby: File.exist?("a.txt")
来源：http://hz.yvedp.cn/gtorouflel.html

C#:   File.Exists("a.txt")
来源：http://hz.quarkkingdee.top/gtzfqigsxo.html

[F06] 删除文件
来源：http://hz.hongshengwenyu.top/gtjtuzxsxx.html

Py:   os.remove("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtncfvkykb.html

PHP:  unlink("a.txt");
来源：http://hz.gotoacloud.top/gtovveznvv.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yanxiufei.cn/gtpnvfpwlo.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.tianlin.xyz/gtdopaicux.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.aibaodan.cn/gtogxfxvvl.html

Go:   os.Remove("a.txt")
来源：http://hz.jyoumei.cn/gtpherodoz.html

Ruby: File.delete("a.txt")
来源：http://hz.9152youxi.cn/gtzwvlfwut.html

C#:   File.Delete("a.txt");
来源：http://hz.316326.xyz/gtxjuuxtuu.html

[F07] 创建目录（含多级）
来源：http://hz.wangdashe.top/gtsdcyranm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.sysykeji.top/gtyihgyzdl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.xuetiantiany.cn/gtozemcqgq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cqqwz.cn/gtqszcakll.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sysykeji.top/gtqwntgysh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.haohaochexian.top/gtebcutjod.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhijiandao.cn/gtyrxxbdza.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jinyuanbaomall.cn/gtqzzwtncl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hnxiangtu.top/gttxlowodx.html

[F08] 遍历目录
来源：http://hz.dashuyun.cn/gtwudwgdvi.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.316326.xyz/gtwibcrvjg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.chenjidiqi.icu/gtlfaogvql.html

JS:   fs.readdirSync("dir")
来源：http://hz.jinyuanbaomall.cn/gtxmokxylw.html

TS:   fs.readdirSync("dir")
来源：http://hz.cashguo.top/gtjvpzpczj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.snrcjt.cn/gtfdxvxmvi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.sysykeji.top/gtnpanwxzi.html

Ruby: Dir.children("dir")
来源：http://hz.hnqzz.top/gtkcvjcutg.html

C#:   Directory.GetFiles("dir")
来源：http://hz.smart0.xyz/gtbdimcydg.html

[F09] 获取文件大小
来源：http://hz.daxiang520.top/gtyiyxkely.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cdnleiting.top/gtdvtqlkcv.html

PHP:  filesize("a.txt");
来源：http://hz.cqqwz.cn/gtbazsvkqc.html

JS:   fs.statSync("a.txt").size
来源：http://hz.cashguo.top/gtqkxrreaj.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ivvv.top/gtqoshuiji.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.sysykeji.top/gtuifnjfzl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.cqqwz.cn/gtomjceesb.html

Ruby: File.size("a.txt")
来源：http://hz.bjfxy.top/gtnaunmxfm.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jqgfzy.top/gtyulnzkfn.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yj20258.top/gtjbwhbxsa.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.sufxvd.cn/gtrwdpnjgj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.cqqwz.cn/gtegdbpdpk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hnqzz.top/gtjwtgyjvz.html

TS:   path.extname("a.txt")
来源：http://hz.wangshuangyany.cn/gttqpdsqst.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hfpthk.cn/gtxofowbut.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.gzhubu.top/gttcgovwgq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jlsjyb.cn/gtjahvockx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.guannengcc.top/gtqdvvqona.html

[F11] 复制与移动文件
来源：http://hz.hfpthk.cn/gtdhsqikoc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yuanzhike.top/gtecelxdpt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yanxiufei.cn/gthpkoibys.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.birdmap.top/gtodtmokcy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sufxvd.cn/gtcvukeibi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ywan-chungtsiang.top/gtfliinpor.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.aizwys.cn/gthozzslac.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jqgfzy.top/gtajdgkzfc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.cqqwz.cn/gtqfqtcbxb.html

[F12] CSV 读写
来源：http://hz.nwbrower.top/gtqndhsgjx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.tanke756.top/gtkjwghdnp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yuxming.cn/gtajwdutnt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yangfankeji.com/gtbgvqlgfj.html

TS:   // 同上
来源：http://hz.jyoumei.cn/gttimwofxs.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.sxryk.cn/gtlvfeggnd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.fzhhl.top/gtytndiskq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.52xcode.cn/gtcirnzasy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.andypj.xyz/gtrxckavcv.html

================================================================================
来源：http://hz.zhongyouzk.top/gttfzcpmsh.html

G. 面向对象
来源：http://hz.feifeiyinyue.top/gttwwfzvdm.html

================================================================================
来源：http://hz.jiagoushi.top/gtrtktvdgn.html

[G01] 定义类
来源：http://hz.hywenlv.cn/gtudnrcooa.html

Py:   class User: pass
来源：http://hz.havefunace.top/gtufglgrsz.html

PHP:  class User {}
来源：http://hz.quarkkingdee.top/gtabudbgni.html

JS:   class User {}
来源：http://hz.yj20258.top/gtkfxlbwfc.html

TS:   class User { name: string = ""; }
来源：http://hz.52xcode.cn/gtfyczclhw.html

Java: class User {}
来源：http://hz.shanyushiyangkeji.top/gtvcyvrerl.html

Go:   type User struct { Name string }
来源：http://hz.yongpay.top/gtaynkhsiu.html

Ruby: class User; end
来源：http://hz.316326.xyz/gtllpgbrxw.html

C#:   class User {}
来源：http://hz.cashguo.top/gtoofaibpe.html

[G02] 构造函数
来源：http://hz.havefunace.top/gtojzfexli.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jinghuilouyu.cn/gtsjpyhffg.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.bjfxy.top/gthfhrmlzd.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xylfe.cn/gtvjwtttkh.html

TS:   constructor(public name: string) {}
来源：http://hz.ybcxt.top/gtubrvcbmf.html

Java: User(String name) { this.name = name; }
来源：http://hz.fengsongda.top/gtjqkzopap.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zdqjudy.top/gtwniahhve.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zhengqikj.top/gtkkqaocdg.html

C#:   public User(string name) { Name = name; }
来源：http://hz.havefunace.top/gtbzjdsscj.html

[G03] 实例属性
来源：http://hz.9152youxi.cn/gtmrrlwcpn.html

Py:   self.name = "x"
来源：http://hz.yueranfly.top/gtakyvprbc.html

PHP:  public string $name = "x";
来源：http://hz.yueranfly.top/gtbyskyddh.html

JS:   this.name = "x";
来源：http://hz.xziqi.cn/gtwjiamcov.html

TS:   name: string = "x";
来源：http://hz.gogol.net.cn/gtgldsetvb.html

Java: private String name;
来源：http://hz.gotoacloud.top/gtaphcfoiy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ppjwa.cn/gtxvoawbfw.html

Ruby: @name = "x"
来源：http://hz.wangshuangyany.cn/gtsopruwgh.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cdnleiting.top/gtvjuyoxfm.html

[G04] 定义方法
来源：http://hz.jqgfzy.top/gtatusivyd.html

Py:   def greet(self): return self.name
来源：http://hz.pengpengdd.cyou/gtyyekdqfp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zycfv.cn/gtjfzzrwdp.html

JS:   greet() { return this.name; }
来源：http://hz.yuanzhike.top/gtxanozymq.html

TS:   greet(): string { return this.name; }
来源：http://hz.tian-w.cn/gtictjujvg.html

Java: String greet() { return name; }
来源：http://hz.shangyingyoupin.top/gtyjcgloxd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ehwqpu.com/gtudrspopx.html

Ruby: def greet; @name; end
来源：http://hz.xylfe.cn/gttqsxrqhn.html

C#:   public string Greet() => Name;
来源：http://hz.jiagoushi.top/gtxnkahuic.html

[G05] 继承
来源：http://hz.cashguo.top/gtgfztaumm.html

Py:   class Admin(User): pass
来源：http://hz.cheryme.top/gttamoobfl.html

PHP:  class Admin extends User {}
来源：http://hz.cucudq.cn/gtvnrirygc.html

JS:   class Admin extends User {}
来源：http://hz.pengpengdd.cyou/gtgunzgrdf.html

TS:   class Admin extends User {}
来源：http://hz.guowangkeji.top/gtsytnknic.html

Java: class Admin extends User {}
来源：http://hz.yangfankeji.com/gtywgeiwci.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.gzhubu.top/gtfrvfhdle.html

Ruby: class Admin < User; end
来源：http://hz.yj20258888.top/gtfhdcmxhm.html

C#:   class Admin : User {}
来源：http://hz.zhengqikj.top/gtzmhllboq.html

[G06] 重写方法
来源：http://hz.kuanghao11.cn/gtkcylyhbj.html

Py:   def greet(self): return "admin"
来源：http://hz.zycfv.cn/gtgucuvvqk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.pengpengdd.cyou/gtfpadsiyp.html

JS:   greet() { return "admin"; }
来源：http://hz.tianlin.xyz/gtfbjweans.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhengqikj.top/gtuvmqhcmt.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.cheryme.top/gtixwqelyn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.chenzaomai.com/gtszkvnnug.html

Ruby: def greet; "admin"; end
来源：http://hz.guowangkeji.top/gtpgaiepol.html

C#:   public override string Greet() => "admin";
来源：http://hz.jinqigufen.top/gtzlfwjbfr.html

[G07] 调用父类方法
来源：http://hz.hammf.cn/gtbqdmikiz.html

Py:   super().greet()
来源：http://hz.dashuyun.cn/gtnwsxlqcl.html

PHP:  parent::greet();
来源：http://hz.zycfv.cn/gtiqwwiqcr.html

JS:   super.greet();
来源：http://hz.guannengcc.top/gttwghekat.html

TS:   super.greet();
来源：http://hz.yuxming.cn/gtejiiskat.html

Java: super.greet();
来源：http://hz.jlsjyb.cn/gtgdeqqsde.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yj202588.top/gtxogjlidn.html

Ruby: super
来源：http://hz.aizwys.cn/gttoklonmd.html

C#:   base.Greet();
来源：http://hz.nanxinkj.top/gtxfcudggi.html

[G08] 静态方法与属性
来源：http://hz.yanxiufei.cn/gtcljrugtg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.shuidangran.top/gtkyvaxpyu.html

PHP:  public static function f() {}
来源：http://hz.svipenyu.cn/gtyaxaizug.html

JS:   static f() {}
来源：http://hz.zhongyouzk.top/gtkaghibxu.html

TS:   static f(): void {}
来源：http://hz.tanke756.top/gtzuutdghx.html

Java: static void f() {}
来源：http://hz.xinyue.icu/gtyflavreh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.tian-w.cn/gturmtbutn.html

Ruby: def self.f; end
来源：http://hz.cashguo.top/gtljorhwbb.html

C#:   public static void F() {}
来源：http://hz.dianchejie.cn/gtvoqcxqfg.html

[G09] 接口 / 抽象类
来源：http://hz.chenjidiqi.icu/gtjxdcdkvm.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.kuanghao11.cn/gtifuaoldt.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.316326.xyz/gtkfcsxeuq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yj202588.top/gtwiaxkzkq.html

TS:   interface Shape { area(): number; }
来源：http://hz.shangyingyoupin.top/gtdibvbbco.html

Java: interface Shape { double area(); }
来源：http://hz.sysykeji.top/gtehpmytox.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.dianchejie.cn/gtrwpbsgxr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jqgufenzy.top/gtplyjfveg.html

C#:   interface IShape { double Area(); }
来源：http://hz.tianlin.xyz/gtnntqryce.html


<!-- 参考信息 -->