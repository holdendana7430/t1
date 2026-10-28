代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jinyuanbaomall.cn/gtzbrztvff.html

[D20] 统计每个元素出现次数
来源：http://hz.yueranfly.top/gtsbfutehy.html

Py:   Counter(arr)
来源：http://hz.svipenyu.cn/gtkxhkbegq.html

PHP:  array_count_values($arr);
来源：http://hz.shanyushiyangkeji.top/gtozvuizkc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yj20258888.top/gtahhvzmdv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhixingplan.top/gtxkutoypm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zhiwuduotai.top/gthmazomid.html

Go:   // 手写 map[T]int
来源：http://hz.sxryk.cn/gtksparopp.html

Ruby: arr.tally
来源：http://hz.jianghu66.top/gtmgowuptt.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.hysaishi.cn/gtjrmfidst.html

[D21] 判断是否包含某元素
来源：http://hz.aibaodan.cn/gtayxfdffm.html

Py:   x in arr
来源：http://hz.bjfxy.top/gtlrlsnkhz.html

PHP:  in_array($x, $arr, true);
来源：http://hz.pycfn.com/gtmlmhkkcz.html

JS:   arr.includes(x)
来源：http://hz.ydzc1.top/gtrgoogbzh.html

TS:   arr.includes(x)
来源：http://hz.cheryme.top/gtwbznwyvl.html

Java: list.contains(x)
来源：http://hz.quarkkingdee.top/gtebyotdey.html

Go:   slices.Contains(arr, x)
来源：http://hz.sxryk.cn/gtpvrnnfka.html

Ruby: arr.include?(x)
来源：http://hz.jlsjyb.cn/gtlmnljupa.html

C#:   list.Contains(x)
来源：http://hz.xziqi.cn/gtzulzakww.html

[D22] 复制数组（避免共享引用）
来源：http://hz.gaohongyu789.top/gtuhshcgmb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.guannengcc.top/gtxvewagiu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.fengsongda.top/gtdtqjwqoj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.bjfxy.top/gtvzlgmuri.html

TS:   [...arr];
来源：http://hz.shanyushiyangtech.top/gtlvapxymq.html

Java: new ArrayList<>(list);
来源：http://hz.andypj.xyz/gthdobupav.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.nanxuanxn.top/gtkiagnnui.html

Ruby: arr.dup;  arr.clone
来源：http://hz.shanyushiyangkeji.top/gtrnfgsiex.html

C#:   new List<int>(list);
来源：http://hz.fengsongda.top/gtgohwhoyu.html

[D23] reduce 累积计算
来源：http://hz.xinyue.icu/gtitdwvoos.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.svipenyu.cn/gtfhfjaqco.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jinyuanbaomall.cn/gteklmixem.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xuetiantiany.cn/gttpbqewas.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hnxiangtu.top/gtmpnswhes.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.wangdashe.top/gtvhkihdje.html

Go:   // 手写循环
来源：http://hz.guowangkeji.top/gtbtfqjycm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.sysykeji.top/gtrenmhmmv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.hnxiangtu.top/gtoahaqfeo.html

[D24] 字典 / Map 基本操作
来源：http://hz.andypj.xyz/gtxcffmxvc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yuanzhike.top/gtbreujauc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.ydzc1.top/gtdptfshgi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.sufxvd.cn/gtsbzuhxnq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.xziqi.cn/gtgytiuslb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yueranfly.top/gtdqlrczfs.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.shanyushiyangtech.top/gtstrcediz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.fzhhl.top/gtpwnvxaiw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.birdmap.top/gtlxsssshd.html

[D25] Set 集合去重与交并差
来源：http://hz.svipenyu.cn/gtnazrclvb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.daxiang520.top/gtsavwszgj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yj20258.top/gtoiooguts.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.cheryme.top/gtwrdclkgl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zhixingplan.top/gthbgyeybe.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yueranfly.top/gtaqomoige.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.xuetiantiany.cn/gtgobxholc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.xuanzx.com/gtmliuzkpz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jiagoushi.top/gtyjejvjfo.html

[D26] 数组转字符串
来源：http://hz.wangdashe.top/gtaxzgtcsa.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zhixingplan.top/gtejsqpowm.html

PHP:  implode(", ", $arr);
来源：http://hz.ydjk.org.cn/gtyavwksfx.html

JS:   arr.join(", ")
来源：http://hz.shzxlz.cn/gtzdzsuovu.html

TS:   arr.join(", ")
来源：http://hz.yonumen.top/gtpyurshqk.html

Java: String.join(", ", list)
来源：http://hz.jianghu66.top/gtxwbafack.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zhixingplan.top/gtbpbgauxm.html

Ruby: arr.join(", ")
来源：http://hz.ppjwa.cn/gtinqwzdsm.html

C#:   string.Join(", ", list)
来源：http://hz.tanke756.top/gtlorigoko.html

================================================================================
来源：http://hz.havefunace.top/gtfbooygxd.html

E. 字符串处理
来源：http://hz.jqgufenzy.top/gthawjlvcq.html

================================================================================
来源：http://hz.cdnleiting.top/gtonhaekwd.html

[E01] 拼接字符串
来源：http://hz.zhoulong.xyz/gtmihlntnw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yuanzhike.top/gtzaewdejh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.aizwys.cn/gtmfqupytl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yj20258888.top/gtefwgfbwb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.iojbl.cn/gtnkcahwga.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.chenjidiqi.icu/gttlaqdgcg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.meibo888.top/gtktnbckth.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.9152youxi.cn/gtrvhauque.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.aizwys.cn/gtzxxabzhw.html

[E02] 重复字符串
来源：http://hz.316326.xyz/gtofqynqac.html

Py:   "ab" * 3
来源：http://hz.yangfankeji.com/gtxairmyri.html

PHP:  str_repeat("ab", 3);
来源：http://hz.shzxlz.cn/gtxspufwwh.html

JS:   "ab".repeat(3)
来源：http://hz.snrcjt.cn/gtcpjyrinv.html

TS:   "ab".repeat(3)
来源：http://hz.haohaochexian.top/gttmzkzcpk.html

Java: "ab".repeat(3)
来源：http://hz.gogol.net.cn/gtgsdwqcku.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yvedp.cn/gtcjivojlq.html

Ruby: "ab" * 3
来源：http://hz.yuxming.cn/gtzflhvdgy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zhijiandao.cn/gtwvaeqenf.html

[E03] 截取子串
来源：http://hz.yueranfly.top/gtyevsubif.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.hysaishi.cn/gtpktddeoj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.dashuyun.cn/gteyoxeaum.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.aibaodan.cn/gtetebxcpi.html

TS:   s.slice(1, 4)
来源：http://hz.xziqi.cn/gtpgjroith.html

Java: s.substring(1, 4)
来源：http://hz.tianlin.xyz/gtqweeayqy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.havefunace.top/gtzvlipbxv.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yueranfly.top/gtttbkkina.html

C#:   s.Substring(1, 3)
来源：http://hz.aibaodan.cn/gtrlmkvzxo.html

[E04] 查找子串位置
来源：http://hz.yangfankeji.com/gtbqkycqzq.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jinqigufen.top/gtrugggfsx.html

PHP:  strpos($s, "x");
来源：http://hz.gogol.net.cn/gtnbcrwrkr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.kuanghao11.cn/gtugfekyzm.html

TS:   s.indexOf("x")
来源：http://hz.yuanzhike.top/gthzpzkiwy.html

Java: s.indexOf("x")
来源：http://hz.c1oappe.top/gtzuqegcsv.html

Go:   strings.Index(s, "x")
来源：http://hz.yongpay.top/gtlmeiafml.html

Ruby: s.index("x")
来源：http://hz.cashguo.top/gtdqqtazpc.html

C#:   s.IndexOf("x")
来源：http://hz.mhx1999.top/gtsoyxuwza.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.haohaochexian.top/gtrxcrjtts.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.316326.xyz/gtdvvqyplc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zdqjudy.top/gtxwuduklm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.fzhhl.top/gtrhnikvjz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.snrcjt.cn/gtfckmsljw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.svipenyu.cn/gtslpkqkcp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.nanxinkj.top/gtzttgsosb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ybcxt.top/gtphoitvzj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.aibaodan.cn/gtvcbhzwoi.html

[E06] 替换子串
来源：http://hz.nanxinkj.top/gtqgrelwmx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jinqigfzy.top/gtekjdyfct.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.birdmap.top/gtywuejbhu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xinyue.icu/gtqzjazugk.html

TS:   s.replaceAll("a", "b")
来源：http://hz.xylfe.cn/gtmpxslbpq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cashguo.top/gtahtgyqaz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.shanyushiyangkeji.top/gttdfqebua.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.c1oappe.top/gtvxtwsmth.html

C#:   s.Replace("a", "b")
来源：http://hz.jyoumei.cn/gtolsgywjx.html

[E07] 按分隔符拆分
来源：http://hz.jlsjyb.cn/gtgltihgrq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.daxiang520.top/gtolagvfcp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.xylfe.cn/gttgxhdlbv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yueranfly.top/gtzdhhyxpo.html

TS:   s.split(",")
来源：http://hz.zhengqikj.top/gtucageedv.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.havefunace.top/gtjokksoyj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zycfv.cn/gtumwdctvh.html

Ruby: s.split(",");  s.split
来源：http://hz.tianlin.xyz/gtyteyjjrf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.dianchejie.cn/gtqzyzpojk.html

[E08] 数组按分隔符合并
来源：http://hz.wangdashe.top/gtleygkkyt.html

Py:   ",".join(items)
来源：http://hz.yanxiufei.cn/gtudyiszvp.html

PHP:  implode(",", $items);
来源：http://hz.nanxuanxn.top/gtkhtjsctt.html

JS:   items.join(",")
来源：http://hz.nwbrower.top/gtfulynplg.html

TS:   items.join(",")
来源：http://hz.zhongyouzk.top/gthatbilwo.html

Java: String.join(",", items)
来源：http://hz.daxiang520.top/gtkhkvcnqt.html

Go:   strings.Join(items, ",")
来源：http://hz.jinghuilouyu.cn/gtmkhbnixi.html

Ruby: items.join(",")
来源：http://hz.shuidangran.top/gtufnkyfdm.html

C#:   string.Join(",", items)
来源：http://hz.9152youxi.cn/gtckyistjx.html

[E09] 去除所有空白字符
来源：http://hz.redwolf501.top/gtyyrgawbj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.daria6918.cn/gtyezblyww.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shanyushiyangkeji.top/gtppxhuzzw.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jinghuilouyu.cn/gtuqflyerc.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.tian-w.cn/gtywnyibtp.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.52xcode.cn/gtbsmuiguq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.cdnleiting.top/gtmxtvqbrx.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zhongyouzk.top/gtbgtornhp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.guowangkeji.top/gtxskdjqaq.html

[E10] 左侧补零 / 定长填充
来源：http://hz.316326.xyz/gtfkzmdgpx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.nwbrower.top/gttuzcynhs.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.nwbrower.top/gtvyjemcqo.html

JS:   "7".padStart(3, "0")
来源：http://hz.shzxlz.cn/gtvfkhjqgn.html

TS:   "7".padStart(3, "0")
来源：http://hz.yuanzhike.top/gtetvznhub.html

Java: String.format("%03d", 7)
来源：http://hz.cucudq.cn/gtndxzlwbg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.shuidangran.top/gtbntoirar.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.fengsongda.top/gtvkclwevq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.fzhhl.top/gtrwbxjmzz.html

[E11] 反转字符串
来源：http://hz.andypj.xyz/gtulntoolj.html

Py:   s[::-1]
来源：http://hz.jianghu66.top/gthgdeovcn.html

PHP:  strrev($s);
来源：http://hz.zdqjudy.top/gtzblycbsi.html

JS:   [...s].reverse().join("")
来源：http://hz.meibo888.top/gtytlkvrhe.html

TS:   [...s].reverse().join("")
来源：http://hz.havefunace.top/gtzkuhfqus.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.ehwqpu.com/gtbrramkss.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.kuanghao11.cn/gtufqonzcy.html

Ruby: s.reverse
来源：http://hz.dianchejie.cn/gtrresdegj.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.meibo888.top/gtymysnhbp.html

[E12] 统计某字符出现次数
来源：http://hz.snrcjt.cn/gtzpzagjtp.html

Py:   s.count("a")
来源：http://hz.xziqi.cn/gtnxvixklj.html

PHP:  substr_count($s, "a");
来源：http://hz.tian-w.cn/gtlcqjkerq.html

JS:   s.split("a").length - 1
来源：http://hz.xziqi.cn/gthwmusadi.html

TS:   s.split("a").length - 1
来源：http://hz.jinqigufen.top/gtvpgonrle.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.hnxiangtu.top/gthqrautsa.html

Go:   strings.Count(s, "a")
来源：http://hz.xziqi.cn/gtktoaqtzp.html

Ruby: s.count("a")
来源：http://hz.tianlin.xyz/gtzerjbxif.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zhengqikj.top/gtxwxwmqfm.html

[E13] 逐字符遍历
来源：http://hz.jinyuanbaomall.cn/gtanpuuhix.html

Py:   for ch in s: print(ch)
来源：http://hz.shzxlz.cn/gtnhcmultk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.nanxuanxn.top/gtmeiqofvg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.aibaodan.cn/gtjiierzim.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ppjwa.cn/gtzzldrnro.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jinqigufen.top/gttqfuhzed.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.wangdashe.top/gtdokzrwla.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.cashguo.top/gtjkgdninv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.0kj1m.cn/gtvtpysccn.html

[E14] URL 编码与 Base64
来源：http://hz.fengsongda.top/gtkkaxzgmg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jinyuanbaomall.cn/gtnpstyzbn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.ybcxt.top/gthcbwqbzj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.havefunace.top/gtacndisml.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.vqdsnc.cn/gtrskrbhpu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.svipenyu.cn/gtxalbvrfa.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhoulong.xyz/gtuovkiqyj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.bjfxy.top/gtpwwehbtb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.haohaochexian.top/gthfulhbcu.html

[E15] HTML 转义 / 反转义
来源：http://hz.sxryk.cn/gtobmtbypp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jlsjyb.cn/gtbfrmfmjc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jiagoushi.top/gtobmczpww.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zdqjudy.top/gtbiddjoji.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yj20258.top/gttajhbwja.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.nwbrower.top/gtxtuzeizc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hnxiangtu.top/gtzuipdjar.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.pengpengdd.cyou/gtumfuymdi.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zhaomingkeji.xyz/gtqxgrfjzm.html

[E16] 数字千分位
来源：http://hz.ydjk.org.cn/gtxswtggoo.html

Py:   f"{1234567:,}"
来源：http://hz.gaohongyu789.top/gtrquuhmes.html

PHP:  number_format(1234567);
来源：http://hz.ydjk.org.cn/gtmvqxnyev.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.tianlin.xyz/gtwgflvzdg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hywenlv.cn/gthvzopysy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.mhx1999.top/gtgewgmssu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhaomingkeji.xyz/gtbvsyahxu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.shangyingyoupin.top/gtmedzhkym.html

C#:   1234567.ToString("N0")
来源：http://hz.cheryme.top/gtppvcngwb.html

[E17] 首字母大写
来源：http://hz.316326.xyz/gtjoefeiwm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.xylfe.cn/gtpnvtlcvw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.ydjk.org.cn/gtnvfehxya.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cucudq.cn/gttdkmrvik.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenjidiqi.icu/gtivmfynio.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.wangdashe.top/gtygyuizvd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.meibo888.top/gtguemllgg.html

Ruby: s.capitalize
来源：http://hz.daria6918.cn/gtxevhqhgg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.hfpthk.cn/gttkmqwcne.html

[E18] 模板占位符替换
来源：http://hz.hfpthk.cn/gtpfurbjml.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.chenjidiqi.icu/gtiphprztl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yueranfly.top/gtnbqwhegs.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jlsjyb.cn/gtqorbhitu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jianghu66.top/gtgcnxrhnd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jlsjyb.cn/gttwjogssj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.hnxiangtu.top/gtfbnqupmt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zhiwuduotai.top/gtwjhrpwin.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ywan-chungtsiang.top/gtrdqjmjrh.html

[E19] 多行文本按行拆分
来源：http://hz.zhengqikj.top/gtkjypbzhf.html

Py:   s.splitlines()
来源：http://hz.guowangkeji.top/gtrxmgltth.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.guowangkeji.top/gtcnzeudpb.html

JS:   s.split(/\r?\n/)
来源：http://hz.nwbrower.top/gtgsvvwxpz.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhoulong.xyz/gtmkodgmjo.html

Java: s.lines().toList()
来源：http://hz.sysykeji.top/gtwwuxiqrd.html

Go:   strings.Split(s, "\n")
来源：http://hz.xuanzx.com/gtijvhvtwz.html

Ruby: s.lines
来源：http://hz.fengsongda.top/gtjhuzwqgz.html

C#:   s.Split('\n')
来源：http://hz.zhaomingkeji.xyz/gtjkphrvjd.html

[E20] 判断字符串是否为空
来源：http://hz.ybcxt.top/gtniehvjyp.html

Py:   if not s:
来源：http://hz.yangfankeji.com/gtbjqavuyq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.chenzaomai.com/gttsyaitwa.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jyoumei.cn/gtmvyfeejh.html

TS:   if (s === "") {}
来源：http://hz.tianlin.xyz/gtznsmnlrr.html

Java: if (s.isEmpty()) {}
来源：http://hz.cucudq.cn/gtzjxmvwoh.html

Go:   if s == "" {}
来源：http://hz.vqdsnc.cn/gtgehnpzeu.html

Ruby: if s.empty?
来源：http://hz.cdnleiting.top/gtfvvsamhq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.pengpengdd.cyou/gtnaftznaa.html

[E21] 超长截断加省略号
来源：http://hz.ybcxt.top/gtbidgciyt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.hammf.cn/gtkxmjzahl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yuxming.cn/gtlttgohmu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhijiandao.cn/gttvyqytuk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.tian-w.cn/gtveswvzot.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yj20258888.top/gtetszvpda.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.chenlongwang.top/gtrpccvvvy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.hfpthk.cn/gtviwmihrb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yj20258888.top/gtogywxcmg.html

[E22] 字节长度与字符长度
来源：http://hz.yanxiufei.cn/gtdwozpqwx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.wangdashe.top/gtewdoknxr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.quarkkingdee.top/gtxglnxwog.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhaomingkeji.xyz/gtrcvpurmy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.bjfxy.top/gtkesnevvh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.andypj.xyz/gtzrkvzkzg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yuxming.cn/gtucrnziiy.html

Ruby: s.bytesize;  s.length
来源：http://hz.guannengcc.top/gtxsimfmpq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xziqi.cn/gtoqihrrjy.html

================================================================================
来源：http://hz.mhx1999.top/gtmrerkdhi.html

F. 文件与目录
来源：http://hz.hnxiangtu.top/gtesajviix.html

================================================================================
来源：http://hz.pycfn.com/gtdtupehfp.html

[F01] 读取整个文件
来源：http://hz.cashguo.top/gtuacebjnh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hnxiangtu.top/gtxmnppuhg.html

PHP:  file_get_contents("a.txt");
来源：http://hz.gaohongyu789.top/gtvbfarpes.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.wangshuangyany.cn/gtmfvozteq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zycfv.cn/gtezffzlil.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhaomingkeji.xyz/gtthlpapmg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jianghu66.top/gtlsgtryei.html

Ruby: File.read("a.txt")
来源：http://hz.aizwys.cn/gtefmosxal.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.sxryk.cn/gtocskcflm.html

[F02] 逐行读取文件
来源：http://hz.zhengqikj.top/gtlifpzfmz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.tian-w.cn/gtivufxnfc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jqgfzy.top/gtiqfneocl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhaomingkeji.xyz/gtxbysuomn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.iojbl.cn/gtbptbadjq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.fengsongda.top/gteboeemtp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hnqzz.top/gtennigawm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.haohaochexian.top/gtlccjqvbt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.sxryk.cn/gttamxrpgc.html

[F03] 写入文件（覆盖）
来源：http://hz.yj202588.top/gtbhxqqxzu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hysaishi.cn/gtqpvroqlv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhoulong.xyz/gtnafaywmp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hammf.cn/gtpqkdnsth.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhaomingkeji.xyz/gtnyigrwnk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.xingfuxueyuan.xyz/gtxsxqaelx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zhengqikj.top/gtnydbjahd.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hywenlv.cn/gtlyujyeym.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.bjfxy.top/gtchsucrcd.html

[F04] 追加写入文件
来源：http://hz.hysaishi.cn/gtmferoolc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jinyuanbaomall.cn/gtxwhmjlyf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhijiandao.cn/gtevslhdlo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shanyushiyangkeji.top/gtdknoytjj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gotoacloud.top/gtnuvvjjpm.html


<!-- 参考信息 -->