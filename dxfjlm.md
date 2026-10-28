代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hywenlv.cn/gthbubperh.html

[R50] awk 求和
来源：http://hz.hnxiangtu.top/gtiaqtayno.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.kuanghao11.cn/gtxspdlmcv.html

[R51] 排序去重取前几
来源：http://hz.daria6918.cn/gtdoxpjhma.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.haohaochexian.top/gtkeskknyv.html

[R52] 统计行数
来源：http://hz.cheryme.top/gtbrdauryv.html

wc -l a.txt
来源：http://hz.yanxiufei.cn/gttosmhddn.html

[R53] 查看文件头与实时尾
来源：http://hz.yonumen.top/gtqcinqygl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jinyuanbaomall.cn/gtqakjahia.html

[R54] 比较两个文件
来源：http://hz.zhoulong.xyz/gtimxppyeh.html

diff a.txt b.txt
来源：http://hz.yj20258888.top/gtxszlqxwh.html

[R55] 压缩与解压
来源：http://hz.jqgfzy.top/gtevmksrss.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.cdnleiting.top/gtoulmcrpc.html

[R56] 远程拷贝
来源：http://hz.yuxming.cn/gtvfokfiub.html

scp file user@host:/path/
来源：http://hz.shanyushiyangtech.top/gtwdktdxuy.html

[R57] 远程执行命令
来源：http://hz.shanyushiyangkeji.top/gtvskyifwn.html

ssh user@host 'uptime'
来源：http://hz.sufxvd.cn/gtepxyihmq.html

[R58] 下载文件
来源：http://hz.cqqwz.cn/gtoisbysmq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.guowangkeji.top/gtxafhcslh.html

[R59] 发 POST JSON
来源：http://hz.jinqigfzy.top/gttrohxttv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.quarkkingdee.top/gtvtyejsin.html

[R60] 只看 HTTP 状态码
来源：http://hz.svipenyu.cn/gtjvqwmmqb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.gotoacloud.top/gtqqriccww.html

[R61] 磁盘占用
来源：http://hz.yueranfly.top/gttneqrbbh.html

df -h;  du -sh *
来源：http://hz.zhijiandao.cn/gtgcatbmos.html

[R62] 找最占空间的文件
来源：http://hz.nwbrower.top/gtuupmoyfw.html

du -ah . | sort -rh | head -10
来源：http://hz.jlsjyb.cn/gtmzgfcgxq.html

[R63] 内存与进程
来源：http://hz.ehwqpu.com/gtsnvfnqxp.html

free -h;  ps aux | grep nginx
来源：http://hz.shanyushiyangkeji.top/gtyuphtiyp.html

[R64] 结束进程
来源：http://hz.ehwqpu.com/gtexehpjts.html

kill -9 $(pgrep -f app.py)
来源：http://hz.svipenyu.cn/gthjaocnnw.html

[R65] 查看端口占用
来源：http://hz.shangyingyoupin.top/gtclowbgij.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zhoulong.xyz/gtnnqoybez.html

[R66] 定时任务
来源：http://hz.havefunace.top/gtdxszgion.html

crontab -e;  crontab -l
来源：http://hz.sufxvd.cn/gttlkccopy.html

[R67] 生成随机十六进制串
来源：http://hz.yueranfly.top/gtnmlgxzvu.html

openssl rand -hex 16
来源：http://hz.shuidangran.top/gtyqgjyaus.html

[R68] 计算文件校验值
来源：http://hz.ydjk.org.cn/gttowtqplc.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.daria6918.cn/gtsxixautu.html

[R69] 生成随机密码
来源：http://hz.zhiwuduotai.top/gtpmzfpoed.html

head -c 16 /dev/urandom | base64
来源：http://hz.xingfuxueyuan.xyz/gtrplxwxdb.html

[R70] 时间戳与互转
来源：http://hz.dianchejie.cn/gtkhsayoqg.html

date +%s;  date -d @1700000000
来源：http://hz.shzxlz.cn/gtocpnyswx.html

[R71] 日期格式化
来源：http://hz.ybcxt.top/gtaytcqhhr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.shzxlz.cn/gtbqhskoou.html

[R72] 等待端口就绪
来源：http://hz.yanxiufei.cn/gtqnbwwgeo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jianghu66.top/gtppzpuxne.html

[R73] 分割大日志
来源：http://hz.iojbl.cn/gtrzpfwlbf.html

split -l 1000 big.log part_
来源：http://hz.c1oappe.top/gttckcmmle.html

[R74] 批量重命名
来源：http://hz.fzhhl.top/gtyvsgnxao.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.snrcjt.cn/gtvtbouetn.html

[R75] 导出环境变量
来源：http://hz.52xcode.cn/gteiduncgm.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.andypj.xyz/gtrmgejfuu.html

[R76] 使用临时文件
来源：http://hz.shzxlz.cn/gtgshbjzff.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.tian-w.cn/gtmbvxbfwm.html

[R77] 读取用户输入
来源：http://hz.yvedp.cn/gtiorxstts.html

read -rp "请输入: " ans
来源：http://hz.xinyue.icu/gtnchbqezs.html

[R78] 交互式菜单
来源：http://hz.fengsongda.top/gtdqvinxmy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.316326.xyz/gtafoekbko.html

[R79] 解析命令行选项
来源：http://hz.zhoulong.xyz/gtwzmckicv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.bjfxy.top/gtjuohzlxm.html

[R80] 查看脚本执行耗时
来源：http://hz.shangyingyoupin.top/gtngtnwujt.html

time ./run.sh
来源：http://hz.zhaomingkeji.xyz/gtokemoozw.html

================================================================================
来源：http://hz.yonumen.top/gtvbtftaty.html

S. C / C++ 专题
来源：http://hz.aibaodan.cn/gtmtaeottm.html

================================================================================
来源：http://hz.zhoulong.xyz/gtrjcdhrjd.html

[S01] C：Hello World
来源：http://hz.xinyue.icu/gtffmeohpy.html

#include <stdio.h>
来源：http://hz.xinyue.icu/gtruqgzhmc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.bjfxy.top/gtnzetjtke.html

[S02] C：变量与格式化输出
来源：http://hz.gaohongyu789.top/gtahrytrpe.html

int a = 10; printf("%d\n", a);
来源：http://hz.nwbrower.top/gtjacenydj.html

[S03] C：读入整数
来源：http://hz.aizwys.cn/gtgpfkexqq.html

int x; scanf("%d", &x);
来源：http://hz.sysykeji.top/gthcsqtcel.html

[S04] C：字符串复制
来源：http://hz.xziqi.cn/gttrysskae.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.tian-w.cn/gtqvinmttj.html

[S05] C：字符串长度
来源：http://hz.meibo888.top/gtbjbhkito.html

strlen(s)
来源：http://hz.9152youxi.cn/gtdcfroiuy.html

[S06] C：字符串比较
来源：http://hz.mhx1999.top/gtvnhbsjyy.html

strcmp(a, b) == 0
来源：http://hz.hnxiangtu.top/gtjxvcwblo.html

[S07] C：数组遍历求和
来源：http://hz.ppjwa.cn/gtziglfegz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hnxiangtu.top/gtgwwafczd.html

[S08] C：动态内存分配与释放
来源：http://hz.iojbl.cn/gtsbguaamw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.xziqi.cn/gtjrkbsvvs.html

[S09] C：结构体定义与初始化
来源：http://hz.tanke756.top/gtyfgvyhnu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.haohaochexian.top/gtamcvtuch.html

[S10] C：指针与解引用
来源：http://hz.mhx1999.top/gtnntokous.html

int *p = &a;  *p = 5;
来源：http://hz.guannengcc.top/gtqwqsghvl.html

[S11] C：逐行读文件
来源：http://hz.havefunace.top/gtoccjoabt.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.iojbl.cn/gtpzpjzvfl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.nanxinkj.top/gtuijoldwk.html

fclose(f);
来源：http://hz.zhiwuduotai.top/gtszdbbknm.html

[S12] C：写文件
来源：http://hz.tanke756.top/gtlugxjysp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.nanxuanxn.top/gtbdsntpoc.html

[S13] C：宏定义
来源：http://hz.nanxuanxn.top/gtjykktvpi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.sufxvd.cn/gtcujymrud.html

[S14] C：枚举
来源：http://hz.zhixingplan.top/gtvaoxthsu.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.birdmap.top/gtwbkbnzzb.html

[S15] C：类型转换
来源：http://hz.zhoulong.xyz/gtrpdrsapl.html

(double) a / b
来源：http://hz.chenzaomai.com/gtocstbkaj.html

[S16] C：位操作置位
来源：http://hz.pycfn.com/gtweaqwqen.html

x |= (1 << 3);
来源：http://hz.chenzaomai.com/gtkrqmqbig.html

[S17] C：安全拼接字符串
来源：http://hz.chenjidiqi.icu/gtpnhhqipa.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ehwqpu.com/gtvoeakdjd.html

[S18] C：命令行参数
来源：http://hz.ivvv.top/gtxrwjsiei.html

int main(int argc, char **argv)
来源：http://hz.dashuyun.cn/gtbnbwhwda.html

[S19] C：快速排序
来源：http://hz.xylfe.cn/gtmcondvum.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.feifeiyinyue.top/gtxasyxrlb.html

[S20] C：二分查找
来源：http://hz.sxryk.cn/gtjearzrei.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhongyouzk.top/gtoyfdhsij.html

[S21] C：字符类别判断
来源：http://hz.gogol.net.cn/gtbymfkufq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.bjfxy.top/gtxxycmszg.html

[S22] C：字符串转数字
来源：http://hz.9152youxi.cn/gtvhjjeksf.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.guowangkeji.top/gtbsvqeawu.html

[S23] C：随机数
来源：http://hz.hfpthk.cn/gtowoyqlno.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.dashuyun.cn/gtukhkktuq.html

[S24] C：获取本地时间
来源：http://hz.jianghu66.top/gtlqmxztuy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jinqigfzy.top/gtermlkfvd.html

[S25] C：内存拷贝
来源：http://hz.xuanzx.com/gtgxftaksu.html

memcpy(dst, src, n);
来源：http://hz.jyoumei.cn/gtkacespub.html

[S26] C：内存清零
来源：http://hz.xuanzx.com/gtcdwpehwd.html

memset(a, 0, sizeof a);
来源：http://hz.sxryk.cn/gtshgqieyr.html

[S27] C：定义常量
来源：http://hz.pengpengdd.cyou/gtrxgxazxx.html

const double PI = 3.14159;
来源：http://hz.jyoumei.cn/gtnvzitbqt.html

[S28] C：静态变量
来源：http://hz.chenjidiqi.icu/gtzqwweoud.html

static int counter = 0;
来源：http://hz.52xcode.cn/gtxquyhhtt.html

[S29] C：变参函数
来源：http://hz.meibo888.top/gtscarjwcc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.snrcjt.cn/gtjzvakjof.html

[S30] C：头文件保护
来源：http://hz.zhoulong.xyz/gtfiiprlwr.html

#ifndef X_H
来源：http://hz.cheryme.top/gtlycsxqyo.html

#define X_H
来源：http://hz.wangdashe.top/gtlvnmtluk.html

#endif
来源：http://hz.haohaochexian.top/gtfvmvwhqn.html

[S31] C++：Hello World
来源：http://hz.hysaishi.cn/gtwxgmlamh.html

#include <iostream>
来源：http://hz.hfpthk.cn/gtcrepvmyk.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.guannengcc.top/gthlcabxen.html

[S32] C++：字符串
来源：http://hz.0kj1m.cn/gtfihynbrb.html

std::string s = "hi";  s += "!";
来源：http://hz.cdnleiting.top/gtsxbbjjkn.html

[S33] C++：vector 增删
来源：http://hz.svipenyu.cn/gtewgxzuwu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.shzxlz.cn/gtsoovdytr.html

[S34] C++：遍历 vector
来源：http://hz.yangfankeji.com/gtntnezblo.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ydzc1.top/gtgwdzawxq.html

[S35] C++：map
来源：http://hz.jinghuilouyu.cn/gthkyqvhvd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhaomingkeji.xyz/gttfvsvktr.html

[S36] C++：unordered_map
来源：http://hz.jinyuanbaomall.cn/gteytfkydm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yonumen.top/gtlxwjoyyc.html

[S37] C++：set
来源：http://hz.xuanzx.com/gtnjfzjnja.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yuanzhike.top/gtsmkromjo.html

[S38] C++：排序
来源：http://hz.yj202588.top/gtwltskefa.html

std::sort(v.begin(), v.end());
来源：http://hz.ppjwa.cn/gtzwyeqiid.html

[S39] C++：自定义比较器排序
来源：http://hz.xuanzx.com/gtfqplyepl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.tianlin.xyz/gttiynhren.html

[S40] C++：查找元素
来源：http://hz.zycfv.cn/gtuvinkfrr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.mhx1999.top/gttjxjhaxo.html

[S41] C++：类与构造函数
来源：http://hz.ppjwa.cn/gtaimoivvi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.cashguo.top/gtdfrkytgu.html

[S42] C++：继承与虚函数
来源：http://hz.nanxuanxn.top/gtazwrkxyf.html

class B : public Base { public: void f() override {} };
来源：http://hz.ppjwa.cn/gttvsurewh.html

[S43] C++：智能指针
来源：http://hz.smart0.xyz/gtmrhhvzhe.html

auto p = std::make_unique<int>(5);
来源：http://hz.wangdashe.top/gtdgieaiqf.html

[S44] C++：引用传参
来源：http://hz.havefunace.top/gtuwwifqaa.html

void inc(int &x) { ++x; }
来源：http://hz.snrcjt.cn/gtqbpubgoq.html

[S45] C++：lambda
来源：http://hz.aizwys.cn/gtcigyeujc.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yuanzhike.top/gtqtfdvfvx.html

[S46] C++：函数模板
来源：http://hz.jinyuanbaomall.cn/gtvvikiaby.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhoulong.xyz/gtsgpzstou.html

[S47] C++：结构化绑定遍历
来源：http://hz.gogol.net.cn/gtqotlwqzd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhixingplan.top/gtgrklojxd.html

[S48] C++：逐行读文件
来源：http://hz.yueranfly.top/gtftinzgwa.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhoulong.xyz/gtgycuzzfj.html

while (std::getline(in, line)) { }
来源：http://hz.hywenlv.cn/gtpknuhnno.html

[S49] C++：写文件
来源：http://hz.kuanghao11.cn/gtqesaobym.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.sysykeji.top/gtgpuktlvr.html

[S50] C++：格式化数字
来源：http://hz.kuanghao11.cn/gtflcrrgdj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.ydzc1.top/gtuylcapuj.html

[S51] C++：显式类型转换
来源：http://hz.zycfv.cn/gtreonehwj.html

static_cast<double>(a) / b
来源：http://hz.vqdsnc.cn/gtkxkxcjfv.html

[S52] C++：const 与 noexcept
来源：http://hz.redwolf501.top/gtjcxhvrwu.html

int size() const noexcept { return n_; }
来源：http://hz.pycfn.com/gtfkyvudwk.html

[S53] C++：移动语义
来源：http://hz.vqdsnc.cn/gtszetspdb.html

std::vector<int> w = std::move(v);
来源：http://hz.ppjwa.cn/gtsmxpgggv.html

[S54] C++：异常处理
来源：http://hz.ppjwa.cn/gtpjezknpk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yangfankeji.com/gtwefeutyf.html

[S55] C++：结构化绑定
来源：http://hz.gzhubu.top/gtumpijdzn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.svipenyu.cn/gtgmxzsppp.html

[S56] C++：optional
来源：http://hz.52xcode.cn/gtmhcgvwpq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.dianchejie.cn/gtluzzxwpj.html

[S57] C++：编译期常量
来源：http://hz.ywan-chungtsiang.top/gtlrnlpqzd.html

constexpr int N = 10;
来源：http://hz.zhiwuduotai.top/gtbeghpkxc.html

[S58] C++：命名空间
来源：http://hz.jqgufenzy.top/gtaizashbu.html

namespace ns { int f() { return 1; } }
来源：http://hz.0kj1m.cn/gtcrlujopv.html

[S59] C++：静态断言
来源：http://hz.yj20258888.top/gtnqqbruss.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.0kj1m.cn/gtsuqayayt.html

[S60] C++：遍历并删除元素
来源：http://hz.yvedp.cn/gtotponawq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.nwbrower.top/gtqrkneckf.html

================================================================================
来源：http://hz.sxryk.cn/gtolhicegs.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shzxlz.cn/gtkulxhchg.html

================================================================================
来源：http://hz.yj20258.top/gtzxtmenen.html

[T01] Kotlin：Hello World
来源：http://hz.yj20258888.top/gtvlmrqlum.html

println("Hello")
来源：http://hz.cucudq.cn/gtdkfdyfvd.html

[T02] Kotlin：变量
来源：http://hz.shangyingyoupin.top/gtyilyrcpk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.sxryk.cn/gtquwrwgri.html

[T03] Kotlin：字符串模板
来源：http://hz.hammf.cn/gtdlhqjnis.html

"值: $b"
来源：http://hz.feifeiyinyue.top/gtimsjcvpa.html

[T04] Kotlin：空安全
来源：http://hz.redwolf501.top/gtlnprnvov.html

val n: String? = null;  n?.length
来源：http://hz.ybcxt.top/gtqoiqayhi.html

[T05] Kotlin：when 表达式
来源：http://hz.shzxlz.cn/gtnleskgcm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jiagoushi.top/gtxszqowge.html

[T06] Kotlin：集合映射
来源：http://hz.feifeiyinyue.top/gttngjhiuq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yangfankeji.com/gtajonjfwa.html

[T07] Kotlin：集合过滤
来源：http://hz.andypj.xyz/gtiytgkbvu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.shanyushiyangkeji.top/gtblziqmfb.html

[T08] Kotlin：数据类
来源：http://hz.nwbrower.top/gthubtymmb.html

data class User(val name: String, val age: Int)
来源：http://hz.cucudq.cn/gtzgpeyefx.html

[T09] Kotlin：扩展函数
来源：http://hz.yanxiufei.cn/gtnfcagryr.html

fun String.exclaim() = this + "!"
来源：http://hz.chenzaomai.com/gtrwqpklgn.html

[T10] Kotlin：默认参数
来源：http://hz.jqgufenzy.top/gtufxuylru.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.cqqwz.cn/gtvcbaefes.html

[T11] Kotlin：协程
来源：http://hz.snrcjt.cn/gtkxbgwvda.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.tianlin.xyz/gtfyfglodr.html

[T12] Kotlin：解构声明
来源：http://hz.cashguo.top/gtzkvcgpqo.html

val (a, b) = Pair(1, 2)
来源：http://hz.iojbl.cn/gtaclchnpa.html

[T13] Kotlin：只读 Map
来源：http://hz.sweek.top/gteqkwgaix.html

val m = mapOf("a" to 1)
来源：http://hz.zhongyouzk.top/gtxwxsezjg.html

[T14] Kotlin：循环
来源：http://hz.mhx1999.top/gtguivawjm.html

for (i in 1..10) println(i)
来源：http://hz.xziqi.cn/gtmzhxuivd.html

[T15] Kotlin：接口
来源：http://hz.ivvv.top/gtygqjacqo.html

interface Shape { fun area(): Double }
来源：http://hz.tian-w.cn/gtrrwiqzbm.html

[T16] Swift：Hello World
来源：http://hz.guannengcc.top/gtkiquhejw.html

print("Hello")
来源：http://hz.gzhubu.top/gtxxadlhtm.html

[T17] Swift：变量与常量
来源：http://hz.xinyue.icu/gtrmohcqqv.html

var a = 1;  let b = 2
来源：http://hz.yanxiufei.cn/gtxfmzocws.html

[T18] Swift：字符串插值
来源：http://hz.hysaishi.cn/gtfoohcqhf.html

"值: \(b)"
来源：http://hz.zhiwuduotai.top/gtntnxoowo.html

[T19] Swift：可选绑定
来源：http://hz.chenlongwang.top/gtgsuczgor.html

if let n = opt { print(n) }
来源：http://hz.xinyue.icu/gtzbdcyufz.html

[T20] Swift：数组操作
来源：http://hz.guowangkeji.top/gtqqyplsqb.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.hnxiangtu.top/gtvwqpciho.html

[T21] Swift：遍历
来源：http://hz.cheryme.top/gtxhznesur.html

for x in a { print(x) }
来源：http://hz.tanke756.top/gtvekivksz.html

[T22] Swift：字典
来源：http://hz.fengsongda.top/gthnppotba.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.yuanzhike.top/gtktiyumdy.html

[T23] Swift：函数
来源：http://hz.daria6918.cn/gtpwokhykx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.daxiang520.top/gtcwqtmscp.html

[T24] Swift：闭包
来源：http://hz.jqgfzy.top/gtbsildxgf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zhixingplan.top/gtjrnzjpib.html

[T25] Swift：结构体
来源：http://hz.aizwys.cn/gtuztxdkth.html

struct P { var x: Int }
来源：http://hz.cdnleiting.top/gtbptchgsr.html

[T26] Swift：类与重写
来源：http://hz.zhengqikj.top/gtfojwvqfr.html

class A: Base { override func f() {} }
来源：http://hz.ydjk.org.cn/gtscrgaalm.html

[T27] Swift：错误处理
来源：http://hz.hfpthk.cn/gtluwzlvmb.html

do { try f() } catch { print(error) }
来源：http://hz.feifeiyinyue.top/gtxwjzzevh.html

[T28] Swift：枚举
来源：http://hz.yongpay.top/gtmndpkass.html

enum Color { case red, green }
来源：http://hz.yanxiufei.cn/gtlmvghdlv.html

[T29] Swift：guard 提前返回
来源：http://hz.guowangkeji.top/gtfymylodh.html

guard let x = opt else { return }
来源：http://hz.shanyushiyangkeji.top/gtmyclznjq.html

[T30] Swift：协议
来源：http://hz.cucudq.cn/gthmfftuti.html

protocol Shape { func area() -> Double }
来源：http://hz.shanyushiyangkeji.top/gtdhyqeavn.html

[T31] Lua：Hello World
来源：http://hz.chenlongwang.top/gtxbjciswu.html

print("Hello")
来源：http://hz.zhijiandao.cn/gtmoykiihz.html

[T32] Lua：局部变量
来源：http://hz.cucudq.cn/gtwfgwxzok.html

local a = 1
来源：http://hz.xuetiantiany.cn/gtmfiznjpi.html

[T33] Lua：表（数组）
来源：http://hz.xuetiantiany.cn/gtsburbicw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.ppjwa.cn/gtxlxvzktp.html

[T34] Lua：遍历表
来源：http://hz.tian-w.cn/gtbllcwvpp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.smart0.xyz/gtjttdplyh.html

[T35] Lua：字典表
来源：http://hz.pycfn.com/gtjvkiyogm.html

local d = { a = 1 };  d.b = 2
来源：http://hz.feifeiyinyue.top/gtpyexzkmo.html

[T36] Lua：函数
来源：http://hz.hfpthk.cn/gtdnzernax.html

function add(a, b) return a + b end
来源：http://hz.birdmap.top/gtacvanvac.html

[T37] Lua：字符串拼接
来源：http://hz.daria6918.cn/gtwnyewiyh.html

"a" .. "b"
来源：http://hz.guowangkeji.top/gtwlujjmoj.html

[T38] Lua：条件
来源：http://hz.gzhubu.top/gtuzmgtoqp.html

if x > 0 then print("正") end
来源：http://hz.daxiang520.top/gtsewxfnqa.html

[T39] Lua：模式匹配
来源：http://hz.tanke756.top/gtkvalskug.html

string.find(s, "%d+")
来源：http://hz.sysykeji.top/gtrahtcfhn.html

[T40] Lua：元表
来源：http://hz.ivvv.top/gtvbbdbonn.html

setmetatable({}, { __index = base })
来源：http://hz.hnqzz.top/gtzljvfhdv.html

[T41] Perl：Hello World
来源：http://hz.9152youxi.cn/gtcpmbcrzt.html

print "Hello\n";
来源：http://hz.chenjidiqi.icu/gtobdazqww.html

[T42] Perl：变量类型
来源：http://hz.yongpay.top/gtwkurkzxt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.hnqzz.top/gtwwnbufnw.html

[T43] Perl：字符串插值
来源：http://hz.chenjidiqi.icu/gtybxtncuf.html

"值: $a"
来源：http://hz.bjfxy.top/gtiyeqaaxu.html

[T44] Perl：条件
来源：http://hz.yongpay.top/gtgejgripn.html

if ($a > 0) { print "正"; }
来源：http://hz.mhx1999.top/gthklaebpv.html

[T45] Perl：数组遍历
来源：http://hz.sweek.top/gtgfujsryz.html

for my $x (@arr) { print $x; }
来源：http://hz.haohaochexian.top/gtymyiimef.html

[T46] Perl：哈希操作
来源：http://hz.jinqigufen.top/gtufjfnzua.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.kuanghao11.cn/gtgrrzthhm.html

[T47] Perl：正则捕获
来源：http://hz.feifeiyinyue.top/gtnepnmpwi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.ybcxt.top/gtkdegmydf.html

[T48] Perl：正则替换
来源：http://hz.iojbl.cn/gtoobvpboc.html

$s =~ s/old/new/g;
来源：http://hz.jinqigufen.top/gtjpajndwo.html

[T49] Perl：函数
来源：http://hz.zdqjudy.top/gtthljulsz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.fengsongda.top/gtrmzedunj.html

[T50] Perl：逐行读文件
来源：http://hz.jinghuilouyu.cn/gtjyouifsa.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jinqigufen.top/gtzfnwrtcn.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.hywenlv.cn/gtphiifcja.html

[T51] Scala：Hello World
来源：http://hz.zhongyouzk.top/gtabqvbgxb.html

println("Hello")
来源：http://hz.zycfv.cn/gtmgnsczsl.html

[T52] Scala：变量
来源：http://hz.bjfxy.top/gtwcuwfnpd.html


<!-- 参考信息 -->