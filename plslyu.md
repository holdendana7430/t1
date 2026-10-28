代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://hz.zycfv.cn/gtwfvadfce.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.smart0.xyz/gtqzrwmxzl.html

TS:   Math.max(...arr);
来源：http://hz.hammf.cn/gtairiyyuc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.316326.xyz/gtdpkbbtmt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yanxiufei.cn/gthfqhnpck.html

Ruby: arr.max;  arr.min
来源：http://hz.yuanzhike.top/gtptdeages.html

C#:   list.Max();  list.Min()
来源：http://hz.sufxvd.cn/gthieolztu.html

[D18] 扁平化嵌套数组
来源：http://hz.cdnleiting.top/gtoeoamwul.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.guowangkeji.top/gttoafbdet.html

PHP:  array_merge(...$nested);
来源：http://hz.zdqjudy.top/gtdabgkkis.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.smart0.xyz/gtxtyfuyvq.html

TS:   nested.flat();
来源：http://hz.guannengcc.top/gtidcgbqdr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zhongyouzk.top/gtqiapgtvs.html

Go:   // 手写双层循环
来源：http://hz.feifeiyinyue.top/gtbczdvufn.html

Ruby: nested.flatten
来源：http://hz.xinyue.icu/gtkzmxosha.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hnqzz.top/gtcyavcqgk.html

[D19] 按字段分组
来源：http://hz.jinghuilouyu.cn/gtvfhezrqh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.chenzaomai.com/gtzkcwdtfq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.chenlongwang.top/gtwhuhjtqp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jqgufenzy.top/gtebiunoci.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yongpay.top/gtipkkpqmr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.c1oappe.top/gtgxrktsly.html

Go:   // 手写 map[string][]T
来源：http://hz.tian-w.cn/gtgcnnrzmk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.quarkkingdee.top/gtfkbupumw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.ehwqpu.com/gtgpluozxe.html

[D20] 统计每个元素出现次数
来源：http://hz.smart0.xyz/gtfcsvucgl.html

Py:   Counter(arr)
来源：http://hz.shzxlz.cn/gtuahuobax.html

PHP:  array_count_values($arr);
来源：http://hz.jinqigufen.top/gtrjceijgg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yj202588.top/gtsvvvyqfo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.dianchejie.cn/gtulwdhhlu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yj20258.top/gtdeutkyxk.html

Go:   // 手写 map[T]int
来源：http://hz.sweek.top/gtkqvsvyyi.html

Ruby: arr.tally
来源：http://hz.zhiwuduotai.top/gtriqicbhp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.316326.xyz/gtyewigryu.html

[D21] 判断是否包含某元素
来源：http://hz.fzhhl.top/gtelgqbntp.html

Py:   x in arr
来源：http://hz.jinqigfzy.top/gtcqkefwon.html

PHP:  in_array($x, $arr, true);
来源：http://hz.chenjidiqi.icu/gtlnpstqab.html

JS:   arr.includes(x)
来源：http://hz.birdmap.top/gtqcfhntez.html

TS:   arr.includes(x)
来源：http://hz.sxryk.cn/gtjsneztst.html

Java: list.contains(x)
来源：http://hz.shzxlz.cn/gturpfgaoz.html

Go:   slices.Contains(arr, x)
来源：http://hz.tianlin.xyz/gtezqfntyg.html

Ruby: arr.include?(x)
来源：http://hz.andypj.xyz/gtrmsyetyz.html

C#:   list.Contains(x)
来源：http://hz.zhengqikj.top/gtihxylbsl.html

[D22] 复制数组（避免共享引用）
来源：http://hz.sweek.top/gtoxbgihdk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ybcxt.top/gtmopbrtdw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.xziqi.cn/gtlbzlylkn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.shuidangran.top/gttormivaf.html

TS:   [...arr];
来源：http://hz.yj202588.top/gtbpeolkss.html

Java: new ArrayList<>(list);
来源：http://hz.ydjk.org.cn/gtthcxmmbi.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.shanyushiyangkeji.top/gtnzsfflnv.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhoulong.xyz/gtkijwukcs.html

C#:   new List<int>(list);
来源：http://hz.shanyushiyangtech.top/gtgvaoucbk.html

[D23] reduce 累积计算
来源：http://hz.gotoacloud.top/gtygpoxxeb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.ywan-chungtsiang.top/gtzdnoobvd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.meibo888.top/gtzntkjmhk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yueranfly.top/gtovxizejq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.gzhubu.top/gtlbkjtzvg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.gzhubu.top/gtwzyomxxy.html

Go:   // 手写循环
来源：http://hz.ydjk.org.cn/gtzilflwef.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zycfv.cn/gttjyloodu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.ivvv.top/gtqiafpysm.html

[D24] 字典 / Map 基本操作
来源：http://hz.316326.xyz/gtpfxdzqnq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.cdnleiting.top/gtkyxszyfj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.guannengcc.top/gtfdmcudho.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yongpay.top/gtplmtyitn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.chenzaomai.com/gtqybaitka.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.hammf.cn/gtorhptpdv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.nwbrower.top/gttpmlzafc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jiagoushi.top/gtclxylmkm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.wangdashe.top/gtynjozqif.html

[D25] Set 集合去重与交并差
来源：http://hz.cdnleiting.top/gtorbziggh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.dashuyun.cn/gtyetofbwt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.ehwqpu.com/gttkuhyzyo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zycfv.cn/gttwhnurfk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jinqigfzy.top/gtjtzcaful.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.xylfe.cn/gtowwwwfuu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.birdmap.top/gtlfsrvnxi.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yuxming.cn/gtkxoibhjm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jinqigfzy.top/gtyuuozhxa.html

[D26] 数组转字符串
来源：http://hz.iojbl.cn/gtyuznqmpr.html

Py:   ", ".join(map(str, arr))
来源：http://hz.guowangkeji.top/gtvxjwsudh.html

PHP:  implode(", ", $arr);
来源：http://hz.daria6918.cn/gtdhskoalf.html

JS:   arr.join(", ")
来源：http://hz.shanyushiyangkeji.top/gtkxnyzxfs.html

TS:   arr.join(", ")
来源：http://hz.pengpengdd.cyou/gtnkyvmobz.html

Java: String.join(", ", list)
来源：http://hz.yonumen.top/gtcvfkqjhi.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hongshengwenyu.top/gtqatjqdvg.html

Ruby: arr.join(", ")
来源：http://hz.smart0.xyz/gttbodldvb.html

C#:   string.Join(", ", list)
来源：http://hz.jyoumei.cn/gtynugmkdb.html

================================================================================
来源：http://hz.nanxuanxn.top/gtahjoxvlc.html

E. 字符串处理
来源：http://hz.pycfn.com/gtlywrzwmb.html

================================================================================
来源：http://hz.yj20258888.top/gteefpcbwp.html

[E01] 拼接字符串
来源：http://hz.chenjidiqi.icu/gtorlzzkkt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yj20258.top/gtqfpyzykq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.haohaochexian.top/gtyuqpdgie.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shangyingyoupin.top/gtkfxhttqd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zycfv.cn/gtkgbognyg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.gotoacloud.top/gtvwdiutxd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.ivvv.top/gtiojivrmh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zdqjudy.top/gtqqqyjniz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.9152youxi.cn/gtdukxzkhx.html

[E02] 重复字符串
来源：http://hz.redwolf501.top/gtmwbijyxo.html

Py:   "ab" * 3
来源：http://hz.dashuyun.cn/gtqlsgbxcu.html

PHP:  str_repeat("ab", 3);
来源：http://hz.52xcode.cn/gtxgjgykzo.html

JS:   "ab".repeat(3)
来源：http://hz.9152youxi.cn/gtgypbcddv.html

TS:   "ab".repeat(3)
来源：http://hz.hnqzz.top/gtbfkxyady.html

Java: "ab".repeat(3)
来源：http://hz.yj20258.top/gtpuoyhyhg.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jinghuilouyu.cn/gtpdunrkbu.html

Ruby: "ab" * 3
来源：http://hz.dashuyun.cn/gtyhgegpiw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.shanyushiyangkeji.top/gtdfifcylq.html

[E03] 截取子串
来源：http://hz.quarkkingdee.top/gtanyyqtae.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ywan-chungtsiang.top/gtexxtdeqb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jlsjyb.cn/gthpydlwbc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yongpay.top/gtwwotkmqh.html

TS:   s.slice(1, 4)
来源：http://hz.sxryk.cn/gtcqrmvikt.html

Java: s.substring(1, 4)
来源：http://hz.cashguo.top/gtpjqrddeq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.tian-w.cn/gtskllwrzp.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yj20258888.top/gthgeulxda.html

C#:   s.Substring(1, 3)
来源：http://hz.yangfankeji.com/gtswdliyde.html

[E04] 查找子串位置
来源：http://hz.zhijiandao.cn/gtuxbljucs.html

Py:   s.find("x");  s.index("x")
来源：http://hz.ydjk.org.cn/gtelndpgly.html

PHP:  strpos($s, "x");
来源：http://hz.bjfxy.top/gtrynyajgd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.hnxiangtu.top/gtxkqmbzsz.html

TS:   s.indexOf("x")
来源：http://hz.fzhhl.top/gtkfolmzpw.html

Java: s.indexOf("x")
来源：http://hz.shangyingyoupin.top/gtnyexmrus.html

Go:   strings.Index(s, "x")
来源：http://hz.xylfe.cn/gtaohdoqil.html

Ruby: s.index("x")
来源：http://hz.yj20258.top/gtpfilgxkp.html

C#:   s.IndexOf("x")
来源：http://hz.sxryk.cn/gtnxwhdlch.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.hnxiangtu.top/gtboeujuzq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jqgfzy.top/gtkpoqjnlm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.xziqi.cn/gtbjxtjpem.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hnqzz.top/gtuzjqrrly.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.nanxinkj.top/gtthtkuswf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ivvv.top/gteygglrca.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yonumen.top/gtualxmdhn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.zhiwuduotai.top/gtfbmbjhmq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.havefunace.top/gtrjnixalp.html

[E06] 替换子串
来源：http://hz.zhiwuduotai.top/gtvkvleenh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.tian-w.cn/gtghcufbcg.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.xuanzx.com/gtcxhiiilr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xuanzx.com/gtuztrcajf.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jinqigufen.top/gtzoehnftn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cashguo.top/gtcpusfkue.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jiagoushi.top/gtfgqyuggp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.snrcjt.cn/gtatseatzi.html

C#:   s.Replace("a", "b")
来源：http://hz.tian-w.cn/gtopywiwny.html

[E07] 按分隔符拆分
来源：http://hz.hfpthk.cn/gticyjqvpf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.zhixingplan.top/gtvshdbsin.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.fengsongda.top/gtutmbkbtq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.dashuyun.cn/gttounpdsx.html

TS:   s.split(",")
来源：http://hz.yueranfly.top/gtgguoubol.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.dianchejie.cn/gtutquyfnc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yonumen.top/gtbnbqukzr.html

Ruby: s.split(",");  s.split
来源：http://hz.wangshuangyany.cn/gtlpihnprk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zycfv.cn/gtiavejbsc.html

[E08] 数组按分隔符合并
来源：http://hz.birdmap.top/gtnmzmfvnj.html

Py:   ",".join(items)
来源：http://hz.zhaomingkeji.xyz/gtavbxwmqo.html

PHP:  implode(",", $items);
来源：http://hz.316326.xyz/gtgzmouaph.html

JS:   items.join(",")
来源：http://hz.0kj1m.cn/gtgvrnzfuj.html

TS:   items.join(",")
来源：http://hz.ehwqpu.com/gtbvplskfo.html

Java: String.join(",", items)
来源：http://hz.sxryk.cn/gtsponqkjb.html

Go:   strings.Join(items, ",")
来源：http://hz.snrcjt.cn/gtsutqpfhi.html

Ruby: items.join(",")
来源：http://hz.jinghuilouyu.cn/gtcaalmzsw.html

C#:   string.Join(",", items)
来源：http://hz.chenlongwang.top/gtyybtqsiy.html

[E09] 去除所有空白字符
来源：http://hz.jinqigfzy.top/gteqylifsf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.sweek.top/gtqjeviutw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jinyuanbaomall.cn/gtyjkrborl.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.xylfe.cn/gtdjciinfd.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ydjk.org.cn/gtqbpmemhp.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.c1oappe.top/gtrxldfoen.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.nanxinkj.top/gtxjlsjavu.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hammf.cn/gtllpyuvmx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.gogol.net.cn/gtizavqvue.html

[E10] 左侧补零 / 定长填充
来源：http://hz.0kj1m.cn/gtxiyjldvm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jlsjyb.cn/gtmrjzmkrs.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.cashguo.top/gttkctleld.html

JS:   "7".padStart(3, "0")
来源：http://hz.jqgufenzy.top/gtjccljaqy.html

TS:   "7".padStart(3, "0")
来源：http://hz.snrcjt.cn/gtwduwocoo.html

Java: String.format("%03d", 7)
来源：http://hz.nwbrower.top/gtygcbybrv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.cashguo.top/gtpitbtdxb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.cqqwz.cn/gtoizwkbje.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yanxiufei.cn/gtbnkjuxsx.html

[E11] 反转字符串
来源：http://hz.yongpay.top/gtdkldjzru.html

Py:   s[::-1]
来源：http://hz.guowangkeji.top/gtflzvezky.html

PHP:  strrev($s);
来源：http://hz.nanxinkj.top/gtmlcnqiqg.html

JS:   [...s].reverse().join("")
来源：http://hz.jinghuilouyu.cn/gtqovkzawq.html

TS:   [...s].reverse().join("")
来源：http://hz.chenzaomai.com/gtalvaobqc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.nanxinkj.top/gtyrrxkqjd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.sweek.top/gtfeokgbpu.html

Ruby: s.reverse
来源：http://hz.havefunace.top/gtvpifeufh.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.tianlin.xyz/gtfrbrvvbh.html

[E12] 统计某字符出现次数
来源：http://hz.pycfn.com/gtugoizvuo.html

Py:   s.count("a")
来源：http://hz.9152youxi.cn/gtjdnxvsag.html

PHP:  substr_count($s, "a");
来源：http://hz.nanxinkj.top/gtncvdsosv.html

JS:   s.split("a").length - 1
来源：http://hz.zhijiandao.cn/gtehfsmzpy.html

TS:   s.split("a").length - 1
来源：http://hz.hysaishi.cn/gtxqusooay.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.sufxvd.cn/gttblzivjx.html

Go:   strings.Count(s, "a")
来源：http://hz.zhijiandao.cn/gtvrbpanuw.html

Ruby: s.count("a")
来源：http://hz.chenlongwang.top/gtlyfrvlmi.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jqgufenzy.top/gttnpznjdp.html

[E13] 逐字符遍历
来源：http://hz.yj20258888.top/gtftvoqnqu.html

Py:   for ch in s: print(ch)
来源：http://hz.smart0.xyz/gtftebdcqt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.shanyushiyangkeji.top/gtlhxsykpp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.0kj1m.cn/gtihffjdvi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhaomingkeji.xyz/gtevviqeaq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.xuanzx.com/gtqdhpuyef.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.guowangkeji.top/gtftragwxo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.c1oappe.top/gtqzlyztbp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zdqjudy.top/gtgdxwdoxd.html

[E14] URL 编码与 Base64
来源：http://hz.yanxiufei.cn/gtrwlnkrts.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.ehwqpu.com/gttqcgojuf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jqgufenzy.top/gtrostrapp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.xinyue.icu/gtppjivazr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yvedp.cn/gtaqpezuic.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhiwuduotai.top/gtkxundpqn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jinghuilouyu.cn/gtxrdbjtyn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.quarkkingdee.top/gtcpnmvcbp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.andypj.xyz/gtafuqtfgx.html

[E15] HTML 转义 / 反转义
来源：http://hz.zhiwuduotai.top/gttlycxxfr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.hammf.cn/gtynnqswsf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yangfankeji.com/gtfuelhzrf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.xuanzx.com/gtybaxqthd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.andypj.xyz/gtjnwlciho.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.fzhhl.top/gtugrjkgaq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.shzxlz.cn/gtkeqdmhfv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.snrcjt.cn/gtrytgggpu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yueranfly.top/gtjizjpyqy.html

[E16] 数字千分位
来源：http://hz.guowangkeji.top/gtyynmkapr.html

Py:   f"{1234567:,}"
来源：http://hz.sxryk.cn/gtxqnyiblf.html

PHP:  number_format(1234567);
来源：http://hz.meibo888.top/gtamzlvurw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.dashuyun.cn/gtcbynnegg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ivvv.top/gtjyazdchz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.tianlin.xyz/gtlskwauyi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.chenzaomai.com/gtueptrzcm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.xuanzx.com/gtfnjofnzd.html

C#:   1234567.ToString("N0")
来源：http://hz.daria6918.cn/gteseweyil.html

[E17] 首字母大写
来源：http://hz.ivvv.top/gtctpbcqxv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.jyoumei.cn/gtsqqxakvn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.iojbl.cn/gtjilyfvuw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhixingplan.top/gtyakfjupi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xuanzx.com/gtnhovvthh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.chenlongwang.top/gtwiylgljo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.guannengcc.top/gtbqeeirfn.html

Ruby: s.capitalize
来源：http://hz.fengsongda.top/gtyyyfzrdw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jyoumei.cn/gtaqgbdxvx.html

[E18] 模板占位符替换
来源：http://hz.gzhubu.top/gtcxdvueak.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.316326.xyz/gtuszhrtiy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jinyuanbaomall.cn/gtvftevugo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.svipenyu.cn/gtmvwdmcyf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.ppjwa.cn/gtcwlhwxxc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jinyuanbaomall.cn/gtczwurdmo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ehwqpu.com/gtzwquvspg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hysaishi.cn/gtepmqxkiv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.kuanghao11.cn/gtbsfoddfm.html

[E19] 多行文本按行拆分
来源：http://hz.hywenlv.cn/gtqdrgbtwc.html

Py:   s.splitlines()
来源：http://hz.jinyuanbaomall.cn/gtgbbtifwh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yonumen.top/gtvyghdsde.html

JS:   s.split(/\r?\n/)
来源：http://hz.fengsongda.top/gtriaqbtbd.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhengqikj.top/gtkxcuslht.html

Java: s.lines().toList()
来源：http://hz.gzhubu.top/gtxzxvqqwx.html

Go:   strings.Split(s, "\n")
来源：http://hz.hfpthk.cn/gtqxchepih.html

Ruby: s.lines
来源：http://hz.yueranfly.top/gtojjdlurv.html

C#:   s.Split('\n')
来源：http://hz.9152youxi.cn/gtzvyppzcb.html

[E20] 判断字符串是否为空
来源：http://hz.yanxiufei.cn/gtfukdohzj.html

Py:   if not s:
来源：http://hz.dianchejie.cn/gtpvumcwok.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ivvv.top/gtgxwvhyfd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.shanyushiyangkeji.top/gtponqhkcw.html

TS:   if (s === "") {}
来源：http://hz.hfpthk.cn/gtpvhrxuom.html

Java: if (s.isEmpty()) {}
来源：http://hz.316326.xyz/gtzxblpynn.html

Go:   if s == "" {}
来源：http://hz.quarkkingdee.top/gtdmbrcadw.html

Ruby: if s.empty?
来源：http://hz.yuanzhike.top/gtualjcjem.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.aibaodan.cn/gtkksgvdev.html

[E21] 超长截断加省略号
来源：http://hz.jyoumei.cn/gttuaqwuhb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.birdmap.top/gtyznobect.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yonumen.top/gtlajeithn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hongshengwenyu.top/gtvsciccft.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.pycfn.com/gtqfcbvdhx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yj20258888.top/gttdjhqbyl.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.chenjidiqi.icu/gtbpudmkzm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.cdnleiting.top/gtsnzjvaqq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.birdmap.top/gtslvquubr.html

[E22] 字节长度与字符长度
来源：http://hz.jinqigfzy.top/gtrdzfxqdp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.fzhhl.top/gtbcyvjopc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.iojbl.cn/gtscgblele.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.fzhhl.top/gtaaptsvqx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xuetiantiany.cn/gtatxrhjgp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jiagoushi.top/gtjkehafkt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.nanxinkj.top/gtvkidrrmd.html

Ruby: s.bytesize;  s.length
来源：http://hz.zhaomingkeji.xyz/gtuypfhpiy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.chenzaomai.com/gtsrryrais.html

================================================================================
来源：http://hz.cdnleiting.top/gttgpkexmi.html

F. 文件与目录
来源：http://hz.kuanghao11.cn/gtryvtvksz.html

================================================================================
来源：http://hz.zhengqikj.top/gtviakcqtn.html

[F01] 读取整个文件
来源：http://hz.jqgfzy.top/gtbujixetd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.shanyushiyangtech.top/gtrrrgiwoi.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yonumen.top/gtosrfmrac.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.0kj1m.cn/gtmomfapxv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.aibaodan.cn/gtaaxqmuzn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yongpay.top/gtqlxiyjtx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.dashuyun.cn/gtujdblqiz.html

Ruby: File.read("a.txt")
来源：http://hz.snrcjt.cn/gtswclqufr.html


<!-- 参考信息 -->