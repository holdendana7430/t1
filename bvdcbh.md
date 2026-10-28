代发 wailian999

[D19] 按字段分组
来源：http://hz.yangfankeji.com/gtphhviaod.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yongpay.top/gtwduzjmiq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.9152youxi.cn/gtoslhbokp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yuanzhike.top/gtrrbravcl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zhijiandao.cn/gtmmvbkjxe.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yvedp.cn/gtsvukexah.html

Go:   // 手写 map[string][]T
来源：http://hz.jinyuanbaomall.cn/gtktflcrcq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.9152youxi.cn/gthldopxwt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.dianchejie.cn/gtbyzugtoa.html

[D20] 统计每个元素出现次数
来源：http://hz.bjfxy.top/gtznxmtawf.html

Py:   Counter(arr)
来源：http://hz.tanke756.top/gtxtkzcujk.html

PHP:  array_count_values($arr);
来源：http://hz.smart0.xyz/gtvenkbwmz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.c1oappe.top/gtfxpstgvw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.wangshuangyany.cn/gtbcevdvjz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.guannengcc.top/gtgmxwgycl.html

Go:   // 手写 map[T]int
来源：http://hz.nwbrower.top/gthepgqzzg.html

Ruby: arr.tally
来源：http://hz.birdmap.top/gtubgfguxg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yuxming.cn/gtdkrukqao.html

[D21] 判断是否包含某元素
来源：http://hz.xylfe.cn/gtonmmyttt.html

Py:   x in arr
来源：http://hz.shuidangran.top/gtqcetmqdy.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zhoulong.xyz/gtwznhcghj.html

JS:   arr.includes(x)
来源：http://hz.iojbl.cn/gtcepodhed.html

TS:   arr.includes(x)
来源：http://hz.zhengqikj.top/gtgqkhdgyb.html

Java: list.contains(x)
来源：http://hz.yj20258.top/gtyxijnbvj.html

Go:   slices.Contains(arr, x)
来源：http://hz.xuetiantiany.cn/gtyuzkpzdc.html

Ruby: arr.include?(x)
来源：http://hz.hywenlv.cn/gtjrsphzop.html

C#:   list.Contains(x)
来源：http://hz.zycfv.cn/gtbxwtwjeg.html

[D22] 复制数组（避免共享引用）
来源：http://hz.cdnleiting.top/gtulnztmus.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.shanyushiyangkeji.top/gtlrflltsx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zdqjudy.top/gtwartwqrb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.fengsongda.top/gtlcrrqpps.html

TS:   [...arr];
来源：http://hz.shzxlz.cn/gtzgnaygpk.html

Java: new ArrayList<>(list);
来源：http://hz.mhx1999.top/gtzliyergp.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jyoumei.cn/gtywsuyvsa.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yuxming.cn/gtxwijzuqo.html

C#:   new List<int>(list);
来源：http://hz.52xcode.cn/gtykfyrawz.html

[D23] reduce 累积计算
来源：http://hz.tianlin.xyz/gtwssqjhyr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zhaomingkeji.xyz/gtnmyuwgtg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.sufxvd.cn/gtlizhytjv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cdnleiting.top/gthwanureq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.316326.xyz/gtvtysyxam.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yongpay.top/gtgzxyttyx.html

Go:   // 手写循环
来源：http://hz.yuxming.cn/gtidldlrxl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jinyuanbaomall.cn/gtfrxskrif.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.xuetiantiany.cn/gtcgjjtqqp.html

[D24] 字典 / Map 基本操作
来源：http://hz.yuxming.cn/gtnbsxfcpa.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhiwuduotai.top/gtfzjikeab.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.quarkkingdee.top/gtpzgnaobv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.sufxvd.cn/gtkdklmsjk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.meibo888.top/gtgprodrbg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.redwolf501.top/gtvtoencjm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.haohaochexian.top/gtkwkalbkp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.ydzc1.top/gttgnkwasz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.xuetiantiany.cn/gtfgnjrubl.html

[D25] Set 集合去重与交并差
来源：http://hz.chenlongwang.top/gtsbzkvgmb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.guannengcc.top/gttgexnwnb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.bjfxy.top/gtaemgcvws.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.chenlongwang.top/gtjjagtdge.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.nanxuanxn.top/gtwuxrxvhg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yuxming.cn/gtrohsfvxc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yj202588.top/gtxqtaodkv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.cashguo.top/gtdubyazpu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.ivvv.top/gtmjrewchi.html

[D26] 数组转字符串
来源：http://hz.yj20258.top/gtmsasggfx.html

Py:   ", ".join(map(str, arr))
来源：http://hz.hywenlv.cn/gtqbhjlbcz.html

PHP:  implode(", ", $arr);
来源：http://hz.hnqzz.top/gtqxgwmosf.html

JS:   arr.join(", ")
来源：http://hz.zhiwuduotai.top/gtrqutsjkj.html

TS:   arr.join(", ")
来源：http://hz.hnxiangtu.top/gtahgeebte.html

Java: String.join(", ", list)
来源：http://hz.snrcjt.cn/gtudoezonr.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yj20258.top/gtgojtmmbo.html

Ruby: arr.join(", ")
来源：http://hz.hammf.cn/gtihumcesm.html

C#:   string.Join(", ", list)
来源：http://hz.jinqigfzy.top/gtgyoartcc.html

================================================================================
来源：http://hz.zdqjudy.top/gttigyrrwj.html

E. 字符串处理
来源：http://hz.ivvv.top/gtxeplsswo.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtjlxbajbf.html

[E01] 拼接字符串
来源：http://hz.tanke756.top/gtdqukvouo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ybcxt.top/gtdukrzvgc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yanxiufei.cn/gtvobjbicf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yonumen.top/gtvumwrobi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.316326.xyz/gtkppwunbe.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.xziqi.cn/gtqjgvljuu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.havefunace.top/gtmtgczwtq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.svipenyu.cn/gtqixenefa.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.shzxlz.cn/gtzignzhxj.html

[E02] 重复字符串
来源：http://hz.zhijiandao.cn/gtftansaof.html

Py:   "ab" * 3
来源：http://hz.feifeiyinyue.top/gtvylzdvbn.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jqgufenzy.top/gtcdgscspi.html

JS:   "ab".repeat(3)
来源：http://hz.yanxiufei.cn/gtvjxpuqkr.html

TS:   "ab".repeat(3)
来源：http://hz.yongpay.top/gtqkvdjvvq.html

Java: "ab".repeat(3)
来源：http://hz.vqdsnc.cn/gtkaylknkx.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zhoulong.xyz/gtmmxoimam.html

Ruby: "ab" * 3
来源：http://hz.tanke756.top/gtfarfguwx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.jinghuilouyu.cn/gtsnnczfet.html

[E03] 截取子串
来源：http://hz.yj20258888.top/gttgafqigc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.fengsongda.top/gtvbntwioz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.pengpengdd.cyou/gtulizqbfl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.cqqwz.cn/gtcvcsvftd.html

TS:   s.slice(1, 4)
来源：http://hz.yonumen.top/gtxrxjjwmn.html

Java: s.substring(1, 4)
来源：http://hz.316326.xyz/gtapundvnl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zhongyouzk.top/gtyedguuiu.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.shuidangran.top/gtjtopuyxw.html

C#:   s.Substring(1, 3)
来源：http://hz.jqgfzy.top/gtpwuhmgkt.html

[E04] 查找子串位置
来源：http://hz.yuxming.cn/gtrrfbogmr.html

Py:   s.find("x");  s.index("x")
来源：http://hz.dashuyun.cn/gtgxtgtqeh.html

PHP:  strpos($s, "x");
来源：http://hz.316326.xyz/gtspohhqjw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.sysykeji.top/gtlpdvdzok.html

TS:   s.indexOf("x")
来源：http://hz.tianlin.xyz/gtarnxafbr.html

Java: s.indexOf("x")
来源：http://hz.shuidangran.top/gtpljyrqet.html

Go:   strings.Index(s, "x")
来源：http://hz.aibaodan.cn/gtngutiatk.html

Ruby: s.index("x")
来源：http://hz.zhengqikj.top/gtqdjugehj.html

C#:   s.IndexOf("x")
来源：http://hz.aizwys.cn/gtzuzukjdo.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.andypj.xyz/gthkwjdylt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.svipenyu.cn/gtqnsahpxf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.hnqzz.top/gtnbwotmcz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.sweek.top/gtyzuhovws.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.gaohongyu789.top/gtqpdxxomw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zdqjudy.top/gtjqiszbco.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.tianlin.xyz/gtsowacyab.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.guowangkeji.top/gtdzuvlnto.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jiagoushi.top/gtvhgkyhss.html

[E06] 替换子串
来源：http://hz.aibaodan.cn/gtfumsfkxe.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.tianlin.xyz/gtewylzrue.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.sweek.top/gtamcvgwdh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.quarkkingdee.top/gtxxcgkjzq.html

TS:   s.replaceAll("a", "b")
来源：http://hz.shzxlz.cn/gtdfsbzsea.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.aibaodan.cn/gtwsyfzrnz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.hnqzz.top/gtsnmeudjc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.jinqigfzy.top/gtnpxzwsjw.html

C#:   s.Replace("a", "b")
来源：http://hz.yuanzhike.top/gtifmcdwzh.html

[E07] 按分隔符拆分
来源：http://hz.zycfv.cn/gtndsekhdg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.sysykeji.top/gtgvhtdwhn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.cheryme.top/gtfvztxtsg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.bjfxy.top/gtdelgbibj.html

TS:   s.split(",")
来源：http://hz.gotoacloud.top/gtuxetwrzt.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yueranfly.top/gtcqfmdgup.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.sysykeji.top/gtcnbppsvx.html

Ruby: s.split(",");  s.split
来源：http://hz.zhixingplan.top/gtjxizhgxj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.shangyingyoupin.top/gtsqyyjkwm.html

[E08] 数组按分隔符合并
来源：http://hz.tanke756.top/gtijiyakwm.html

Py:   ",".join(items)
来源：http://hz.9152youxi.cn/gttorbtiqk.html

PHP:  implode(",", $items);
来源：http://hz.ivvv.top/gtxtvqzvsv.html

JS:   items.join(",")
来源：http://hz.zhijiandao.cn/gtvnjzkzcq.html

TS:   items.join(",")
来源：http://hz.yj20258888.top/gtzgnuczop.html

Java: String.join(",", items)
来源：http://hz.daxiang520.top/gtxlqynlye.html

Go:   strings.Join(items, ",")
来源：http://hz.nanxinkj.top/gtcpbzceaj.html

Ruby: items.join(",")
来源：http://hz.shuidangran.top/gtsdgosjcz.html

C#:   string.Join(",", items)
来源：http://hz.hammf.cn/gtwnupwbwt.html

[E09] 去除所有空白字符
来源：http://hz.vqdsnc.cn/gtmrkqkmvd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.0kj1m.cn/gtwfbgbcao.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.guannengcc.top/gtpmficcqu.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.hfpthk.cn/gtbhbscpmg.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.xuetiantiany.cn/gtblkryjsu.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.ydjk.org.cn/gtzdpidaqx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.0kj1m.cn/gtniyjlruu.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.316326.xyz/gthchwfobm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.tianlin.xyz/gteentvesl.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xylfe.cn/gtqeseclyl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ywan-chungtsiang.top/gtcgqtsdhg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jlsjyb.cn/gtrxdobfcy.html

JS:   "7".padStart(3, "0")
来源：http://hz.gotoacloud.top/gtfhkrqzqf.html

TS:   "7".padStart(3, "0")
来源：http://hz.yanxiufei.cn/gtnakhqplr.html

Java: String.format("%03d", 7)
来源：http://hz.yvedp.cn/gtliulwgrn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.havefunace.top/gtxllpzjvf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.svipenyu.cn/gtxtdpzfsn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.daxiang520.top/gtbowefwsf.html

[E11] 反转字符串
来源：http://hz.chenlongwang.top/gttbesufof.html

Py:   s[::-1]
来源：http://hz.yonumen.top/gtyaibarnq.html

PHP:  strrev($s);
来源：http://hz.daxiang520.top/gtxamozkgs.html

JS:   [...s].reverse().join("")
来源：http://hz.vqdsnc.cn/gttrhvcfuy.html

TS:   [...s].reverse().join("")
来源：http://hz.xinyue.icu/gtnmsggyrq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.ehwqpu.com/gtjyvkzhki.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.gogol.net.cn/gtmqrpyyjo.html

Ruby: s.reverse
来源：http://hz.chenzaomai.com/gtaxenwqfw.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yj20258.top/gtrikcbvhj.html

[E12] 统计某字符出现次数
来源：http://hz.shanyushiyangtech.top/gtcfjrqkyc.html

Py:   s.count("a")
来源：http://hz.hongshengwenyu.top/gtwovolckc.html

PHP:  substr_count($s, "a");
来源：http://hz.xinyue.icu/gtwxwxhnmm.html

JS:   s.split("a").length - 1
来源：http://hz.shzxlz.cn/gtwjweriyg.html

TS:   s.split("a").length - 1
来源：http://hz.316326.xyz/gtrajwhtub.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.hongshengwenyu.top/gtuhpvwini.html

Go:   strings.Count(s, "a")
来源：http://hz.cdnleiting.top/gtpglvqhrt.html

Ruby: s.count("a")
来源：http://hz.iojbl.cn/gthbmnrizq.html

C#:   s.Count(c => c == 'a')
来源：http://hz.shanyushiyangkeji.top/gtxfhdtjlp.html

[E13] 逐字符遍历
来源：http://hz.pengpengdd.cyou/gtsjuncvsh.html

Py:   for ch in s: print(ch)
来源：http://hz.sysykeji.top/gtsknwqbpk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.shangyingyoupin.top/gtlqasqgct.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.smart0.xyz/gtxmanbver.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yanxiufei.cn/gtzqhzyywt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.zhiwuduotai.top/gtnwrrcyci.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jinyuanbaomall.cn/gtsqgmirra.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.daxiang520.top/gtupxvdlai.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.smart0.xyz/gtdqanndpl.html

[E14] URL 编码与 Base64
来源：http://hz.sufxvd.cn/gtaqnnnuri.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhaomingkeji.xyz/gtwjponvkq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.cqqwz.cn/gtkffubjzn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jinqigfzy.top/gtojhbhzxn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.fzhhl.top/gtweyruklb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.sufxvd.cn/gtgmscjzjo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zdqjudy.top/gtzkgifszl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.quarkkingdee.top/gtapqqjmqa.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.pengpengdd.cyou/gtwrzlygfp.html

[E15] HTML 转义 / 反转义
来源：http://hz.gzhubu.top/gtharalaky.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.fengsongda.top/gtduvbczkx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.feifeiyinyue.top/gtwkoyndbc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.chenjidiqi.icu/gtncujgikl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.xylfe.cn/gtdlielqns.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.havefunace.top/gtepzyedzl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yueranfly.top/gtxxsanstq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.guowangkeji.top/gtreibfdej.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.cashguo.top/gtzglqjznb.html

[E16] 数字千分位
来源：http://hz.jlsjyb.cn/gtoeleayue.html

Py:   f"{1234567:,}"
来源：http://hz.yangfankeji.com/gtibccifnf.html

PHP:  number_format(1234567);
来源：http://hz.ywan-chungtsiang.top/gtmyvaeyck.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ybcxt.top/gtoituqaqk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.cashguo.top/gtleflehgh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yuxming.cn/gtcexnufce.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.tanke756.top/gtungmdbwb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.xziqi.cn/gtualdetuc.html

C#:   1234567.ToString("N0")
来源：http://hz.tian-w.cn/gtiysbwxmj.html

[E17] 首字母大写
来源：http://hz.chenzaomai.com/gtcefvpkdc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.jqgfzy.top/gtuqbqslcb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.xziqi.cn/gtaqabajtw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinyuanbaomall.cn/gtwtmpcfko.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.wangshuangyany.cn/gtilipmnrl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.snrcjt.cn/gtfqzslmcl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.haohaochexian.top/gtxfbaumkk.html

Ruby: s.capitalize
来源：http://hz.tanke756.top/gtkemjwfhu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.smart0.xyz/gtfebxsrml.html

[E18] 模板占位符替换
来源：http://hz.mhx1999.top/gtdwhlbktk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.cqqwz.cn/gtphfnjoqy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.ydjk.org.cn/gtrfqlhzuj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.52xcode.cn/gtggabjxol.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.cashguo.top/gtkarucyly.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jinghuilouyu.cn/gtuhllhzoj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.fengsongda.top/gtyvnhpaws.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zhijiandao.cn/gtvcyetlhm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.chenzaomai.com/gtkatknykb.html

[E19] 多行文本按行拆分
来源：http://hz.zycfv.cn/gtvynjsiwk.html

Py:   s.splitlines()
来源：http://hz.hysaishi.cn/gtxzyjlrmw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.pengpengdd.cyou/gttxvecnut.html

JS:   s.split(/\r?\n/)
来源：http://hz.hfpthk.cn/gtkvghxjiw.html

TS:   s.split(/\r?\n/)
来源：http://hz.guowangkeji.top/gthqoyepdc.html

Java: s.lines().toList()
来源：http://hz.andypj.xyz/gtajglnwtr.html

Go:   strings.Split(s, "\n")
来源：http://hz.hammf.cn/gtaqrcyzuv.html

Ruby: s.lines
来源：http://hz.ppjwa.cn/gtjzhvaglx.html

C#:   s.Split('\n')
来源：http://hz.jqgfzy.top/gtrtkowiig.html

[E20] 判断字符串是否为空
来源：http://hz.yonumen.top/gtwvrnkyzj.html

Py:   if not s:
来源：http://hz.jyoumei.cn/gttctfspqb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yj202588.top/gtnujoactm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hammf.cn/gtlwoeanvc.html

TS:   if (s === "") {}
来源：http://hz.zhaomingkeji.xyz/gtjpdkcivl.html

Java: if (s.isEmpty()) {}
来源：http://hz.yuanzhike.top/gtiowqhdbs.html

Go:   if s == "" {}
来源：http://hz.gogol.net.cn/gttdxeifzo.html

Ruby: if s.empty?
来源：http://hz.birdmap.top/gtwoahmdui.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zhoulong.xyz/gtlrqubmko.html

[E21] 超长截断加省略号
来源：http://hz.yj202588.top/gtexauwous.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ppjwa.cn/gtbrqkzqyu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhoulong.xyz/gttlzlpdol.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yuxming.cn/gtfhwhnifn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhoulong.xyz/gtllermefr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.hnqzz.top/gtcdjrhjfz.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.bjfxy.top/gtdqsijsej.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.xuanzx.com/gtmsgvidne.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.c1oappe.top/gtpxpfidmy.html

[E22] 字节长度与字符长度
来源：http://hz.shuidangran.top/gthzkvdehr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.sxryk.cn/gtjdaatlhr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hfpthk.cn/gtvqhlvohb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.guannengcc.top/gtehvpupgv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cucudq.cn/gtwqmfjenu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jiagoushi.top/gtmxbxgpss.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.xuanzx.com/gtdkuayryd.html

Ruby: s.bytesize;  s.length
来源：http://hz.hammf.cn/gtamglbycl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.gzhubu.top/gtwkggodvl.html

================================================================================
来源：http://hz.ydzc1.top/gtbnpsixfv.html

F. 文件与目录
来源：http://hz.yj20258888.top/gtzhwkmjke.html

================================================================================
来源：http://hz.zycfv.cn/gtetjfmfnf.html

[F01] 读取整个文件
来源：http://hz.smart0.xyz/gtimnbpdkw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zdqjudy.top/gtdargthpx.html

PHP:  file_get_contents("a.txt");
来源：http://hz.meibo888.top/gtfnmydqxa.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.wangshuangyany.cn/gtswwtotzx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.dashuyun.cn/gthwbmvikj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.andypj.xyz/gtajelrtzl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.fengsongda.top/gttrzzcxng.html

Ruby: File.read("a.txt")
来源：http://hz.shuidangran.top/gtfnjdbtmb.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.sysykeji.top/gtntdyiysu.html

[F02] 逐行读取文件
来源：http://hz.zycfv.cn/gtkajufjxm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.hnqzz.top/gtjqlmghhu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.hnxiangtu.top/gtqgdcyhvt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gaohongyu789.top/gtcwkiokor.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zdqjudy.top/gtpoocqnux.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.sweek.top/gtcsixzxjc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.daxiang520.top/gtaoemulaq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.dashuyun.cn/gtsslvxymu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jianghu66.top/gtbxtecwrw.html

[F03] 写入文件（覆盖）
来源：http://hz.kuanghao11.cn/gtnaftxuor.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.sweek.top/gtdujszsid.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.xuanzx.com/gtywegotvp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.guowangkeji.top/gttakjttwx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj202588.top/gtplhkcjmc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.xinyue.icu/gteptsvjkf.html


<!-- 参考信息 -->