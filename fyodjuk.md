代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gqjjxwvki.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fehbvm.com/Article/details/gzooknfer.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/gbpddmeak.sHtML

Go:   // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gwgpfwpna.sHtML

Ruby: a, b = pair
来源：http://mobile.hesvh.cn/Article/details/gxhuyuvjd.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gqfrvqpsb.sHtML

[C16] 函数 / 方法重载
来源：http://wap.zdbjq.cn/Article/details/guvjikscm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.zdbjq.cn/Article/details/grugnlswa.sHtML

PHP:  // 无重载
来源：http://www.share.hesvh.cn/Article/details/gawmynvxs.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/ggtarssoq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/grlcfshju.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcserkrgl.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/grmchacji.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.zdbjq.cn/Article/details/gqckocfer.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.zdbjq.cn/Article/details/gtxzmjspc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjwlqsnkw.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.hesvh.cn/Article/details/gpvktchnf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grhdpower.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/gkkrvsrum.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fehbvm.com/Article/details/gkgyyqpzn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/gdvoisgsb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.zdbjq.cn/Article/details/goeapclgq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.zdbjq.cn/Article/details/gahfmxqvq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/gejapsbzu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.zdbjq.cn/Article/details/gaybpgzyc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.hesvh.cn/Article/details/ggmbdxvqs.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.hesvh.cn/Article/details/gpaamokvq.sHtML

[D02] 追加元素到末尾
来源：http://baike.fehbvm.com/Article/details/gleveulhe.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/gexrvjjnx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/gmuzmgeeq.sHtML

JS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gkquupxre.sHtML

TS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/ghwitzlhs.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/gqagyjxbh.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gdlforbaz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/glysmlugq.sHtML

C#:   list.Add(4);
来源：http://baike.hesvh.cn/Article/details/gxjfuwuvv.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/gazxxxtuj.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.hesvh.cn/Article/details/gesolbine.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.hesvh.cn/Article/details/glogvmjwp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/gmbkughol.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/gsyycylqg.sHtML

Java: list.add(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/golrzxrbl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.hesvh.cn/Article/details/glaogvbiu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/gnqehuhua.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gjbtbjypn.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/gtlcsvhzu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/gbybzeuoy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gcfxukhpf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.hesvh.cn/Article/details/gcbzltvci.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/gmiibkmbn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.hesvh.cn/Article/details/ggtvbwoyk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fehbvm.com/Article/details/glcfdpnni.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/gcsbbzapn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.hesvh.cn/Article/details/gqzbpnkpn.sHtML

[D05] 访问与修改元素
来源：http://wap.fehbvm.com/Article/details/gfsmsnlrh.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gnftztkel.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gcnptzbto.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gmrwjltga.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gzcpvnjlz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/gonblykar.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/grhuwvmle.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gdqbhbqht.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gytokbysq.sHtML

[D06] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gjyuluczs.sHtML

Py:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gerhjacgq.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gulfxvyqr.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gmdndkdrj.sHtML

TS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gbrplxxia.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/gipibdzwd.sHtML

Go:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gjdnthrvp.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/gljshumlz.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gvbfeckbb.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.zdbjq.cn/Article/details/gfnrqxuvn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.zdbjq.cn/Article/details/gsfsowxqy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.hesvh.cn/Article/details/gaolhmvxf.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gubklknwu.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gldkxvjye.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gnpbpudsf.sHtML

Go:   arr[1:4]
来源：http://3g.fehbvm.com/Article/details/gwodzzpmu.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gczigzygq.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/gzrfjodzk.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/gmczcpyup.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/gzpenqttk.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fehbvm.com/Article/details/gkmliqafw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/gwxumundo.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/gktglcmwv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gftedofmw.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gthxvahwm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.hesvh.cn/Article/details/gdpgrxxnq.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gvxskmmiy.sHtML

[D09] 排序（升序）
来源：http://baike.hesvh.cn/Article/details/gzmvzwpkn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gvtwevaux.sHtML

PHP:  sort($arr);
来源：http://read.share.zdbjq.cn/Article/details/gwoyzbxxu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/gapsxnkqs.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/gphtrmnvp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fehbvm.com/Article/details/gxwdenqdp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gekvvoagw.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gfegvwqlm.sHtML

C#:   list.Sort();
来源：http://wap.hesvh.cn/Article/details/gkyjkhfxc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/gywerinlg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gfeyqkden.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gyhnkcmmm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gwrmzvmpi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/ggdircebw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.hesvh.cn/Article/details/gybkvaaby.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gsanjnsxr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/gwwcqoqgp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/gokjkeeon.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/gjwrsyzxp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/gmlygfzpb.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/guihanxxq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/gzqmfhrzw.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gcmdprqlf.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/gvhwtkcyq.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fehbvm.com/Article/details/gisjufxrw.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/gwudzygok.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/gstrofcqd.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/gobcxuhbe.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gbfhkytvg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gimczmsiz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gvgvjbale.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gqevvrzui.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.zdbjq.cn/Article/details/gnfrtxfmt.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gufcwjchz.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/gpzehkhxm.sHtML

C#:   list.IndexOf(x);
来源：http://wap.zdbjq.cn/Article/details/gtjfxnnxp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/gumqcynir.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/gezlkfjpf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/gkxfedlqy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/ghxxlommo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gocqhkhtk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fehbvm.com/Article/details/gagoafoee.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/ghwesibjs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/gcqtvufcz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/ggsptsxwd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.hesvh.cn/Article/details/gmkqrltbm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/gunvrbakq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.hesvh.cn/Article/details/geiorfkbm.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gyjonfdka.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/ghfjsmayo.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/gsykjnesb.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gcrdvqhyf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.zdbjq.cn/Article/details/ggvzicljo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gnhakgwmb.sHtML

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/ghbyvjcon.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gjixmarcz.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gnqqoxitl.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gejmfsvmu.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/giplkregk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fehbvm.com/Article/details/gloqcicif.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.hesvh.cn/Article/details/gxnpjnqsp.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gxfanrztw.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/gsimlheav.sHtML

[D16] 求和与平均值
来源：http://read.share.hesvh.cn/Article/details/gzoxwjvyh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gizlvwbtd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fehbvm.com/Article/details/giixehqkr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gpbzjisbm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/glymhczyg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/ggzirgize.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/gcugkvndt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.zdbjq.cn/Article/details/grooqgkkf.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/gvixrfsow.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/glppbddjl.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gxskgxqdf.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/gxnjrivpf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.hesvh.cn/Article/details/gkzyvvmav.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/ggzhtkraz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/gxpqrfopb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/gnidtltqq.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.zdbjq.cn/Article/details/ghklwcerx.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fehbvm.com/Article/details/gzbdhusjf.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/gidvbsncs.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/gbcappvlo.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/giwmnkmyx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/gqkzsvgei.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/gfbuduzne.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fehbvm.com/Article/details/goetkjxsn.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/gxiuwbxyz.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/gdizjpybp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gftntyozl.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/ghvjppdao.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/guxosllil.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gsozljlds.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fehbvm.com/Article/details/gdipvtmep.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gymqyxwui.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.zdbjq.cn/Article/details/gnhjgkuds.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.zdbjq.cn/Article/details/gmrzotkms.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/gdzllvarz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.zdbjq.cn/Article/details/gmtjklxxt.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/gkfpkaisc.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/gvwiykmby.sHtML

PHP:  array_count_values($arr);
来源：http://3g.hesvh.cn/Article/details/gjdaiqesd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gmsyjwzlh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gkcmdbzuw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/gcuoqardm.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/gpsaoidkc.sHtML

Ruby: arr.tally
来源：http://www.blog.hesvh.cn/Article/details/grdfhkrxf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/goeslspth.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/gqvlkqgmm.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/gqtzzcksv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gjztvljqb.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gpczrmxbf.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gaeuudqes.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/gxxhmdano.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gqhymgmoe.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/glcujdbfa.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/ggugmfrue.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/gmmttxbxp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/gbvxknhvw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/gvrxissqi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/gmlyknjhw.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/gckrjwpzq.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/glvsweqjq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/gnfvcimwt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/gyouougxs.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/gbwryxozr.sHtML

[D23] reduce 累积计算
来源：http://www.share.fehbvm.com/Article/details/gwarfyxpr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.zdbjq.cn/Article/details/gkabrmito.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/gjjpguptn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gmayyvecf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gzelwxsnr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/ghqggxiei.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gnnunnuyz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/giwevqnrj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.zdbjq.cn/Article/details/ghsxkgxko.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/ggojwbior.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gtterojxi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/gnxinwfev.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fehbvm.com/Article/details/gjjtfjjuy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gepkrjblo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gxpmptiom.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/ghhrdbknt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/ggwkykkif.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fehbvm.com/Article/details/ggeoeurow.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/gkfiqqfmp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.hesvh.cn/Article/details/gzpjbmwoy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/gcveymvvw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fehbvm.com/Article/details/gynugfrgc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/gymdtaezv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gwzqjqfbq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.hesvh.cn/Article/details/giypbqhsa.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/gefvpagsw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.zdbjq.cn/Article/details/ggradsvdd.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gmzmtecwg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/gxwepeewu.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/grdcdgzmf.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gzmmovdht.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gopgnwjoe.sHtML

Java: String.join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gyiwsznqq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gvtzjbwvz.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gyumommmh.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gqlbehkde.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/guqjkfoud.sHtML

E. 字符串处理
来源：http://baike.zdbjq.cn/Article/details/gbofzzyim.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtvamybln.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/goxkpflva.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.hesvh.cn/Article/details/galdoayjj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/gefgilyfm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gtvafdufq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gmzskrxof.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/gauzygkme.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.zdbjq.cn/Article/details/gytvkefat.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fehbvm.com/Article/details/gvnsxjmnl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fehbvm.com/Article/details/gbhkoujcq.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gjxlzobzc.sHtML

Py:   "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gmrshhmvz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/ggxcabteb.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/glweubvzt.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gxvvygzor.sHtML

Java: "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gwstzfrxx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/gbwixbvdy.sHtML

Ruby: "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gavdleuyc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.hesvh.cn/Article/details/gvaiasxya.sHtML

[E03] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gkbmqsnrl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/gyvqieioe.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gnqoybeix.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gvxztnkgp.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fehbvm.com/Article/details/gqtqakygc.sHtML

Java: s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/ghuvfalui.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.zdbjq.cn/Article/details/gswjywohh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/gupgubndc.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/grxxicpxm.sHtML

[E04] 查找子串位置
来源：http://m.share.hesvh.cn/Article/details/guuszyubv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gaeccmbzn.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.zdbjq.cn/Article/details/geuoedhnn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/glhmxpmgc.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/ghitgpnvy.sHtML

Java: s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gwhrcaccg.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/gigzibgdw.sHtML

Ruby: s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gopqlnbjf.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gwlieaxyr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fehbvm.com/Article/details/grhabpyxl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fehbvm.com/Article/details/gxbrawuja.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/gjgkobwkl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/ggxdoqooc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.zdbjq.cn/Article/details/gspeaerfi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gqzrccuyy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.zdbjq.cn/Article/details/gnukkumya.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/gluxidlqs.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.hesvh.cn/Article/details/giovzksrh.sHtML


<!-- 参考信息 -->