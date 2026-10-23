代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3tjokkozd.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3gchvqgkt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3jhazpfow.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3tuyxltsm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rpxdpeha.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zsqxlbzy.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3wleyjifv.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3edjskimz.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3rgngxftk.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3dgkeaefg.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3gdzwqnnc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3drgtybvm.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3blcchxuc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3eupvqvme.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3zhukvvvw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pwtpbdeq.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3nfnoeepu.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3qhjalisv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jwengufq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iwyxovka.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3nwsyzzel.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ybejufxr.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3zxbfcbqn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3zszxcmpe.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3wxpgpjpk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3wzfrqybp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3kpwqtvvc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3shtojbyr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3jlhavmmu.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3jvquzsny.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3awfuzbue.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3xgnfexad.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3iokfaeof.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3ptedhfdn.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tvhxhmrc.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3nzffjpra.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3taznrksp.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jrrlyzzi.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3frqriagb.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3jcgrcykd.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3hcqrtttj.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3dfgbehgs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3itizajtn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3oichyjjx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3pozvyfuu.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3macomxof.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3yuxvbjsv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3hfcudnjo.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ailsvyig.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3wwnivjok.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3eadbybys.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3lafmfbkt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3expfzvrs.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3lqpzwxsv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ybdymgxk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3wqonjhwg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3yptybcbp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3cohwjreq.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3obfthdjb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3chpkypwq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3skadwccy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3pnqexksn.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3vdkhdohb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3uvscffhv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3npeytclj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3rffzqcxi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rajfgzeu.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3gzofpskd.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vufzcytk.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3llceytlj.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3mjaqtxjn.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3gbmegnwn.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3nijixefz.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qzscyaew.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3xukikaou.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3haynlhiu.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3wjtuajax.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3hnjjodrz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ermgnhth.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3hxgusfmg.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xqezgjqm.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3frghkoff.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3rlrrqfzw.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3bjcbvcwh.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qyhfrmia.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3zljvsalo.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3pzwzazdh.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3yrsxwyst.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3jjntpgbd.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3tsfzgawv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3plkhxtoz.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3hulnpqib.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3edowkdbl.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uxmcklba.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3hoxrduhx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3tgsyhvso.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vfabdrip.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3mxoksbtx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3ldiesyzt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3qiuyfkmp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ahvubacq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3wosoetuf.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3jmfjzzfx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3wanzkxii.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3lrklcucb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bxwhatcn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3vrbeckyz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3fxbrpxra.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ifpshutk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3rjylakfs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3gekuxngg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3srotcwsd.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3oblrqnel.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ugmridnj.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3edfdjfyp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3eclncmdy.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3pyzvxsxs.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3mdpfreow.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3mvxwrwhx.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3okpgjwva.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3rpgohsse.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3pclzcztg.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3lfgtntgh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3zahjugfm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cniojatl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3upzrsqwh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3xlgagwdc.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nnohicrw.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3deubvxie.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3xahvrwqk.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3nwugsfkb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jxaromuu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3cbjmdeon.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mkoyfrbg.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3plkkkfkm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xixzuavp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3tqxpapxb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3asnyqpjn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gzherduq.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3sfbmbjys.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3ckdghtmb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3kqjhlwjp.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3yolfsvid.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3lmevvqwm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jgoonfpt.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3fclavrhb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dkkasxfc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yuybnvay.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3hnnzgoaq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3wklmaniv.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3ydezxsbq.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3rbncxsix.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vvyezugv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3rewqagnp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3rnonkfdy.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3lyajrusy.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fvgnkkxg.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3ckgfdwxv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3iwftdfug.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mnozkccr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jufmmhxx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bfvzsyke.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3dfcibvpp.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3qldszhlf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3uyrndjvv.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3bvvbplrm.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3skwetzrd.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3soyqlaps.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3tjlsukni.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3cwrlcudh.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3apqzbikg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3riifhodd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ikhosvpw.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3usckziav.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3zsjepqzu.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3pvrdmyug.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3smiihtnx.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3uihcaetf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ekavmkid.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3thzmrnrm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3tqwjencm.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3zoglpsfi.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3dvbtybdl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ndotehmh.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3zynkdnen.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3elycaiut.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3hbnthfdq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3hkzfxson.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3qdsshnnp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3jhxrvwlo.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3nokwauov.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3tbwcpxlf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3iouuzxbh.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3jblbkxsw.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3veozqiac.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xhztmjlx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3zconfakt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3rzariuyz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3mwbkejjs.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3pibnxqqa.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3sthhrcje.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3uairpvvq.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3sakmkqdg.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3fvnlnbyj.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qnvdmghb.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rgtdqioe.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ybyuywqb.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3agkhqxbp.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qhpmzvxb.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ugeevxky.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mjolzufl.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3aiisrgxb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3ngvhtnab.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3nqqbmnje.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3zikznigm.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3vajnzzxy.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3qkoqzyjw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3mpaaxboy.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3xcqjwkrr.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3yhlamugf.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3edemtbvw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fzsyjuee.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fxuwsejr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3octhegqg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wmanzths.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3drxpcada.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3bsmjmnvx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3houjrhph.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3ezsvfmdz.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3fgsxdmwo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3mdeswyef.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3ijrcwsui.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3etbsvdkn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hobkdpup.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3hfrlqrea.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3hymanlmi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3fzoxnrhz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3bkdtrech.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3zgifgbyw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3hfaemgik.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3cmpwnxmg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iyedxwuq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3uvczunxs.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3fxkmevwj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3gekkrtib.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3unnwanmk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hoocznep.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kppmkbmh.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3sbdrusgw.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qwumwjdb.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3sgoztapo.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3zknnwxqv.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3vlopighs.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3qxlwtzeg.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3fgpgphgg.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ljrmgcob.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ylfrvibh.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3mjssemhm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zszshvwr.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fnfrvwmk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3fyozdjfm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rjbvcjvd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mokudevp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3sgsodwnc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3dfsmvccj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3xwraytiv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3szoxgtca.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jwqdoejk.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3ioycdldb.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3qcoblgfi.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ouhdclpo.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ufygtrse.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hnibylzm.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lgvgtzyd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gbqwofav.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3lkbgczhx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ahjekbqc.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3pfqvwptw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3rtlbgqil.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3krajkpxa.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3okljdfdu.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ukcmuzhh.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tmotzeej.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ypnrubli.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3iyquxzjv.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ugmkalqs.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3maelpegq.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wctjqayo.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3mrmjazzp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3olmiowjf.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3rltuumio.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bwclnezx.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3crdtvrbp.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pmidltif.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xksuzbns.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3wuwboiin.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3tgfzanwc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ptbxxxkw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3oidcjhyu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ovymrscz.html


<!-- 参考信息 -->