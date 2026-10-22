代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2kykrokgk.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2zaetyiwl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2jsrdwtlw.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2nqffkrpe.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2srukefho.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rqtvxouq.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2mgwyqyks.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ngjjwumi.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2azdrsxrf.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2zxgkltkk.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2inpiuevu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2rjqdkrot.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2houibxht.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2gufmexnh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2duvfnhhw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ypaqilod.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ofwyqcob.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2zktrldjs.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zdunbqwp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yyadhzzt.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ztctlfqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bfpstlce.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2bwglmttm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2ijwcrhts.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2mdyebpph.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2kgkmjqrp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2mrqszdit.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2umqnxqnq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2xavyhahd.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2sbafijkl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2pfthdmed.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2qarcfjoa.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2evsooymw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2nfrzvakz.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fwgftxyx.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wzeubdir.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2voguqeur.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ibmrzyxv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2tenkalnc.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2qxmwseyy.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2phpjzoyi.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xsgmyjgi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2hvlbanqp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ecgcljak.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vsfvlplc.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ntentyfk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2uirdhisr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2tsvixiwz.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2myfgjsuv.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2cuaesoyb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kywtjicy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2pwwpjmmk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2wjquhqwy.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2vtehnynu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2fgbiykie.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2qkijbtit.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2looginuo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2uvgehcou.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2ygzmimth.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2joungoks.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jpaqsplf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2soyihcki.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2aldyxzco.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2xkilhngg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2raaiczce.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2bvozrtpu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2yqtfvxxm.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2vegvqewq.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zzdwunbn.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2imocsmds.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2achjoplc.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2zuwdlrss.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2evthhucd.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2lqcqmzlg.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2axnhqcet.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2euhqevud.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2musdhswl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2qnehflxv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sbniiqyv.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2kbxnzosa.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jjkmurek.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2fduqbfek.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2uxctnapa.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2nuolvopf.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2shtrpflv.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2xlqbpczs.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zqwgclnf.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2graaxaiu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2eaqaeysf.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2gtvtvowk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2brensggq.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2yrabbfmk.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2itkdvcjh.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2edtowfkt.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2mwtawcbz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2aamucvjd.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2sbqqotyz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2hrbnbzge.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2qnefssje.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2wenbknoq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2checzbvb.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2huutjutg.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2mflmqoan.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2yvwspclt.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2turkevff.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2fjpciodm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2acrsevfh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2enticxvz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2rzpnfzvp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2liazvxuz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2hgdjgswi.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2ofknkxwu.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2fnnfvmsj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2fzxkoarm.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kkppenmo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2pfrvalse.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2eptwhukj.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jjyepwsj.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xdosklpj.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jlxkuzgx.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2rcybfrdj.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2kggxaqgp.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2vzerruho.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2lydbbupd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2chhnkfgw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2azlllcwe.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2ucoxpxfm.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lpeosbhl.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2zahiqdac.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2rcqefydl.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2zpiuqlgb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2lsaxlraq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2xvajhoyl.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2yigqrnmp.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2xuhwciua.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xrrdrcyh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2pptdkasi.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2dlqibjue.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lfyzwkul.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2bjgalmlr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hrhelmta.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2qefrhiaj.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xnndunnk.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2bsqleafc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2pfkqncqc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2rgzsavtq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2mtgzlqdt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fkqidcuf.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2ublxlmgj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2eijojdhp.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dbmwjuoz.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2pbenfzdv.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2uydrbpxs.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2wmdccjac.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2fyijjydc.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2msehbkaa.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2vezezolc.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2pggumaxd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2eqzphhao.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2voguhbxl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rrhuwwwl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aegxacbw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2fhipivkr.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2hugupirk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2lzozwdmw.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2ophalczz.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2xjzbhcpo.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2aaqopkze.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2jdkdolcb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2fijbcvqq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tkhbemto.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2mtgiyfei.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2zwlqrqak.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2rxomdxwn.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2uuvzrgjx.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2bkxwcruh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2pmpsaihk.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2knmdccmm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2dfzhcnot.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2okinnivf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lslcmicm.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2smszyvgx.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2ejdxphji.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kmarsgrb.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2gzffevbg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2iwdgwoxt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2cabtsynj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2uelhohcf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2zlqndgzb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2loxnzeka.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2jwrawgvi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2tmbvsoui.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2bmifgrfd.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ploiqupc.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2pdhxjkii.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ohzilbmo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2vvaunvbb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2uqgpmdnh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2lzhcodjb.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2mxyzjfnf.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2slsxptrm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2fknpvirs.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2jjjopcfd.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2fsdixzuf.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qkghqbjy.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gazlghep.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ineoxvue.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ovxvqmku.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mcpqfnkd.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yycrrkro.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pswtfxga.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2bhyoituw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2blkqfmxv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2jgaqyugm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2tledcyxc.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2aqldkdmt.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hztwitve.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2gwbcqetk.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2vdifphcs.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fclbmpdn.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2yfbuspub.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xhdzmoeg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gmmcdyke.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2pchakcrj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2szyucvla.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2dqmcuvlj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2kglakoup.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2rzeqkpwf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2ebyfzxep.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2mlknmpwq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2yfwepomv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cmolntga.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2fxtrdamu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2llyhxkzl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2pfjhpbjh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2kfyhnasf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2vvfptdtx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ygvgrggb.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2xtojahdf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2vpwkkpek.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2amxhwuiw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iphtcyxo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2gdjsslyn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2yuxcovxq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2oyzljfgw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gweqikim.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2kkzdevlr.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ifzxcgct.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vraupxli.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2acthdaot.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2pnvahvsk.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jmewodtl.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2uztndinf.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2hoqbqyho.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dwkolujf.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ynhiepja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qjgcsiqk.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2edinhmma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mldxeefb.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2snpeoegs.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ihjsqpre.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2yblprcgr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2gnlrpbfc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2empvvjdf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2qagixnvx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2wnvwahtx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2gfiyqpww.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wcjvwokp.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2znzketqk.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2zxzjqhtw.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2khwgiaim.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xkveaszx.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ydycubgb.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2bismsigi.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2oldvodyu.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2bqdiftim.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2fyugcgby.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2sidywmin.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2hufksnci.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2erqnjsgv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2sgriakzk.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2jivwcsqw.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2kceyvefe.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2fimcqruc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2pqyzcqwi.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2chtwujsp.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2rpnpddmz.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2cukjivsu.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2zepmqicj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2lawhdriu.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lcmrnzpy.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nuwbmods.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2xzyaceqf.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2samogrcm.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2eedjxjmb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2bnmsedyp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2eqepnaao.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2imheqmff.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nhjofmjp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hjbcyohd.html


<!-- 参考信息 -->