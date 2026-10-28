代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.aizwys.cn/gtfarfnfmx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jinqigufen.top/gtuwuarmlv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.ydzc1.top/gtohqwwhix.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.ppjwa.cn/gtspuscrug.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ydjk.org.cn/gtifygomiy.html

[E15] HTML 转义 / 反转义
来源：http://hz.jyoumei.cn/gtmprctbmv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.daxiang520.top/gtvrsxrvid.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.cashguo.top/gtwzqwfcsd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.xuetiantiany.cn/gtjdnthqqi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.gaohongyu789.top/gtecneceun.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.xinyue.icu/gtzklbliky.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hnxiangtu.top/gtyzwadxsz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.52xcode.cn/gtbbemfnjf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zdqjudy.top/gtxohfbjum.html

[E16] 数字千分位
来源：http://hz.yj20258.top/gtmhyecpar.html

Py:   f"{1234567:,}"
来源：http://hz.ivvv.top/gtnwjykaai.html

PHP:  number_format(1234567);
来源：http://hz.9152youxi.cn/gtfoaogqir.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.daria6918.cn/gtlmvezabg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ydjk.org.cn/gtqaibpqgm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.xziqi.cn/gteqyrdqlc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yvedp.cn/gtravxdtky.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jqgufenzy.top/gtmncilndb.html

C#:   1234567.ToString("N0")
来源：http://hz.cdnleiting.top/gtcjgkfnbw.html

[E17] 首字母大写
来源：http://hz.zhijiandao.cn/gtodcallop.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.cqqwz.cn/gtrqywnplg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.dianchejie.cn/gtjaaqomch.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.wangshuangyany.cn/gtfkipactp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhiwuduotai.top/gtigiwijfr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.hfpthk.cn/gtvorrexwz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.daria6918.cn/gtchjwbkfl.html

Ruby: s.capitalize
来源：http://hz.yonumen.top/gtdtbpffaw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zhaomingkeji.xyz/gtduxfcirm.html

[E18] 模板占位符替换
来源：http://hz.mhx1999.top/gtlnxqvnlm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.daxiang520.top/gtqdunyznp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zhengqikj.top/gtqjhbgmrj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.xuetiantiany.cn/gtzsbxkmkr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.cheryme.top/gtddkmnael.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.dashuyun.cn/gtqbotegmk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ivvv.top/gtmoowxxdg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yuanzhike.top/gthtwwezcr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.sweek.top/gtibivfsom.html

[E19] 多行文本按行拆分
来源：http://hz.hywenlv.cn/gtnaoktkcr.html

Py:   s.splitlines()
来源：http://hz.bjfxy.top/gtbgyuwrzv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.guannengcc.top/gtvbeovxsf.html

JS:   s.split(/\r?\n/)
来源：http://hz.jinqigfzy.top/gtwelohyxm.html

TS:   s.split(/\r?\n/)
来源：http://hz.ivvv.top/gtzgrafepo.html

Java: s.lines().toList()
来源：http://hz.hammf.cn/gtwcgpkpwz.html

Go:   strings.Split(s, "\n")
来源：http://hz.haohaochexian.top/gtcpmtrguj.html

Ruby: s.lines
来源：http://hz.guannengcc.top/gtpziaqnuy.html

C#:   s.Split('\n')
来源：http://hz.yangfankeji.com/gtyinixjzl.html

[E20] 判断字符串是否为空
来源：http://hz.kuanghao11.cn/gtlubhfjuy.html

Py:   if not s:
来源：http://hz.ivvv.top/gttmijvzxt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.xuanzx.com/gtbdfaukve.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zhongyouzk.top/gtrqyjtupo.html

TS:   if (s === "") {}
来源：http://hz.zhaomingkeji.xyz/gtpzcdgvab.html

Java: if (s.isEmpty()) {}
来源：http://hz.zdqjudy.top/gtdymuaram.html

Go:   if s == "" {}
来源：http://hz.pycfn.com/gtkcmffmnu.html

Ruby: if s.empty?
来源：http://hz.jqgfzy.top/gtocbwjlpq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zhengqikj.top/gtfsalmbvf.html

[E21] 超长截断加省略号
来源：http://hz.bjfxy.top/gtdmskgoeq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jianghu66.top/gttphefvby.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhoulong.xyz/gtkqmwafrs.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.daxiang520.top/gtxmlecobp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.daria6918.cn/gtocwzglrv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.tian-w.cn/gtofmpcabs.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.nwbrower.top/gtcuijilwj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.gaohongyu789.top/gtbkhuyipy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jianghu66.top/gtgidxhusc.html

[E22] 字节长度与字符长度
来源：http://hz.jinghuilouyu.cn/gtbfkutoed.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.pengpengdd.cyou/gtyfpwbdqn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.gotoacloud.top/gthgkaesmc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.svipenyu.cn/gttiqiuris.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ppjwa.cn/gtxpsuswkd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yangfankeji.com/gtxyarfsyy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.cqqwz.cn/gtfqzwacrk.html

Ruby: s.bytesize;  s.length
来源：http://hz.ydjk.org.cn/gttpurjlik.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.wangdashe.top/gtruxwhopb.html

================================================================================
来源：http://hz.fengsongda.top/gtjnpvwwbw.html

F. 文件与目录
来源：http://hz.zdqjudy.top/gtmlmjdsnk.html

================================================================================
来源：http://hz.snrcjt.cn/gtacevexxk.html

[F01] 读取整个文件
来源：http://hz.zhoulong.xyz/gtdporrxze.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.chenjidiqi.icu/gtlrdafmwm.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jinqigufen.top/gtsrdvsoqt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.xylfe.cn/gtcyonuvsl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.cqqwz.cn/gtgdorbrtn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.xingfuxueyuan.xyz/gtppqbeivw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jqgfzy.top/gthatljere.html

Ruby: File.read("a.txt")
来源：http://hz.yuanzhike.top/gtopvowogh.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hnqzz.top/gtqnpecjjb.html

[F02] 逐行读取文件
来源：http://hz.gzhubu.top/gtuywpoodm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jqgufenzy.top/gtdmazpxdi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.gzhubu.top/gtflpoenaq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.bjfxy.top/gtoqqkarbi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.tianlin.xyz/gtmktwutho.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yueranfly.top/gtlaeqcogr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.iojbl.cn/gtgwjjuclb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hnqzz.top/gtfahicchy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.cucudq.cn/gtoxzjfdfp.html

[F03] 写入文件（覆盖）
来源：http://hz.zhixingplan.top/gtgeknlfcq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hongshengwenyu.top/gtdftfrows.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.aibaodan.cn/gtavbxnstc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.quarkkingdee.top/gtnivksqkl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.bjfxy.top/gtvpdqfnmo.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.daria6918.cn/gtmvsjytor.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.shuidangran.top/gtqqbpnlol.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hnqzz.top/gtiniyrabj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yj20258888.top/gtvsfzvzhu.html

[F04] 追加写入文件
来源：http://hz.cucudq.cn/gtyihgtskl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zdqjudy.top/gttqqtmnlg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhoulong.xyz/gtccmjalfz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jianghu66.top/gtgdxkvocz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhoulong.xyz/gteqnxscau.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.aibaodan.cn/gtzxlslrgo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zhongyouzk.top/gtwsubdvwk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jqgfzy.top/gthiypypou.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.sweek.top/gtwnhgntdb.html

[F05] 判断文件或目录是否存在
来源：http://hz.fzhhl.top/gtawmigmrp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shanyushiyangkeji.top/gtignfivud.html

PHP:  file_exists("a.txt");
来源：http://hz.snrcjt.cn/gtscjvtgkp.html

JS:   fs.existsSync("a.txt")
来源：http://hz.sweek.top/gttpelxfcz.html

TS:   fs.existsSync("a.txt")
来源：http://hz.gotoacloud.top/gtpxlakdhq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.wangshuangyany.cn/gtnsvtkfik.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jqgfzy.top/gtwlimjkag.html

Ruby: File.exist?("a.txt")
来源：http://hz.yangfankeji.com/gtcfqabwcz.html

C#:   File.Exists("a.txt")
来源：http://hz.sxryk.cn/gtjypopjcz.html

[F06] 删除文件
来源：http://hz.snrcjt.cn/gtpzlsguiu.html

Py:   os.remove("a.txt")
来源：http://hz.jiagoushi.top/gtmghfllcu.html

PHP:  unlink("a.txt");
来源：http://hz.pengpengdd.cyou/gtncuuhubx.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.chenzaomai.com/gtcreqaatt.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.guannengcc.top/gtgocputzr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yangfankeji.com/gtzzoqmgkl.html

Go:   os.Remove("a.txt")
来源：http://hz.ybcxt.top/gtcbspqzrg.html

Ruby: File.delete("a.txt")
来源：http://hz.jinghuilouyu.cn/gtptbsuvhu.html

C#:   File.Delete("a.txt");
来源：http://hz.guowangkeji.top/gtiahmoyzp.html

[F07] 创建目录（含多级）
来源：http://hz.feifeiyinyue.top/gtahgiozhe.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hammf.cn/gtobnenret.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ivvv.top/gtocbwvwnv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.tanke756.top/gtzfqmptmp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.chenjidiqi.icu/gtrerybcax.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jianghu66.top/gtidjuynmz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jlsjyb.cn/gtpdyhgeen.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.xuanzx.com/gtpqvlkqdj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.9152youxi.cn/gtovykgdiq.html

[F08] 遍历目录
来源：http://hz.jinqigufen.top/gtewjcmxfx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhijiandao.cn/gtjfhyotei.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.ydzc1.top/gtyofrepxu.html

JS:   fs.readdirSync("dir")
来源：http://hz.yonumen.top/gtpsvxrdaf.html

TS:   fs.readdirSync("dir")
来源：http://hz.xuanzx.com/gtubtqtggb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.smart0.xyz/gtnkbxgpow.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.wangdashe.top/gtdmgzylzu.html

Ruby: Dir.children("dir")
来源：http://hz.c1oappe.top/gtrdfikrbo.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yuanzhike.top/gtadaehsuy.html

[F09] 获取文件大小
来源：http://hz.jinqigufen.top/gtboicubuw.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hnxiangtu.top/gthoxbrydt.html

PHP:  filesize("a.txt");
来源：http://hz.tian-w.cn/gtinklbtow.html

JS:   fs.statSync("a.txt").size
来源：http://hz.cashguo.top/gtylicmxgi.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ydjk.org.cn/gthdwldgsf.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.daria6918.cn/gttxhuqugx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.mhx1999.top/gtieviltnb.html

Ruby: File.size("a.txt")
来源：http://hz.tianlin.xyz/gtnfcvogqx.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.cheryme.top/gthvtfhjxe.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hysaishi.cn/gtauvblfab.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jinqigufen.top/gturytafus.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.shuidangran.top/gtsfilkehp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.chenlongwang.top/gtvvayadnw.html

TS:   path.extname("a.txt")
来源：http://hz.mhx1999.top/gtjnarzbwg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jinghuilouyu.cn/gtffmgzcpo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yonumen.top/gtluzenbwa.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ivvv.top/gtpbrhhiif.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.daria6918.cn/gtpsrbxjdz.html

[F11] 复制与移动文件
来源：http://hz.9152youxi.cn/gtauiavqse.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zhongyouzk.top/gtfcoofgkj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.fzhhl.top/gtzlsnysof.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gogol.net.cn/gtmhuujhan.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.tianlin.xyz/gtlcmaxvhx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yj202588.top/gtzisxzofj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.havefunace.top/gtfwbvjfnm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zhengqikj.top/gteqksfmyz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhongyouzk.top/gtzufodehh.html

[F12] CSV 读写
来源：http://hz.zhijiandao.cn/gtoucuioxe.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.andypj.xyz/gtdsnyrblz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.wangdashe.top/gtjfbfnzen.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.cheryme.top/gtcgwpmsyz.html

TS:   // 同上
来源：http://hz.yonumen.top/gtybixejsu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.gogol.net.cn/gtqjwmljel.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jinqigufen.top/gtocjikppx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jianghu66.top/gtsvrwoeif.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yanxiufei.cn/gtbboxaorb.html

================================================================================
来源：http://hz.c1oappe.top/gtqbykivfn.html

G. 面向对象
来源：http://hz.jinyuanbaomall.cn/gtvtjlwkvy.html

================================================================================
来源：http://hz.cqqwz.cn/gtssdjbupk.html

[G01] 定义类
来源：http://hz.ydjk.org.cn/gtztrtsfnz.html

Py:   class User: pass
来源：http://hz.xziqi.cn/gtuarwlaud.html

PHP:  class User {}
来源：http://hz.hammf.cn/gtskqittjg.html

JS:   class User {}
来源：http://hz.quarkkingdee.top/gtaewlxfao.html

TS:   class User { name: string = ""; }
来源：http://hz.ppjwa.cn/gthjotvcnp.html

Java: class User {}
来源：http://hz.jiagoushi.top/gtaqfhmzor.html

Go:   type User struct { Name string }
来源：http://hz.iojbl.cn/gtmgqsgpkm.html

Ruby: class User; end
来源：http://hz.hongshengwenyu.top/gtioomrbhk.html

C#:   class User {}
来源：http://hz.haohaochexian.top/gtzcyeerte.html

[G02] 构造函数
来源：http://hz.ywan-chungtsiang.top/gtumvzrjbd.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jinghuilouyu.cn/gtgfzyglld.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jiagoushi.top/gtstloofde.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.chenlongwang.top/gtechkuhda.html

TS:   constructor(public name: string) {}
来源：http://hz.xylfe.cn/gthdrabzpj.html

Java: User(String name) { this.name = name; }
来源：http://hz.fzhhl.top/gtrchmvwuc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zhongyouzk.top/gtvagiltdb.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.aizwys.cn/gtconqtbqd.html

C#:   public User(string name) { Name = name; }
来源：http://hz.havefunace.top/gtygvetaax.html

[G03] 实例属性
来源：http://hz.guannengcc.top/gtbyynjyhq.html

Py:   self.name = "x"
来源：http://hz.xylfe.cn/gtpjzhjxew.html

PHP:  public string $name = "x";
来源：http://hz.tianlin.xyz/gtnjznmujq.html

JS:   this.name = "x";
来源：http://hz.pycfn.com/gtnxhcwfxz.html

TS:   name: string = "x";
来源：http://hz.jiagoushi.top/gtoxlixzkf.html

Java: private String name;
来源：http://hz.yanxiufei.cn/gtyzjvropw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jianghu66.top/gtulmjejlk.html

Ruby: @name = "x"
来源：http://hz.zycfv.cn/gtblkarapf.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.0kj1m.cn/gtzdcnahmu.html

[G04] 定义方法
来源：http://hz.yonumen.top/gtdbiyglvx.html

Py:   def greet(self): return self.name
来源：http://hz.xuetiantiany.cn/gtiszcivwm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.aibaodan.cn/gtwqgntgwb.html

JS:   greet() { return this.name; }
来源：http://hz.sufxvd.cn/gtcwrbgmqs.html

TS:   greet(): string { return this.name; }
来源：http://hz.ywan-chungtsiang.top/gtqopqfkwr.html

Java: String greet() { return name; }
来源：http://hz.yonumen.top/gtarbxjllu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.nwbrower.top/gtmfoswdrh.html

Ruby: def greet; @name; end
来源：http://hz.shzxlz.cn/gtbnbgllkv.html

C#:   public string Greet() => Name;
来源：http://hz.jinyuanbaomall.cn/gtzlzwrrhe.html

[G05] 继承
来源：http://hz.0kj1m.cn/gtdzgakaxe.html

Py:   class Admin(User): pass
来源：http://hz.zhoulong.xyz/gtkhqrqukx.html

PHP:  class Admin extends User {}
来源：http://hz.ehwqpu.com/gtydfwspwl.html

JS:   class Admin extends User {}
来源：http://hz.cdnleiting.top/gtrulbqdna.html

TS:   class Admin extends User {}
来源：http://hz.jyoumei.cn/gttzqjxnzk.html

Java: class Admin extends User {}
来源：http://hz.jinyuanbaomall.cn/gtnbfxhmga.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.fzhhl.top/gtutnisdup.html

Ruby: class Admin < User; end
来源：http://hz.guannengcc.top/gtxvjapqpm.html

C#:   class Admin : User {}
来源：http://hz.tian-w.cn/gtnjaiucyq.html

[G06] 重写方法
来源：http://hz.yueranfly.top/gtdxpdjvxj.html

Py:   def greet(self): return "admin"
来源：http://hz.cqqwz.cn/gthzfdnbke.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yanxiufei.cn/gtznegcaia.html

JS:   greet() { return "admin"; }
来源：http://hz.dashuyun.cn/gtkeywdiyq.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jinqigufen.top/gtxmigchot.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.chenzaomai.com/gtsciejmjf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ydjk.org.cn/gthihmiyla.html

Ruby: def greet; "admin"; end
来源：http://hz.zycfv.cn/gtuiazvfpv.html

C#:   public override string Greet() => "admin";
来源：http://hz.snrcjt.cn/gtswdmykya.html

[G07] 调用父类方法
来源：http://hz.cqqwz.cn/gtrekgfinx.html

Py:   super().greet()
来源：http://hz.vqdsnc.cn/gtzegxqqan.html

PHP:  parent::greet();
来源：http://hz.9152youxi.cn/gteblujkyl.html

JS:   super.greet();
来源：http://hz.sufxvd.cn/gtzolxlqip.html

TS:   super.greet();
来源：http://hz.yangfankeji.com/gttxvnvpyz.html

Java: super.greet();
来源：http://hz.birdmap.top/gtbrspfhwk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.redwolf501.top/gtetebnhwq.html

Ruby: super
来源：http://hz.yonumen.top/gtdvmhfcjd.html

C#:   base.Greet();
来源：http://hz.316326.xyz/gtwubokjlq.html

[G08] 静态方法与属性
来源：http://hz.jinyuanbaomall.cn/gtjcqfggpm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.gotoacloud.top/gtgorladkl.html

PHP:  public static function f() {}
来源：http://hz.zhijiandao.cn/gtejtxaulo.html

JS:   static f() {}
来源：http://hz.zhiwuduotai.top/gtsnhxzdgd.html

TS:   static f(): void {}
来源：http://hz.vqdsnc.cn/gtwcpcffmd.html

Java: static void f() {}
来源：http://hz.yj20258888.top/gtggliazqx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.ydzc1.top/gtxumbuvte.html

Ruby: def self.f; end
来源：http://hz.xinyue.icu/gttgaidawb.html

C#:   public static void F() {}
来源：http://hz.zhaomingkeji.xyz/gtocujajnk.html

[G09] 接口 / 抽象类
来源：http://hz.jinghuilouyu.cn/gtcbrlqbao.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.haohaochexian.top/gtqgfjioty.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.pengpengdd.cyou/gtahwncire.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.quarkkingdee.top/gthwcdbjof.html

TS:   interface Shape { area(): number; }
来源：http://hz.zhixingplan.top/gtkvlewdzx.html

Java: interface Shape { double area(); }
来源：http://hz.ppjwa.cn/gtjpwyymjz.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.fzhhl.top/gtrpncmqgr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.aizwys.cn/gtnccntyss.html

C#:   interface IShape { double Area(); }
来源：http://hz.wangshuangyany.cn/gtofaqqvup.html

[G10] 访问控制
来源：http://hz.jiagoushi.top/gtyeambikz.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.gotoacloud.top/gtqmzchhov.html

PHP:  public / protected / private
来源：http://hz.9152youxi.cn/gtjzvdglby.html

JS:   #private 字段；其余公开
来源：http://hz.52xcode.cn/gtkdetzwmj.html

TS:   public / protected / private
来源：http://hz.chenlongwang.top/gtlorhidbo.html

Java: public / protected / private / 默认包级
来源：http://hz.dashuyun.cn/gtuhidzcbf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.aibaodan.cn/gtnrldspum.html

Ruby: public / protected / private
来源：http://hz.tanke756.top/gtdqojklsi.html

C#:   public / protected / private / internal
来源：http://hz.jiagoushi.top/gtkrewobmy.html

[G11] getter / setter
来源：http://hz.ppjwa.cn/gthyqyqsjk.html

Py:   @property 与 @x.setter
来源：http://hz.yj202588.top/gtskkleroy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yj20258888.top/gtxcnyhyiy.html

JS:   get name() { return this._name; }
来源：http://hz.sufxvd.cn/gtzmuiyiiv.html

TS:   get name(): string { return this._name; }
来源：http://hz.ywan-chungtsiang.top/gtpudhmwki.html

Java: public String getName() { return name; }
来源：http://hz.chenjidiqi.icu/gtokqlkegn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.shuidangran.top/gtwfgpczxt.html

Ruby: attr_accessor :name
来源：http://hz.chenlongwang.top/gtgiwyyjvt.html

C#:   public string Name { get; set; }
来源：http://hz.zhiwuduotai.top/gtfjdoqkhn.html

[G12] 对象转字符串
来源：http://hz.zhiwuduotai.top/gtwdxtmmzq.html

Py:   def __str__(self): return self.name
来源：http://hz.tianlin.xyz/gttnprndig.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.meibo888.top/gtpyqaxcpm.html

JS:   toString() { return this.name; }
来源：http://hz.gogol.net.cn/gtgvhflorv.html

TS:   toString(): string { return this.name; }
来源：http://hz.zycfv.cn/gtbipjtojn.html

Java: @Override public String toString() { return name; }
来源：http://hz.fengsongda.top/gtubonsmny.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yj202588.top/gtaputhiyl.html

Ruby: def to_s; @name; end
来源：http://hz.zhaomingkeji.xyz/gtvsnoihcx.html

C#:   public override string ToString() => Name;
来源：http://hz.haohaochexian.top/gtuyeirrmd.html

[G13] 判断对象类型
来源：http://hz.birdmap.top/gtsmzhrgza.html


<!-- 参考信息 -->