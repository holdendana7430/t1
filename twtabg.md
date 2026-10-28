代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zhoulong.xyz/gtinfkvyus.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.xinyue.icu/gtghkwmwkf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.fzhhl.top/gttjesihqm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.shzxlz.cn/gtawfgqlmr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.xziqi.cn/gtxxwiotvw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.hnxiangtu.top/gteptgeglz.html

[E16] 数字千分位
来源：http://hz.aizwys.cn/gtuykcxpvw.html

Py:   f"{1234567:,}"
来源：http://hz.jlsjyb.cn/gtyxrjlzyo.html

PHP:  number_format(1234567);
来源：http://hz.feifeiyinyue.top/gtxcxiyosh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ybcxt.top/gtewwyjegt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.iojbl.cn/gtllpymvjq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.c1oappe.top/gtvpqfrkwq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ydjk.org.cn/gtqkfehxkl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.cheryme.top/gtqhomhsai.html

C#:   1234567.ToString("N0")
来源：http://hz.yuxming.cn/gtmijdxlzi.html

[E17] 首字母大写
来源：http://hz.pengpengdd.cyou/gtpjisbntk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.gogol.net.cn/gtrxavnxov.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.316326.xyz/gtqbxhizyq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xingfuxueyuan.xyz/gtpubwxizd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sxryk.cn/gtakrliviu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.daxiang520.top/gttwivroam.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.havefunace.top/gtbnljcolv.html

Ruby: s.capitalize
来源：http://hz.jlsjyb.cn/gtsrfyskiv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.gaohongyu789.top/gtdqonptjf.html

[E18] 模板占位符替换
来源：http://hz.shangyingyoupin.top/gttbmcjxnw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jinyuanbaomall.cn/gthdngochv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.feifeiyinyue.top/gtdnggvtke.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.sufxvd.cn/gtzpvvkmdm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zdqjudy.top/gtzutjqoyu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.daxiang520.top/gtznizjmaz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.vqdsnc.cn/gtexnzkwjr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.redwolf501.top/gtvdetjsrx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yanxiufei.cn/gtjgnddcsj.html

[E19] 多行文本按行拆分
来源：http://hz.xziqi.cn/gtbdztgruk.html

Py:   s.splitlines()
来源：http://hz.jinghuilouyu.cn/gtekolejog.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.dianchejie.cn/gtewfyknft.html

JS:   s.split(/\r?\n/)
来源：http://hz.daxiang520.top/gteykrjsfx.html

TS:   s.split(/\r?\n/)
来源：http://hz.snrcjt.cn/gtrmhnwxfs.html

Java: s.lines().toList()
来源：http://hz.nanxinkj.top/gtnuyycmiv.html

Go:   strings.Split(s, "\n")
来源：http://hz.wangdashe.top/gtiofdmbnu.html

Ruby: s.lines
来源：http://hz.svipenyu.cn/gtsudlccln.html

C#:   s.Split('\n')
来源：http://hz.gaohongyu789.top/gtxalfiqeb.html

[E20] 判断字符串是否为空
来源：http://hz.iojbl.cn/gtijwvsjpk.html

Py:   if not s:
来源：http://hz.andypj.xyz/gtxamutllv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.hywenlv.cn/gtawlmkwtq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yonumen.top/gtkiykykku.html

TS:   if (s === "") {}
来源：http://hz.yonumen.top/gttmrojlwy.html

Java: if (s.isEmpty()) {}
来源：http://hz.shanyushiyangtech.top/gtciukjreu.html

Go:   if s == "" {}
来源：http://hz.52xcode.cn/gtcvpbpqrq.html

Ruby: if s.empty?
来源：http://hz.birdmap.top/gtsjsgbxuh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.dashuyun.cn/gtltwzighj.html

[E21] 超长截断加省略号
来源：http://hz.yuanzhike.top/gtbveiphel.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.iojbl.cn/gthicvxnta.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.cucudq.cn/gtmqaufnqh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yvedp.cn/gtumrukqgf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.fzhhl.top/gtczvumdkp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.daxiang520.top/gtobqxlmrq.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.cucudq.cn/gtlkqwxyuh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.quarkkingdee.top/gtdojixoyr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yvedp.cn/gtptiltkfj.html

[E22] 字节长度与字符长度
来源：http://hz.quarkkingdee.top/gtphlrjdni.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jlsjyb.cn/gtfsihpgax.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.c1oappe.top/gtulntfjsz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.mhx1999.top/gtdajrxixd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yuxming.cn/gtmquejovi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.cucudq.cn/gtgxnfszvw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.guowangkeji.top/gtbrlhrgde.html

Ruby: s.bytesize;  s.length
来源：http://hz.havefunace.top/gtnebtrtms.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.c1oappe.top/gtihxgzlbs.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtxujbgqvx.html

F. 文件与目录
来源：http://hz.tian-w.cn/gtdqzehequ.html

================================================================================
来源：http://hz.mhx1999.top/gtnmdkhxxd.html

[F01] 读取整个文件
来源：http://hz.aizwys.cn/gtououvyru.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jqgufenzy.top/gtkzprvkut.html

PHP:  file_get_contents("a.txt");
来源：http://hz.9152youxi.cn/gthzlojstm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zhoulong.xyz/gtqfsrmifa.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yanxiufei.cn/gtbrdpttmp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhiwuduotai.top/gtdaufsrbi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.daria6918.cn/gtqwvwwsqe.html

Ruby: File.read("a.txt")
来源：http://hz.nanxinkj.top/gtpfrijjgd.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jianghu66.top/gtrscrnlqr.html

[F02] 逐行读取文件
来源：http://hz.vqdsnc.cn/gtccxtvblh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ivvv.top/gtjqcbzvoz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.quarkkingdee.top/gtwuirtasz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hywenlv.cn/gtfhwyuiwi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.fzhhl.top/gtnbrfnann.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.snrcjt.cn/gtpbmqvsed.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.shuidangran.top/gtrhkcvvxo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.wangdashe.top/gtugtfxzvd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.meibo888.top/gtjeiqderu.html

[F03] 写入文件（覆盖）
来源：http://hz.tanke756.top/gtibzmfcfj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jqgufenzy.top/gtjsfqjsqe.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.redwolf501.top/gtckpnenid.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yuxming.cn/gtymyehdyo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.chenlongwang.top/gttkgoyehp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.nanxuanxn.top/gtscrqwsdg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.bjfxy.top/gtqnwmzudw.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hywenlv.cn/gtmhrcvrqk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.xingfuxueyuan.xyz/gtuqviykzt.html

[F04] 追加写入文件
来源：http://hz.meibo888.top/gtxucqqiut.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jyoumei.cn/gteznmkhwx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yuxming.cn/gtvdmrvzhx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ydjk.org.cn/gtjqnlaezz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ehwqpu.com/gtruxgtcye.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yuxming.cn/gtvqzbchcz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xinyue.icu/gtwvmwpykr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.wangshuangyany.cn/gtqzspkwsm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ybcxt.top/gtifqoajpc.html

[F05] 判断文件或目录是否存在
来源：http://hz.hnxiangtu.top/gtaulfarcj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.chenzaomai.com/gtsohwgjjw.html

PHP:  file_exists("a.txt");
来源：http://hz.shanyushiyangtech.top/gtqmvymgiz.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hongshengwenyu.top/gtxkhidstn.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yuxming.cn/gtgjvmzhja.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ybcxt.top/gtvifnjrsl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.bjfxy.top/gtwabydhqn.html

Ruby: File.exist?("a.txt")
来源：http://hz.tianlin.xyz/gtcfwutuvg.html

C#:   File.Exists("a.txt")
来源：http://hz.jiagoushi.top/gtypvkamle.html

[F06] 删除文件
来源：http://hz.shzxlz.cn/gtfdmjpssi.html

Py:   os.remove("a.txt")
来源：http://hz.cheryme.top/gtnjapkwyd.html

PHP:  unlink("a.txt");
来源：http://hz.guowangkeji.top/gthdhlemrr.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yanxiufei.cn/gtwpyaseer.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.0kj1m.cn/gtccdyrbbg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jqgufenzy.top/gtoggqzfkc.html

Go:   os.Remove("a.txt")
来源：http://hz.ehwqpu.com/gtderejtmd.html

Ruby: File.delete("a.txt")
来源：http://hz.zhoulong.xyz/gtkvktnmhe.html

C#:   File.Delete("a.txt");
来源：http://hz.yanxiufei.cn/gtcenxcwfx.html

[F07] 创建目录（含多级）
来源：http://hz.ppjwa.cn/gtgnnvvnyr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jinyuanbaomall.cn/gturbfqmlr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.nwbrower.top/gtwqhqzcjx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.nwbrower.top/gtujoihfcq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhijiandao.cn/gtlaxasbph.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zdqjudy.top/gtoovmgdqy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.guowangkeji.top/gtvpvvhhjv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zdqjudy.top/gtlhsnkudl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.kuanghao11.cn/gtnnhuzsta.html

[F08] 遍历目录
来源：http://hz.gaohongyu789.top/gtqfikqluu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xuetiantiany.cn/gteurlvuhg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.shangyingyoupin.top/gtssqkkrxe.html

JS:   fs.readdirSync("dir")
来源：http://hz.snrcjt.cn/gtpdmaqhon.html

TS:   fs.readdirSync("dir")
来源：http://hz.birdmap.top/gtmdykcako.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.cashguo.top/gtxnnymrhc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yj20258.top/gtxjqztjdr.html

Ruby: Dir.children("dir")
来源：http://hz.xuetiantiany.cn/gtyqxjqixs.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yvedp.cn/gtyfpdjgxv.html

[F09] 获取文件大小
来源：http://hz.havefunace.top/gtfxjraxdi.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yangfankeji.com/gtsrmrzxtb.html

PHP:  filesize("a.txt");
来源：http://hz.tian-w.cn/gttaiogkeo.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hywenlv.cn/gtrrmtawqm.html

TS:   fs.statSync("a.txt").size
来源：http://hz.redwolf501.top/gtljdjfdip.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.quarkkingdee.top/gtuiqtqcbr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jiagoushi.top/gtkvzxleaz.html

Ruby: File.size("a.txt")
来源：http://hz.gaohongyu789.top/gtjdhqyqvt.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yuanzhike.top/gttsaeqiqz.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.0kj1m.cn/gtxufypixw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.sufxvd.cn/gtwqjjotwe.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.shanyushiyangtech.top/gtsowpugjf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtbtonnjlc.html

TS:   path.extname("a.txt")
来源：http://hz.pycfn.com/gtpnwnhrys.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.nanxuanxn.top/gthykhwxrn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.52xcode.cn/gtvcraxqff.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ivvv.top/gttppfkqgl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jinqigufen.top/gtsiagtyft.html

[F11] 复制与移动文件
来源：http://hz.hongshengwenyu.top/gtscvyuxts.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.guowangkeji.top/gticszmspn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yueranfly.top/gtqdpiieti.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ybcxt.top/gtmynelauv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ywan-chungtsiang.top/gtalwwytwr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hfpthk.cn/gtbitrvpbj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zhaomingkeji.xyz/gtdzqymwco.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.tanke756.top/gtdwdtsagj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yonumen.top/gtzosyvnnm.html

[F12] CSV 读写
来源：http://hz.316326.xyz/gtcpgguuqh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.sweek.top/gthyuffdkl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.fzhhl.top/gtpveatfal.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yj20258.top/gtnvrsadmj.html

TS:   // 同上
来源：http://hz.gogol.net.cn/gtcyjsziua.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhengqikj.top/gtzfmkmtbc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhixingplan.top/gthcjdrouv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.smart0.xyz/gtmsithzey.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.daxiang520.top/gtrrsregbo.html

================================================================================
来源：http://hz.gogol.net.cn/gtywfmtedr.html

G. 面向对象
来源：http://hz.zhijiandao.cn/gtkmrxeeby.html

================================================================================
来源：http://hz.dashuyun.cn/gtqwgdodjy.html

[G01] 定义类
来源：http://hz.jinghuilouyu.cn/gtopeubtym.html

Py:   class User: pass
来源：http://hz.xuetiantiany.cn/gtpypwdmfw.html

PHP:  class User {}
来源：http://hz.chenzaomai.com/gtkortxzoj.html

JS:   class User {}
来源：http://hz.pycfn.com/gtwecmujgj.html

TS:   class User { name: string = ""; }
来源：http://hz.ywan-chungtsiang.top/gtsiutvcdi.html

Java: class User {}
来源：http://hz.vqdsnc.cn/gtrdpdzhhs.html

Go:   type User struct { Name string }
来源：http://hz.xylfe.cn/gtctlomnyr.html

Ruby: class User; end
来源：http://hz.316326.xyz/gtrimtecjm.html

C#:   class User {}
来源：http://hz.gogol.net.cn/gtflrrudmv.html

[G02] 构造函数
来源：http://hz.zhixingplan.top/gtwzybobpv.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.nanxuanxn.top/gtfarhtuvh.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ppjwa.cn/gtnoczhlau.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ehwqpu.com/gtalaqbdud.html

TS:   constructor(public name: string) {}
来源：http://hz.yangfankeji.com/gtxlxmxxxn.html

Java: User(String name) { this.name = name; }
来源：http://hz.xinyue.icu/gtaezaczwt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.fengsongda.top/gtakqlxyia.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.sxryk.cn/gtqchdajrm.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hnqzz.top/gtlxuknage.html

[G03] 实例属性
来源：http://hz.zhongyouzk.top/gtcbdcxcdy.html

Py:   self.name = "x"
来源：http://hz.hammf.cn/gtaafubmdz.html

PHP:  public string $name = "x";
来源：http://hz.chenlongwang.top/gtahwaqwab.html

JS:   this.name = "x";
来源：http://hz.gogol.net.cn/gtwrjnorlv.html

TS:   name: string = "x";
来源：http://hz.jinqigfzy.top/gtqacxdkqu.html

Java: private String name;
来源：http://hz.cucudq.cn/gtstvxhbyr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xingfuxueyuan.xyz/gtkzdmwgbn.html

Ruby: @name = "x"
来源：http://hz.guowangkeji.top/gthweqhcna.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hnxiangtu.top/gtwqcrarcu.html

[G04] 定义方法
来源：http://hz.yj202588.top/gtposwmjqy.html

Py:   def greet(self): return self.name
来源：http://hz.pengpengdd.cyou/gtpgyyvvzo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.guannengcc.top/gtovdvibfg.html

JS:   greet() { return this.name; }
来源：http://hz.jianghu66.top/gtgdnuihxp.html

TS:   greet(): string { return this.name; }
来源：http://hz.jlsjyb.cn/gttseezcnn.html

Java: String greet() { return name; }
来源：http://hz.wangshuangyany.cn/gthicxuczb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hongshengwenyu.top/gtweqzidhc.html

Ruby: def greet; @name; end
来源：http://hz.jqgfzy.top/gtnedhkdom.html

C#:   public string Greet() => Name;
来源：http://hz.jiagoushi.top/gtoevopvbi.html

[G05] 继承
来源：http://hz.vqdsnc.cn/gtrtqhouke.html

Py:   class Admin(User): pass
来源：http://hz.zhaomingkeji.xyz/gtpmbhiqdz.html

PHP:  class Admin extends User {}
来源：http://hz.tianlin.xyz/gtajfezlwf.html

JS:   class Admin extends User {}
来源：http://hz.birdmap.top/gtlmxajowa.html

TS:   class Admin extends User {}
来源：http://hz.jiagoushi.top/gtqqnlhpme.html

Java: class Admin extends User {}
来源：http://hz.bjfxy.top/gttdkcumtj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.shangyingyoupin.top/gtaqynreor.html

Ruby: class Admin < User; end
来源：http://hz.aibaodan.cn/gtbvmcexjg.html

C#:   class Admin : User {}
来源：http://hz.cheryme.top/gtwolfxdua.html

[G06] 重写方法
来源：http://hz.ydjk.org.cn/gtqbvnyich.html

Py:   def greet(self): return "admin"
来源：http://hz.jinyuanbaomall.cn/gtxvmluvqo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ydjk.org.cn/gtlfxybele.html

JS:   greet() { return "admin"; }
来源：http://hz.daxiang520.top/gtlwkmswrh.html

TS:   greet(): string { return "admin"; }
来源：http://hz.fzhhl.top/gtkoubfwcb.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jlsjyb.cn/gtabutlrzi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.sweek.top/gtmwfocrvo.html

Ruby: def greet; "admin"; end
来源：http://hz.hfpthk.cn/gtdmjcrlhe.html

C#:   public override string Greet() => "admin";
来源：http://hz.shzxlz.cn/gtvzgfwloy.html

[G07] 调用父类方法
来源：http://hz.dianchejie.cn/gtpshrosrb.html

Py:   super().greet()
来源：http://hz.iojbl.cn/gttosnesqa.html

PHP:  parent::greet();
来源：http://hz.ydjk.org.cn/gtdqcnulpu.html

JS:   super.greet();
来源：http://hz.hnxiangtu.top/gtexkcihmx.html

TS:   super.greet();
来源：http://hz.ehwqpu.com/gtzrpgcdoj.html

Java: super.greet();
来源：http://hz.feifeiyinyue.top/gtsqkspyrg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yj202588.top/gtslsvzalf.html

Ruby: super
来源：http://hz.c1oappe.top/gtpigfpzou.html

C#:   base.Greet();
来源：http://hz.52xcode.cn/gtmtegffxc.html

[G08] 静态方法与属性
来源：http://hz.316326.xyz/gtlmmulozw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.guowangkeji.top/gtazhjoveu.html

PHP:  public static function f() {}
来源：http://hz.sxryk.cn/gteniuzrig.html

JS:   static f() {}
来源：http://hz.chenlongwang.top/gtofnlycyu.html

TS:   static f(): void {}
来源：http://hz.xingfuxueyuan.xyz/gtymklzplp.html

Java: static void f() {}
来源：http://hz.yuanzhike.top/gtgvtzbxqx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.tian-w.cn/gtgopisbak.html

Ruby: def self.f; end
来源：http://hz.chenjidiqi.icu/gtmvyuctmb.html

C#:   public static void F() {}
来源：http://hz.xinyue.icu/gtzbghvoyi.html

[G09] 接口 / 抽象类
来源：http://hz.jinghuilouyu.cn/gtgcjgplzz.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.cqqwz.cn/gtosxigskw.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.nanxuanxn.top/gtjrqwvoat.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.sweek.top/gtwhgcrmtv.html

TS:   interface Shape { area(): number; }
来源：http://hz.zhoulong.xyz/gtzvfmwtfh.html

Java: interface Shape { double area(); }
来源：http://hz.haohaochexian.top/gtjfzzlnrf.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.snrcjt.cn/gtydiphpew.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhijiandao.cn/gtmraysuzk.html

C#:   interface IShape { double Area(); }
来源：http://hz.shzxlz.cn/gtlbmjuvpo.html

[G10] 访问控制
来源：http://hz.zhaomingkeji.xyz/gtfdyefqve.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.c1oappe.top/gtxeyxocer.html

PHP:  public / protected / private
来源：http://hz.nwbrower.top/gtahrypcus.html

JS:   #private 字段；其余公开
来源：http://hz.yonumen.top/gtnoziqtfe.html

TS:   public / protected / private
来源：http://hz.nanxuanxn.top/gtpqbizbti.html

Java: public / protected / private / 默认包级
来源：http://hz.shuidangran.top/gtmzxvkyyg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.52xcode.cn/gtuaztvvzm.html

Ruby: public / protected / private
来源：http://hz.hnqzz.top/gtuvmgkyqa.html

C#:   public / protected / private / internal
来源：http://hz.cheryme.top/gtthakktgy.html

[G11] getter / setter
来源：http://hz.zhengqikj.top/gtxtkazrqa.html

Py:   @property 与 @x.setter
来源：http://hz.tanke756.top/gtgjuuarey.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.dianchejie.cn/gtbjrtfmrj.html

JS:   get name() { return this._name; }
来源：http://hz.yongpay.top/gthktsapmi.html

TS:   get name(): string { return this._name; }
来源：http://hz.hnqzz.top/gthucgnqnn.html

Java: public String getName() { return name; }
来源：http://hz.zhixingplan.top/gtdneotmxt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.wangshuangyany.cn/gtkrtwndly.html

Ruby: attr_accessor :name
来源：http://hz.yvedp.cn/gtichjsibz.html

C#:   public string Name { get; set; }
来源：http://hz.daria6918.cn/gtsqktaszv.html

[G12] 对象转字符串
来源：http://hz.cqqwz.cn/gtjdjrrsig.html

Py:   def __str__(self): return self.name
来源：http://hz.gogol.net.cn/gtkwtyedyu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yj202588.top/gtqgcahjms.html

JS:   toString() { return this.name; }
来源：http://hz.andypj.xyz/gtgbjgufrs.html

TS:   toString(): string { return this.name; }
来源：http://hz.dashuyun.cn/gtkvbbgfgd.html

Java: @Override public String toString() { return name; }
来源：http://hz.xinyue.icu/gtejdtskbs.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.mhx1999.top/gtckedtggb.html

Ruby: def to_s; @name; end
来源：http://hz.feifeiyinyue.top/gtlpxomaix.html

C#:   public override string ToString() => Name;
来源：http://hz.dashuyun.cn/gtzbeqmwhh.html

[G13] 判断对象类型
来源：http://hz.yongpay.top/gtwrnekgfi.html

Py:   isinstance(u, User)
来源：http://hz.redwolf501.top/gtilsnqydp.html

PHP:  $u instanceof User
来源：http://hz.bjfxy.top/gtdfuikolb.html

JS:   u instanceof User
来源：http://hz.aizwys.cn/gtzwhcobmh.html

TS:   u instanceof User
来源：http://hz.jinyuanbaomall.cn/gteufzwpjc.html

Java: u instanceof User
来源：http://hz.yuanzhike.top/gtwqqpryvi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.pengpengdd.cyou/gtrbiqeyst.html

Ruby: u.is_a?(User)
来源：http://hz.zdqjudy.top/gtihzyfojy.html

C#:   u is User
来源：http://hz.zhengqikj.top/gtmacntevm.html


<!-- 参考信息 -->