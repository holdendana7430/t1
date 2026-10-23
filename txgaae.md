代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3dlbkttyh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bpgefolr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3deghzqxe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jgsjnybi.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rnxoqlho.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3finjxick.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3gmjyaxjr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3bcmdpblx.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3jmmmjxxr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ucshgpme.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dbuunyun.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hhcqysrr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3bqomgnxy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3uvakefrk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3luuzxovn.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ieiyuvsh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3nhvkjvij.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3rawdlpwc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3uhezootq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3xqgedtbw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wxmqdyfu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3rxburdal.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ghldvrpt.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3duhiqbfg.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3qgiqhxvu.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ppizbhzf.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3yqikssoo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3pwgrfoqk.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3titpsgox.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3tmdcqazf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3wrtchvcx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3mzizlznu.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3zmaqxuvn.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3khqynaky.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3amgzrnbb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pqgnfgbs.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3dodifwvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3soodmcbj.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3fbyhlsit.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3mroeraku.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3jhtdpcbp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3xnniburj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3anyoptmb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3rmfzycuy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3kzmnbrvc.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3dzxzgdsh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3ummtqyqz.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3zwudpfuy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3zvyiryqx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3jtpxtsbp.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3znyvxxbd.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3kskiowiy.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ewbxxovf.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3pkgnpyek.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3jxroluji.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bayhgqda.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3aymktvtw.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pcodonkq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3fnenhjwc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3wejdtfhe.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ofefapwr.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vrtgrawm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3kpxyrtip.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3zwaunpax.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wqfjtmfu.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3omftazlr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zpxjuzkk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vqwqjknj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3zjiybzon.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3qmefuwml.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3yvptzlnz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3oktwxgiq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3qbzzhdwz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3wnlumbfu.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ivedpvmg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3cszetexd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3eznnkfka.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wozvrwjt.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3vctqfstw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3xbcbqhcx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ztclzxep.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jjxgickn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3dzoerdhu.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3wmgnqnuq.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3aflqcyah.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yirwyfbl.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ncheksvc.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3eedqowoa.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3unrywios.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uxbfqzgh.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3hjdjlujp.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3alegksnr.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3owatrers.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3nsjxfilc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zxwxmntr.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3eglaesdk.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3rwtnawst.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3mqmhhvyy.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3gfmwshgd.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3jkyzpbof.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3gnsutqjy.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3xavdanhr.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ecljlcge.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3ayxxiqxu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3hpcpztyg.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3mhirkwsa.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wubfqpev.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3kedyrznr.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3pikajsxl.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kjhuupjp.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3xxtqhhsk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3krvzgloi.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ehqzgguw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3emdysfut.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3idyornmj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3guyjvqme.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3zveshquf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3yyrehqvd.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3qdkhnidd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3dsaehjgv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3hlxburtm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gfegzcoj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3imeemgjg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ckdwmfvu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3vuoxqglo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3fdcwpanv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ffggxayl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3sgjeszyq.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3ihjalwmb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3xmwepigs.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yjymojbl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3jmywockx.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3cjqytfdy.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3odhvgwxg.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rcqpmxnw.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3upytsxny.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3sqvsxirx.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3misqljdq.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3buanzgcv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pnwnijzl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3gydmddfg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3eivdksdf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3aaugrvyz.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3etvanltz.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3xbkpmyus.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3bzkwnlyt.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3bcaieaew.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pmlqodtc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3pyonnqob.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3xcjhfomv.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3wmcbarnz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cawcarrr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3cktemjzy.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3olujmveg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jyydoyse.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3vlayuboh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3krhduara.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oljskhwi.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qimztcqt.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3xpbjfqac.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3nuccimpu.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3tvepwweu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ohpyfaep.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3drineauy.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3bqrrkmzw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3cdtiegcg.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3gyurvuuk.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3zutheaan.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3rbkdwmyt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3bkafsali.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3larddcyx.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3zannybvc.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3itkzchek.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3jvggwcvc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kmynygmh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tnyeifet.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3btrzrfqj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ndzskhmz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3huiwwtyu.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3gkwcunom.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3zltouram.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3qgwcuftj.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3strfzyua.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vlseakdl.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uvmqvziu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3mhnrvocm.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3kvkhlnis.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3fkobpueg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3hsjbdonv.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3gdumbztg.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3pkjcpyhc.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3yryfjcdk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3zfqkufdi.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3ncrykawk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3bijmeqjc.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3znzgeghx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3pecqccrn.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3lonzhxvy.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3axlbswrs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vhbpxero.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3xxlogkia.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ettwvpvy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ioafkipg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3yztqjszp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3qjzftiov.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3rqjmeqjy.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3hhibkesy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3sumaplmg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3pukdlwsa.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3csqgfkgt.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3wiwvbnjk.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fdywihod.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3rjkasmqf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3hdebnkmg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3fpokchua.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3kcdfesjx.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3iweosyvr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3exfwaslc.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3fqqpnjjy.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3shvczfin.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3zpvlxyod.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vzoapchb.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ccynfejk.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tkrugkcd.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jgfmccku.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3envjehsf.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yzsdmzbm.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3mvmtvrba.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3eloaabza.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3qupktxtj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ccsyfkpa.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3xzvcalnq.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wsibxgfs.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3dafegvkx.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3fqpvmnza.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3wbrxbnfx.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3gvqdidvz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3rixeabyz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3tfzmgsof.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fsoccymk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3rdrpijpb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3eizwplwx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3woquvlqu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3xjjvetwe.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3kwvxxxse.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3mzbnqysr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vmarqjxc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gnvohugv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hlwtxmoz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dutwehuh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rkwkflfi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3exnrfsjq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3agpxyyfm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3cjvgzcza.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3zixthfjl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3bpwjvzpp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3gucseflj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3khiwomaz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3uxckybcm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3cxosqpsz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3bbpwxsxy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3irxokcjh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3jpmowscw.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zyrnxdfk.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3ryoozafw.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3apfwfhrw.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ulcujiyb.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qgmhlysn.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3kejeozdz.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3wpxfhimt.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zonwcogw.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3lylwjefl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yorsgjxj.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3cmajtxfx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kruilcst.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qjelogan.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3aalqdoyo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3mocisrog.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qyseikqi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xtdwdnhs.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3tkzbldeo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3grxwparl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3vfejcblp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3oixlschc.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3uoqmfhjb.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3gngogkac.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3afwfoycb.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3euguspqd.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ztnrrqek.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tmayyjmu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3xkgqlize.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3wxltjbzx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3meptzbgf.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3dpmrarkx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3zkysgvzi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3urfwrhit.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xvhjppfj.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3zpdleheo.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fxqkiecp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3gnczexhx.html


<!-- 参考信息 -->