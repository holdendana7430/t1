代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.xingfuxueyuan.xyz/gtlndcqugs.html

PHP:  array_merge(...$nested);
来源：http://hz.sufxvd.cn/gtjutyydnt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yongpay.top/gtspuqmqcm.html

TS:   nested.flat();
来源：http://hz.mhx1999.top/gtmwfvysat.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.hnqzz.top/gtcicwwecg.html

Go:   // 手写双层循环
来源：http://hz.gogol.net.cn/gtpgpbjqsj.html

Ruby: nested.flatten
来源：http://hz.sxryk.cn/gtzcgzoogb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.nanxinkj.top/gtaeqgchdl.html

[D19] 按字段分组
来源：http://hz.52xcode.cn/gtgikvzwpj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.havefunace.top/gtvpaqpkhj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.dashuyun.cn/gthefxexwl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yanxiufei.cn/gtlsuqrsxa.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.tanke756.top/gtadyfverp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jqgufenzy.top/gtrfcysblf.html

Go:   // 手写 map[string][]T
来源：http://hz.ydjk.org.cn/gtcguqnzqh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.xinyue.icu/gtkpesqzje.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yueranfly.top/gtfloiecgn.html

[D20] 统计每个元素出现次数
来源：http://hz.wangshuangyany.cn/gtsojsazsc.html

Py:   Counter(arr)
来源：http://hz.ywan-chungtsiang.top/gttswhytpz.html

PHP:  array_count_values($arr);
来源：http://hz.yj20258.top/gtycydpdrt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xuanzx.com/gtimvoqjsv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.smart0.xyz/gtlocdbyzx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ivvv.top/gtgticjpkz.html

Go:   // 手写 map[T]int
来源：http://hz.xingfuxueyuan.xyz/gtinkyqlkd.html

Ruby: arr.tally
来源：http://hz.hfpthk.cn/gtsylvxznk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.hysaishi.cn/gtvtazrgxs.html

[D21] 判断是否包含某元素
来源：http://hz.vqdsnc.cn/gthfffwfgj.html

Py:   x in arr
来源：http://hz.shuidangran.top/gtcbbgukyq.html

PHP:  in_array($x, $arr, true);
来源：http://hz.mhx1999.top/gtjnbwhihu.html

JS:   arr.includes(x)
来源：http://hz.hongshengwenyu.top/gtuuovfuvi.html

TS:   arr.includes(x)
来源：http://hz.zhoulong.xyz/gtivdjljdz.html

Java: list.contains(x)
来源：http://hz.gzhubu.top/gtdzvsxmzx.html

Go:   slices.Contains(arr, x)
来源：http://hz.zhijiandao.cn/gtrftomzty.html

Ruby: arr.include?(x)
来源：http://hz.zhongyouzk.top/gtronqypuu.html

C#:   list.Contains(x)
来源：http://hz.jiagoushi.top/gtnhpsyuod.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zdqjudy.top/gtsorhvfyc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ppjwa.cn/gtxwzuhkfl.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.ydjk.org.cn/gtbaljywvy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.shanyushiyangtech.top/gtxrvhhqqu.html

TS:   [...arr];
来源：http://hz.nanxuanxn.top/gtwarapvgr.html

Java: new ArrayList<>(list);
来源：http://hz.shangyingyoupin.top/gtbdqgqryh.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.316326.xyz/gtnmafaagy.html

Ruby: arr.dup;  arr.clone
来源：http://hz.pengpengdd.cyou/gtpgrpoxdz.html

C#:   new List<int>(list);
来源：http://hz.yj20258888.top/gtpddprybi.html

[D23] reduce 累积计算
来源：http://hz.aibaodan.cn/gtqtfwspxn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.redwolf501.top/gtueajhvjw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zycfv.cn/gtpuakkijz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.chenlongwang.top/gteoqiktxk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.52xcode.cn/gtvkcjokjh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yvedp.cn/gtrqbukydr.html

Go:   // 手写循环
来源：http://hz.gogol.net.cn/gtufwpnntm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.xziqi.cn/gtssjafbsk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.redwolf501.top/gtofkzlqgq.html

[D24] 字典 / Map 基本操作
来源：http://hz.fzhhl.top/gtehesacbo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yanxiufei.cn/gtqngkwzcb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yuanzhike.top/gtrdcraftk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.hywenlv.cn/gthrpxnwrv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.shzxlz.cn/gtoqypoknv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.daria6918.cn/gtgjhftzas.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.nanxinkj.top/gtxiuwpvth.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.meibo888.top/gtahxcitjy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.ywan-chungtsiang.top/gtmrcnkyhl.html

[D25] Set 集合去重与交并差
来源：http://hz.aizwys.cn/gterkbhrdr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jiagoushi.top/gtzueenbtv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jinqigufen.top/gtcqgxipag.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.guowangkeji.top/gtsuiibebl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.sysykeji.top/gtakqotliz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.svipenyu.cn/gtgazaojup.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.nanxinkj.top/gthxvffszv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.tanke756.top/gtnqeoawqv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.havefunace.top/gtvkpxxsos.html

[D26] 数组转字符串
来源：http://hz.dianchejie.cn/gtfbekqcyk.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zhaomingkeji.xyz/gtvpxktlzf.html

PHP:  implode(", ", $arr);
来源：http://hz.birdmap.top/gtrjmnlsoq.html

JS:   arr.join(", ")
来源：http://hz.yongpay.top/gtuoejvram.html

TS:   arr.join(", ")
来源：http://hz.mhx1999.top/gtidqbsxty.html

Java: String.join(", ", list)
来源：http://hz.ybcxt.top/gtcdnakwed.html

Go:   strings.Join(strs, ", ")
来源：http://hz.cqqwz.cn/gtoepoilul.html

Ruby: arr.join(", ")
来源：http://hz.0kj1m.cn/gtladweugd.html

C#:   string.Join(", ", list)
来源：http://hz.jlsjyb.cn/gtzzazilag.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtihlkykwj.html

E. 字符串处理
来源：http://hz.jinqigufen.top/gtoptvexov.html

================================================================================
来源：http://hz.gzhubu.top/gtzvmoxjug.html

[E01] 拼接字符串
来源：http://hz.hammf.cn/gtpxjopbky.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yj20258888.top/gtfvzbwhjz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yangfankeji.com/gtkqdnhgej.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.quarkkingdee.top/gtwnmoqfks.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.316326.xyz/gtzrvtkwoz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.ybcxt.top/gtnknkuuhr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jlsjyb.cn/gtyizehzqu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.tianlin.xyz/gthuuseqkj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jqgufenzy.top/gtfgupdzxg.html

[E02] 重复字符串
来源：http://hz.quarkkingdee.top/gtyabcofak.html

Py:   "ab" * 3
来源：http://hz.tanke756.top/gtdywzcryy.html

PHP:  str_repeat("ab", 3);
来源：http://hz.hnxiangtu.top/gtlszlinoa.html

JS:   "ab".repeat(3)
来源：http://hz.yanxiufei.cn/gthtzihpks.html

TS:   "ab".repeat(3)
来源：http://hz.xziqi.cn/gtpkzuaafb.html

Java: "ab".repeat(3)
来源：http://hz.sysykeji.top/gtresizkzz.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.bjfxy.top/gtvncwyagk.html

Ruby: "ab" * 3
来源：http://hz.hywenlv.cn/gtukbjndjb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yuanzhike.top/gtfjccqnyg.html

[E03] 截取子串
来源：http://hz.yuanzhike.top/gtshwmepbi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.fengsongda.top/gtgrulvhfz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yj20258.top/gtydrmyxyy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.ivvv.top/gtittbacxp.html

TS:   s.slice(1, 4)
来源：http://hz.smart0.xyz/gtvtlpfbdk.html

Java: s.substring(1, 4)
来源：http://hz.hysaishi.cn/gtmcdbiwwt.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.wangshuangyany.cn/gtaiyrsdvm.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.xinyue.icu/gtoxnqchoa.html

C#:   s.Substring(1, 3)
来源：http://hz.xziqi.cn/gtrwvojpst.html

[E04] 查找子串位置
来源：http://hz.jlsjyb.cn/gtyffvguvh.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yueranfly.top/gtiimwmbzb.html

PHP:  strpos($s, "x");
来源：http://hz.jinqigufen.top/gtkrnavyoj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.daxiang520.top/gtbzwtqolz.html

TS:   s.indexOf("x")
来源：http://hz.yuxming.cn/gtsbnefwlp.html

Java: s.indexOf("x")
来源：http://hz.hammf.cn/gtfbocrbui.html

Go:   strings.Index(s, "x")
来源：http://hz.jinqigfzy.top/gtxzpqbrpc.html

Ruby: s.index("x")
来源：http://hz.cucudq.cn/gthadezack.html

C#:   s.IndexOf("x")
来源：http://hz.cucudq.cn/gtfrpffsql.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.xylfe.cn/gtzvtfpyxl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.wangdashe.top/gtvlurgmvg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhixingplan.top/gtunohkvol.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.snrcjt.cn/gtvuyipvti.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.cheryme.top/gterkdphex.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hywenlv.cn/gtbtkpfbss.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.sweek.top/gtuulsidie.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.nanxinkj.top/gtaiwzsabv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.316326.xyz/gtbgfrdbgv.html

[E06] 替换子串
来源：http://hz.sufxvd.cn/gtosyedppj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jiagoushi.top/gthkkjwkma.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.ivvv.top/gtppbmukxr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.meibo888.top/gttbxgdgez.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zhixingplan.top/gtfuwuyzmo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zycfv.cn/gthlqqzhti.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jyoumei.cn/gtxyppkkgi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.cheryme.top/gtyjuidlla.html

C#:   s.Replace("a", "b")
来源：http://hz.xziqi.cn/gtknhicbnk.html

[E07] 按分隔符拆分
来源：http://hz.bjfxy.top/gtzfszzgaf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.sweek.top/gtivhoeqxv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yvedp.cn/gthvvhdmsu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.jinghuilouyu.cn/gtlgbipdiz.html

TS:   s.split(",")
来源：http://hz.chenjidiqi.icu/gtgnnjgayd.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.xziqi.cn/gteklqvygj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zdqjudy.top/gtkmnutypa.html

Ruby: s.split(",");  s.split
来源：http://hz.chenzaomai.com/gtjmhcbpnz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yueranfly.top/gtsghlxbpf.html

[E08] 数组按分隔符合并
来源：http://hz.daria6918.cn/gtjsshlska.html

Py:   ",".join(items)
来源：http://hz.52xcode.cn/gtxloafbwl.html

PHP:  implode(",", $items);
来源：http://hz.sufxvd.cn/gtnqhrxlpb.html

JS:   items.join(",")
来源：http://hz.ppjwa.cn/gtbqoydkpf.html

TS:   items.join(",")
来源：http://hz.hammf.cn/gtzpooeelx.html

Java: String.join(",", items)
来源：http://hz.havefunace.top/gtntlbolmw.html

Go:   strings.Join(items, ",")
来源：http://hz.yonumen.top/gtmqreulrb.html

Ruby: items.join(",")
来源：http://hz.dashuyun.cn/gtjuewttuc.html

C#:   string.Join(",", items)
来源：http://hz.dashuyun.cn/gtlqvwxryy.html

[E09] 去除所有空白字符
来源：http://hz.iojbl.cn/gtgmndpobc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zdqjudy.top/gtshnddzha.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.havefunace.top/gtvxopyowd.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jiagoushi.top/gtfpgjutcb.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.9152youxi.cn/gttpmhvhrn.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.c1oappe.top/gtuodgldiy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yuanzhike.top/gttptmlpws.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zhijiandao.cn/gtlzctfioo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.redwolf501.top/gtmrpsqrdn.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ywan-chungtsiang.top/gtawhkkzxb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.birdmap.top/gtxswuebny.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.nanxinkj.top/gtnxmfdnaf.html

JS:   "7".padStart(3, "0")
来源：http://hz.ehwqpu.com/gtbqemlbmb.html

TS:   "7".padStart(3, "0")
来源：http://hz.cashguo.top/gtnnsahxgk.html

Java: String.format("%03d", 7)
来源：http://hz.yanxiufei.cn/gtkdztqjhc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.shanyushiyangtech.top/gtjypuqhoo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.ydjk.org.cn/gtbvtvludy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.nanxuanxn.top/gtujjnsygw.html

[E11] 反转字符串
来源：http://hz.shzxlz.cn/gtgrghfgru.html

Py:   s[::-1]
来源：http://hz.gaohongyu789.top/gtvcasdtgk.html

PHP:  strrev($s);
来源：http://hz.jianghu66.top/gtcoanjcnh.html

JS:   [...s].reverse().join("")
来源：http://hz.redwolf501.top/gtmmhnxuvl.html

TS:   [...s].reverse().join("")
来源：http://hz.jinqigfzy.top/gtlvnkmaxj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.guannengcc.top/gthwmaogfr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ppjwa.cn/gtidasrxxq.html

Ruby: s.reverse
来源：http://hz.hnqzz.top/gtuqdwrned.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.ydjk.org.cn/gtcdajztph.html

[E12] 统计某字符出现次数
来源：http://hz.hongshengwenyu.top/gtlpyectes.html

Py:   s.count("a")
来源：http://hz.jqgufenzy.top/gtsnjjllnl.html

PHP:  substr_count($s, "a");
来源：http://hz.guannengcc.top/gtxehsixop.html

JS:   s.split("a").length - 1
来源：http://hz.ydzc1.top/gteceegpol.html

TS:   s.split("a").length - 1
来源：http://hz.zhaomingkeji.xyz/gteaplieug.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.mhx1999.top/gtniumdpll.html

Go:   strings.Count(s, "a")
来源：http://hz.sxryk.cn/gtxkzkmpvi.html

Ruby: s.count("a")
来源：http://hz.shuidangran.top/gtvaztdscn.html

C#:   s.Count(c => c == 'a')
来源：http://hz.dashuyun.cn/gtkffbkpwm.html

[E13] 逐字符遍历
来源：http://hz.jinghuilouyu.cn/gtlafbsoeb.html

Py:   for ch in s: print(ch)
来源：http://hz.ydzc1.top/gtubaodmhh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ivvv.top/gttzbsoawp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xylfe.cn/gtyzndttjh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.havefunace.top/gtwggyysod.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jinyuanbaomall.cn/gtvvngojxg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.cdnleiting.top/gtdzrlqvau.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yuxming.cn/gtkynxezhi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jinghuilouyu.cn/gtshzyhaki.html

[E14] URL 编码与 Base64
来源：http://hz.yvedp.cn/gthijvcvpx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.guannengcc.top/gtygthmlxu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.fzhhl.top/gthzgtycce.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jqgfzy.top/gtokbuwrfu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.hfpthk.cn/gtsqeoqfbd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yvedp.cn/gtkixdwqcn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.shanyushiyangtech.top/gtcfusmnxz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.shanyushiyangkeji.top/gtvhgvfwjk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhijiandao.cn/gtgdbpxvyl.html

[E15] HTML 转义 / 反转义
来源：http://hz.9152youxi.cn/gtrtugjlao.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.nanxinkj.top/gtwxugacyu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jinyuanbaomall.cn/gtkuatapvx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ppjwa.cn/gtrdugsrqd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.cdnleiting.top/gthbnzertn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jinqigufen.top/gthkzyahev.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.cucudq.cn/gtztcgmyek.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.aibaodan.cn/gthdrdpwkt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.hnxiangtu.top/gtbdgimatk.html

[E16] 数字千分位
来源：http://hz.tian-w.cn/gtivrxpvrv.html

Py:   f"{1234567:,}"
来源：http://hz.smart0.xyz/gtviyzurso.html

PHP:  number_format(1234567);
来源：http://hz.shangyingyoupin.top/gtfboajgfh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.nanxinkj.top/gtydwjgblz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.cheryme.top/gtwxrxsbue.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.nwbrower.top/gtupxkuqcv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jianghu66.top/gteoazmqbi.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.ivvv.top/gtqzxqwxap.html

C#:   1234567.ToString("N0")
来源：http://hz.cqqwz.cn/gtsssxiqyf.html

[E17] 首字母大写
来源：http://hz.zhixingplan.top/gtukthudkf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yongpay.top/gtdvingdxl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.316326.xyz/gtyjtglfwn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jiagoushi.top/gtoiqclckz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jianghu66.top/gtnwnddzya.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zhiwuduotai.top/gtoumwbljw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.havefunace.top/gtcwedpjeb.html

Ruby: s.capitalize
来源：http://hz.birdmap.top/gtknkiggte.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.52xcode.cn/gtnphrziwj.html

[E18] 模板占位符替换
来源：http://hz.nwbrower.top/gtfjpxijzm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.xylfe.cn/gtivtmcqly.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yuxming.cn/gtvxiyckbw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.pycfn.com/gtyqxzaarq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.xylfe.cn/gturfinjvj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hysaishi.cn/gtwkrghwmu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ydzc1.top/gtlesaxmrl.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hammf.cn/gtwaokpgbz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.gogol.net.cn/gteyqekaug.html

[E19] 多行文本按行拆分
来源：http://hz.wangshuangyany.cn/gtojoumole.html

Py:   s.splitlines()
来源：http://hz.ydjk.org.cn/gtpxjnaitp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.havefunace.top/gtbvovkjjx.html

JS:   s.split(/\r?\n/)
来源：http://hz.bjfxy.top/gtkzdoqxzd.html

TS:   s.split(/\r?\n/)
来源：http://hz.daxiang520.top/gttlmnoaif.html

Java: s.lines().toList()
来源：http://hz.hnqzz.top/gtwyokmxpu.html

Go:   strings.Split(s, "\n")
来源：http://hz.tianlin.xyz/gtwsfmxzuu.html

Ruby: s.lines
来源：http://hz.kuanghao11.cn/gtrtyixjxq.html

C#:   s.Split('\n')
来源：http://hz.fzhhl.top/gtgzukepbk.html

[E20] 判断字符串是否为空
来源：http://hz.xingfuxueyuan.xyz/gtbynumdzy.html

Py:   if not s:
来源：http://hz.redwolf501.top/gtudfqhwtx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.shanyushiyangkeji.top/gtgrvtxxmn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jyoumei.cn/gtsqrlxkjw.html

TS:   if (s === "") {}
来源：http://hz.daria6918.cn/gtzghguyyi.html

Java: if (s.isEmpty()) {}
来源：http://hz.dashuyun.cn/gtfpaftqoj.html

Go:   if s == "" {}
来源：http://hz.shuidangran.top/gtsouwmwqy.html

Ruby: if s.empty?
来源：http://hz.mhx1999.top/gtukdeatjs.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.316326.xyz/gtqyyvgycw.html

[E21] 超长截断加省略号
来源：http://hz.zhoulong.xyz/gtwsdpmrwz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.xuetiantiany.cn/gtdntxdbcv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.hammf.cn/gtnvrmkofh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.pengpengdd.cyou/gtbwjzsbwc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.nanxinkj.top/gtyxyrfkax.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.shanyushiyangkeji.top/gtkxbmuhgc.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ppjwa.cn/gtxtdukfkt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.fzhhl.top/gtbnshckmg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ywan-chungtsiang.top/gtntjkcquc.html

[E22] 字节长度与字符长度
来源：http://hz.ehwqpu.com/gtdxeojpfa.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.wangdashe.top/gtqsrvffqv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.iojbl.cn/gtiluuvgls.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhiwuduotai.top/gtaihodbxt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.nanxuanxn.top/gtivoqtbzb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yonumen.top/gtpzocqjdk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.svipenyu.cn/gtlywoward.html

Ruby: s.bytesize;  s.length
来源：http://hz.kuanghao11.cn/gtclgmlhqv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.hnqzz.top/gtrmqspneq.html

================================================================================
来源：http://hz.cqqwz.cn/gtwuvziasc.html

F. 文件与目录
来源：http://hz.guannengcc.top/gtwefihfes.html

================================================================================
来源：http://hz.daria6918.cn/gtlyqsopju.html

[F01] 读取整个文件
来源：http://hz.ehwqpu.com/gtecltbgyo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.gzhubu.top/gtkfcrsndg.html

PHP:  file_get_contents("a.txt");
来源：http://hz.tanke756.top/gtlnppejhg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.gaohongyu789.top/gtzuhkurtp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.ydzc1.top/gtbxlslfhy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.9152youxi.cn/gtdnktlklm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.feifeiyinyue.top/gtcbmshmyr.html

Ruby: File.read("a.txt")
来源：http://hz.yj20258.top/gtmuldxykh.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yanxiufei.cn/gterafpbgt.html

[F02] 逐行读取文件
来源：http://hz.snrcjt.cn/gtvovreliy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.shanyushiyangkeji.top/gtkozmgfve.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jyoumei.cn/gtnteuegwe.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cqqwz.cn/gtltcmutlk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.guannengcc.top/gtltkccglk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hnxiangtu.top/gtxxgdjfnp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.c1oappe.top/gtkodxwvir.html


<!-- 参考信息 -->