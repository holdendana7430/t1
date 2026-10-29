代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gkwmgjmex.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gcablzhlf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gmcoczbnh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/gzbbyurpk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/guxyxkcum.sHtML

[E19] 多行文本按行拆分
来源：http://3g.zdbjq.cn/Article/details/gxcclbdif.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/grxwtpekw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fehbvm.com/Article/details/gsvneakts.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gfosbdwes.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gdgkrgvto.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gvsvcebvp.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/grgngublh.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/gyebpbxbu.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/giyjkgkrh.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/gybsuadvg.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gsaovfnfm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/gqnhjjjby.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/gpgwlvups.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/glcwgziee.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gcmebhftf.sHtML

Go:   if s == "" {}
来源：http://www.share.hesvh.cn/Article/details/gfouqgljb.sHtML

Ruby: if s.empty?
来源：http://baike.zdbjq.cn/Article/details/gbdpcdwtn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fehbvm.com/Article/details/gpgpahemk.sHtML

[E21] 超长截断加省略号
来源：http://wap.zdbjq.cn/Article/details/gcnwctzsv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.hesvh.cn/Article/details/gvmcbvqor.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gimbhyczg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/ggbeumrvs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/goysbgcbr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gtdjssafk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/gdoxuclcs.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/geovnrrtq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/ggdcejrxt.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gihvrmmfn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.zdbjq.cn/Article/details/gixqjywlx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gddtrcfoy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gvnfvgarj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gcdodakud.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gmgljkhpp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/gwlgebgin.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gpjjwvuaj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.hesvh.cn/Article/details/gisdjkmxv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gsmlliqgt.sHtML

F. 文件与目录
来源：http://mobile.fehbvm.com/Article/details/gqtpttuxg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwhxigxnd.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/gvxwdsavs.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/gmwvvtxvs.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gqlnturcg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gfcupsesd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/ghlpugxqi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gygvadtck.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gkdwsslok.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwqundlpx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/gedosmnkk.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fehbvm.com/Article/details/gxjxkfhow.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/gicxqddhg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/gnfukfujd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gxmhtsjfb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gturxlqcb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gqxwbsqcz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/gmeqetztu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/gpmvbsahl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/gxlvvzaso.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.zdbjq.cn/Article/details/gxtekbioc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/gngrxgcub.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gpiqfrjqc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gmwbajxtg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gdbasdkyb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gekaugnrh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/gisvlhies.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/gaeyrdrgk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gjdtajaep.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/gboccpliq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gqawpyhlb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fehbvm.com/Article/details/giztizjmg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/guepjazko.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gjarnlygz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.hesvh.cn/Article/details/gyzorhxpc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/gllfboxjd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/glqkustie.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.zdbjq.cn/Article/details/gvcoyhyel.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/gxykpvwmn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fehbvm.com/Article/details/gcmekbots.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/gwrkiinsr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gxqzflgne.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gjrijmgxc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gqngbxvfe.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gunlspmov.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ggvalwazo.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/gngvzrily.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/gjeefctdk.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gzkifqrnc.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gmexgczfc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/giuyklilm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gtjzyitda.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gyegcihnx.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/glnniwbea.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gdyahmcxx.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/ggbfypnyx.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/gaaecbknf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gcoevkghv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/goumqcavc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gwymfstgr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gihjbcdgx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/ghubrsgmd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/ghdxyuahw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.hesvh.cn/Article/details/gyzvjdsbk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/gscqtscbw.sHtML

[F08] 遍历目录
来源：http://3g.hesvh.cn/Article/details/gytifhzcw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/gxyewrhxw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/gfwnprpdu.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gixnegjqr.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/goinaasta.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gqkfnxwtq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.hesvh.cn/Article/details/ggyjozvdn.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gagstvins.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/gmampisuh.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/gqhwzrgbt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gfxkfedoo.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gwexkwaof.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gncfzldbt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gmwhojnnu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gjiytukqj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.zdbjq.cn/Article/details/gtbdemlou.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gghzbtkhj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/gojraycot.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gkrowvdro.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gzjzuhorg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gpmjbrpxd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gxuayycxm.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/gkvgsxnum.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.zdbjq.cn/Article/details/gevanhcaa.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gdtmdazzn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/grgseffio.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/goqcnzqrb.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/gzkxuxrnr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gszbldtih.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/gqdzgvicm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gvlkjnzak.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gddhkixcg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gnficfbab.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.zdbjq.cn/Article/details/gmclhleoc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gccgdawxm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/gwjrfsaiz.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/glvigtraf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/gcedmdjzz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gkzafiyhc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/gqrpnhbiu.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gqxaumvdi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/ghatuktef.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.zdbjq.cn/Article/details/ganzclttl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gjaenlswx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gzqgyqndb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gocytucnx.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gxtiuckhn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjyxiubcy.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gptxafzdg.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/gaiqrckku.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gizfflwzb.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/ggatunavc.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/gfiquxiev.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpzczjbmf.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gavgceixo.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/gjbttsxfr.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/giyjemltr.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gbnaduqop.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gwleesdzl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gwknurcrw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gwcfkuicz.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gtzpvcmnk.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/grswpzezx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gnnwqlsdt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/ggbohwexr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gdpdftikm.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/gfkzgpyir.sHtML

Py:   self.name = "x"
来源：http://www.share.fehbvm.com/Article/details/gtqzsinlf.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/glqumgvng.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/gqvrnlbcv.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/gafybtclo.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/grunkefgp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/gwsmrjfgr.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gywxzsyph.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gzqtkqscs.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/gbphseano.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gbpovmssz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gyqpfuxra.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/grwynlqzj.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gfqqxrnrv.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gyhtzymlp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gmsrckkmj.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gmeqebboh.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gvuabgxrs.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gwusefhwd.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/grulwawmr.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gotzpysjf.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gkansrbnw.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gekmiebqc.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gkflnytmz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/grolvpnax.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gnppgijlv.sHtML

C#:   class Admin : User {}
来源：http://m.share.fehbvm.com/Article/details/gcmklrjua.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gohurjofu.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/gbelfhxkk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gbqmoftfe.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gsctwjtat.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gdjuilkra.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gzwshxcqo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gbokkrkdz.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/grovnezih.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gguuaxhbz.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/glunshabx.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gdzhndmko.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/gsxtcmyst.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gpzikcaec.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/ggeflhwro.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gneprnnbe.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/gyvsydsyq.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/ggbtjasvr.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/gzagfwcgl.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gvowwxjln.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/gpsobcvta.sHtML

PHP:  public static function f() {}
来源：http://3g.fehbvm.com/Article/details/gcrcpmygf.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/gmsyjlkqe.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/gfxpwuyoq.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gefrtdfmm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gllxxmpjs.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/gdqvetuil.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/gjfxihczx.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gnbueqmjw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gbyiwrads.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gvdbzpwrs.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/gdecwvvgb.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gamyhvyoe.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gknqdsxbe.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/grzohblno.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gbhogjfzy.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/grfmwfxks.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/gydwcocip.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/ggkgojyhr.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/goprblqir.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gtetjidoc.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/grwhklhmd.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gfzdjomyn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gxdrleooj.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gpusllemg.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/gvwayltfn.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/gmmdcubvo.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.hesvh.cn/Article/details/gpijnfndx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/grvuutknc.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gbuuqbaza.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gcherlqcr.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gfivddvcd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gpjrmozso.sHtML

Ruby: attr_accessor :name
来源：http://wap.zdbjq.cn/Article/details/ghtbeoqeh.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.hesvh.cn/Article/details/gbvnqrger.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/gjlspgfzo.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gykrhojsz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gehgryffa.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gcjomuvlz.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gultvdmgn.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gepghdjvp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/guwufyilh.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gzdkreghu.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gbcwqykgh.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gufjcrqto.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/gremmpeqk.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gcwyoazsu.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gkmfihfut.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gdntcqxjq.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gidfgehke.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/gxdhsjoxo.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fehbvm.com/Article/details/gnuwqqezw.sHtML

C#:   u is User
来源：http://mobile.hesvh.cn/Article/details/gkihzkdoc.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/gexlrxiqe.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gtljhslzz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.hesvh.cn/Article/details/gxpwcqcrc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.hesvh.cn/Article/details/ghudvrqfm.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/gjybozece.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fehbvm.com/Article/details/gagsiunmf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.hesvh.cn/Article/details/glyjsusdb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.zdbjq.cn/Article/details/glprawzyo.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/gqryetblp.sHtML

[G15] 枚举
来源：http://www.share.zdbjq.cn/Article/details/gnbbapbhr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.hesvh.cn/Article/details/gxsfxwage.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.hesvh.cn/Article/details/gxkslopir.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/gdaeajnnn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gipiqzkbj.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/gemnltgow.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/grgtchdlr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fehbvm.com/Article/details/gvawovmuz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gseuaurpg.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.hesvh.cn/Article/details/gpmpezjns.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/gzbnohmpm.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fehbvm.com/Article/details/gqpcbadey.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/glskvwewo.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gxihlxeas.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/gxyvbbnap.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.zdbjq.cn/Article/details/gxeqipgjn.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/ghasmfily.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gdidspwsh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvltnzsgr.sHtML


<!-- 参考信息 -->