代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://hz.yj202588.top/gtkdgcoeta.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.ppjwa.cn/gtzjgokrjo.html

TS:   Math.max(...arr);
来源：http://hz.xinyue.icu/gtorwsubmq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.cucudq.cn/gtfquekmlt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.52xcode.cn/gtngundrya.html

Ruby: arr.max;  arr.min
来源：http://hz.nanxuanxn.top/gtprssahkn.html

C#:   list.Max();  list.Min()
来源：http://hz.chenjidiqi.icu/gtmenxolsp.html

[D18] 扁平化嵌套数组
来源：http://hz.hfpthk.cn/gtkrgucqes.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.sysykeji.top/gtdggzhpwx.html

PHP:  array_merge(...$nested);
来源：http://hz.nanxinkj.top/gtowcqaigv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.cashguo.top/gtlvestolb.html

TS:   nested.flat();
来源：http://hz.jinyuanbaomall.cn/gtylpzkyaz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.guowangkeji.top/gtbwxgnyiq.html

Go:   // 手写双层循环
来源：http://hz.tianlin.xyz/gthfbzjije.html

Ruby: nested.flatten
来源：http://hz.zycfv.cn/gtefopjvov.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.dashuyun.cn/gtixqiysuw.html

[D19] 按字段分组
来源：http://hz.shzxlz.cn/gtqtkdwcnl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.daria6918.cn/gtnvkeempa.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.tianlin.xyz/gtqtdndljt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.52xcode.cn/gtxaeybmoi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.xingfuxueyuan.xyz/gtceanfbeg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zycfv.cn/gtuselxyqa.html

Go:   // 手写 map[string][]T
来源：http://hz.daxiang520.top/gtsbaiwscr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.cheryme.top/gtorgkxpeu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhaomingkeji.xyz/gtdspyxobj.html

[D20] 统计每个元素出现次数
来源：http://hz.cheryme.top/gtlnafjwfz.html

Py:   Counter(arr)
来源：http://hz.tanke756.top/gtlfszfyzh.html

PHP:  array_count_values($arr);
来源：http://hz.havefunace.top/gtmcmgqbzf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.wangshuangyany.cn/gtwallclkm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yanxiufei.cn/gttsmtpjxk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.hammf.cn/gtcezyhzuw.html

Go:   // 手写 map[T]int
来源：http://hz.zycfv.cn/gtwfqaykan.html

Ruby: arr.tally
来源：http://hz.xylfe.cn/gtyggusory.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.guannengcc.top/gtadozrcou.html

[D21] 判断是否包含某元素
来源：http://hz.ivvv.top/gtyceenoks.html

Py:   x in arr
来源：http://hz.cucudq.cn/gtajhrlgzy.html

PHP:  in_array($x, $arr, true);
来源：http://hz.haohaochexian.top/gtgbpzvedw.html

JS:   arr.includes(x)
来源：http://hz.tanke756.top/gtqpnubyka.html

TS:   arr.includes(x)
来源：http://hz.zdqjudy.top/gtweiuztox.html

Java: list.contains(x)
来源：http://hz.yuanzhike.top/gtdwvzwghq.html

Go:   slices.Contains(arr, x)
来源：http://hz.zhiwuduotai.top/gtunrchuaz.html

Ruby: arr.include?(x)
来源：http://hz.9152youxi.cn/gtsorejpcv.html

C#:   list.Contains(x)
来源：http://hz.pengpengdd.cyou/gtojcuxjpq.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jiagoushi.top/gtbcguodic.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.0kj1m.cn/gtmgefhozx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jlsjyb.cn/gtnkrndxgh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jiagoushi.top/gthfnwvqfb.html

TS:   [...arr];
来源：http://hz.jyoumei.cn/gtkpcscxgp.html

Java: new ArrayList<>(list);
来源：http://hz.c1oappe.top/gtiigxqbyc.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yuxming.cn/gtvgmjcsdx.html

Ruby: arr.dup;  arr.clone
来源：http://hz.bjfxy.top/gtjyrbbgzy.html

C#:   new List<int>(list);
来源：http://hz.0kj1m.cn/gtstdyormm.html

[D23] reduce 累积计算
来源：http://hz.ehwqpu.com/gtqzrktbbu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.ywan-chungtsiang.top/gtejqecqvd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.hywenlv.cn/gtutrlrpcd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.0kj1m.cn/gtnbteqifg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hywenlv.cn/gtyzihrybu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.tian-w.cn/gtcslgqdnk.html

Go:   // 手写循环
来源：http://hz.ydjk.org.cn/gtvvknazeq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yangfankeji.com/gtuzvofyjr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.redwolf501.top/gtcxsgchpr.html

[D24] 字典 / Map 基本操作
来源：http://hz.jlsjyb.cn/gtnhffceqv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.smart0.xyz/gtjquwejax.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.zhongyouzk.top/gtlafpicsp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yj20258.top/gtdnhkwvwk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.zhijiandao.cn/gtlgqiainu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.xziqi.cn/gtvhjzstgs.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.nwbrower.top/gtawquumij.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.hysaishi.cn/gtbnwvaetj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.havefunace.top/gtzygmwbgd.html

[D25] Set 集合去重与交并差
来源：http://hz.haohaochexian.top/gtsqkxpgau.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.mhx1999.top/gtdxyeqcah.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.dianchejie.cn/gtvtbemrdp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhengqikj.top/gtdfcefdoh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.hysaishi.cn/gtcdwfkjxs.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.redwolf501.top/gtcajbkzxm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.cdnleiting.top/gtidwcwhej.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zhoulong.xyz/gtoargpwaa.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.sxryk.cn/gtumybrwrj.html

[D26] 数组转字符串
来源：http://hz.haohaochexian.top/gtvygtprzb.html

Py:   ", ".join(map(str, arr))
来源：http://hz.haohaochexian.top/gtjdwmikqt.html

PHP:  implode(", ", $arr);
来源：http://hz.zdqjudy.top/gtnffwhmib.html

JS:   arr.join(", ")
来源：http://hz.hnxiangtu.top/gtjcmvhsij.html

TS:   arr.join(", ")
来源：http://hz.pycfn.com/gteghxrdgt.html

Java: String.join(", ", list)
来源：http://hz.redwolf501.top/gtkogvuckp.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yj20258.top/gtzajbrvhw.html

Ruby: arr.join(", ")
来源：http://hz.snrcjt.cn/gthwirarph.html

C#:   string.Join(", ", list)
来源：http://hz.tianlin.xyz/gtlugmoxwn.html

================================================================================
来源：http://hz.jqgufenzy.top/gtmajhkboh.html

E. 字符串处理
来源：http://hz.sufxvd.cn/gthzxrmhtt.html

================================================================================
来源：http://hz.316326.xyz/gtjtkkonlb.html

[E01] 拼接字符串
来源：http://hz.iojbl.cn/gtqxxapavc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.dashuyun.cn/gtyatatorq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jiagoushi.top/gtgllqgulz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jqgfzy.top/gthtcsubld.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hywenlv.cn/gtazsartfc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.zhoulong.xyz/gtfsgusscy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.snrcjt.cn/gtanqggsfi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.tianlin.xyz/gtccmddrsy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jinqigfzy.top/gtnqpgfgxa.html

[E02] 重复字符串
来源：http://hz.quarkkingdee.top/gtabqnjpqz.html

Py:   "ab" * 3
来源：http://hz.xuetiantiany.cn/gtldriaord.html

PHP:  str_repeat("ab", 3);
来源：http://hz.cheryme.top/gtcrhuozjd.html

JS:   "ab".repeat(3)
来源：http://hz.fengsongda.top/gtzmjrvubk.html

TS:   "ab".repeat(3)
来源：http://hz.dianchejie.cn/gtciirjfag.html

Java: "ab".repeat(3)
来源：http://hz.ywan-chungtsiang.top/gtgkdwzpxm.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jinghuilouyu.cn/gtzrywrkbs.html

Ruby: "ab" * 3
来源：http://hz.dianchejie.cn/gtpqmbxmuy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.hnxiangtu.top/gtmexqbamf.html

[E03] 截取子串
来源：http://hz.bjfxy.top/gtmhtqzdzl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.tianlin.xyz/gtxdrazkxq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jqgfzy.top/gtrkaeirim.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.tianlin.xyz/gtvrkjaygu.html

TS:   s.slice(1, 4)
来源：http://hz.sweek.top/gtpoqiyfax.html

Java: s.substring(1, 4)
来源：http://hz.zhengqikj.top/gtspiugmly.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.9152youxi.cn/gtotnbvaor.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.guannengcc.top/gtkxdoqvpf.html

C#:   s.Substring(1, 3)
来源：http://hz.fengsongda.top/gtgifgthdi.html

[E04] 查找子串位置
来源：http://hz.smart0.xyz/gttiplscnz.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jinqigfzy.top/gtshogzagv.html

PHP:  strpos($s, "x");
来源：http://hz.hnqzz.top/gteldxhznn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.hywenlv.cn/gtgtvwwxmg.html

TS:   s.indexOf("x")
来源：http://hz.shangyingyoupin.top/gtcsptnevr.html

Java: s.indexOf("x")
来源：http://hz.pengpengdd.cyou/gtxmcjzsde.html

Go:   strings.Index(s, "x")
来源：http://hz.shanyushiyangtech.top/gtzbzctoje.html

Ruby: s.index("x")
来源：http://hz.yuanzhike.top/gtcdyshski.html

C#:   s.IndexOf("x")
来源：http://hz.shangyingyoupin.top/gteubxlcer.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.gogol.net.cn/gtwaleehop.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.andypj.xyz/gtxdermggw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.pycfn.com/gtczdymqyq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.bjfxy.top/gtmwiyahzh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.ybcxt.top/gtsbekkbbh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.pengpengdd.cyou/gthszoojre.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jinqigufen.top/gthhwckcfu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.cheryme.top/gttimxvpfn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.hfpthk.cn/gtwceaavnj.html

[E06] 替换子串
来源：http://hz.birdmap.top/gtykefsfhn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jinqigufen.top/gtmzfweijo.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.xylfe.cn/gtqbbayzmv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yj20258888.top/gtwozrefgr.html

TS:   s.replaceAll("a", "b")
来源：http://hz.nwbrower.top/gtlrgblgmj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ehwqpu.com/gtanuqgyqf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zhoulong.xyz/gtwndsiakt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.0kj1m.cn/gthcshebwb.html

C#:   s.Replace("a", "b")
来源：http://hz.cdnleiting.top/gthovifpgp.html

[E07] 按分隔符拆分
来源：http://hz.cucudq.cn/gtjkuobwpa.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.xuetiantiany.cn/gtojuxmszs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.aibaodan.cn/gtgoaudkrr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yanxiufei.cn/gtmtvqqllv.html

TS:   s.split(",")
来源：http://hz.shanyushiyangtech.top/gtrkvtsiyl.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yongpay.top/gtyjzanzsv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.wangdashe.top/gtytctzfrh.html

Ruby: s.split(",");  s.split
来源：http://hz.daxiang520.top/gtfzxdjrrp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.sweek.top/gtngtgygfu.html

[E08] 数组按分隔符合并
来源：http://hz.jqgufenzy.top/gtxxphleuh.html

Py:   ",".join(items)
来源：http://hz.andypj.xyz/gtdrctjsix.html

PHP:  implode(",", $items);
来源：http://hz.pycfn.com/gtzrntaejy.html

JS:   items.join(",")
来源：http://hz.guannengcc.top/gtehhyqfoz.html

TS:   items.join(",")
来源：http://hz.jinqigfzy.top/gtqgagegdp.html

Java: String.join(",", items)
来源：http://hz.vqdsnc.cn/gthcpwfvql.html

Go:   strings.Join(items, ",")
来源：http://hz.jinyuanbaomall.cn/gtspplhdwl.html

Ruby: items.join(",")
来源：http://hz.52xcode.cn/gtamjlsvle.html

C#:   string.Join(",", items)
来源：http://hz.quarkkingdee.top/gtfdtcitjy.html

[E09] 去除所有空白字符
来源：http://hz.jinyuanbaomall.cn/gtkewgtkqt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yonumen.top/gtaktwtboi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.sweek.top/gtqqrmlhot.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.chenlongwang.top/gtmxprogiz.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yangfankeji.com/gtalavrovm.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.xuetiantiany.cn/gtqavxxyyf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.jqgfzy.top/gtkgbjsxqx.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hywenlv.cn/gtydslbowe.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jqgfzy.top/gtewipegoz.html

[E10] 左侧补零 / 定长填充
来源：http://hz.birdmap.top/gtobkgyent.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.mhx1999.top/gtbihbvhxs.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.52xcode.cn/gtibjgqfjg.html

JS:   "7".padStart(3, "0")
来源：http://hz.sysykeji.top/gtxyhfptub.html

TS:   "7".padStart(3, "0")
来源：http://hz.yueranfly.top/gtcviiicco.html

Java: String.format("%03d", 7)
来源：http://hz.jianghu66.top/gtcwgmmsug.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.hnqzz.top/gtsbvtopmq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.hammf.cn/gtcccdjevg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.chenlongwang.top/gtfnvtegbl.html

[E11] 反转字符串
来源：http://hz.c1oappe.top/gtelruvdpf.html

Py:   s[::-1]
来源：http://hz.hfpthk.cn/gthuxlfnvh.html

PHP:  strrev($s);
来源：http://hz.shzxlz.cn/gtetueshgs.html

JS:   [...s].reverse().join("")
来源：http://hz.wangshuangyany.cn/gtpzetomms.html

TS:   [...s].reverse().join("")
来源：http://hz.hfpthk.cn/gtmcevdgko.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.shangyingyoupin.top/gtjsqhfowq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jyoumei.cn/gtuelcbknt.html

Ruby: s.reverse
来源：http://hz.fzhhl.top/gtqlpycymg.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.gzhubu.top/gtryjexxsd.html

[E12] 统计某字符出现次数
来源：http://hz.fengsongda.top/gtvqwceupj.html

Py:   s.count("a")
来源：http://hz.zhixingplan.top/gtnrwkodil.html

PHP:  substr_count($s, "a");
来源：http://hz.jyoumei.cn/gtbdlwaxyb.html

JS:   s.split("a").length - 1
来源：http://hz.cdnleiting.top/gtqzebgzns.html

TS:   s.split("a").length - 1
来源：http://hz.hongshengwenyu.top/gtepgdlqfi.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zhengqikj.top/gtrrcrjdgi.html

Go:   strings.Count(s, "a")
来源：http://hz.jiagoushi.top/gtnpycszaq.html

Ruby: s.count("a")
来源：http://hz.yj202588.top/gtdzvrrims.html

C#:   s.Count(c => c == 'a')
来源：http://hz.xuanzx.com/gtyslbncte.html

[E13] 逐字符遍历
来源：http://hz.sxryk.cn/gtdjgfrgsj.html

Py:   for ch in s: print(ch)
来源：http://hz.vqdsnc.cn/gtnzzlafyw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhixingplan.top/gtxwnfokui.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhoulong.xyz/gteylmgcow.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shuidangran.top/gtoqlfhqef.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.316326.xyz/gtqhppfjnc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.dashuyun.cn/gtszuwlznj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.ywan-chungtsiang.top/gtdyyhypuf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hywenlv.cn/gtpjjqtauq.html

[E14] URL 编码与 Base64
来源：http://hz.xylfe.cn/gtkbtneinn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.mhx1999.top/gthjyptjef.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jinyuanbaomall.cn/gtlhiuomyv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.chenjidiqi.icu/gtymwjoyjh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.xylfe.cn/gtclegldhf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.dashuyun.cn/gtlcgwnlzu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.chenlongwang.top/gtijunxdti.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jinyuanbaomall.cn/gtbbrobknl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ywan-chungtsiang.top/gtxifjjtmh.html

[E15] HTML 转义 / 反转义
来源：http://hz.yongpay.top/gtcjeovzji.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jinqigufen.top/gtpdurgejw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.kuanghao11.cn/gtkwmgdtth.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.hfpthk.cn/gtaimxhpjd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.xziqi.cn/gtjxjubjqf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.sweek.top/gtenqiqrrj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.gaohongyu789.top/gtlgchazmj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.birdmap.top/gtxpktgzek.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.dianchejie.cn/gtmjzduwlq.html

[E16] 数字千分位
来源：http://hz.52xcode.cn/gtqrgokzan.html

Py:   f"{1234567:,}"
来源：http://hz.yanxiufei.cn/gtbmjlrxgf.html

PHP:  number_format(1234567);
来源：http://hz.aizwys.cn/gtvtmowhmz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.guowangkeji.top/gtchdhbuue.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jyoumei.cn/gtxjsewkhw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.sysykeji.top/gtzvbrpirl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.sxryk.cn/gtjgeplbno.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.c1oappe.top/gthsswlvci.html

C#:   1234567.ToString("N0")
来源：http://hz.52xcode.cn/gthzricpxn.html

[E17] 首字母大写
来源：http://hz.jqgfzy.top/gtiudskmob.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.nwbrower.top/gtcelrtghg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.xziqi.cn/gtcgvivodi.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shanyushiyangtech.top/gtdslximon.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sysykeji.top/gtcuilhihi.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.kuanghao11.cn/gtqmszrtgo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.gaohongyu789.top/gttdssgxxd.html

Ruby: s.capitalize
来源：http://hz.c1oappe.top/gtnloxctnn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.cqqwz.cn/gtohsonaas.html

[E18] 模板占位符替换
来源：http://hz.wangdashe.top/gtohqqbxmv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.fengsongda.top/gtmyeagslj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.shangyingyoupin.top/gtwvrropce.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.wangdashe.top/gtjfjshdrt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.vqdsnc.cn/gtqqvevjnf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.tian-w.cn/gteidwfneq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ppjwa.cn/gtkwpfkisi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.meibo888.top/gtktrobyoo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.sweek.top/gtimfcfvqw.html

[E19] 多行文本按行拆分
来源：http://hz.hammf.cn/gtqqlpfttr.html

Py:   s.splitlines()
来源：http://hz.tianlin.xyz/gtnbusauut.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.aizwys.cn/gtutjgqvlt.html

JS:   s.split(/\r?\n/)
来源：http://hz.ywan-chungtsiang.top/gtkazroddp.html

TS:   s.split(/\r?\n/)
来源：http://hz.ywan-chungtsiang.top/gtvpiucvqy.html

Java: s.lines().toList()
来源：http://hz.yongpay.top/gtjioduxqe.html

Go:   strings.Split(s, "\n")
来源：http://hz.yanxiufei.cn/gtjvklpjss.html

Ruby: s.lines
来源：http://hz.chenjidiqi.icu/gtzxhdcloy.html

C#:   s.Split('\n')
来源：http://hz.shanyushiyangkeji.top/gtnzgvjvcn.html

[E20] 判断字符串是否为空
来源：http://hz.havefunace.top/gtlwwikdyb.html

Py:   if not s:
来源：http://hz.zhongyouzk.top/gtyfkjvklr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yueranfly.top/gteihnvfnd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.smart0.xyz/gtsoxdrome.html

TS:   if (s === "") {}
来源：http://hz.9152youxi.cn/gtbuojumsl.html

Java: if (s.isEmpty()) {}
来源：http://hz.zhiwuduotai.top/gtesjretay.html

Go:   if s == "" {}
来源：http://hz.zhijiandao.cn/gtivandglq.html

Ruby: if s.empty?
来源：http://hz.dashuyun.cn/gtndzhixhn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hongshengwenyu.top/gtrfkpgccp.html

[E21] 超长截断加省略号
来源：http://hz.hfpthk.cn/gtskvdtkvz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.wangshuangyany.cn/gtvcuyasey.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.hywenlv.cn/gtvckgyzgn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hongshengwenyu.top/gtphsjsoru.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cucudq.cn/gtnyyiuwer.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jyoumei.cn/gtjhcijlui.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hysaishi.cn/gtaldhvbhu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.zhaomingkeji.xyz/gtozpavqch.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ehwqpu.com/gtxtevvxpu.html

[E22] 字节长度与字符长度
来源：http://hz.zhaomingkeji.xyz/gtceumjinm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.gaohongyu789.top/gthjxhlgzi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yueranfly.top/gtljqgbotr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yvedp.cn/gtfdlztrcy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.9152youxi.cn/gtgjnlqnch.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.gogol.net.cn/gtpueybpfh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.vqdsnc.cn/gtlpbfrlvj.html

Ruby: s.bytesize;  s.length
来源：http://hz.yueranfly.top/gtzaktqbwf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.redwolf501.top/gtkxozgmgv.html

================================================================================
来源：http://hz.cucudq.cn/gtziexzvfr.html

F. 文件与目录
来源：http://hz.c1oappe.top/gtewepkfqx.html

================================================================================
来源：http://hz.fengsongda.top/gteztfmlxq.html

[F01] 读取整个文件
来源：http://hz.cdnleiting.top/gtqbwozqmd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.kuanghao11.cn/gtabpwhpbb.html

PHP:  file_get_contents("a.txt");
来源：http://hz.c1oappe.top/gtzoktugjd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.shangyingyoupin.top/gtlcfmpajv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.shanyushiyangtech.top/gtuzypeqit.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hammf.cn/gtwctydpgp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.hywenlv.cn/gtqtzusmye.html

Ruby: File.read("a.txt")
来源：http://hz.9152youxi.cn/gtvefoeykq.html


<!-- 参考信息 -->