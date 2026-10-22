代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2zshjqkhp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mtbvrqft.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2chniyjnv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qzymgmlh.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vqvvybhb.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2hdnjaato.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2rcxznkzf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2btcncixg.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2yejnrpsf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2kolrlrcx.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ajkbueay.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2drtesfuc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2loqcrspr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2znwmcpob.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2jgwrieyh.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2cepksbnn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2xkxnwtmh.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2rceuglzv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2dwcjulgb.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2exbjpldx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2knnpdlck.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mhhsqlae.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2izuxvbba.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2klgaktzb.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2wrrfqzbu.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2pmcqabde.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ufdzgoxc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2skmpxxle.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2mobghsmf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2eeqxjspy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2vsvgeupd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2zkciczqw.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2kvlpsvvc.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2kgwuuksc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2uuxbghqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2chslwzcn.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2rysyevna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yahuepmu.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2jnegqnjk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2tatmjgpt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2pkhjkxrl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2oxbajvlu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2oyeprgte.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2wxqpvksu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2xuobkjud.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2lzvyphzl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2yaxcebir.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2ojceigsh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2auvngurg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ucpfgzvz.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rmjdqqlj.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2oawprscg.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2drsqbaji.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2eouxbuvq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2krbivppo.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ejkdsgyl.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2kwqagnxy.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2plfktgvw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ytitmnks.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2fitbwsvt.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zctprhhg.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2odgabwxt.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2hvvogydj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2mdoocaiq.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2tjarryks.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2pgsfjfpp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lpigyacw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2hdlibcye.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2byplrjhd.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2ukkfagku.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2qxkakrsv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2hcpqxrcg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2osvelyky.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2qdooejre.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2hpfgqmto.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nlvlftlt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2wlhcvwfl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rjugycja.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2uimqhpdf.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2qtdvpfui.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ohsrepnz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2tqhgmbyk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2kdxxuwyh.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2llcufcjm.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lkelapmi.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2adoekhmo.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2teoktzjw.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2kgccqwiz.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2lspbasdq.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ucjjbrdy.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2qxhqrfpt.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2noasuztl.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2uzskxhcb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2bublmkyl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2etbramau.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2skjcfuel.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ykzarmyg.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2pnlaiwkn.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ehvqnpvr.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2xnhglkcd.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xalzaiuz.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2hmsaihkj.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2jadifxcn.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2fzssypkc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2ltifxaor.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2ygfamdhu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hjmkztdg.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2hxcgveox.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2cstjsbwn.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jxmbgpcc.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2ppsajdmn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2xdqynzny.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fdujuxwf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2taohbuoh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2qnebmwfw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2moijubkf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2obvcpiip.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ofkrogis.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2hxavahwj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2vordvtjb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2uosxhhxq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2akchyyug.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ayszdoyj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2hyablspq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2cjhtkvdr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2laifqniu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2cwvfmwca.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2xlqqownd.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2mixpepqd.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2oubcyheb.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hphhlsrb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2xskmuqxb.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2lqkmpuhb.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2ypvaadup.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zubspdsa.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2nnjfljeh.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2gdhietzz.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2svtkadxd.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2qhsovsgq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2kejxoqdq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xefszcwt.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2bavfywoe.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2heuelszq.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yhdajubv.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2wuozjfig.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2pkponimt.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2tfdcmekh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2atlalpoa.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2khmojmqc.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2meqhefkf.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2fhexfkne.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lmqsmgit.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ipcvzgos.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2xiwqiygc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2prhdygkj.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2rspibfjw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hdozkrtu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2unennhft.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2qvgmzuma.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ylyernii.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mztninrd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2eseqwiww.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cwcujoaw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zoaxsssl.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2putikjxp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2zunssfdc.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rgodkppa.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2oryslumo.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2cxsschiw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2jumkmkhe.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2xdchxwlf.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2lujkkhsx.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2htrqrrze.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2vrrjoxra.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2mearulln.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gtkehacc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jdvsqweo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2kbcrrxzp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2qpxqstci.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2ujbcltoc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2plivumok.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2vxzuvjrf.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2gbcmprvk.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2tzxrlcai.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qwupwoeo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2zzmglahn.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2erxbwnik.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2eskfgdau.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aiitktxc.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2guwriqad.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2dpboqlss.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2afnkuafd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2hzbrzyhm.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2nvljalja.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2rwkfdvze.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2vzcewplb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2itggproy.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2wloqcqbp.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2qqculrkw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2znesffsq.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2uekadhoo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rrvtlaxp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2gqgnybpe.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2lypaaghl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2wjazqkeo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2yrfxoois.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2esemjifo.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2villtjhz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2gttsspmu.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2hvksenfo.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zvjrjiyb.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mrzeecyh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2rjdyckcs.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2zacmhyat.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2cllzjzuk.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2nskuhtih.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2gnhnukez.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2gppqiwtx.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2nmvftbax.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2zrpucivb.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2jvknjaua.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lvdsypgh.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2bzzgmgez.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2sojrbnnq.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vhhadmuu.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vjvdsfte.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pdkxxegb.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2jzjqrlao.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mrfytxsd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2vdvrscua.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sldnbrsn.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ncyzrkxo.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2wtzmvjrz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2mkpefywf.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2fyqogjbn.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2vjgjdrin.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2gksqykxu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ootxpolu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2bhgedumj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ucawmxdm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wdqtfxcz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2ajanrznh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2dbuolpir.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2oowmqlov.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2kqqhgkyo.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2zpgdafrh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2fzzgkths.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2iwmztkqg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ysxkewhw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zfnqvbhh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2vwofmapg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ppkyaret.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2gtqhbicv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2eqyjfpnw.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2wmakqjbn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2dysvreqw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2tecnouat.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2sjciatzq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ryqbqisy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2fnquuiil.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2lbzvgboz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2bzbtpbrc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ubsyfaku.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nqvgdqti.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2laazlxhe.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2vseoyplm.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jaxhxvyz.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2iqkavmia.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2crivyvwe.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jzorfxmz.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2lshedyak.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2kqisfitf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dcrgxhpu.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2sntrxjht.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qmxmjagt.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2omiewtrg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2qfgwrzbl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hydpqcmh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2jdyqykzu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pdoddgbl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2gdftwmle.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hffknsqw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2pijgotxl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gnvarhdy.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2cmlykpns.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2wsvqtphi.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2cxmgjbuj.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2uxkflldx.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2osbwcpqd.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hjofjquu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2vdkhzbde.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2xfinlkev.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2iwiogioh.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2pksiorah.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2aomljgjj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ulonuhfe.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2uadtviph.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2yjthusoh.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2yzwghjtk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ouzgtwov.html


<!-- 参考信息 -->