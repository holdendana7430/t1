代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fehbvm.com/Article/details/gsfqgpzxq.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.hesvh.cn/Article/details/gxerpgtfp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.hesvh.cn/Article/details/gajfzycgd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.zdbjq.cn/Article/details/gweqigeev.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/grigzavwl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/ggawmzrma.sHtML

Java: // 无解构
来源：http://www.share.hesvh.cn/Article/details/gelkhpsqi.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/gdkhcocsd.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/ghgxjbbyl.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/gftpvlspo.sHtML

[C16] 函数 / 方法重载
来源：http://baike.zdbjq.cn/Article/details/gcihhumyf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fehbvm.com/Article/details/gyonpiodj.sHtML

PHP:  // 无重载
来源：http://read.share.fehbvm.com/Article/details/gdwpmsvfu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.zdbjq.cn/Article/details/gmdyrzygp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.zdbjq.cn/Article/details/guqhnguuk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/gqvyhefjh.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.zdbjq.cn/Article/details/gjwpgawzo.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.hesvh.cn/Article/details/gekrmlntq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.hesvh.cn/Article/details/gfhthfiug.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnlybhedj.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/gghwfkems.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gencmuvhn.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gpdkcdkbm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.hesvh.cn/Article/details/gbtgamopt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gsdabssdn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/gtlespbiy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/galrgwddp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fehbvm.com/Article/details/gdctejggg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.hesvh.cn/Article/details/gwezyrziv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/gwnpxyjex.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.zdbjq.cn/Article/details/gcnbywetd.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/gmecziapz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fehbvm.com/Article/details/gomrfqnqp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/ggqxknbyj.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/guflxvifa.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gwpchzsmy.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/gokoyvfps.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.zdbjq.cn/Article/details/gxjcqahsf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.hesvh.cn/Article/details/gfsbqcxop.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/giszuysjw.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/gvusvwgzc.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fehbvm.com/Article/details/gaajqvxlx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.hesvh.cn/Article/details/gprholrfp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/gjlusjixd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gpwgscslq.sHtML

Java: list.add(0, 0);
来源：http://blog.fehbvm.com/Article/details/ghatycbyz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.hesvh.cn/Article/details/gvacutqda.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.zdbjq.cn/Article/details/giapltnht.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/gmkwfmcqg.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gpplmpviz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/gljjjllxa.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.zdbjq.cn/Article/details/giidzfdbq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/gmynbfdom.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.hesvh.cn/Article/details/gthfmwxpg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gtfbekhtu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/ghsxbyfll.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gaidbbypf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gasjogeae.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/gzqvakxol.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gfmyljkdi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gxwaropot.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gtncjhqrv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.hesvh.cn/Article/details/gqyxyvpsj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/gdbqltvov.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gyfkrhods.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gdwowkyfl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gfmmoajlh.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/guadafsvw.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/ggcrjnuut.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/gclwyasix.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/giezktddi.sHtML

TS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gouoogndp.sHtML

Java: list.size();
来源：http://mobile.fehbvm.com/Article/details/gccpnlptm.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gtiabbici.sHtML

Ruby: arr.length; arr.size
来源：http://blog.hesvh.cn/Article/details/gydohqlgo.sHtML

C#:   list.Count;
来源：http://3g.zdbjq.cn/Article/details/gbqzdrxba.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.zdbjq.cn/Article/details/gjrpgviqw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/gftokoryc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fehbvm.com/Article/details/gtamhunko.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/grqffrzov.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gieoiytvi.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gootszmwk.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/gpoeaqjmd.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/gsgitlzcx.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/guvdfrfbp.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/gbsaiczxv.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.zdbjq.cn/Article/details/gqdgsklbq.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/gxazxjqhn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/gevlbldct.sHtML

TS:   [...a, ...b];
来源：http://www.blog.hesvh.cn/Article/details/guvndgtcg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/ggoevpawq.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/gtffgnmyc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/ggnpoecvd.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gtymimask.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/ghqwcruts.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gyowhxrti.sHtML

PHP:  sort($arr);
来源：http://3g.zdbjq.cn/Article/details/gfvoqehwc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/gfqbyxahf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fehbvm.com/Article/details/gztmbprzz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/goxpdmlku.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/ggfepwyxw.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gxjiisjdc.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/ghghvtxnx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fehbvm.com/Article/details/gxyhgsefk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fehbvm.com/Article/details/gadnmgsva.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gmyxutzqm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gasppbyfl.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gmhbmvosa.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/gmwvqlkmg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/gbnhmzgdu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.zdbjq.cn/Article/details/ggbtfozyt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.hesvh.cn/Article/details/gfmkaqtpn.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/glyrpbqfa.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/gohocfpjt.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/gghdrontc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/gxpenzgwi.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/glznmpccl.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/gupsqpbap.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/gyqfijjqi.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gejzqoquj.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/ggxcvchdm.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/guteynyww.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.zdbjq.cn/Article/details/gfdezpofa.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gmttyeknv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gwntqjoqm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gillrlcjb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.hesvh.cn/Article/details/gtnmjzszb.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gktwtprbq.sHtML

Ruby: arr.index(x)
来源：http://wap.hesvh.cn/Article/details/gmsfewqlh.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gysdwnglk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/gwujgtswl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gpthxzkot.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/gkjufdpme.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gdckiufmu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gpuratwlb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gdfxpuupd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/gzbzpimwe.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/guswvrnsr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gzewszkke.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/gawpobqdg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/giadxdpuk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gofnzlaeo.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gjbfhjdfx.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gkdrnlnpf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/gwdqjvsiu.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gdunpnfki.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gwhdgffav.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gtwhyevrr.sHtML

[D15] 去重
来源：http://wap.hesvh.cn/Article/details/gqmdmepgs.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gjrmubcox.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/gbsttdiol.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/guqncheoy.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gpzhprsjx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.hesvh.cn/Article/details/ggufjbkst.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/gszvkuqkb.sHtML

Ruby: arr.uniq
来源：http://m.share.hesvh.cn/Article/details/gyeczwjta.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fehbvm.com/Article/details/gmmwhtbta.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/gozckcgiz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gabcdehtp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/gnsocduft.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gjxnpdzxd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gewkxqejy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/gzcvzoema.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/gmfahopuj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/gaocdcnyh.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.zdbjq.cn/Article/details/gzcvwdzqa.sHtML

[D17] 最大值与最小值
来源：http://baike.fehbvm.com/Article/details/gtfiribus.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.zdbjq.cn/Article/details/gonzetfmt.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/gjzqibfww.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.zdbjq.cn/Article/details/gwvbvkewp.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/gfpntplgm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.zdbjq.cn/Article/details/gqzpwuvfg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/gwxgbjptt.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/gcdgznapo.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gqikdaluq.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/grjassrva.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.hesvh.cn/Article/details/gbdpdooxn.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/gcidqhlhn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fehbvm.com/Article/details/gtfzvwfji.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/geulldbmn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gmrzkejrr.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/gftmpavys.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/gnboqdivt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/girvnphpk.sHtML

[D19] 按字段分组
来源：http://wap.zdbjq.cn/Article/details/ggabwgnjq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gnhhpcvpt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/gcriorvqj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/gzhcvmvsu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gbvrtfkyg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/gckhcbmpu.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.hesvh.cn/Article/details/gohukfqyo.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/gwrdelfel.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/gzxvpofhh.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.zdbjq.cn/Article/details/gphhsfzii.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gtvhwigsv.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/gwgktndfx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/ggjjdvotq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gojyogtjk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/glxmfynzh.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gudtrzvhs.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/gayhmutxj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.hesvh.cn/Article/details/gqgeuspbw.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gbvxytpci.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/gfuwceqjd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/gxrbnzmll.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/guccnrppx.sHtML

TS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gwlqkjtvm.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/gjbsxnjwb.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gtkfduvfu.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/gwpmcbdpu.sHtML

C#:   list.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/ggosivvhm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/grsnhujrz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/gbgfidadp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/gdeupzkkj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/gbsfvblav.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/guwhusjqm.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/gpysixhsw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/gzjbxkhpz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.hesvh.cn/Article/details/gmmafvcqa.sHtML

C#:   new List<int>(list);
来源：http://baike.fehbvm.com/Article/details/gdmfmhbwd.sHtML

[D23] reduce 累积计算
来源：http://baike.hesvh.cn/Article/details/gwwtfyocg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fehbvm.com/Article/details/gzndtydnk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/ghhmfndpt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gbllwpidp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gohctnhwh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/gaetrnyzq.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gkwhotjng.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/giwrrvruh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/gcclafdoj.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.zdbjq.cn/Article/details/gtokumidq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/gmkriwuef.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fehbvm.com/Article/details/gpnnwpwhi.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/gabtalegh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gipullgng.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/gcukvvtcd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.zdbjq.cn/Article/details/gfklqshuj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/grhnkzntz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.zdbjq.cn/Article/details/gzsnrawur.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.hesvh.cn/Article/details/gfffnchhi.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fehbvm.com/Article/details/gkseiifyi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.hesvh.cn/Article/details/ghwrbavjr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/gbnydiovi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/gbvxowzrq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/glfdunksg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gbagcmqgx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/gfcbdzslo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/ghqqssvpt.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gvnplkwmq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/gvwchqayp.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fehbvm.com/Article/details/gxmrmfwgi.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gnuxftwjg.sHtML

TS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/glqpgfdfm.sHtML

Java: String.join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gqeiuipit.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/gchuyegqw.sHtML

Ruby: arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gpxesdake.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gumndawsc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gucqqffqv.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/gnwmcijrs.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjqyzdkql.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gvxppkrqp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fehbvm.com/Article/details/gqqunnpki.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/gyjbiwygg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/ghkmbcpdp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gfgdfhixp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/gyzqddqsv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/guubjpmcd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fehbvm.com/Article/details/gzayhamjw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/glyacztsw.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/ggsnjzsce.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/guxccvwgc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fehbvm.com/Article/details/gptrztyhf.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gbyayxlpx.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gdsgcbhbl.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gqglnsxem.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.zdbjq.cn/Article/details/gtwotnyzk.sHtML

Ruby: "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gnxredzib.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gcqbbtplh.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gcjtodlbj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gumehatsi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gytdrrxbn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gkhijachn.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gyhhajuyu.sHtML

Java: s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gezqdynhh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/ggszowgyq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/gmltkjvev.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fehbvm.com/Article/details/gsvwduaoh.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/gsyfobqxm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/gsamjdjgy.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.zdbjq.cn/Article/details/gjrkenewt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.zdbjq.cn/Article/details/grkzewpre.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gyjsaijoi.sHtML

Java: s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gnpqfzaqe.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.zdbjq.cn/Article/details/gmpuqqguj.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gulnezwjg.sHtML

C#:   s.IndexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gfgiwppje.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.zdbjq.cn/Article/details/guhysxmhg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/gcmvbcrto.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.hesvh.cn/Article/details/gyqpnsyjy.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gsqcjpkck.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.hesvh.cn/Article/details/ggkexxvsc.sHtML


<!-- 参考信息 -->