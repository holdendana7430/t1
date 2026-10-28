代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jqgfzy.top/gtwkousdjd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.chenlongwang.top/gtlsxqebps.html

Go:   // 手写 map[string][]T
来源：http://hz.yj20258888.top/gtekwjnawr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.cqqwz.cn/gtpqwqzjuv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yonumen.top/gtzsgedktv.html

[D20] 统计每个元素出现次数
来源：http://hz.yangfankeji.com/gtutlnefyv.html

Py:   Counter(arr)
来源：http://hz.chenlongwang.top/gtugqvcure.html

PHP:  array_count_values($arr);
来源：http://hz.shanyushiyangkeji.top/gtivjldrgh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.iojbl.cn/gtmjoqhcac.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yvedp.cn/gtpoopleby.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.meibo888.top/gtovbsxfvx.html

Go:   // 手写 map[T]int
来源：http://hz.yj20258.top/gtseifpzsr.html

Ruby: arr.tally
来源：http://hz.hammf.cn/gtvwyslkgv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yangfankeji.com/gttazzaugl.html

[D21] 判断是否包含某元素
来源：http://hz.zdqjudy.top/gtmxfluqyn.html

Py:   x in arr
来源：http://hz.jinqigufen.top/gthzrgxvyj.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zhijiandao.cn/gtuvlmcfcd.html

JS:   arr.includes(x)
来源：http://hz.shuidangran.top/gtcxqnhiyf.html

TS:   arr.includes(x)
来源：http://hz.tian-w.cn/gtutrecoma.html

Java: list.contains(x)
来源：http://hz.tian-w.cn/gtdjujbvdc.html

Go:   slices.Contains(arr, x)
来源：http://hz.yueranfly.top/gtqzhyuiin.html

Ruby: arr.include?(x)
来源：http://hz.ydzc1.top/gtodljnnfg.html

C#:   list.Contains(x)
来源：http://hz.chenjidiqi.icu/gthmsyyikr.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jinyuanbaomall.cn/gtbqzmukot.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.sufxvd.cn/gtozchqaoz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zdqjudy.top/gtzmlxrgns.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.nwbrower.top/gtipplqotl.html

TS:   [...arr];
来源：http://hz.ydzc1.top/gtpitrymif.html

Java: new ArrayList<>(list);
来源：http://hz.feifeiyinyue.top/gtydnsvnhl.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.52xcode.cn/gttxyzbqmy.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zdqjudy.top/gtkxbubwqc.html

C#:   new List<int>(list);
来源：http://hz.ywan-chungtsiang.top/gtlzbyoamx.html

[D23] reduce 累积计算
来源：http://hz.c1oappe.top/gtmpjdtiwz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jianghu66.top/gtuejwxjad.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.svipenyu.cn/gtvwtkbznj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.9152youxi.cn/gtglnrljlq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xingfuxueyuan.xyz/gtggvlulvu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yj202588.top/gtqpyoebpi.html

Go:   // 手写循环
来源：http://hz.yangfankeji.com/gtowauvtjn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yj20258.top/gtavwpbhye.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.zhoulong.xyz/gtpslgtfmm.html

[D24] 字典 / Map 基本操作
来源：http://hz.jinghuilouyu.cn/gtmgkfmqbn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.aizwys.cn/gtjmvwhgpl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.iojbl.cn/gtnlfxxivf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jyoumei.cn/gttczbjagj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yanxiufei.cn/gtbovhhtsw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.fzhhl.top/gtnearwcyy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yuxming.cn/gtpmljxdkh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.nanxuanxn.top/gtqnyxurlm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.gzhubu.top/gtlabxuynq.html

[D25] Set 集合去重与交并差
来源：http://hz.cashguo.top/gtwasfxxuu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.sweek.top/gtoffhtqwc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.snrcjt.cn/gtlgyqwubu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.snrcjt.cn/gtgnrwunev.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.tianlin.xyz/gtqujvoexn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.feifeiyinyue.top/gtxxnbujme.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.bjfxy.top/gtqmtfsxfr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.feifeiyinyue.top/gtrydhzcue.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.shanyushiyangtech.top/gtduhmnrpm.html

[D26] 数组转字符串
来源：http://hz.yongpay.top/gtoaqbqeos.html

Py:   ", ".join(map(str, arr))
来源：http://hz.cdnleiting.top/gtvrlvinht.html

PHP:  implode(", ", $arr);
来源：http://hz.bjfxy.top/gtppvosilw.html

JS:   arr.join(", ")
来源：http://hz.gzhubu.top/gtozwslozu.html

TS:   arr.join(", ")
来源：http://hz.snrcjt.cn/gteqbkbzdc.html

Java: String.join(", ", list)
来源：http://hz.ydzc1.top/gtwppmrxyh.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yanxiufei.cn/gtzoypamcs.html

Ruby: arr.join(", ")
来源：http://hz.gotoacloud.top/gtwoyiehtn.html

C#:   string.Join(", ", list)
来源：http://hz.c1oappe.top/gtftjybqwl.html

================================================================================
来源：http://hz.havefunace.top/gterswqmdh.html

E. 字符串处理
来源：http://hz.cucudq.cn/gtelqjkloq.html

================================================================================
来源：http://hz.gzhubu.top/gttnatysgw.html

[E01] 拼接字符串
来源：http://hz.xingfuxueyuan.xyz/gtarrfodhx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zhixingplan.top/gtabwdhrnl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.xziqi.cn/gtoyfmuvmp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.quarkkingdee.top/gtllgoyxna.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.tanke756.top/gthbinhpcf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.sweek.top/gtnpfawmuj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.chenzaomai.com/gtpmikphcp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.fzhhl.top/gtzohyprhs.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.nwbrower.top/gtzdsfyotq.html

[E02] 重复字符串
来源：http://hz.yj202588.top/gtdjzwmewd.html

Py:   "ab" * 3
来源：http://hz.hfpthk.cn/gtcychgfby.html

PHP:  str_repeat("ab", 3);
来源：http://hz.cdnleiting.top/gtqlpqxjrh.html

JS:   "ab".repeat(3)
来源：http://hz.yanxiufei.cn/gttmvpdccv.html

TS:   "ab".repeat(3)
来源：http://hz.yanxiufei.cn/gtyfzfkjvm.html

Java: "ab".repeat(3)
来源：http://hz.sxryk.cn/gtzvkndvjn.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zhoulong.xyz/gtvsnmqpfi.html

Ruby: "ab" * 3
来源：http://hz.zhijiandao.cn/gtyuczuntj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.dashuyun.cn/gtnxqgialn.html

[E03] 截取子串
来源：http://hz.zhixingplan.top/gtxkdxlgtw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.tanke756.top/gtmllchiet.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.aizwys.cn/gtxqjuqhpm.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jinqigufen.top/gttpkdngpj.html

TS:   s.slice(1, 4)
来源：http://hz.yangfankeji.com/gtntpxzugn.html

Java: s.substring(1, 4)
来源：http://hz.hnxiangtu.top/gtmciqeyum.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.aizwys.cn/gtuypyrvys.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.nanxinkj.top/gtvqnthpbd.html

C#:   s.Substring(1, 3)
来源：http://hz.pycfn.com/gtdmkysnrw.html

[E04] 查找子串位置
来源：http://hz.xinyue.icu/gtnvsjtopb.html

Py:   s.find("x");  s.index("x")
来源：http://hz.cqqwz.cn/gtxttdduxz.html

PHP:  strpos($s, "x");
来源：http://hz.dashuyun.cn/gtcwdyiqhp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.dianchejie.cn/gtjoymqmtj.html

TS:   s.indexOf("x")
来源：http://hz.shzxlz.cn/gtijpxvoka.html

Java: s.indexOf("x")
来源：http://hz.yongpay.top/gthxdwxvny.html

Go:   strings.Index(s, "x")
来源：http://hz.jinqigfzy.top/gtoucgqkvx.html

Ruby: s.index("x")
来源：http://hz.ivvv.top/gtfjtxjsvm.html

C#:   s.IndexOf("x")
来源：http://hz.jinqigfzy.top/gtwypvvozp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.316326.xyz/gtwnbonfle.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.xuanzx.com/gtdjvqvvbk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.gotoacloud.top/gtcsmidlvq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jyoumei.cn/gtvauzwsbk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.wangdashe.top/gtmshrfkhp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.kuanghao11.cn/gtgtnwjwaf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.shuidangran.top/gtiovagewr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.zycfv.cn/gtzqowopln.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.xingfuxueyuan.xyz/gtiizlrvvf.html

[E06] 替换子串
来源：http://hz.hfpthk.cn/gtfgpyzjqy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.sxryk.cn/gtoahtzxyy.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jinqigfzy.top/gtvimmbftz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xinyue.icu/gtyhdlswlh.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jqgfzy.top/gtirjzdqgz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jlsjyb.cn/gtqardqlgl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yj20258888.top/gtekdnpcbn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yueranfly.top/gtokmaceyc.html

C#:   s.Replace("a", "b")
来源：http://hz.hongshengwenyu.top/gtfhfpegwe.html

[E07] 按分隔符拆分
来源：http://hz.yj20258.top/gtmfcifcpe.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.cheryme.top/gtrevbiyoe.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.dianchejie.cn/gtibqiabel.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.hnxiangtu.top/gtyltbncsl.html

TS:   s.split(",")
来源：http://hz.yueranfly.top/gtvmbhqaol.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.nanxuanxn.top/gtgzkvlvqc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.fzhhl.top/gtdgspzppp.html

Ruby: s.split(",");  s.split
来源：http://hz.316326.xyz/gtvltbtovh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yonumen.top/gtuwtfmzkk.html

[E08] 数组按分隔符合并
来源：http://hz.jinqigfzy.top/gtizdzdpkr.html

Py:   ",".join(items)
来源：http://hz.yangfankeji.com/gtzpwpjcmh.html

PHP:  implode(",", $items);
来源：http://hz.tian-w.cn/gtqycrctuo.html

JS:   items.join(",")
来源：http://hz.cdnleiting.top/gtclixismn.html

TS:   items.join(",")
来源：http://hz.yangfankeji.com/gtnufaibbz.html

Java: String.join(",", items)
来源：http://hz.zhijiandao.cn/gtlmtfbkvf.html

Go:   strings.Join(items, ",")
来源：http://hz.sweek.top/gtjbaradcz.html

Ruby: items.join(",")
来源：http://hz.meibo888.top/gtlozwidnr.html

C#:   string.Join(",", items)
来源：http://hz.chenjidiqi.icu/gtkdaizgiu.html

[E09] 去除所有空白字符
来源：http://hz.shzxlz.cn/gthunsoksr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.quarkkingdee.top/gtzbqgowjh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.snrcjt.cn/gthzoxahkv.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yonumen.top/gtjsghsvgd.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.haohaochexian.top/gtmohilnct.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.svipenyu.cn/gtczyuvdzi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.jinghuilouyu.cn/gtnmqdcmxs.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jyoumei.cn/gtsblhpqne.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.vqdsnc.cn/gtkluhtfrc.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yongpay.top/gttdndnbzs.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.svipenyu.cn/gtrtzzrxkj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jinqigfzy.top/gtbjmlxbub.html

JS:   "7".padStart(3, "0")
来源：http://hz.zhixingplan.top/gtltiijqki.html

TS:   "7".padStart(3, "0")
来源：http://hz.ppjwa.cn/gteocecvzj.html

Java: String.format("%03d", 7)
来源：http://hz.snrcjt.cn/gtsybcbpaj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.hysaishi.cn/gtupgvunht.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yongpay.top/gttmiadufq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.tanke756.top/gtrvqcnckz.html

[E11] 反转字符串
来源：http://hz.yuanzhike.top/gtamkaotnk.html

Py:   s[::-1]
来源：http://hz.chenlongwang.top/gtuphylsuv.html

PHP:  strrev($s);
来源：http://hz.pycfn.com/gtjmnpkmzl.html

JS:   [...s].reverse().join("")
来源：http://hz.zhongyouzk.top/gtsxtmvnuw.html

TS:   [...s].reverse().join("")
来源：http://hz.fzhhl.top/gtnemghvtq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.sweek.top/gtytsshiwt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.0kj1m.cn/gtpqnqtwkx.html

Ruby: s.reverse
来源：http://hz.quarkkingdee.top/gtnxwohjdm.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jyoumei.cn/gtmneqekuy.html

[E12] 统计某字符出现次数
来源：http://hz.chenzaomai.com/gtczgegsui.html

Py:   s.count("a")
来源：http://hz.tian-w.cn/gtjqhegmgl.html

PHP:  substr_count($s, "a");
来源：http://hz.pycfn.com/gtfdwehcve.html

JS:   s.split("a").length - 1
来源：http://hz.cucudq.cn/gtujaahrnn.html

TS:   s.split("a").length - 1
来源：http://hz.guowangkeji.top/gtzgyjbixp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.gaohongyu789.top/gtiurnjezx.html

Go:   strings.Count(s, "a")
来源：http://hz.yueranfly.top/gtvuxevuys.html

Ruby: s.count("a")
来源：http://hz.hammf.cn/gtzhphfrhh.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jianghu66.top/gtyazxvobn.html

[E13] 逐字符遍历
来源：http://hz.zhengqikj.top/gtdlstfsoe.html

Py:   for ch in s: print(ch)
来源：http://hz.jyoumei.cn/gtohejqaka.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.gotoacloud.top/gtafujwkxq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sxryk.cn/gtpfbdadxc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.tanke756.top/gtwrwhwbky.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.bjfxy.top/gtxlgeytfm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.c1oappe.top/gtmmgdhowz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.pengpengdd.cyou/gtcirdukkm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.snrcjt.cn/gtmgwigxzw.html

[E14] URL 编码与 Base64
来源：http://hz.gaohongyu789.top/gtdemrabim.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.havefunace.top/gtwzopfskk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.tian-w.cn/gtnsdhjgte.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yj20258888.top/gtcgtrmpxw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.0kj1m.cn/gtktxbhmtw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jinghuilouyu.cn/gtgjzgyrxy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.shangyingyoupin.top/gtldtgmxjf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.chenlongwang.top/gtvwnjlvvi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhixingplan.top/gtvmxzwzfm.html

[E15] HTML 转义 / 反转义
来源：http://hz.jianghu66.top/gtboflbzwd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.hnxiangtu.top/gtfxkluatn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.shzxlz.cn/gtqghgvrcb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.sufxvd.cn/gtmscbhvps.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.guannengcc.top/gtnoxwqlrv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yj202588.top/gttliofxrj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.chenlongwang.top/gtoooyehet.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.snrcjt.cn/gtxrncsxza.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.sxryk.cn/gthvkmpvak.html

[E16] 数字千分位
来源：http://hz.zycfv.cn/gtdtnncvzj.html

Py:   f"{1234567:,}"
来源：http://hz.shangyingyoupin.top/gtshcefaal.html

PHP:  number_format(1234567);
来源：http://hz.tianlin.xyz/gtxcwhlhnp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yuanzhike.top/gtsedehlco.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ehwqpu.com/gtlpyrlnko.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.havefunace.top/gtsnnrsfch.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.cdnleiting.top/gtzcbjqynm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.gzhubu.top/gtsyojxcdq.html

C#:   1234567.ToString("N0")
来源：http://hz.iojbl.cn/gtzbmgmyxt.html

[E17] 首字母大写
来源：http://hz.fzhhl.top/gtchxwbpdw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.vqdsnc.cn/gtdiqtidsy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.ivvv.top/gtvqsymmbb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sweek.top/gtbbefkivt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.vqdsnc.cn/gtgoroamrp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.daxiang520.top/gthyaiqdzr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.hongshengwenyu.top/gtlewmmnme.html

Ruby: s.capitalize
来源：http://hz.birdmap.top/gturqirutm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.bjfxy.top/gttwtgewnj.html

[E18] 模板占位符替换
来源：http://hz.52xcode.cn/gtebmgldot.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.52xcode.cn/gticueccaq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.tian-w.cn/gtagatcdfs.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yuanzhike.top/gtwwalwmdp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.chenzaomai.com/gtaiuaceql.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.daria6918.cn/gtbbdttfgi.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zhixingplan.top/gtiognjriq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.chenlongwang.top/gtwvxihakr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.birdmap.top/gtzexrjdck.html

[E19] 多行文本按行拆分
来源：http://hz.chenzaomai.com/gtxoqqwidr.html

Py:   s.splitlines()
来源：http://hz.9152youxi.cn/gtywqbpjfo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yj20258888.top/gtbgekmxzx.html

JS:   s.split(/\r?\n/)
来源：http://hz.meibo888.top/gtcgiraqcb.html

TS:   s.split(/\r?\n/)
来源：http://hz.jinqigufen.top/gtlimtybdp.html

Java: s.lines().toList()
来源：http://hz.guannengcc.top/gtynoyhhxt.html

Go:   strings.Split(s, "\n")
来源：http://hz.shangyingyoupin.top/gttwrqyjpy.html

Ruby: s.lines
来源：http://hz.iojbl.cn/gtrzdwhovt.html

C#:   s.Split('\n')
来源：http://hz.ivvv.top/gtlgaqcilz.html

[E20] 判断字符串是否为空
来源：http://hz.zhaomingkeji.xyz/gtgxzfliew.html

Py:   if not s:
来源：http://hz.yonumen.top/gtqpxbstqg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zhiwuduotai.top/gtkvmmybhc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.aibaodan.cn/gtvprnyjdo.html

TS:   if (s === "") {}
来源：http://hz.andypj.xyz/gtxuhbowtl.html

Java: if (s.isEmpty()) {}
来源：http://hz.zhijiandao.cn/gtlgvyzxas.html

Go:   if s == "" {}
来源：http://hz.guannengcc.top/gtspsanpdz.html

Ruby: if s.empty?
来源：http://hz.nanxinkj.top/gtucfvyfvm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.52xcode.cn/gtnamgzbjg.html

[E21] 超长截断加省略号
来源：http://hz.wangdashe.top/gtdeoajnym.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.nanxinkj.top/gtervkoavt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.c1oappe.top/gtrfgteegw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yangfankeji.com/gtuxanbpnp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hnqzz.top/gttbbxucxv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jqgfzy.top/gtnjtqqdwd.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.cdnleiting.top/gtcbmgicpz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.nanxinkj.top/gtxdcgeqkx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.bjfxy.top/gtmplzmebf.html

[E22] 字节长度与字符长度
来源：http://hz.yuanzhike.top/gtwgrwqhwj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yonumen.top/gtijttejam.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hfpthk.cn/gtyesdoxuz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ehwqpu.com/gtjgqfjcbm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hongshengwenyu.top/gtkejiswgr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yueranfly.top/gtfweuihts.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jqgfzy.top/gtbniqgdle.html

Ruby: s.bytesize;  s.length
来源：http://hz.9152youxi.cn/gtitjfazss.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.vqdsnc.cn/gtckbudhza.html

================================================================================
来源：http://hz.yueranfly.top/gtcgauhqxu.html

F. 文件与目录
来源：http://hz.9152youxi.cn/gtfbngnkyt.html

================================================================================
来源：http://hz.sufxvd.cn/gtfrouuimz.html

[F01] 读取整个文件
来源：http://hz.jyoumei.cn/gtfmwymabd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jinghuilouyu.cn/gtomjcwnyk.html

PHP:  file_get_contents("a.txt");
来源：http://hz.pengpengdd.cyou/gtntpwswai.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yangfankeji.com/gtfhqjoeno.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.sweek.top/gtxqavmsdv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.guowangkeji.top/gtjlxlcphq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.gzhubu.top/gtqriasdqe.html

Ruby: File.read("a.txt")
来源：http://hz.ehwqpu.com/gtyemolqgr.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jinghuilouyu.cn/gtteqxzryi.html

[F02] 逐行读取文件
来源：http://hz.316326.xyz/gtzqntfgrs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.tian-w.cn/gtmfvpgypm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.hongshengwenyu.top/gtsfxpvtxx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sweek.top/gtjiovgojp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nwbrower.top/gtndpxbdsi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.gaohongyu789.top/gtvfrntfla.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hnxiangtu.top/gtkrfyyvsy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.guowangkeji.top/gtiouftzes.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.mhx1999.top/gtzmvxutnv.html

[F03] 写入文件（覆盖）
来源：http://hz.jinqigufen.top/gtlziddvwy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jlsjyb.cn/gtuwhwrrls.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yanxiufei.cn/gtmyrnqmcy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.snrcjt.cn/gtwfewumxt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jlsjyb.cn/gtdzfobsrm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jiagoushi.top/gtutkqdcpa.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zycfv.cn/gtetdqpwpg.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.gzhubu.top/gtvyhepdzr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.haohaochexian.top/gtfggpsdxl.html

[F04] 追加写入文件
来源：http://hz.nanxuanxn.top/gtwvzcekwc.html


<!-- 参考信息 -->