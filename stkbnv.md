代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3xkldqins.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3agngbiqp.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3vgzwbqon.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3tponwelx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3crsmkhpe.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3grqlbyxu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3vcjfvzxp.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3odarxrts.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3gpkoxuyf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnahxheq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3baufrpuv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tuerphsb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mokiaucw.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3uyyfzsjo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3jyegnppz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3qzpxvwoq.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3paayupmd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3uwyswjpe.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3carlsxyt.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3clzrrkcx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3dcoilbix.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3lgfrvowy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3ygbhmuwf.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3wrlyrvaw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3myofnuzt.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3ciuvzeto.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3wvuvraxi.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3xmhudvuq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cuviqyup.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hunhfxic.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3katvgftv.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3xjlpmecf.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3hqzivvtj.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3cvmattas.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3rpumoyly.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ubawwgzq.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3zepculoe.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3rxgjegur.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3zdevicqm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mivelzly.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3fkjcmavf.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3gnxwljni.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3dlarqrqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ajdgbxvi.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3obrqvsns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rkwydxut.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3qjnuwzhk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3kahmsicj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3xksagray.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3svtebmiv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3vqglimlb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3pkqtedcz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3nntgetaw.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3whhvdmhe.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3sogtlohr.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3magkbtms.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3qpizzbgz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3nqpwkqyb.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tglcxhsk.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nvzxtvmq.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3suwrmsrn.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tjuoogsy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3ddkewdbo.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xizupodd.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3ceeksodh.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kcdvlaqy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3tyykzkea.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3qugizaat.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tvcchdfu.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3uyyvryeg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3jeswpgeq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3egfvhkng.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gbtwjdti.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3oytnmzof.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zxvjvtjj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3pnfzxkzn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3rteqxksk.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3ydahxbow.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rfdquhfx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3jtjizjcs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cjwlstxo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3tccyupkv.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ybsxxllj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zsqbzcgh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3fedzjayw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3zkunqmpc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3ztgcyabo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3xrvswquy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3tyffrmuq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wegeodue.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3mazqoyvc.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3mdcwgrdj.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3itqjpewl.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3lxpumczb.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3lgvyxjqu.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3yjkpavbx.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3gavbagrx.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ncpxmwgl.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3wlrrsjdy.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3ayagwqfw.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3uxgguhic.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3dnjaawtj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3usntnkhy.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3vczmztme.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3phpvmqiw.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qxqyvgdn.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3pxznchlx.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ufbailoc.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3rmgfreet.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3bhbzsxnt.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3lorjwier.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3pecmzdht.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3srhaebky.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3hoklnjgt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3azzzfcut.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3maiorfne.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3svretcdl.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lsvcjjvs.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3usuzpchl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ketsaije.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3yacbxlll.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3bydlixzg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3hdaollwe.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3yiqrpopm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3jxpjudkz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3qruywqsk.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3ugquxpdy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3nhznpuxg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3qkxgaimf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ooztfahq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3zuylzarm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3xkqmwqmh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3vrygftde.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3llsugzxl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ycqdiutd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3aanpmbqa.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3rbvqdzuc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3sfyopvku.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hyfqljsm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3hzqlimay.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3lbzgthch.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3kshsdzyi.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zwnbptwo.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3njhogxut.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3efbtllwl.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3hmnoqtxv.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3eeqthfjj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lrqapiay.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yzewxtmf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3rjaqygbh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3pqcrdtko.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vrntcnex.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3erpqyaho.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3fvianjam.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3pncngaee.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3srbsivwe.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3kphutzft.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3gnmwnsvo.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dxcdusrm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3xsrkcztb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3mvrvvijr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3qrztvsgi.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3pkcrimyt.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3tymfffby.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yljkrphf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vikvkknq.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3arpcfuce.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3tpslgjcr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3utfquolk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3grdjquqg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mmtwakbt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lshplmjl.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3eggkcrdl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3hxrpjeiu.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rahprsap.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3bmeftfpe.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3hevalegq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3txwsgnbh.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3nyivcapz.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3kjdekkdm.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lnijkquc.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ijwjtmln.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3pnzthhlk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zbnbrfkw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3yhdumeod.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3svxmajtx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3oezqszad.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3tcwzpqod.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3rgafyqjw.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3nybdmnqr.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3mhtjhznk.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ilzldciq.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3fusurxcx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iwvvbksd.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vwscswks.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qiezbgri.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ybgccvxx.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ghidmmkh.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3novisbnk.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3fnbslgdd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3rfqnfzqt.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3vsmotzis.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3wgjqsxxh.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3nkizfkhr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3rusbhmrt.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3hyhkrhnq.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3jlssjqlr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3uovmzvfo.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3rlhrgpbs.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3sihlqzxh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3xrugimbp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3luhyebpv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3yfrftmjv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3ssbeywcl.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3uzazpmgt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3jdohoukg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3jlezkbkf.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3trcqxpso.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3kkkuecmi.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ulyboteo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3sgypetpj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3woyiyhmj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3syrtugtl.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3tsnvawik.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3sxrjzomt.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3sgcaimbi.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3hftvhqfu.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3konalgqv.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wqqrapen.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lsoyrdmc.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bcyojfsm.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zjocenmb.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gtcnkwvq.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lppjolvf.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3utbsouvu.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3sqqilqth.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3dzobemgx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3etmshxtm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3yxnvpfyo.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3ztujjguj.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lkrzgxgu.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3udpoxhxc.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3wlpnvlgy.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dkgmvbxh.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3uzjtwsbv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3rqhvhbyn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ghnoeupm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3bohmabis.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uaeessej.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3dxvpjxlf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3qfpaxdbt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3kfgnaugx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3uiphfvlu.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3sbxuiblm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3tvnhmxtr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nvlrzpne.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yynqwkxn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hypzjatb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3wighwtrn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3lqapkaao.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3tkrcqxes.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3dfqairzq.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3bdwdlceo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3weqqlkfu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3mqtnctdt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3hepsemmj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3cfkvwofy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3msobwlvp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3udnokvsj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3isbpgpsl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3vdoobtfa.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3dhkgxiej.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3czcckpfe.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kzrwvnbc.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fsnqampa.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3evfzukvm.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3gswfbpmh.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ruforftw.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vewodvnh.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3wqlkbolk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bxlbhezx.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3wywoplxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cwwlywwq.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xgcqrbda.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3nqllubfq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3xtmuydje.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3culelelt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vzvighhz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3srvcjxhh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3gzrxmtja.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3zkoevtrl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gwkwixmo.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uoayknci.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3lomkssxk.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sduqxwvf.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dcvklhpj.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3cuzedclu.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3waanaozm.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3moitvggo.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3hhpslubh.html


<!-- 参考信息 -->