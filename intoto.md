代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jsozsqaf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3mdbjvtlt.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3mztqxruu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3rpasxrhm.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3zlweoppe.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3fdkbpgum.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3zhukmjbl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3yxofpkfg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ltirwziz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3odvrszvw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3licdsxzc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3gnyeusjt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3dsuevohg.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3gnxfrpor.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3xlcsopnz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3kztovccn.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3kmstlwin.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3kztfocpe.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3csezognv.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3himagmzh.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3ulvnzvmx.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3zcfitmey.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3iyyvuoxa.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3bhlqfhus.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3edonwskv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bznkthdr.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3npgwlfeo.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3zbbmvvak.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3girnephz.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3rehiuyab.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3zifjzcch.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3qabtxeub.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3mkynldug.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ocgpjpsi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yngecacu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rsopfatw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zfjdzdsy.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ctpnwsof.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qekhydzb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vslcezli.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3dppjwdej.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yappnpyi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wvstsyep.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3uwhkckde.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rdkdwtub.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3nczfebxe.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3qvjqxdpk.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3elxgecbp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3aqnalgog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qkilztbg.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3wywlqxdl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mqbjxbdy.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3fyxyzhom.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3bmkyxgbz.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ouvjprhy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3guewrgqu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3qnjfxphv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3agygvqwr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3hhwxvxco.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gdfvfphn.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ofxkdmwn.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3faqgvmjf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3tdxkztjo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ryiawiwa.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3asqmcvsp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ykusddjo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3lrmftqyk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3estpkfsv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3qwoqvijl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3xkbyneaf.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3wqeqstnk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3dawkrwnc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jckuzobf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ufnkkmvt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ogqacfso.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ybvlsxkg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3bgdxygbo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3tsveeukk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3vuxaxcsf.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3xwxfthxm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3pcwvlqqo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3xjindezq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gqnoarmt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3evgkikjw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3oexverkv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dyhiaysq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3lohqwgfy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3nrpyltjk.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3rpsjqsau.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3uhfleopa.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3knqprzmg.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hrfqpcxn.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kyijzuwz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3saallcog.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3wcpmwcom.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lhcwcict.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mojebdtl.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ekfxveex.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fgujcokt.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jlerugbs.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xcdxpaar.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iycizani.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3myghqcyv.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sjjrcnfa.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rlordxsi.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cibesenn.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3ifbsvekc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3oxwqcijk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3yzzrxoyd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3lzaxlytn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3afkdexev.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3nqgkibam.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3fhoyzizi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3smzfjrvi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3vhivhznt.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3rdyihwan.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3zebywtre.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3fbrkyrzf.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3mejdqwgd.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3jmfmncje.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3yhojqyhg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3raiclgob.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dhcnhicx.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3gjlyybpt.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3wqlecfeh.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wlyfknje.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pjhcobqm.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3xanlukis.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3eeqcjjok.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ouodhjxc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3agetitnq.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ccohldhu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3jhaywhqf.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3aygdleyi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3efnpypsc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xjbqrcik.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wcrumcih.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tetloonn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3iszszwsc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3irwvxrpp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jksndvsi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ullzijkb.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3yxewgtfg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hpadypfq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kmnypext.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zthxazdr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ulejnxyx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3nobldetf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3stlmxvqs.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yfnggkut.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3flxrzxbh.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3szsjbkvn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3oxowlwbc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3jashunax.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3tygvmzaf.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3yvooyxyl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3oikomqoj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3opjsxtgb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3punrtaex.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3cytcynph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kagaonah.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3nctykccc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kyscoyoq.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3gzduxtcb.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3swzgovlj.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3jepjnics.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cdtbvsya.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3dcowcori.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hvkzchab.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3okurpkbp.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3rsfkflsu.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gopnfpen.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3vgtgagjs.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3rvhailei.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qqrvevwl.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3vloiosug.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3zzwjsgoa.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ewmpvrrf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3euctqrld.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jutzgxfo.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdqetmqf.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3tyfwzzun.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ianifhhq.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3jsosodrb.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hroberem.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3iyrgvcas.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3jntoafjs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3bxadvsqm.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3vmnphojs.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3suqxgisg.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3hriqeaue.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3syntpmtz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3wowaabzq.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nduxbjsr.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kcfodrex.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mnblyiaw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3uvcemabh.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3eadzaawe.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3irwxpnoz.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3oprcjkqr.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3qcgldtkx.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3tjbhhfez.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gjetfsrz.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3yyzvulnv.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xrzbnylz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3butatzew.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3yylojqwr.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bbnfpjmw.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3ftclnuau.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ynhwpefg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wulynamy.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hefubkjd.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhtuxsqf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3drdwpbdq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3doeipkem.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3nlblmtfm.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3zodabwqb.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3srzjawhx.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3bswozsdk.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ufryqqll.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3iacigqbo.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3lhbhckny.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ffjtrnkj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3fwbqyhis.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3oczvukbn.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zbyoqhet.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ozutcuzm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3mnwajlfr.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3lxgyoklx.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3nbodmzsa.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3xiriyagw.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3uikixbef.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ywqwfexx.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ahjjhbjq.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qqpmqfsn.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3tlzzzrzr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3tipqxinf.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3zrsogojb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3aakbkavd.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3gyvhboae.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gbpobdve.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3ciqyusui.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3tfjzccdm.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fhlyxzwx.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3dznyzmrm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3vwveqmjq.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3dnaiwcjg.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3uyhbjblj.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3edbbrrwb.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3ouairmbo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3ilnnirwr.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xcuovdmo.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3gvafbzyr.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3yzyeybof.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3pdjqrbhg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3piljwsdd.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bnzldiir.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbcldnyd.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmtpindw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3rsfcdlgm.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3hirvxurz.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3aiyoxpak.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tevvzqfk.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3teolfpnt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mytrluix.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dukpkdzu.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfidxtxz.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbhuxwss.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3eeisppsg.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ryzgsdxt.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ocnqfgtt.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3vrinydsr.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3akxouxfz.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3onhvkudd.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wbgxwyvz.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zetwbypb.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pevjuqsc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3odjqmzod.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3glysisly.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3tqpiiqmz.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3bpefecnc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3rkocornf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3cxbxflae.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3lndlqydy.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3qspocyxg.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qlvnhxil.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3piejdmmu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3pkxgjpwc.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3tmmcslia.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ipbzegba.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3wwtjnkzq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxdwernf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3pafsryua.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3yuhwvstm.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3gppqlyul.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3ddebrvxs.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3qcwftuzf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3epowfznu.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3nsgdpndi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3wffbawdv.html


<!-- 参考信息 -->