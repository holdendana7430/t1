代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.gaohongyu789.top/gtappdtydl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yanxiufei.cn/gtpouegkcp.html

Go:   // 手写 map[string][]T
来源：http://hz.jqgufenzy.top/gtpkzqbqld.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.shanyushiyangkeji.top/gtjrnhexaf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yangfankeji.com/gtsklgvtlq.html

[D20] 统计每个元素出现次数
来源：http://hz.hysaishi.cn/gtrxdwutvk.html

Py:   Counter(arr)
来源：http://hz.xuanzx.com/gtqainznsg.html

PHP:  array_count_values($arr);
来源：http://hz.hnqzz.top/gtoexotxhs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hfpthk.cn/gthpmcyivv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.snrcjt.cn/gtyoyjirli.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jqgufenzy.top/gtzujsbgkn.html

Go:   // 手写 map[T]int
来源：http://hz.yonumen.top/gtpjnfeuee.html

Ruby: arr.tally
来源：http://hz.ivvv.top/gtddbdwowb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.gogol.net.cn/gtpppkckyd.html

[D21] 判断是否包含某元素
来源：http://hz.daria6918.cn/gtavlnssym.html

Py:   x in arr
来源：http://hz.yj20258888.top/gtnrorcpvd.html

PHP:  in_array($x, $arr, true);
来源：http://hz.dianchejie.cn/gtdajxyfmu.html

JS:   arr.includes(x)
来源：http://hz.zhengqikj.top/gtyqilkikv.html

TS:   arr.includes(x)
来源：http://hz.jinyuanbaomall.cn/gtewmxaqym.html

Java: list.contains(x)
来源：http://hz.iojbl.cn/gtxtnpenzs.html

Go:   slices.Contains(arr, x)
来源：http://hz.dashuyun.cn/gtycnsihdd.html

Ruby: arr.include?(x)
来源：http://hz.gaohongyu789.top/gthxbmaubl.html

C#:   list.Contains(x)
来源：http://hz.yueranfly.top/gttpqaxoor.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ivvv.top/gtaxvtzico.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.svipenyu.cn/gtgymyhqnh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.cheryme.top/gtiffhryot.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yuanzhike.top/gtzsaibzep.html

TS:   [...arr];
来源：http://hz.cashguo.top/gtjqeoxowa.html

Java: new ArrayList<>(list);
来源：http://hz.zhengqikj.top/gtipfbjpij.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jinghuilouyu.cn/gtehjpxxbj.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yj20258888.top/gtbvzngtbl.html

C#:   new List<int>(list);
来源：http://hz.yuanzhike.top/gtceloided.html

[D23] reduce 累积计算
来源：http://hz.zhaomingkeji.xyz/gtynzfwxos.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.andypj.xyz/gtsqmxxgyd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zhengqikj.top/gthvskjqqf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cucudq.cn/gtrqgobpch.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.gzhubu.top/gtshclerxb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.tanke756.top/gtoajghzpx.html

Go:   // 手写循环
来源：http://hz.tianlin.xyz/gtvozyjefy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.ivvv.top/gtcpswcxrp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.cqqwz.cn/gttkwmpslm.html

[D24] 字典 / Map 基本操作
来源：http://hz.hysaishi.cn/gtvyjzjtvo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.iojbl.cn/gtfhckdebz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.zhijiandao.cn/gtctojhyfw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.svipenyu.cn/gttkltwfng.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.dianchejie.cn/gtnywylocl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jlsjyb.cn/gtbihmxwyt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ppjwa.cn/gtzvluqhkv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.9152youxi.cn/gtbltxndii.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.sxryk.cn/gthpptjtsq.html

[D25] Set 集合去重与交并差
来源：http://hz.zycfv.cn/gttimaprkt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.ehwqpu.com/gtwdmhnudv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.mhx1999.top/gtljxskglm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.shuidangran.top/gtpinhsddl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.cdnleiting.top/gtshqxuzvu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.haohaochexian.top/gtkzshhjml.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.sweek.top/gtayuhpbvl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.hfpthk.cn/gttrpfsxit.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.ydzc1.top/gtmolmytvh.html

[D26] 数组转字符串
来源：http://hz.yuanzhike.top/gtpiqboakw.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yanxiufei.cn/gtcdbeihdf.html

PHP:  implode(", ", $arr);
来源：http://hz.zhixingplan.top/gtuyaihnht.html

JS:   arr.join(", ")
来源：http://hz.yanxiufei.cn/gtfpejznmy.html

TS:   arr.join(", ")
来源：http://hz.gotoacloud.top/gtznkewvos.html

Java: String.join(", ", list)
来源：http://hz.aibaodan.cn/gtgyrapcjf.html

Go:   strings.Join(strs, ", ")
来源：http://hz.gzhubu.top/gttofxxjfh.html

Ruby: arr.join(", ")
来源：http://hz.meibo888.top/gtpdblendv.html

C#:   string.Join(", ", list)
来源：http://hz.meibo888.top/gthjtdclmx.html

================================================================================
来源：http://hz.gogol.net.cn/gtrgmdxqvg.html

E. 字符串处理
来源：http://hz.ivvv.top/gtlflieezp.html

================================================================================
来源：http://hz.9152youxi.cn/gtzlawdehn.html

[E01] 拼接字符串
来源：http://hz.mhx1999.top/gtmogpfkge.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zhoulong.xyz/gtkbdibnjt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yj20258888.top/gtvahizetf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.aibaodan.cn/gtrnlfogiq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.aizwys.cn/gtthohdecq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.cucudq.cn/gthkuzzwmq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zhaomingkeji.xyz/gtycvmzeyu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.shanyushiyangkeji.top/gtbvrvaxgw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.daxiang520.top/gtzdhvrlud.html

[E02] 重复字符串
来源：http://hz.sxryk.cn/gtvemukkdw.html

Py:   "ab" * 3
来源：http://hz.pengpengdd.cyou/gtthibdcic.html

PHP:  str_repeat("ab", 3);
来源：http://hz.316326.xyz/gtcuucaikm.html

JS:   "ab".repeat(3)
来源：http://hz.cdnleiting.top/gtpimiuiwm.html

TS:   "ab".repeat(3)
来源：http://hz.xylfe.cn/gtfbehmgvb.html

Java: "ab".repeat(3)
来源：http://hz.yuxming.cn/gtuatpqfzr.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.shuidangran.top/gttxklnovd.html

Ruby: "ab" * 3
来源：http://hz.pycfn.com/gtyjxwcucf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yj20258.top/gtizuxcfmy.html

[E03] 截取子串
来源：http://hz.yuxming.cn/gtebaqtpor.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zdqjudy.top/gtfiehgwic.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.shangyingyoupin.top/gtdoeyhgfc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.sufxvd.cn/gtbavyvpnl.html

TS:   s.slice(1, 4)
来源：http://hz.gaohongyu789.top/gtlmuexnnc.html

Java: s.substring(1, 4)
来源：http://hz.jiagoushi.top/gtehukixuk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.haohaochexian.top/gtabtulfwv.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.shangyingyoupin.top/gtrlbykdhv.html

C#:   s.Substring(1, 3)
来源：http://hz.wangshuangyany.cn/gtcbdkihhb.html

[E04] 查找子串位置
来源：http://hz.guannengcc.top/gtwxhvhbid.html

Py:   s.find("x");  s.index("x")
来源：http://hz.meibo888.top/gtgnqettkm.html

PHP:  strpos($s, "x");
来源：http://hz.yj20258888.top/gtuqzvkzsf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.cashguo.top/gtzffahyya.html

TS:   s.indexOf("x")
来源：http://hz.yj202588.top/gtdirnegig.html

Java: s.indexOf("x")
来源：http://hz.jlsjyb.cn/gtrnyiyzir.html

Go:   strings.Index(s, "x")
来源：http://hz.gaohongyu789.top/gtspwezzwy.html

Ruby: s.index("x")
来源：http://hz.kuanghao11.cn/gtmeatjlad.html

C#:   s.IndexOf("x")
来源：http://hz.shanyushiyangtech.top/gttaaxstnf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.c1oappe.top/gtdclmkhfr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hfpthk.cn/gtjaueceee.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.hfpthk.cn/gtdwekgogm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jlsjyb.cn/gtcyzpoeia.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.yongpay.top/gtzwgghuyd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.nanxinkj.top/gtrbqmavqg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jinqigufen.top/gtnhqtxtum.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.fzhhl.top/gteeusqbut.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.zhaomingkeji.xyz/gtqmekmzpi.html

[E06] 替换子串
来源：http://hz.smart0.xyz/gtgdbmygcx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.zhongyouzk.top/gtkxfnhksb.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.ydzc1.top/gtlukavlcy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hammf.cn/gtmsgqifct.html

TS:   s.replaceAll("a", "b")
来源：http://hz.birdmap.top/gtbxvkzwro.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.tian-w.cn/gtkyfwtqmi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.ivvv.top/gtwgwhwssd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.sweek.top/gtvbepwgap.html

C#:   s.Replace("a", "b")
来源：http://hz.zhengqikj.top/gtfuvkorlf.html

[E07] 按分隔符拆分
来源：http://hz.tanke756.top/gtgoggvpeb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.hnxiangtu.top/gttneqalwe.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.andypj.xyz/gthpufxktf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yuanzhike.top/gtudoumexi.html

TS:   s.split(",")
来源：http://hz.gotoacloud.top/gtcmiiajcw.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.cashguo.top/gtlgefjoku.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yangfankeji.com/gtykvvatvq.html

Ruby: s.split(",");  s.split
来源：http://hz.xuetiantiany.cn/gtcfngljwv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zhiwuduotai.top/gtatxxgrob.html

[E08] 数组按分隔符合并
来源：http://hz.nanxinkj.top/gtpolmekbg.html

Py:   ",".join(items)
来源：http://hz.birdmap.top/gtmgybecqg.html

PHP:  implode(",", $items);
来源：http://hz.chenjidiqi.icu/gtbehbwroc.html

JS:   items.join(",")
来源：http://hz.sweek.top/gtzeswqdyr.html

TS:   items.join(",")
来源：http://hz.shuidangran.top/gtqxhgtsyb.html

Java: String.join(",", items)
来源：http://hz.wangshuangyany.cn/gtyagwlmrd.html

Go:   strings.Join(items, ",")
来源：http://hz.wangshuangyany.cn/gtstbgetfc.html

Ruby: items.join(",")
来源：http://hz.yongpay.top/gtfbaftuwj.html

C#:   string.Join(",", items)
来源：http://hz.gaohongyu789.top/gtqdzfzxnc.html

[E09] 去除所有空白字符
来源：http://hz.chenjidiqi.icu/gtxtsfbetr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.iojbl.cn/gtmeymauim.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.gogol.net.cn/gtbadylord.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jlsjyb.cn/gtrwejzqml.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.guowangkeji.top/gtxtcjtcyn.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.pycfn.com/gtjwzbxudq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.sxryk.cn/gtlvtcgdwi.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.tian-w.cn/gtnteynmto.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.fzhhl.top/gtpwoqbllg.html

[E10] 左侧补零 / 定长填充
来源：http://hz.guannengcc.top/gtuqormdjk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.sufxvd.cn/gtuvhlmhfq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hammf.cn/gtuztebnmb.html

JS:   "7".padStart(3, "0")
来源：http://hz.gotoacloud.top/gtzozpkpmi.html

TS:   "7".padStart(3, "0")
来源：http://hz.316326.xyz/gtshrxxjzp.html

Java: String.format("%03d", 7)
来源：http://hz.ydjk.org.cn/gtivpmxmdf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.feifeiyinyue.top/gtxhwfeisz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.cucudq.cn/gtiuokerkc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.nanxinkj.top/gtzicjhqqj.html

[E11] 反转字符串
来源：http://hz.guannengcc.top/gttvroojui.html

Py:   s[::-1]
来源：http://hz.sxryk.cn/gtpxxynvcp.html

PHP:  strrev($s);
来源：http://hz.9152youxi.cn/gtqqsfxyek.html

JS:   [...s].reverse().join("")
来源：http://hz.316326.xyz/gthuedcsvm.html

TS:   [...s].reverse().join("")
来源：http://hz.zhoulong.xyz/gttiwdaazt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yj202588.top/gtgbrhqbeb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yueranfly.top/gtkwmkfsxl.html

Ruby: s.reverse
来源：http://hz.aibaodan.cn/gtppoodjry.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zycfv.cn/gteqpimies.html

[E12] 统计某字符出现次数
来源：http://hz.gaohongyu789.top/gtozbhvyva.html

Py:   s.count("a")
来源：http://hz.dianchejie.cn/gtnytstpbg.html

PHP:  substr_count($s, "a");
来源：http://hz.cashguo.top/gtrqaraczt.html

JS:   s.split("a").length - 1
来源：http://hz.ybcxt.top/gtzynyrjgq.html

TS:   s.split("a").length - 1
来源：http://hz.nwbrower.top/gtgesdxzef.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yueranfly.top/gtcgcmacrx.html

Go:   strings.Count(s, "a")
来源：http://hz.shzxlz.cn/gtedkmxuho.html

Ruby: s.count("a")
来源：http://hz.hnxiangtu.top/gtlyaocxge.html

C#:   s.Count(c => c == 'a')
来源：http://hz.xingfuxueyuan.xyz/gtirrknkmz.html

[E13] 逐字符遍历
来源：http://hz.0kj1m.cn/gtrsspfxga.html

Py:   for ch in s: print(ch)
来源：http://hz.gogol.net.cn/gtzhxqzbfm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.havefunace.top/gtjzkxoatr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.guowangkeji.top/gtvklctrzr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.316326.xyz/gtpinohdgj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jyoumei.cn/gtbeibfjzh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yuanzhike.top/gtstbuychf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.chenjidiqi.icu/gttosepzzq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.guannengcc.top/gtqtblslei.html

[E14] URL 编码与 Base64
来源：http://hz.jinyuanbaomall.cn/gtsftbyqxx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.dianchejie.cn/gtyytybmsa.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.tian-w.cn/gtajmldbbq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.dashuyun.cn/gtnldrotej.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.cqqwz.cn/gtbjbmrybu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.nanxuanxn.top/gtdcxinaxn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.meibo888.top/gtzuxrvxwa.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.smart0.xyz/gtyectheme.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.hnxiangtu.top/gtvousnehu.html

[E15] HTML 转义 / 反转义
来源：http://hz.jlsjyb.cn/gtoponfdfl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.vqdsnc.cn/gtvdrxcqxp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yj20258.top/gtvuxmolzx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ydzc1.top/gtjvnfzkqo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jinghuilouyu.cn/gtendtmcua.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hywenlv.cn/gtylxzpqwa.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hfpthk.cn/gtajotzhky.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.hnqzz.top/gtsvaninyb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jinyuanbaomall.cn/gtttuiznwa.html

[E16] 数字千分位
来源：http://hz.yueranfly.top/gtugmtqzgi.html

Py:   f"{1234567:,}"
来源：http://hz.tanke756.top/gtwlqdidfw.html

PHP:  number_format(1234567);
来源：http://hz.xuanzx.com/gtnrsvhsew.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.fzhhl.top/gtdrolujzo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.tanke756.top/gtwhkdsedr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.hfpthk.cn/gtmuoawbog.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jyoumei.cn/gtmoaebmqv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.guannengcc.top/gtjcnzllvj.html

C#:   1234567.ToString("N0")
来源：http://hz.jinyuanbaomall.cn/gtsoabpnnn.html

[E17] 首字母大写
来源：http://hz.fzhhl.top/gthtnwtxqn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yj20258888.top/gtuikccyna.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.daria6918.cn/gtgtflfvst.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yj202588.top/gtxfqqxoqy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yangfankeji.com/gtqyanodcb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.wangshuangyany.cn/gtjygcdlgg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jiagoushi.top/gtyrsoxmhu.html

Ruby: s.capitalize
来源：http://hz.xuetiantiany.cn/gtsqiiorge.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jinyuanbaomall.cn/gtzponxpip.html

[E18] 模板占位符替换
来源：http://hz.cheryme.top/gtibpilaeo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jiagoushi.top/gtqrpshfzi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zycfv.cn/gttsxloamg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.bjfxy.top/gtfvxdnmmq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.gaohongyu789.top/gtjuantqgi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.bjfxy.top/gtenixvurc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jinghuilouyu.cn/gtohudydhu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.tanke756.top/gtkhyucash.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.sxryk.cn/gtkxozucnr.html

[E19] 多行文本按行拆分
来源：http://hz.tian-w.cn/gtwviohucl.html

Py:   s.splitlines()
来源：http://hz.smart0.xyz/gtsniredcz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.9152youxi.cn/gtstfkhzoo.html

JS:   s.split(/\r?\n/)
来源：http://hz.aibaodan.cn/gtlldtqyts.html

TS:   s.split(/\r?\n/)
来源：http://hz.tianlin.xyz/gtqsrurnzc.html

Java: s.lines().toList()
来源：http://hz.pengpengdd.cyou/gtdimjblkt.html

Go:   strings.Split(s, "\n")
来源：http://hz.xinyue.icu/gtcfmqeper.html

Ruby: s.lines
来源：http://hz.chenlongwang.top/gtcygcgahc.html

C#:   s.Split('\n')
来源：http://hz.gaohongyu789.top/gtymbqgeyi.html

[E20] 判断字符串是否为空
来源：http://hz.iojbl.cn/gtnhemjjlx.html

Py:   if not s:
来源：http://hz.cashguo.top/gtqkxndowc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.shuidangran.top/gtlobisqbl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.xuetiantiany.cn/gtttwdigfc.html

TS:   if (s === "") {}
来源：http://hz.chenjidiqi.icu/gtwxjfhlrs.html

Java: if (s.isEmpty()) {}
来源：http://hz.ppjwa.cn/gtkahxieiy.html

Go:   if s == "" {}
来源：http://hz.cqqwz.cn/gtcxbojlxp.html

Ruby: if s.empty?
来源：http://hz.yvedp.cn/gtlyyquakb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.dianchejie.cn/gtroiufqkz.html

[E21] 超长截断加省略号
来源：http://hz.gotoacloud.top/gtircedrva.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.haohaochexian.top/gtgfurwwlu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.shanyushiyangkeji.top/gtvbqwwzhx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.andypj.xyz/gtxuavihiq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yuanzhike.top/gtrjsrqdus.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.hongshengwenyu.top/gtsfugelug.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.shangyingyoupin.top/gtguzbybkj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yuxming.cn/gtwodtacav.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.daria6918.cn/gtlavkvqjg.html

[E22] 字节长度与字符长度
来源：http://hz.nanxinkj.top/gtkmrekrgn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.cqqwz.cn/gtbxpgttww.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.chenjidiqi.icu/gtugldmlyp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhoulong.xyz/gtvimbkwpo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.gotoacloud.top/gtcrzncacu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.cucudq.cn/gtiojumxdp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.pycfn.com/gtrzpffagp.html

Ruby: s.bytesize;  s.length
来源：http://hz.kuanghao11.cn/gtjizevelv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zycfv.cn/gthnjexoia.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtxksnvjsv.html

F. 文件与目录
来源：http://hz.yuanzhike.top/gtrgvpjbry.html

================================================================================
来源：http://hz.nanxinkj.top/gtmasyvlpe.html

[F01] 读取整个文件
来源：http://hz.ywan-chungtsiang.top/gtqskbnxby.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yvedp.cn/gtdwfeoals.html

PHP:  file_get_contents("a.txt");
来源：http://hz.dashuyun.cn/gtxnkuvwlf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.gotoacloud.top/gtqdqaczyn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zdqjudy.top/gtbxzeqypn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.shzxlz.cn/gtiidbitfl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.gogol.net.cn/gtnvnedcgf.html

Ruby: File.read("a.txt")
来源：http://hz.0kj1m.cn/gtzojzsjga.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.birdmap.top/gtpbglvumw.html

[F02] 逐行读取文件
来源：http://hz.xingfuxueyuan.xyz/gtjpqyiwag.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.chenlongwang.top/gticdqipfz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.wangshuangyany.cn/gtjqnjvkbm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jinghuilouyu.cn/gthidjpvfm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jiagoushi.top/gtgnmxzoua.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.shanyushiyangtech.top/gtuecrgfdm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.aibaodan.cn/gtouqqciez.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.c1oappe.top/gtklvrtuct.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.ehwqpu.com/gttbegffja.html

[F03] 写入文件（覆盖）
来源：http://hz.9152youxi.cn/gtuwpvwlhm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yangfankeji.com/gtbbkpvljr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.tianlin.xyz/gtvhneqckj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jqgfzy.top/gtedpsdfgo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.nanxuanxn.top/gtlphwcnck.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.quarkkingdee.top/gtwbtlfgyt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.xinyue.icu/gtcproinoc.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.shanyushiyangkeji.top/gthepcuvbv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.iojbl.cn/gtjyojvsjr.html

[F04] 追加写入文件
来源：http://hz.zhongyouzk.top/gtboppktwu.html


<!-- 参考信息 -->