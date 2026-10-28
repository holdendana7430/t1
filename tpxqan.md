代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yj202588.top/gtebhfrchg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.kuanghao11.cn/gtiyahfrry.html

Go:   // 手写 map[string][]T
来源：http://hz.ydjk.org.cn/gtkzarfrke.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jqgfzy.top/gthssiokkz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.tianlin.xyz/gtistupnqf.html

[D20] 统计每个元素出现次数
来源：http://hz.wangdashe.top/gtjerkwbyy.html

Py:   Counter(arr)
来源：http://hz.yj202588.top/gtmmabdmla.html

PHP:  array_count_values($arr);
来源：http://hz.cheryme.top/gterdksgwa.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ybcxt.top/gtonychiae.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.chenjidiqi.icu/gtjskxaamw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.pengpengdd.cyou/gtucdbymzq.html

Go:   // 手写 map[T]int
来源：http://hz.ehwqpu.com/gteegkhcjy.html

Ruby: arr.tally
来源：http://hz.ybcxt.top/gtatgalxtk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.tianlin.xyz/gtxxggerev.html

[D21] 判断是否包含某元素
来源：http://hz.guowangkeji.top/gtcopmsctc.html

Py:   x in arr
来源：http://hz.dianchejie.cn/gtntvhsqjd.html

PHP:  in_array($x, $arr, true);
来源：http://hz.gzhubu.top/gtdmdlqbhv.html

JS:   arr.includes(x)
来源：http://hz.smart0.xyz/gthunfblms.html

TS:   arr.includes(x)
来源：http://hz.dashuyun.cn/gtriuznbyn.html

Java: list.contains(x)
来源：http://hz.ydjk.org.cn/gtkqculvhu.html

Go:   slices.Contains(arr, x)
来源：http://hz.shzxlz.cn/gtokwfiubq.html

Ruby: arr.include?(x)
来源：http://hz.cashguo.top/gteddiknbe.html

C#:   list.Contains(x)
来源：http://hz.sufxvd.cn/gtyhcjuwpj.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ywan-chungtsiang.top/gttjomrqfy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jinqigufen.top/gtisvqhuej.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.ybcxt.top/gtgpmoaqbr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.hongshengwenyu.top/gtwmjrvwcu.html

TS:   [...arr];
来源：http://hz.hnxiangtu.top/gtltqxozza.html

Java: new ArrayList<>(list);
来源：http://hz.jinyuanbaomall.cn/gtyjfhanql.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.chenlongwang.top/gtdqkwaion.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jinghuilouyu.cn/gtwwzgchwz.html

C#:   new List<int>(list);
来源：http://hz.yj20258.top/gtfswwywav.html

[D23] reduce 累积计算
来源：http://hz.bjfxy.top/gtoteasshu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.gogol.net.cn/gtrcgextmg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.birdmap.top/gtezvaoqhf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.gzhubu.top/gtvvikzjkl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.sufxvd.cn/gtqgligmdj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.fengsongda.top/gtmtkiyeoe.html

Go:   // 手写循环
来源：http://hz.tian-w.cn/gtkvfickll.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.ywan-chungtsiang.top/gtpmedwonc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.ybcxt.top/gtecxlgdlx.html

[D24] 字典 / Map 基本操作
来源：http://hz.shanyushiyangtech.top/gtjvdagvqw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yueranfly.top/gtnnjissbu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.gogol.net.cn/gtlrkdjvsn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.nanxinkj.top/gtpcdrimss.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.52xcode.cn/gtbhmgdkyf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.aibaodan.cn/gtlcurfnma.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.gotoacloud.top/gthqombkpt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.hongshengwenyu.top/gtoyswtbyy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.nanxuanxn.top/gtdiwzenus.html

[D25] Set 集合去重与交并差
来源：http://hz.bjfxy.top/gtoebnfsta.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.shzxlz.cn/gtwforbobl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.chenjidiqi.icu/gthtaxjgdo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.snrcjt.cn/gtkkgcfbqf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.tian-w.cn/gttldtfalr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.feifeiyinyue.top/gtxnxjftnr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.havefunace.top/gtetjikcxu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yuxming.cn/gtykuwdlhd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.fzhhl.top/gtrtiqukgk.html

[D26] 数组转字符串
来源：http://hz.yj20258.top/gtqbygxlly.html

Py:   ", ".join(map(str, arr))
来源：http://hz.cqqwz.cn/gtchhruftm.html

PHP:  implode(", ", $arr);
来源：http://hz.9152youxi.cn/gtgaxvgher.html

JS:   arr.join(", ")
来源：http://hz.birdmap.top/gtsptetaor.html

TS:   arr.join(", ")
来源：http://hz.feifeiyinyue.top/gtsuztozbb.html

Java: String.join(", ", list)
来源：http://hz.pycfn.com/gtuwcrrmse.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jqgfzy.top/gtbchkubok.html

Ruby: arr.join(", ")
来源：http://hz.zhoulong.xyz/gttmrmqhtn.html

C#:   string.Join(", ", list)
来源：http://hz.xziqi.cn/gtuxwagfeq.html

================================================================================
来源：http://hz.smart0.xyz/gteqxxjzsn.html

E. 字符串处理
来源：http://hz.316326.xyz/gtjtsfzglr.html

================================================================================
来源：http://hz.shzxlz.cn/gtldtnnscc.html

[E01] 拼接字符串
来源：http://hz.wangdashe.top/gttsxfilxe.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.gotoacloud.top/gtixqnjwbp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yj202588.top/gtrxkxenck.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.dashuyun.cn/gtmucxgtlt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinqigfzy.top/gtxibkejyv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.ehwqpu.com/gtmlnmrwdh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yj20258888.top/gtjthhuwyp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.aizwys.cn/gthcjeijhl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.xuetiantiany.cn/gtkrbsabrk.html

[E02] 重复字符串
来源：http://hz.zycfv.cn/gtvpbxcotj.html

Py:   "ab" * 3
来源：http://hz.cucudq.cn/gtsmiufest.html

PHP:  str_repeat("ab", 3);
来源：http://hz.smart0.xyz/gthgucchvl.html

JS:   "ab".repeat(3)
来源：http://hz.nanxinkj.top/gtbiwzpapo.html

TS:   "ab".repeat(3)
来源：http://hz.hywenlv.cn/gtvtmibosf.html

Java: "ab".repeat(3)
来源：http://hz.jianghu66.top/gtpzcyjcdu.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.aibaodan.cn/gtmmfkoekw.html

Ruby: "ab" * 3
来源：http://hz.yj202588.top/gtotsponmp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.gzhubu.top/gtdjzroexc.html

[E03] 截取子串
来源：http://hz.yj20258.top/gtvfankjyr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.wangdashe.top/gtvdvhmzek.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.ywan-chungtsiang.top/gtcracvbqb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yongpay.top/gtcpidvory.html

TS:   s.slice(1, 4)
来源：http://hz.jiagoushi.top/gtrxfqxfzk.html

Java: s.substring(1, 4)
来源：http://hz.aizwys.cn/gtpxmbtivz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yj20258888.top/gtmqgndodx.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yvedp.cn/gthpdvbiqp.html

C#:   s.Substring(1, 3)
来源：http://hz.ppjwa.cn/gthpfumjvx.html

[E04] 查找子串位置
来源：http://hz.chenzaomai.com/gtkzpamwrh.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zhengqikj.top/gtmdncnyqj.html

PHP:  strpos($s, "x");
来源：http://hz.nanxinkj.top/gtgghhgiyk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.iojbl.cn/gtbqtmojjf.html

TS:   s.indexOf("x")
来源：http://hz.hammf.cn/gtzwmlowjl.html

Java: s.indexOf("x")
来源：http://hz.jqgufenzy.top/gtcxbppciq.html

Go:   strings.Index(s, "x")
来源：http://hz.yangfankeji.com/gtcusenejr.html

Ruby: s.index("x")
来源：http://hz.jinghuilouyu.cn/gtzqachozr.html

C#:   s.IndexOf("x")
来源：http://hz.zhijiandao.cn/gttkqqclge.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.cheryme.top/gteqvlngqh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.shzxlz.cn/gtogtzxwyk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.snrcjt.cn/gthfcpeyev.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.aizwys.cn/gtslkghesp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.haohaochexian.top/gtbecmzkos.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.andypj.xyz/gtjalaeatx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.feifeiyinyue.top/gtpbfyyilv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.hywenlv.cn/gtiyekeymn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ydzc1.top/gtqcehgdpp.html

[E06] 替换子串
来源：http://hz.sweek.top/gtxhviizjx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.sweek.top/gtxpdazjug.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.svipenyu.cn/gtxrclvtfe.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.andypj.xyz/gtnsbcpbdp.html

TS:   s.replaceAll("a", "b")
来源：http://hz.cashguo.top/gtljmdaovo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ywan-chungtsiang.top/gtdvcxqlyu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.ybcxt.top/gtadytpywo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.tianlin.xyz/gtjjeflxww.html

C#:   s.Replace("a", "b")
来源：http://hz.fengsongda.top/gtzxhyghnv.html

[E07] 按分隔符拆分
来源：http://hz.jqgufenzy.top/gtmogawyez.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.nwbrower.top/gtqjztdwuj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.smart0.xyz/gthtaunnqp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.daxiang520.top/gtscprmthi.html

TS:   s.split(",")
来源：http://hz.chenzaomai.com/gteopqjefb.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.hywenlv.cn/gtfdknlwkl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.daxiang520.top/gtwelydojl.html

Ruby: s.split(",");  s.split
来源：http://hz.nanxuanxn.top/gtmnacmhpt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.xinyue.icu/gtayjysrsh.html

[E08] 数组按分隔符合并
来源：http://hz.pengpengdd.cyou/gtfmtagimo.html

Py:   ",".join(items)
来源：http://hz.zhoulong.xyz/gtyrvrzryj.html

PHP:  implode(",", $items);
来源：http://hz.zycfv.cn/gtiiwjwczu.html

JS:   items.join(",")
来源：http://hz.hfpthk.cn/gtydbwmsxh.html

TS:   items.join(",")
来源：http://hz.xuetiantiany.cn/gtnafandtj.html

Java: String.join(",", items)
来源：http://hz.ehwqpu.com/gtemnterat.html

Go:   strings.Join(items, ",")
来源：http://hz.jqgfzy.top/gtuxbqpani.html

Ruby: items.join(",")
来源：http://hz.52xcode.cn/gtqnpuwetk.html

C#:   string.Join(",", items)
来源：http://hz.jqgufenzy.top/gtiuhhjhzl.html

[E09] 去除所有空白字符
来源：http://hz.wangdashe.top/gtmiyypaty.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jinyuanbaomall.cn/gttpnpitru.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.gotoacloud.top/gtbvcjpghc.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.tanke756.top/gtnkvgdyli.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.wangshuangyany.cn/gtpcsftjpo.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.gotoacloud.top/gtrqukybrd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.ppjwa.cn/gtpwtrswtx.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zhengqikj.top/gtiecdzant.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hywenlv.cn/gtifhetmma.html

[E10] 左侧补零 / 定长填充
来源：http://hz.gaohongyu789.top/gtwnaloetl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.hywenlv.cn/gtoxncrimf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.mhx1999.top/gttxidgvnb.html

JS:   "7".padStart(3, "0")
来源：http://hz.ydzc1.top/gtbyyllqji.html

TS:   "7".padStart(3, "0")
来源：http://hz.jinqigufen.top/gtrbmanvzc.html

Java: String.format("%03d", 7)
来源：http://hz.ehwqpu.com/gtwgeqalsw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ywan-chungtsiang.top/gtfuysmiij.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jinghuilouyu.cn/gtfnrwqogq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.shzxlz.cn/gtqsutgekx.html

[E11] 反转字符串
来源：http://hz.ydzc1.top/gtsbgothqm.html

Py:   s[::-1]
来源：http://hz.gaohongyu789.top/gtjihnfybt.html

PHP:  strrev($s);
来源：http://hz.haohaochexian.top/gtxoehggau.html

JS:   [...s].reverse().join("")
来源：http://hz.xuanzx.com/gtxesubhcb.html

TS:   [...s].reverse().join("")
来源：http://hz.ydzc1.top/gtkswfqoml.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.shuidangran.top/gtbejghxur.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yj20258888.top/gtsfnphhhd.html

Ruby: s.reverse
来源：http://hz.zdqjudy.top/gtsgqutiux.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.ppjwa.cn/gtjeiemnxn.html

[E12] 统计某字符出现次数
来源：http://hz.sxryk.cn/gtercaswiv.html

Py:   s.count("a")
来源：http://hz.cashguo.top/gtdpsahucr.html

PHP:  substr_count($s, "a");
来源：http://hz.andypj.xyz/gtvrtkvkqu.html

JS:   s.split("a").length - 1
来源：http://hz.iojbl.cn/gtpzjwxdox.html

TS:   s.split("a").length - 1
来源：http://hz.fengsongda.top/gtbayksmgh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.ydjk.org.cn/gtscmipvmv.html

Go:   strings.Count(s, "a")
来源：http://hz.cqqwz.cn/gtgnpfuczc.html

Ruby: s.count("a")
来源：http://hz.jinghuilouyu.cn/gtbdjyfzlg.html

C#:   s.Count(c => c == 'a')
来源：http://hz.shanyushiyangkeji.top/gtycspjxbk.html

[E13] 逐字符遍历
来源：http://hz.yongpay.top/gtnbnkcdlv.html

Py:   for ch in s: print(ch)
来源：http://hz.jinyuanbaomall.cn/gttgbtwgyw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.andypj.xyz/gtgaypaarv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.snrcjt.cn/gtaxubpkee.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yvedp.cn/gtbiwboasx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.redwolf501.top/gtwnfxxjpz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yj20258888.top/gtsmnidelp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.kuanghao11.cn/gtstmhuged.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yuanzhike.top/gtgjjmsfkm.html

[E14] URL 编码与 Base64
来源：http://hz.andypj.xyz/gtvtsefipi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.chenzaomai.com/gtyinccivd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.pengpengdd.cyou/gtjhthzywq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.shzxlz.cn/gtsdtkljmg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.sxryk.cn/gtlhjwsloy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.guannengcc.top/gthmsoplga.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhengqikj.top/gtigfmbfsp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.wangdashe.top/gtlwzvilyx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.hongshengwenyu.top/gtgjrndjfo.html

[E15] HTML 转义 / 反转义
来源：http://hz.zhoulong.xyz/gtrebyseyd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.haohaochexian.top/gtqorpdobg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hammf.cn/gtdhutcqys.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.havefunace.top/gtiuyjpqhr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.sweek.top/gtshaynpox.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.gaohongyu789.top/gtcwcxhzir.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.aizwys.cn/gtgutxjnhb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.ybcxt.top/gterswdrky.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jyoumei.cn/gtjmtpsijq.html

[E16] 数字千分位
来源：http://hz.daxiang520.top/gtkmywkfsg.html

Py:   f"{1234567:,}"
来源：http://hz.52xcode.cn/gtevdwrbne.html

PHP:  number_format(1234567);
来源：http://hz.chenlongwang.top/gtqitqopqu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yongpay.top/gtpmyvpnth.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ydzc1.top/gtreahyphd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.sweek.top/gtfvzlxhmd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.sysykeji.top/gtrxbbathg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.meibo888.top/gtoorhbexo.html

C#:   1234567.ToString("N0")
来源：http://hz.hammf.cn/gtgegdjsty.html

[E17] 首字母大写
来源：http://hz.zhoulong.xyz/gtuyeolfnc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.ydjk.org.cn/gtzknmzbri.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.gzhubu.top/gtdvhggtft.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.redwolf501.top/gtmnslqvgv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shangyingyoupin.top/gtdnwygbgf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.52xcode.cn/gtemonmuod.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.9152youxi.cn/gtmwjddezs.html

Ruby: s.capitalize
来源：http://hz.cqqwz.cn/gtdmsfofgd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.cqqwz.cn/gtfjkkfzdp.html

[E18] 模板占位符替换
来源：http://hz.yj20258888.top/gtmdxqjmci.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.c1oappe.top/gtbxbxdbzw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.aizwys.cn/gtkmkbbnvb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yvedp.cn/gtylmarigd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zycfv.cn/gtvnpfyzhm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.gotoacloud.top/gthtgtcyyu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.tian-w.cn/gtklkeyawu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.nanxuanxn.top/gtgpcbdocy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yanxiufei.cn/gtcdhsixrg.html

[E19] 多行文本按行拆分
来源：http://hz.redwolf501.top/gtfuqrnecd.html

Py:   s.splitlines()
来源：http://hz.dashuyun.cn/gtvhjzaqjl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.ivvv.top/gtdxwzlbqt.html

JS:   s.split(/\r?\n/)
来源：http://hz.guowangkeji.top/gtnukdkeha.html

TS:   s.split(/\r?\n/)
来源：http://hz.shzxlz.cn/gtbgpbrowu.html

Java: s.lines().toList()
来源：http://hz.zhijiandao.cn/gttuxwnttu.html

Go:   strings.Split(s, "\n")
来源：http://hz.bjfxy.top/gtdgmztlpj.html

Ruby: s.lines
来源：http://hz.birdmap.top/gtrjbnrpiy.html

C#:   s.Split('\n')
来源：http://hz.xuetiantiany.cn/gtqplshcag.html

[E20] 判断字符串是否为空
来源：http://hz.jlsjyb.cn/gtpimsovoc.html

Py:   if not s:
来源：http://hz.zhijiandao.cn/gtwegmzdbx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jiagoushi.top/gtuhushimq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yj202588.top/gtdypbsbfc.html

TS:   if (s === "") {}
来源：http://hz.yj20258.top/gtcpvzhida.html

Java: if (s.isEmpty()) {}
来源：http://hz.daria6918.cn/gtfqwffneh.html

Go:   if s == "" {}
来源：http://hz.jyoumei.cn/gtnhbkosss.html

Ruby: if s.empty?
来源：http://hz.daria6918.cn/gttrngidaf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ppjwa.cn/gtdsjsyuyr.html

[E21] 超长截断加省略号
来源：http://hz.kuanghao11.cn/gthwnxlbvu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.sysykeji.top/gtqdsmdhnn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.xylfe.cn/gtrgnegyvl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shanyushiyangkeji.top/gtnfrlotat.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.aibaodan.cn/gtswimlomm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jinqigufen.top/gtigqassup.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yueranfly.top/gtdofuxgpu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yuxming.cn/gtcvnydszm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.guannengcc.top/gtapnllnhz.html

[E22] 字节长度与字符长度
来源：http://hz.zhiwuduotai.top/gtoszbtbig.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.cdnleiting.top/gtkzpfvzby.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.aibaodan.cn/gtvhohegxo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xuetiantiany.cn/gtuckslcai.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.gzhubu.top/gtnoudwblz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.shanyushiyangtech.top/gtacveudto.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yangfankeji.com/gtwtaignrv.html

Ruby: s.bytesize;  s.length
来源：http://hz.chenlongwang.top/gtjqnqiqkx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jqgfzy.top/gtserhjljn.html

================================================================================
来源：http://hz.shuidangran.top/gtvfkkbndl.html

F. 文件与目录
来源：http://hz.chenzaomai.com/gtxtvnelpd.html

================================================================================
来源：http://hz.yuanzhike.top/gtyxvltdiz.html

[F01] 读取整个文件
来源：http://hz.tianlin.xyz/gtuvrdzbnr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.ivvv.top/gtxlsmflpc.html

PHP:  file_get_contents("a.txt");
来源：http://hz.fengsongda.top/gtdfjynazi.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.bjfxy.top/gtiivrzdzp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.meibo888.top/gtcejekmie.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.9152youxi.cn/gtozjfdlbe.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.ybcxt.top/gtpwvdalft.html

Ruby: File.read("a.txt")
来源：http://hz.xuetiantiany.cn/gtjcfkryuo.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.guowangkeji.top/gtyrvviypr.html

[F02] 逐行读取文件
来源：http://hz.jinqigfzy.top/gtweeubgqo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.xuanzx.com/gtxypyyljd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.redwolf501.top/gtdozccqnq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.guowangkeji.top/gtfopefaej.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.fzhhl.top/gtkdxoolit.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.daxiang520.top/gtbprdcjic.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.xuanzx.com/gtivnewzdm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zhoulong.xyz/gtetgwdylg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.hywenlv.cn/gtdbjnfjtg.html

[F03] 写入文件（覆盖）
来源：http://hz.ydjk.org.cn/gtozdvrzyn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.bjfxy.top/gttvmzsjjw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.cheryme.top/gtgkpjyabx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.chenzaomai.com/gthqqvefxp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xylfe.cn/gtozoftrsu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.nwbrower.top/gtpmnfmjxl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.0kj1m.cn/gtuhrlwshl.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.xziqi.cn/gtjydrahkn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.shuidangran.top/gtbqqebxyv.html

[F04] 追加写入文件
来源：http://hz.cashguo.top/gtownxkjfw.html


<!-- 参考信息 -->