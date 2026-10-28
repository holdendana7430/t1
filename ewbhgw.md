代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ybcxt.top/gtmnjowmef.html

PHP:  array_merge(...$nested);
来源：http://hz.xinyue.icu/gtwegxycbk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yangfankeji.com/gtvzbvziqv.html

TS:   nested.flat();
来源：http://hz.52xcode.cn/gtujzdwimb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.sweek.top/gtkmluwmey.html

Go:   // 手写双层循环
来源：http://hz.jinqigufen.top/gtsnbzrixt.html

Ruby: nested.flatten
来源：http://hz.yueranfly.top/gtjynaimoj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.sxryk.cn/gtvpfedsfj.html

[D19] 按字段分组
来源：http://hz.birdmap.top/gtjzgrahhv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yuanzhike.top/gtqiczjchk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.haohaochexian.top/gtyeszfalk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.ehwqpu.com/gtsnkjrerg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.redwolf501.top/gtsorbppoq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.daria6918.cn/gthuajzbem.html

Go:   // 手写 map[string][]T
来源：http://hz.pengpengdd.cyou/gtyudqyezj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.chenlongwang.top/gtqytojxur.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhiwuduotai.top/gtwzyhcnpf.html

[D20] 统计每个元素出现次数
来源：http://hz.shanyushiyangkeji.top/gttlqwgzoe.html

Py:   Counter(arr)
来源：http://hz.316326.xyz/gtfkjybtbv.html

PHP:  array_count_values($arr);
来源：http://hz.chenjidiqi.icu/gttfpdwwll.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yj20258.top/gtewgjmqns.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.nanxuanxn.top/gtxsfkyucq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yanxiufei.cn/gtrlkcowac.html

Go:   // 手写 map[T]int
来源：http://hz.chenlongwang.top/gtjijtdmgg.html

Ruby: arr.tally
来源：http://hz.birdmap.top/gtbhkdqdpq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.316326.xyz/gtdjpxsnab.html

[D21] 判断是否包含某元素
来源：http://hz.birdmap.top/gtoeuceyxm.html

Py:   x in arr
来源：http://hz.jlsjyb.cn/gtnypycbax.html

PHP:  in_array($x, $arr, true);
来源：http://hz.smart0.xyz/gtqqqoowlm.html

JS:   arr.includes(x)
来源：http://hz.jianghu66.top/gtktmvrpvx.html

TS:   arr.includes(x)
来源：http://hz.zycfv.cn/gtoywbldeb.html

Java: list.contains(x)
来源：http://hz.ybcxt.top/gthwjdgoos.html

Go:   slices.Contains(arr, x)
来源：http://hz.chenzaomai.com/gtcabvixmy.html

Ruby: arr.include?(x)
来源：http://hz.wangshuangyany.cn/gtmmlqjlch.html

C#:   list.Contains(x)
来源：http://hz.meibo888.top/gthsuqbxhz.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ydzc1.top/gtigxmleth.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.iojbl.cn/gtrilzuvpv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yuanzhike.top/gtmblybtke.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.dashuyun.cn/gtmbumhffd.html

TS:   [...arr];
来源：http://hz.yj202588.top/gtqdwdaewz.html

Java: new ArrayList<>(list);
来源：http://hz.birdmap.top/gtxhzdldlp.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yj20258888.top/gtmuqwmmen.html

Ruby: arr.dup;  arr.clone
来源：http://hz.iojbl.cn/gtowmpygfn.html

C#:   new List<int>(list);
来源：http://hz.0kj1m.cn/gtmamqaequ.html

[D23] reduce 累积计算
来源：http://hz.yuanzhike.top/gtghuuzdmw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.smart0.xyz/gtklbsebfi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.xziqi.cn/gtfdbqcqds.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.wangdashe.top/gtczpspkmz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ybcxt.top/gtnupeqail.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.svipenyu.cn/gtkcddhtdp.html

Go:   // 手写循环
来源：http://hz.guannengcc.top/gtsifirxlt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jinqigfzy.top/gtqqlmtsuq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jqgfzy.top/gtksofqivo.html

[D24] 字典 / Map 基本操作
来源：http://hz.cucudq.cn/gtfqhxaitf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ywan-chungtsiang.top/gttprlbhyp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.zhengqikj.top/gtzenofccl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yvedp.cn/gtlevbvsgm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.c1oappe.top/gtdzjipsvz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.cucudq.cn/gtvebnugdf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.chenlongwang.top/gtcyordmkm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhaomingkeji.xyz/gtlunfspnh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.52xcode.cn/gthluzhggu.html

[D25] Set 集合去重与交并差
来源：http://hz.kuanghao11.cn/gtwqtepnkr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.shangyingyoupin.top/gtrcufvaeb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.iojbl.cn/gtuudirzft.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.cqqwz.cn/gtvspteugs.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.gogol.net.cn/gtqcwhhlje.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yongpay.top/gttkbsrosd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.gotoacloud.top/gtajovzedd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.xziqi.cn/gtfvldbcvf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.0kj1m.cn/gtedesazsy.html

[D26] 数组转字符串
来源：http://hz.pengpengdd.cyou/gtjplmzyvy.html

Py:   ", ".join(map(str, arr))
来源：http://hz.hnqzz.top/gtuzhbcoak.html

PHP:  implode(", ", $arr);
来源：http://hz.jlsjyb.cn/gtwffbynsn.html

JS:   arr.join(", ")
来源：http://hz.birdmap.top/gtaeguucfk.html

TS:   arr.join(", ")
来源：http://hz.zhoulong.xyz/gttbkglohd.html

Java: String.join(", ", list)
来源：http://hz.jqgfzy.top/gtjjerqtmt.html

Go:   strings.Join(strs, ", ")
来源：http://hz.cucudq.cn/gtwtaycyng.html

Ruby: arr.join(", ")
来源：http://hz.cashguo.top/gtxkubplhc.html

C#:   string.Join(", ", list)
来源：http://hz.ydjk.org.cn/gtlxvtlarg.html

================================================================================
来源：http://hz.wangdashe.top/gtmucjftwt.html

E. 字符串处理
来源：http://hz.pengpengdd.cyou/gtjmztwtpk.html

================================================================================
来源：http://hz.jinqigfzy.top/gtwluotqed.html

[E01] 拼接字符串
来源：http://hz.ywan-chungtsiang.top/gtxtajsxld.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.hysaishi.cn/gtwusqhicd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.meibo888.top/gtjtmtnpfu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jianghu66.top/gtpollqifh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yonumen.top/gthnulwwyf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.feifeiyinyue.top/gtgximyiev.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.316326.xyz/gtizpfhgjz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.hfpthk.cn/gtwjloahni.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.cdnleiting.top/gtazbecrwu.html

[E02] 重复字符串
来源：http://hz.yanxiufei.cn/gtnhhtxbny.html

Py:   "ab" * 3
来源：http://hz.guannengcc.top/gtescxfbhw.html

PHP:  str_repeat("ab", 3);
来源：http://hz.sufxvd.cn/gtsvqhwrwy.html

JS:   "ab".repeat(3)
来源：http://hz.jinghuilouyu.cn/gtoukvtdmg.html

TS:   "ab".repeat(3)
来源：http://hz.nanxinkj.top/gtfvlllviu.html

Java: "ab".repeat(3)
来源：http://hz.yj20258888.top/gtulyqeuba.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.cdnleiting.top/gtazngwokz.html

Ruby: "ab" * 3
来源：http://hz.meibo888.top/gteucuiopl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.fengsongda.top/gtvwszhyfq.html

[E03] 截取子串
来源：http://hz.jlsjyb.cn/gtijeibrfu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yvedp.cn/gtgskovlzh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.xziqi.cn/gtfcznxubx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.xuetiantiany.cn/gtqiorokly.html

TS:   s.slice(1, 4)
来源：http://hz.cheryme.top/gtofmghwjy.html

Java: s.substring(1, 4)
来源：http://hz.zycfv.cn/gtvyapgtnz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.smart0.xyz/gtgwepdjdd.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.birdmap.top/gthkdayybe.html

C#:   s.Substring(1, 3)
来源：http://hz.dianchejie.cn/gtbtwgdqhn.html

[E04] 查找子串位置
来源：http://hz.sysykeji.top/gtstdrkpju.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jiagoushi.top/gtcjsvbaot.html

PHP:  strpos($s, "x");
来源：http://hz.zdqjudy.top/gtgjpzroxt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.cucudq.cn/gtiykkdnvf.html

TS:   s.indexOf("x")
来源：http://hz.pengpengdd.cyou/gtusyuvhvr.html

Java: s.indexOf("x")
来源：http://hz.hnqzz.top/gtpyzivzbi.html

Go:   strings.Index(s, "x")
来源：http://hz.dianchejie.cn/gtcqqbvxhg.html

Ruby: s.index("x")
来源：http://hz.tian-w.cn/gtcytxledj.html

C#:   s.IndexOf("x")
来源：http://hz.0kj1m.cn/gtjoekzgji.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.gzhubu.top/gtojerhkjf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.c1oappe.top/gtjkuzwzxx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.yanxiufei.cn/gtaaorycvw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cqqwz.cn/gtczqvrbru.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.c1oappe.top/gtuutdcvcc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.gzhubu.top/gtxdppyupf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.chenjidiqi.icu/gtarfkenrh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.smart0.xyz/gtqajawfzc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.gotoacloud.top/gtcgcitcql.html

[E06] 替换子串
来源：http://hz.316326.xyz/gtrtnlyafe.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.cqqwz.cn/gteyqovfsj.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.zhaomingkeji.xyz/gtjcczmxkh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.wangshuangyany.cn/gtdtiypepp.html

TS:   s.replaceAll("a", "b")
来源：http://hz.vqdsnc.cn/gtbefprnjk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.guowangkeji.top/gtoctwjucl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.dashuyun.cn/gtmpdiutlm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.tian-w.cn/gtmjaqqjys.html

C#:   s.Replace("a", "b")
来源：http://hz.gogol.net.cn/gtmoqgkzyc.html

[E07] 按分隔符拆分
来源：http://hz.cdnleiting.top/gtediqmvet.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jinqigufen.top/gtfzihfflb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.cheryme.top/gtwkozirhu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.shanyushiyangtech.top/gtxpfzdebr.html

TS:   s.split(",")
来源：http://hz.yueranfly.top/gtutnfgvga.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.havefunace.top/gtfhysbxsi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.sufxvd.cn/gtbwiukrre.html

Ruby: s.split(",");  s.split
来源：http://hz.zycfv.cn/gtgrrruzvb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.aizwys.cn/gtyoiqsvcd.html

[E08] 数组按分隔符合并
来源：http://hz.jyoumei.cn/gtebgcvtoz.html

Py:   ",".join(items)
来源：http://hz.jinqigufen.top/gtseuxvscf.html

PHP:  implode(",", $items);
来源：http://hz.jinghuilouyu.cn/gtfaiekkcl.html

JS:   items.join(",")
来源：http://hz.zhongyouzk.top/gtxvzcubjp.html

TS:   items.join(",")
来源：http://hz.zhengqikj.top/gthhzzwlpr.html

Java: String.join(",", items)
来源：http://hz.xylfe.cn/gtibzshtjx.html

Go:   strings.Join(items, ",")
来源：http://hz.cqqwz.cn/gtzqfuvbpq.html

Ruby: items.join(",")
来源：http://hz.meibo888.top/gtbjzopich.html

C#:   string.Join(",", items)
来源：http://hz.c1oappe.top/gtiabfqfry.html

[E09] 去除所有空白字符
来源：http://hz.ywan-chungtsiang.top/gtyzmgxjri.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.havefunace.top/gttxkkmqzo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jianghu66.top/gtxpgdekyu.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.ywan-chungtsiang.top/gtagbpqxir.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yuanzhike.top/gthmuzryqv.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.daria6918.cn/gtojqfrzjs.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.ydjk.org.cn/gtqbruyhhr.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zdqjudy.top/gtigpcxywg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.shanyushiyangkeji.top/gtfsetaasz.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xylfe.cn/gtxgjrfrwe.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.meibo888.top/gtnrbqvile.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yueranfly.top/gtqhkmjkel.html

JS:   "7".padStart(3, "0")
来源：http://hz.haohaochexian.top/gtttbrmoko.html

TS:   "7".padStart(3, "0")
来源：http://hz.ivvv.top/gtuvoccqdv.html

Java: String.format("%03d", 7)
来源：http://hz.hnqzz.top/gtdjrgseel.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jinqigufen.top/gtwkwfgxzq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jqgfzy.top/gtghujmywy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yangfankeji.com/gtdrfuatbw.html

[E11] 反转字符串
来源：http://hz.ydjk.org.cn/gtevozlljb.html

Py:   s[::-1]
来源：http://hz.aibaodan.cn/gtznsrbvxb.html

PHP:  strrev($s);
来源：http://hz.feifeiyinyue.top/gtwrntgjdq.html

JS:   [...s].reverse().join("")
来源：http://hz.wangshuangyany.cn/gtncqqlyzo.html

TS:   [...s].reverse().join("")
来源：http://hz.zhongyouzk.top/gtenmiyurp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yj20258888.top/gtxmxyhrpg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhoulong.xyz/gtvceazccs.html

Ruby: s.reverse
来源：http://hz.xinyue.icu/gtfpdwslya.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.kuanghao11.cn/gtqhbsvriy.html

[E12] 统计某字符出现次数
来源：http://hz.haohaochexian.top/gtmmvaczio.html

Py:   s.count("a")
来源：http://hz.smart0.xyz/gtqucxcvad.html

PHP:  substr_count($s, "a");
来源：http://hz.cucudq.cn/gtnrqyecqv.html

JS:   s.split("a").length - 1
来源：http://hz.hongshengwenyu.top/gtbxnohbct.html

TS:   s.split("a").length - 1
来源：http://hz.nwbrower.top/gtajhpebvs.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yuxming.cn/gtyixsideo.html

Go:   strings.Count(s, "a")
来源：http://hz.hammf.cn/gtmrqgzzyt.html

Ruby: s.count("a")
来源：http://hz.xziqi.cn/gtvluchldv.html

C#:   s.Count(c => c == 'a')
来源：http://hz.shanyushiyangkeji.top/gtmjdbibhb.html

[E13] 逐字符遍历
来源：http://hz.daxiang520.top/gthhjcgtdr.html

Py:   for ch in s: print(ch)
来源：http://hz.pengpengdd.cyou/gtjmzfjkgz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhiwuduotai.top/gtgzajmmpn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sysykeji.top/gtifxbyrhz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.guannengcc.top/gtxwxviqdc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yvedp.cn/gtewbanbrx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.tianlin.xyz/gtbuajgorv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.shanyushiyangtech.top/gtwhktjjxl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.sysykeji.top/gthunyigtf.html

[E14] URL 编码与 Base64
来源：http://hz.guowangkeji.top/gtxxceessq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.fengsongda.top/gtpwhmmvpu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hfpthk.cn/gtclbnxyey.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yuanzhike.top/gtkzwlvvdh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.cqqwz.cn/gtjyqiqyoz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.chenzaomai.com/gtdoxshbix.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.gaohongyu789.top/gtsykeeecq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhiwuduotai.top/gtpvayyffs.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ywan-chungtsiang.top/gtotuludku.html

[E15] HTML 转义 / 反转义
来源：http://hz.yueranfly.top/gtsjacdccz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.shanyushiyangtech.top/gtjbvnlron.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.dashuyun.cn/gtoijhdmve.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.hnqzz.top/gtuzacxiqm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yvedp.cn/gtvzfrymae.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jlsjyb.cn/gteceyhbno.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jqgufenzy.top/gtnbielrkk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yonumen.top/gtrcafomhl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.gaohongyu789.top/gtezttylcf.html

[E16] 数字千分位
来源：http://hz.hfpthk.cn/gtwkadfpxb.html

Py:   f"{1234567:,}"
来源：http://hz.chenjidiqi.icu/gtttarhnvs.html

PHP:  number_format(1234567);
来源：http://hz.shanyushiyangtech.top/gtcghlamua.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.0kj1m.cn/gtysmrwqyv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yuanzhike.top/gtqrpwlvrg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.9152youxi.cn/gtffvuicel.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yanxiufei.cn/gtrqnhojpy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.52xcode.cn/gtzuovppev.html

C#:   1234567.ToString("N0")
来源：http://hz.zhijiandao.cn/gtyivsprmt.html

[E17] 首字母大写
来源：http://hz.cashguo.top/gtpejzebpz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.shanyushiyangtech.top/gturvlbuvk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yuxming.cn/gtmbznjrli.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sxryk.cn/gtqpunirev.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xuetiantiany.cn/gtwalncmom.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.shanyushiyangtech.top/gtdinyhzmf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.pycfn.com/gtvwdosgsf.html

Ruby: s.capitalize
来源：http://hz.zdqjudy.top/gtdcjcqcdc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.ybcxt.top/gtlumuhwwa.html

[E18] 模板占位符替换
来源：http://hz.shanyushiyangtech.top/gtevfjjgqs.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.dianchejie.cn/gtqnrwzeix.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.tanke756.top/gtgsnghpgm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhengqikj.top/gtilfvdyux.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.vqdsnc.cn/gtuxomzvuy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.nanxinkj.top/gtasetyofw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ydzc1.top/gturljdxoj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.shzxlz.cn/gtgkddakyj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yj202588.top/gtzgdcxwse.html

[E19] 多行文本按行拆分
来源：http://hz.pycfn.com/gtuhzcxycq.html

Py:   s.splitlines()
来源：http://hz.ppjwa.cn/gtejyyfabq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.c1oappe.top/gtpfaogmlk.html

JS:   s.split(/\r?\n/)
来源：http://hz.guowangkeji.top/gtbvkjnhvg.html

TS:   s.split(/\r?\n/)
来源：http://hz.mhx1999.top/gtvzglkqod.html

Java: s.lines().toList()
来源：http://hz.ppjwa.cn/gtnwomvokr.html

Go:   strings.Split(s, "\n")
来源：http://hz.jiagoushi.top/gtmnwemcdy.html

Ruby: s.lines
来源：http://hz.hnqzz.top/gtluepzkvd.html

C#:   s.Split('\n')
来源：http://hz.sysykeji.top/gtvodyeoax.html

[E20] 判断字符串是否为空
来源：http://hz.ydjk.org.cn/gtsqwiqfop.html

Py:   if not s:
来源：http://hz.nwbrower.top/gtxemgjbkm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.cucudq.cn/gtpilkozum.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.svipenyu.cn/gtkvcnoxuf.html

TS:   if (s === "") {}
来源：http://hz.shanyushiyangkeji.top/gtantaumrx.html

Java: if (s.isEmpty()) {}
来源：http://hz.zhiwuduotai.top/gthwwimewc.html

Go:   if s == "" {}
来源：http://hz.shuidangran.top/gtetbbokqu.html

Ruby: if s.empty?
来源：http://hz.xylfe.cn/gtbigmbhgf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.nwbrower.top/gtxmugrqqd.html

[E21] 超长截断加省略号
来源：http://hz.vqdsnc.cn/gtlayyggmv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ydjk.org.cn/gtbgabylar.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.nanxuanxn.top/gtlmylutdj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhoulong.xyz/gtyjptukph.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.9152youxi.cn/gtvlavuppy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.meibo888.top/gtsuhrnykx.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jlsjyb.cn/gtvwpsaprt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.wangshuangyany.cn/gtpmzjexum.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ydjk.org.cn/gtxuqufblp.html

[E22] 字节长度与字符长度
来源：http://hz.nanxuanxn.top/gtxlguzjsq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zhixingplan.top/gtsbpcygcq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hnqzz.top/gtrjhkuisa.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jlsjyb.cn/gttyqdjmdq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhixingplan.top/gtsfkkzoyr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.quarkkingdee.top/gthnkhowjc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.iojbl.cn/gtryiklpat.html

Ruby: s.bytesize;  s.length
来源：http://hz.dianchejie.cn/gtykgywaau.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jqgufenzy.top/gtbgzxgqci.html

================================================================================
来源：http://hz.yangfankeji.com/gtdqcgkwkh.html

F. 文件与目录
来源：http://hz.tianlin.xyz/gtyxvgdnjc.html

================================================================================
来源：http://hz.dianchejie.cn/gtadhcpaht.html

[F01] 读取整个文件
来源：http://hz.xylfe.cn/gtraubyzma.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hywenlv.cn/gthbgktuyk.html

PHP:  file_get_contents("a.txt");
来源：http://hz.sxryk.cn/gtwnwztzno.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.c1oappe.top/gtktntbixl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yuxming.cn/gtvavirhjz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.sxryk.cn/gtttzolhco.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.nanxuanxn.top/gtepwtjvxs.html

Ruby: File.read("a.txt")
来源：http://hz.ydzc1.top/gteqjtniug.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.gogol.net.cn/gtcgeshttw.html

[F02] 逐行读取文件
来源：http://hz.gotoacloud.top/gtkwtlpwqs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zycfv.cn/gtxlvlmebn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.xingfuxueyuan.xyz/gtrbvaqgqz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cheryme.top/gtfctlnrsd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.havefunace.top/gtzfsldzij.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ppjwa.cn/gthawlbeqh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.sysykeji.top/gtifrfqhga.html


<!-- 参考信息 -->