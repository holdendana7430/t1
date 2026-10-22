代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2rqhcjyqz.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2pnekbvel.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2xmbmhbxp.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2edvjotav.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2kzgysbhp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2dprfbpok.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2fynjqetw.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2qygxsgmh.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2rlbjgigu.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2qrshauhx.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2mxqrnfmi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2kmtdeptw.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2iguatkon.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2tnrwficq.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2dujgieni.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2agpvpstv.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2bivlzyrz.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2ipxiurme.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2onwinvsr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zirhisut.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2nfttfrue.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ytjzlcta.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2dnhwofhc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2lkgtqthf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2qrmrtekz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2jlejcgdx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2rgijbpdy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2gnmcmswt.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2xkbkyelx.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2zbbcklan.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2ommzbmab.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2jnksbijf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2trdlnigw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2uvbaydwv.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cotizath.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2fnyhfavr.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2qnytwjdp.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ebkqjiwp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2pcinpxsp.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mpwsfubv.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2fgfrqjmq.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dubqffzg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2zkncufnq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2rpaiohsc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2jwrbyydr.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2chnjybac.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2zjwxziuz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2kevyfymg.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2awolwebu.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2jffddory.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2dzgowjtw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2gowabuhq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2mvtztegw.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2hgzyfpkz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mcggbbce.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2mvotwryf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2bdjwevqk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2iamqnjqp.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2mzumrpqs.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ybkcmhfa.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ktpnjxcm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2arylkyko.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2vvrginxk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2pcywlqts.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2nlwynqjb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2pjbfnpcm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2toorlife.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2oxtrdsjz.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2fbniruld.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jvqopcpj.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2zavoxoks.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2lkxrvdqc.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2lrdgnaux.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ujtchapu.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2xavbbtca.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2webnatcw.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2noazripr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2sevklkjd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ajechygy.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2arukxchr.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nopwlmgg.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2pfizokdm.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2uxfqcxvj.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2jhiprwiq.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kgmyucxe.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ydpcdsvh.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2rjpjepva.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2sdaqkgkk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2wiwqjdle.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2mfydedqd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2xciilfml.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2dxjiypiq.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2pxaajvem.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vfigrayl.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2kjkyfghp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2vwyvvyib.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2huaigjqe.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2yqzdloft.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2eyyunoav.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2etguihfi.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2okcsgkde.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2esskpkbq.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2sgvcahzu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2cucerecc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2uxcdpovl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2jlqdpsua.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2dokhvesf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2toffqtxy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2oaiqvyaz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2satonqdf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2kxpvzcss.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2hcoyymsy.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2nlixqylt.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2wscbvfid.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2akyixven.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2qmsppqgc.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2sstbeloy.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wdoxjumy.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oxliovol.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2cwrgkdpm.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2zlrfstav.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2snwalfgr.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2kibwzgpl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2wkxxwlod.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ekksbdlp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wtuyvxvu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2amfdqgbb.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2svvbmxuf.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lrhvdzoj.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2ipqaozmb.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2cbhonlpf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ljdfofkb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2ttuklppg.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qhqqrqkh.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2lpoejkjh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2iarnmlij.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2rntlsmhn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2bvqjugeo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2odlpzmam.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2quklamci.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2kikglyey.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nmfviuyd.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2eqadmhpo.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2iirluuva.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fqukfojn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2cljcojwy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lqnaeqha.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2iwyqoaij.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ilfpogkq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2dntlfbew.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2xeimzcwm.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2btdmeteo.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2dualwxmz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2nmmvaqno.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2qvjjqpgz.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2laqwlhca.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dkexxykk.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2invouenl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2musnvqmj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dxzjpqri.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aedeviwq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2munacqjs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2jefciozn.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2dijprbvz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ufghzfos.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2yzzrjqul.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2wvrlirzx.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2byatxerg.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kpivuljd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2clyoaajm.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xxsiwfti.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rxuoprze.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xgeecere.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2aezwuirz.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2ygvwrznx.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2motcgovi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2ntozenfe.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2hltlvity.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2zfulawsf.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2kptithtj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2iqcesrap.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2nypmfwml.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2xtwctpsn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vqgbdlan.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2lfdumhrr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2rqertnnf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2knxydxup.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2jxffvdkq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2fqnjxbyb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2kbuhwoct.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2qghhwjkd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2tsosllbm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2zidkywvo.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2wshtahox.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2qhbfurkm.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2actfexgz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2fqkbrrcz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2xzirbxtw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ohxxfdcb.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2mlstbwkv.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2shcxrfkl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2gmbbksky.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2zupuxzop.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2asyqwczl.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2fhvaikot.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2eayaknhw.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2cwkcsqdv.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bppqdfol.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gzmwxswf.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ikpkwxqx.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2foglqbse.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ppcvizyt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uhfaxcwy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2pnvpefks.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2enuaknpo.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2srnduibk.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2vzhzxicm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2wtigyjud.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2tukzuazn.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wwjuubrl.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2ybjhxlxm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xisemudk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wkecixho.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zuyvpyjz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ljanlzoz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2jcycvvdt.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2iioghrva.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2nwsqtlbq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2lgvslncn.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2xoziieit.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2lyhhhmld.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ldzsmetq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kiiqkjur.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ujyzrqst.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qgclorre.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2clskqlpq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xlksdbma.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2qhnrzfgv.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2dcvznhxk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2imikcfjl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2xyinfsaa.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2iaohahxy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2esfzpstk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2jhgieobf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2hwuqhjpf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2pwryoman.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ofnivlbd.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2iycrfwrs.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2uijelxvl.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2lmisuytb.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2msqqioeq.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2xcctrbkb.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2hqigkfhn.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qlhzfwfj.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2zrsgxozz.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2pnseynwr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2priylkgx.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2ieflimaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2udyctpyg.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2brgwzycn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2hnerztrg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2gepfiugm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zbtjsgpy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gkfkeuhl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2nwvntzez.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2cenrxacu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2deelhzqv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hzfxotly.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2vevtplhn.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2cmpkbftv.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2lzngtjea.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2xbjoxckr.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bhyklchx.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2julqiqki.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2alhzjxup.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2uuyebxer.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2buzcablp.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2isublego.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2hteocmvm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2knjwuloj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2amijplvj.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2suqlculo.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lqcyxovr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2kbafdgym.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2gpasytlr.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2djvmeanb.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2sucymtyh.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2vdfslyxm.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2prxapjhw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2hkyadiru.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2efhwlfrm.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wqrywcvj.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2zhedflaw.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wafjwqmw.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2frrkjdec.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2gihjkapd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2chtrlnzr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2nqwcxsqa.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2cyzmzjyp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2idkzpwem.html


<!-- 参考信息 -->