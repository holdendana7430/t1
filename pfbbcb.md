代发 wailian999

[D15] 去重
来源：http://hz.jlsjyb.cn/gtapworqmu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zycfv.cn/gtbdmpksmi.html

PHP:  array_unique($arr);
来源：http://hz.shuidangran.top/gtwhueaxpn.html

JS:   [...new Set(arr)]
来源：http://hz.yvedp.cn/gtbbtgypqb.html

TS:   [...new Set(arr)]
来源：http://hz.hnxiangtu.top/gtgcbojsjp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hammf.cn/gtcyxkukbe.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hnxiangtu.top/gtvqzxaosx.html

Ruby: arr.uniq
来源：http://hz.ybcxt.top/gtyqktbxbm.html

C#:   list.Distinct().ToList()
来源：http://hz.xuetiantiany.cn/gtewxobxpx.html

[D16] 求和与平均值
来源：http://hz.52xcode.cn/gtteygucut.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jinqigufen.top/gthyhgbhbl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.ppjwa.cn/gtypwvybxe.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cdnleiting.top/gtpqaasyav.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ydjk.org.cn/gtnrtdewux.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yanxiufei.cn/gtppbblykz.html

Go:   // 手写循环累加
来源：http://hz.pengpengdd.cyou/gttibdntcu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhongyouzk.top/gtmvtzeawi.html

C#:   list.Sum();  list.Average()
来源：http://hz.jinqigufen.top/gtljenjbmm.html

[D17] 最大值与最小值
来源：http://hz.tianlin.xyz/gtccemkyog.html

Py:   max(arr);  min(arr)
来源：http://hz.316326.xyz/gtnqazylto.html

PHP:  max($arr);  min($arr);
来源：http://hz.c1oappe.top/gtbuthokog.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.ywan-chungtsiang.top/gtjsdqpvan.html

TS:   Math.max(...arr);
来源：http://hz.hfpthk.cn/gtbwdmloib.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.xziqi.cn/gtqawnzdph.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.sysykeji.top/gtlvjuxgwx.html

Ruby: arr.max;  arr.min
来源：http://hz.shuidangran.top/gtkoavobbg.html

C#:   list.Max();  list.Min()
来源：http://hz.tanke756.top/gtqrkxdewh.html

[D18] 扁平化嵌套数组
来源：http://hz.yvedp.cn/gtxhjijgfy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.hnqzz.top/gtqvjfwtdl.html

PHP:  array_merge(...$nested);
来源：http://hz.yangfankeji.com/gtbobuwduk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.svipenyu.cn/gtyjakoycu.html

TS:   nested.flat();
来源：http://hz.jqgfzy.top/gtoiywdjft.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ybcxt.top/gtlvpgykvk.html

Go:   // 手写双层循环
来源：http://hz.cheryme.top/gthnosvydc.html

Ruby: nested.flatten
来源：http://hz.jinqigufen.top/gtacqhhidc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.sysykeji.top/gtahubrdlg.html

[D19] 按字段分组
来源：http://hz.hnxiangtu.top/gtqhjgewzf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.svipenyu.cn/gtlmozalub.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jlsjyb.cn/gtzovsitlj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.sysykeji.top/gtncivjbpm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.snrcjt.cn/gtbwwwdrlp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.xylfe.cn/gtutkpkowk.html

Go:   // 手写 map[string][]T
来源：http://hz.jqgfzy.top/gtaylvwmmb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.cdnleiting.top/gtidseziod.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.c1oappe.top/gtiridaqqg.html

[D20] 统计每个元素出现次数
来源：http://hz.xuetiantiany.cn/gtgipdarww.html

Py:   Counter(arr)
来源：http://hz.jyoumei.cn/gthacuktag.html

PHP:  array_count_values($arr);
来源：http://hz.xuetiantiany.cn/gtsimaqegv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinqigfzy.top/gtzkbgxiyx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.havefunace.top/gtsysyhkca.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.chenzaomai.com/gtyzwatzgi.html

Go:   // 手写 map[T]int
来源：http://hz.tian-w.cn/gtlkgoxvcg.html

Ruby: arr.tally
来源：http://hz.jiagoushi.top/gtxnlxgwbj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.xuanzx.com/gtdhjjjdrr.html

[D21] 判断是否包含某元素
来源：http://hz.pengpengdd.cyou/gtejfnounw.html

Py:   x in arr
来源：http://hz.hfpthk.cn/gtpmhjogdy.html

PHP:  in_array($x, $arr, true);
来源：http://hz.tanke756.top/gtgbnrsjdy.html

JS:   arr.includes(x)
来源：http://hz.kuanghao11.cn/gtoxmrqvoc.html

TS:   arr.includes(x)
来源：http://hz.hnqzz.top/gtrssiueem.html

Java: list.contains(x)
来源：http://hz.aibaodan.cn/gtpfsejjuu.html

Go:   slices.Contains(arr, x)
来源：http://hz.yongpay.top/gttocrtqvi.html

Ruby: arr.include?(x)
来源：http://hz.ywan-chungtsiang.top/gtbqygfrrt.html

C#:   list.Contains(x)
来源：http://hz.dianchejie.cn/gtakokryor.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zhaomingkeji.xyz/gtftmmpsmt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.cashguo.top/gtypnuhdba.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.cucudq.cn/gtmabswkpt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.redwolf501.top/gtorsidwba.html

TS:   [...arr];
来源：http://hz.xinyue.icu/gtavajjtxm.html

Java: new ArrayList<>(list);
来源：http://hz.shuidangran.top/gtcsjfkgnq.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.havefunace.top/gtfryqobvy.html

Ruby: arr.dup;  arr.clone
来源：http://hz.wangdashe.top/gtrnhxgksz.html

C#:   new List<int>(list);
来源：http://hz.jqgfzy.top/gtnkiospjg.html

[D23] reduce 累积计算
来源：http://hz.kuanghao11.cn/gtkfbnbkpi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jqgufenzy.top/gtwwiuyzde.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.cheryme.top/gtghzbwyvu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.svipenyu.cn/gtwndccqlg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.quarkkingdee.top/gtigsqfvcb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zycfv.cn/gtwgofbcuv.html

Go:   // 手写循环
来源：http://hz.tianlin.xyz/gtvhxzmksg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zhijiandao.cn/gtcsmxrdno.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.svipenyu.cn/gtpwntsktg.html

[D24] 字典 / Map 基本操作
来源：http://hz.zycfv.cn/gtlazijopz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.xuanzx.com/gtunnaqigr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.cheryme.top/gtjelxatvk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.chenlongwang.top/gtffjymrct.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.xingfuxueyuan.xyz/gtcekhlowl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zhiwuduotai.top/gtyedrburf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.shzxlz.cn/gturfenndk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.hysaishi.cn/gtdkbwdctl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.mhx1999.top/gtgpvmrlgj.html

[D25] Set 集合去重与交并差
来源：http://hz.jinyuanbaomall.cn/gtxvnjqfmq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.wangshuangyany.cn/gtoqawmfnq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.shzxlz.cn/gthtoxavjj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.0kj1m.cn/gtjnkqdibr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.pengpengdd.cyou/gtgsmumizu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.ywan-chungtsiang.top/gtnydedoit.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.shangyingyoupin.top/gtnswitwip.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jlsjyb.cn/gtyjycgvrw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.quarkkingdee.top/gtnuaxgpav.html

[D26] 数组转字符串
来源：http://hz.hnxiangtu.top/gtqiebebdl.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zhixingplan.top/gtbbophlgq.html

PHP:  implode(", ", $arr);
来源：http://hz.ivvv.top/gtoygsbcgp.html

JS:   arr.join(", ")
来源：http://hz.yuxming.cn/gttmmpvsjl.html

TS:   arr.join(", ")
来源：http://hz.mhx1999.top/gtkvvgjmkj.html

Java: String.join(", ", list)
来源：http://hz.c1oappe.top/gttclmntoc.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yanxiufei.cn/gtixpmrwhn.html

Ruby: arr.join(", ")
来源：http://hz.gzhubu.top/gtljmnvzph.html

C#:   string.Join(", ", list)
来源：http://hz.zhongyouzk.top/gtvizrpgkx.html

================================================================================
来源：http://hz.xinyue.icu/gtcykyduvw.html

E. 字符串处理
来源：http://hz.kuanghao11.cn/gtmfhephvt.html

================================================================================
来源：http://hz.jlsjyb.cn/gtjehehqop.html

[E01] 拼接字符串
来源：http://hz.andypj.xyz/gtzqeqczij.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ybcxt.top/gthmvpgavd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.daxiang520.top/gtphdvlgvu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinqigfzy.top/gtkmrzmvhs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenjidiqi.icu/gtqxuyyyxt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.zycfv.cn/gthucuxxsd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zhixingplan.top/gtcfixasxj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.chenlongwang.top/gtiordvqih.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.316326.xyz/gtmoivnnmk.html

[E02] 重复字符串
来源：http://hz.jyoumei.cn/gtdlojfmdc.html

Py:   "ab" * 3
来源：http://hz.hysaishi.cn/gthiktsqrr.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zycfv.cn/gtkfeggzla.html

JS:   "ab".repeat(3)
来源：http://hz.svipenyu.cn/gtjqvnwiok.html

TS:   "ab".repeat(3)
来源：http://hz.hfpthk.cn/gtzitgvqmf.html

Java: "ab".repeat(3)
来源：http://hz.c1oappe.top/gtxdoqofdw.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.hammf.cn/gtpuqtvqzh.html

Ruby: "ab" * 3
来源：http://hz.svipenyu.cn/gtrqfftray.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.guowangkeji.top/gthwbbbruq.html

[E03] 截取子串
来源：http://hz.yueranfly.top/gtiucafmcf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.cqqwz.cn/gtigvtlrfd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.hammf.cn/gtqquijywj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.aibaodan.cn/gtjtkgftrp.html

TS:   s.slice(1, 4)
来源：http://hz.fengsongda.top/gtdkxvviqk.html

Java: s.substring(1, 4)
来源：http://hz.ydjk.org.cn/gtpmblacmf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.chenlongwang.top/gtssycpqyq.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jinqigufen.top/gtsywfzdpz.html

C#:   s.Substring(1, 3)
来源：http://hz.jqgufenzy.top/gtoatmburq.html

[E04] 查找子串位置
来源：http://hz.feifeiyinyue.top/gtpckfifby.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jinghuilouyu.cn/gtyknqfdhb.html

PHP:  strpos($s, "x");
来源：http://hz.yuxming.cn/gtqdnvpzoi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.fengsongda.top/gtpntesgxe.html

TS:   s.indexOf("x")
来源：http://hz.cdnleiting.top/gtbkjddmge.html

Java: s.indexOf("x")
来源：http://hz.redwolf501.top/gtozdbxucu.html

Go:   strings.Index(s, "x")
来源：http://hz.ppjwa.cn/gtieiwxaig.html

Ruby: s.index("x")
来源：http://hz.hammf.cn/gtrsbdkwvv.html

C#:   s.IndexOf("x")
来源：http://hz.yongpay.top/gtjmfjbbsi.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.hysaishi.cn/gtjwmrcexk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.daria6918.cn/gtndttzumi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhongyouzk.top/gtynmujdwq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xziqi.cn/gtcpidnpan.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhixingplan.top/gtqljnnpba.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yanxiufei.cn/gtavnhzgiy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.zhoulong.xyz/gtwdbxiesx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.zhengqikj.top/gtvmexjttx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.dashuyun.cn/gthkawezna.html

[E06] 替换子串
来源：http://hz.yanxiufei.cn/gtrnabdukc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.gzhubu.top/gthuqcnhbt.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.mhx1999.top/gtnytcxajr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sweek.top/gtpdbctrjb.html

TS:   s.replaceAll("a", "b")
来源：http://hz.cdnleiting.top/gtbxolalny.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yongpay.top/gtfmnquytv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.vqdsnc.cn/gtebagjwku.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.haohaochexian.top/gtguhyblxi.html

C#:   s.Replace("a", "b")
来源：http://hz.zhijiandao.cn/gtnvbwqibd.html

[E07] 按分隔符拆分
来源：http://hz.ydzc1.top/gtkhfgsqjq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.fengsongda.top/gtvuhagszi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.52xcode.cn/gtgknotlui.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.sweek.top/gtcbshkpve.html

TS:   s.split(",")
来源：http://hz.meibo888.top/gtkcncbtjy.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.tanke756.top/gtospthdxh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.sufxvd.cn/gtdeltxfuv.html

Ruby: s.split(",");  s.split
来源：http://hz.gogol.net.cn/gtzdjxoqsr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.chenlongwang.top/gttbuugqtr.html

[E08] 数组按分隔符合并
来源：http://hz.zhixingplan.top/gtminwbwlq.html

Py:   ",".join(items)
来源：http://hz.hnxiangtu.top/gtotdcmzkq.html

PHP:  implode(",", $items);
来源：http://hz.cqqwz.cn/gtniysiacu.html

JS:   items.join(",")
来源：http://hz.zycfv.cn/gtyukeacgd.html

TS:   items.join(",")
来源：http://hz.jqgfzy.top/gthxoxyudk.html

Java: String.join(",", items)
来源：http://hz.gotoacloud.top/gtqpidwjcy.html

Go:   strings.Join(items, ",")
来源：http://hz.yuxming.cn/gtttfdqyub.html

Ruby: items.join(",")
来源：http://hz.chenjidiqi.icu/gtjnmprkpz.html

C#:   string.Join(",", items)
来源：http://hz.wangdashe.top/gtiecunxye.html

[E09] 去除所有空白字符
来源：http://hz.pycfn.com/gtwtbdlapg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.nwbrower.top/gtnpajulcn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.andypj.xyz/gtiomcaove.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.havefunace.top/gtvcfibkbm.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yonumen.top/gtqqwawohu.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.hywenlv.cn/gtsmksmodh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.nanxuanxn.top/gtysafmwsw.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.xuanzx.com/gtfrgwllqk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.c1oappe.top/gtmrxcwlmi.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xziqi.cn/gtmqvektzl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.smart0.xyz/gtpelhpxuf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.zhijiandao.cn/gtwmbjhjzb.html

JS:   "7".padStart(3, "0")
来源：http://hz.0kj1m.cn/gtrmhsgjhu.html

TS:   "7".padStart(3, "0")
来源：http://hz.ydjk.org.cn/gtemhfaluq.html

Java: String.format("%03d", 7)
来源：http://hz.jinghuilouyu.cn/gtzcalubif.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ppjwa.cn/gtbfpvbwba.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.nanxinkj.top/gtzogxgnok.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.mhx1999.top/gtzfzymgim.html

[E11] 反转字符串
来源：http://hz.yueranfly.top/gtetmelzxx.html

Py:   s[::-1]
来源：http://hz.shzxlz.cn/gtarughpga.html

PHP:  strrev($s);
来源：http://hz.daxiang520.top/gtkkbpbzzv.html

JS:   [...s].reverse().join("")
来源：http://hz.nanxuanxn.top/gtllmquaom.html

TS:   [...s].reverse().join("")
来源：http://hz.ywan-chungtsiang.top/gtqkavdslc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.xingfuxueyuan.xyz/gtuhjhyedk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hnxiangtu.top/gtlqjgoypf.html

Ruby: s.reverse
来源：http://hz.sufxvd.cn/gtqcbjjahh.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.shanyushiyangkeji.top/gtdrkfdrgs.html

[E12] 统计某字符出现次数
来源：http://hz.9152youxi.cn/gtipiujkeq.html

Py:   s.count("a")
来源：http://hz.jlsjyb.cn/gtjgftcsit.html

PHP:  substr_count($s, "a");
来源：http://hz.yvedp.cn/gtvnwuvigo.html

JS:   s.split("a").length - 1
来源：http://hz.aizwys.cn/gtywrouerb.html

TS:   s.split("a").length - 1
来源：http://hz.sysykeji.top/gtiwumogcj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.c1oappe.top/gtwwbibzig.html

Go:   strings.Count(s, "a")
来源：http://hz.yangfankeji.com/gtwzeztnbr.html

Ruby: s.count("a")
来源：http://hz.ppjwa.cn/gtlzwnzbcz.html

C#:   s.Count(c => c == 'a')
来源：http://hz.aizwys.cn/gtpklxzmya.html

[E13] 逐字符遍历
来源：http://hz.zhongyouzk.top/gtcdsdwalj.html

Py:   for ch in s: print(ch)
来源：http://hz.shuidangran.top/gtjyimfbzu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.fzhhl.top/gtudjmtbhb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gaohongyu789.top/gtqarmquut.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.redwolf501.top/gtzxfirmkv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.haohaochexian.top/gtlmrbadhh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jlsjyb.cn/gtumbtjiqb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.hywenlv.cn/gtiucgidtv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jyoumei.cn/gtjllpppyb.html

[E14] URL 编码与 Base64
来源：http://hz.redwolf501.top/gtddarmraj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.gotoacloud.top/gthtjnfhix.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yuxming.cn/gttdwnelcb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.ivvv.top/gtcukkyklq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.shanyushiyangkeji.top/gtrelzdwbw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.tianlin.xyz/gtjpneohgr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.cucudq.cn/gtxswfsbjz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yj20258888.top/gthkegwxmp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xingfuxueyuan.xyz/gtunqhayln.html

[E15] HTML 转义 / 反转义
来源：http://hz.c1oappe.top/gtedzzibwu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.wangdashe.top/gtfeizmpzd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.sysykeji.top/gtuyfiwnuh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zhengqikj.top/gtnvexbofx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.cucudq.cn/gtykvpifam.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jinghuilouyu.cn/gtxboejtjr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.gotoacloud.top/gturidfgpy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.ybcxt.top/gtmdkegrwg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jlsjyb.cn/gtyzwzgagm.html

[E16] 数字千分位
来源：http://hz.wangshuangyany.cn/gtenfamfiw.html

Py:   f"{1234567:,}"
来源：http://hz.fengsongda.top/gtvnujuvqi.html

PHP:  number_format(1234567);
来源：http://hz.guannengcc.top/gtnuuhymlb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.shzxlz.cn/gteoaxkabs.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.aizwys.cn/gtuvvscxwe.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.dianchejie.cn/gtltubgrxl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.xuetiantiany.cn/gtlpbopcaq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.havefunace.top/gtxachrwwq.html

C#:   1234567.ToString("N0")
来源：http://hz.hammf.cn/gtjimhwtxu.html

[E17] 首字母大写
来源：http://hz.iojbl.cn/gtvtjuuvuf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.jinyuanbaomall.cn/gtafhihnqk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.ydjk.org.cn/gtqtplwflq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhoulong.xyz/gtgsamycqe.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ydzc1.top/gtqdewvyyc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.andypj.xyz/gtjvkxavwi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.sufxvd.cn/gtoblieleb.html

Ruby: s.capitalize
来源：http://hz.pycfn.com/gtzssgkkns.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yuanzhike.top/gtqkxavmmr.html

[E18] 模板占位符替换
来源：http://hz.xylfe.cn/gtolcmitkp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.redwolf501.top/gtpknbiwth.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jlsjyb.cn/gtncdbfsee.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.smart0.xyz/gtvezivqse.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.52xcode.cn/gtheftjncq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.fengsongda.top/gtmzohfeeb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.smart0.xyz/gtwttsxsdb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.daxiang520.top/gtzfcpgjvy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yongpay.top/gtcnhatayw.html

[E19] 多行文本按行拆分
来源：http://hz.shanyushiyangkeji.top/gtbbxnsxhv.html

Py:   s.splitlines()
来源：http://hz.pengpengdd.cyou/gthboedmrj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.ivvv.top/gteaxbagqb.html

JS:   s.split(/\r?\n/)
来源：http://hz.cqqwz.cn/gtlxisaxzj.html

TS:   s.split(/\r?\n/)
来源：http://hz.jianghu66.top/gtmuqyzywk.html

Java: s.lines().toList()
来源：http://hz.0kj1m.cn/gtouaeqskl.html

Go:   strings.Split(s, "\n")
来源：http://hz.zhoulong.xyz/gtzfumwydr.html

Ruby: s.lines
来源：http://hz.xinyue.icu/gtrhyfqwxl.html

C#:   s.Split('\n')
来源：http://hz.meibo888.top/gttlcljnwx.html

[E20] 判断字符串是否为空
来源：http://hz.zhoulong.xyz/gtppmexpow.html

Py:   if not s:
来源：http://hz.dashuyun.cn/gtfsnoldnw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.aibaodan.cn/gtshmiijwm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.xingfuxueyuan.xyz/gtrqhhcuoi.html

TS:   if (s === "") {}
来源：http://hz.yangfankeji.com/gtjbksurnh.html

Java: if (s.isEmpty()) {}
来源：http://hz.zhengqikj.top/gtgtitpizv.html

Go:   if s == "" {}
来源：http://hz.zdqjudy.top/gtywaduoup.html

Ruby: if s.empty?
来源：http://hz.hfpthk.cn/gtycotgvii.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.daxiang520.top/gttsiyxzap.html

[E21] 超长截断加省略号
来源：http://hz.tianlin.xyz/gtuwnzkmeb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.9152youxi.cn/gtevmasyxa.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yonumen.top/gtmvienmgp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ydzc1.top/gtmdpgeulb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinqigufen.top/gtinioungh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.shanyushiyangtech.top/gttkeaarrr.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.sufxvd.cn/gtikmviwwx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.vqdsnc.cn/gtpxwyhxww.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.316326.xyz/gtxtnkfxdu.html


<!-- 参考信息 -->