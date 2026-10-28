代发 wailian999

find . -name "*.tmp" -delete
来源：http://hz.redwolf501.top/gtgbjcnwnw.html

[R46] 递归替换文件内容
来源：http://hz.yj202588.top/gtbevwiifd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.guowangkeji.top/gtgujcelqb.html

[R47] sed 单行替换
来源：http://hz.316326.xyz/gtvjtpfnhf.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.aibaodan.cn/gtjztqkgmk.html

[R48] awk 取指定列
来源：http://hz.yj20258888.top/gtryeqprft.html

awk '{print $1, $3}' a.txt
来源：http://hz.jianghu66.top/gttwblhtoo.html

[R49] awk 带条件
来源：http://hz.yj20258888.top/gtqfppxbxp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhengqikj.top/gtnzsgrmkn.html

[R50] awk 求和
来源：http://hz.bjfxy.top/gtkxpyclhi.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.gogol.net.cn/gtrmilrtfu.html

[R51] 排序去重取前几
来源：http://hz.quarkkingdee.top/gtztthkjcy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.9152youxi.cn/gtvjrybnbx.html

[R52] 统计行数
来源：http://hz.pengpengdd.cyou/gtljrieoff.html

wc -l a.txt
来源：http://hz.ybcxt.top/gtitolpbtk.html

[R53] 查看文件头与实时尾
来源：http://hz.gzhubu.top/gthrvjviyb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.shuidangran.top/gtlkuncjju.html

[R54] 比较两个文件
来源：http://hz.yuanzhike.top/gtbgiekddh.html

diff a.txt b.txt
来源：http://hz.xuanzx.com/gtcofumtga.html

[R55] 压缩与解压
来源：http://hz.xinyue.icu/gthbhuoaql.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xylfe.cn/gtwydivcek.html

[R56] 远程拷贝
来源：http://hz.vqdsnc.cn/gtaaxchunp.html

scp file user@host:/path/
来源：http://hz.dashuyun.cn/gtruybajhr.html

[R57] 远程执行命令
来源：http://hz.jinqigfzy.top/gtoexzwddt.html

ssh user@host 'uptime'
来源：http://hz.hywenlv.cn/gtxwnfjkow.html

[R58] 下载文件
来源：http://hz.zhiwuduotai.top/gtnxmzcwyr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.redwolf501.top/gtxtmshvtv.html

[R59] 发 POST JSON
来源：http://hz.zhengqikj.top/gtxsicsomd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.smart0.xyz/gtiftjttwp.html

[R60] 只看 HTTP 状态码
来源：http://hz.hywenlv.cn/gtnfxtapiw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.chenzaomai.com/gtnqsiedxv.html

[R61] 磁盘占用
来源：http://hz.jinqigfzy.top/gtslumuvyt.html

df -h;  du -sh *
来源：http://hz.jianghu66.top/gtmyotbytr.html

[R62] 找最占空间的文件
来源：http://hz.yvedp.cn/gtlxnyhkzg.html

du -ah . | sort -rh | head -10
来源：http://hz.gzhubu.top/gttfkjnbtp.html

[R63] 内存与进程
来源：http://hz.zhijiandao.cn/gtnhyyrnxy.html

free -h;  ps aux | grep nginx
来源：http://hz.pycfn.com/gtiqnblsfn.html

[R64] 结束进程
来源：http://hz.quarkkingdee.top/gtiywjfwaq.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zdqjudy.top/gtlviudsti.html

[R65] 查看端口占用
来源：http://hz.sufxvd.cn/gtzcdrecwp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.gaohongyu789.top/gtzcvkyqsk.html

[R66] 定时任务
来源：http://hz.jianghu66.top/gtrjpkejxh.html

crontab -e;  crontab -l
来源：http://hz.316326.xyz/gtsaotllld.html

[R67] 生成随机十六进制串
来源：http://hz.9152youxi.cn/gtcchkddiz.html

openssl rand -hex 16
来源：http://hz.nwbrower.top/gtmeedynbi.html

[R68] 计算文件校验值
来源：http://hz.ywan-chungtsiang.top/gtqkauacko.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.shuidangran.top/gtiynhxkwd.html

[R69] 生成随机密码
来源：http://hz.aizwys.cn/gtinelrkug.html

head -c 16 /dev/urandom | base64
来源：http://hz.sysykeji.top/gtkecbnhin.html

[R70] 时间戳与互转
来源：http://hz.zhoulong.xyz/gtniokxwgn.html

date +%s;  date -d @1700000000
来源：http://hz.hysaishi.cn/gtvjaerzht.html

[R71] 日期格式化
来源：http://hz.xylfe.cn/gtupygtrra.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yuxming.cn/gthttnmbbz.html

[R72] 等待端口就绪
来源：http://hz.gzhubu.top/gtfqjcfhpl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.snrcjt.cn/gtapvpbrzd.html

[R73] 分割大日志
来源：http://hz.guannengcc.top/gtpzyijqgz.html

split -l 1000 big.log part_
来源：http://hz.tian-w.cn/gtiwxwrgqa.html

[R74] 批量重命名
来源：http://hz.jinghuilouyu.cn/gteabsrmtc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jinghuilouyu.cn/gtjiwnywkd.html

[R75] 导出环境变量
来源：http://hz.gzhubu.top/gtrtivcywe.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yangfankeji.com/gtabffrvsd.html

[R76] 使用临时文件
来源：http://hz.hammf.cn/gtkvxvccxw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.aizwys.cn/gthuwifzfy.html

[R77] 读取用户输入
来源：http://hz.pengpengdd.cyou/gtozjejcfb.html

read -rp "请输入: " ans
来源：http://hz.havefunace.top/gtbzmizyjt.html

[R78] 交互式菜单
来源：http://hz.smart0.xyz/gtpliudkvp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yongpay.top/gtkcnoppgl.html

[R79] 解析命令行选项
来源：http://hz.nanxinkj.top/gtsjykuwjn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.dashuyun.cn/gtfhmulzpq.html

[R80] 查看脚本执行耗时
来源：http://hz.hywenlv.cn/gtqlsacygo.html

time ./run.sh
来源：http://hz.xziqi.cn/gtylblyisr.html

================================================================================
来源：http://hz.jyoumei.cn/gthvnrscrx.html

S. C / C++ 专题
来源：http://hz.havefunace.top/gtujuxvkvr.html

================================================================================
来源：http://hz.zdqjudy.top/gtjifhtzyn.html

[S01] C：Hello World
来源：http://hz.guannengcc.top/gtrtasznnx.html

#include <stdio.h>
来源：http://hz.hfpthk.cn/gtthvmbjhp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zycfv.cn/gtiwzothwi.html

[S02] C：变量与格式化输出
来源：http://hz.hongshengwenyu.top/gthrpzgxbn.html

int a = 10; printf("%d\n", a);
来源：http://hz.jinghuilouyu.cn/gtiinjoxhm.html

[S03] C：读入整数
来源：http://hz.yj20258.top/gtsqmblbji.html

int x; scanf("%d", &x);
来源：http://hz.jqgfzy.top/gtyqltcthf.html

[S04] C：字符串复制
来源：http://hz.andypj.xyz/gtrzeteilj.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhijiandao.cn/gtdccibrlv.html

[S05] C：字符串长度
来源：http://hz.yj20258888.top/gtakeiargy.html

strlen(s)
来源：http://hz.jqgufenzy.top/gtrehstaob.html

[S06] C：字符串比较
来源：http://hz.9152youxi.cn/gtkksgcsbv.html

strcmp(a, b) == 0
来源：http://hz.hongshengwenyu.top/gtaeqldfqk.html

[S07] C：数组遍历求和
来源：http://hz.sufxvd.cn/gtvfczfqqf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zhengqikj.top/gtkmcraeis.html

[S08] C：动态内存分配与释放
来源：http://hz.nanxinkj.top/gttdlunkzn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zdqjudy.top/gtduoaplto.html

[S09] C：结构体定义与初始化
来源：http://hz.chenzaomai.com/gtmspcjhlt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.quarkkingdee.top/gtuqyluprd.html

[S10] C：指针与解引用
来源：http://hz.hnxiangtu.top/gtlghtjmcp.html

int *p = &a;  *p = 5;
来源：http://hz.daria6918.cn/gtlrqvvbqb.html

[S11] C：逐行读文件
来源：http://hz.dashuyun.cn/gtqzogyyru.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.ydjk.org.cn/gtgprbvgrk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.havefunace.top/gtqhqjcxag.html

fclose(f);
来源：http://hz.redwolf501.top/gtssafrjtp.html

[S12] C：写文件
来源：http://hz.ybcxt.top/gtewhncxqp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yvedp.cn/gtxsrejkif.html

[S13] C：宏定义
来源：http://hz.havefunace.top/gtoyhhqhsl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hongshengwenyu.top/gtijcwyqha.html

[S14] C：枚举
来源：http://hz.haohaochexian.top/gtpjiqhuhz.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.gogol.net.cn/gtvfcklave.html

[S15] C：类型转换
来源：http://hz.mhx1999.top/gtdujtrhvj.html

(double) a / b
来源：http://hz.hnxiangtu.top/gtqziwmpjs.html

[S16] C：位操作置位
来源：http://hz.birdmap.top/gtgagrtiyt.html

x |= (1 << 3);
来源：http://hz.xziqi.cn/gtdksgqwmk.html

[S17] C：安全拼接字符串
来源：http://hz.yuxming.cn/gtwuxehcqd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.shanyushiyangtech.top/gtjvgpnrcw.html

[S18] C：命令行参数
来源：http://hz.tian-w.cn/gtdrrtutmn.html

int main(int argc, char **argv)
来源：http://hz.sxryk.cn/gtxhprpdbt.html

[S19] C：快速排序
来源：http://hz.nanxinkj.top/gtklsptxtc.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.guannengcc.top/gttruitrnb.html

[S20] C：二分查找
来源：http://hz.hongshengwenyu.top/gtlswkcfgs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ywan-chungtsiang.top/gtlztjxrnd.html

[S21] C：字符类别判断
来源：http://hz.gzhubu.top/gtzazrpmaa.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jlsjyb.cn/gtgltwqckg.html

[S22] C：字符串转数字
来源：http://hz.shangyingyoupin.top/gtnlcasrjp.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.cqqwz.cn/gtnnhkxwtn.html

[S23] C：随机数
来源：http://hz.vqdsnc.cn/gthyevtoee.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhongyouzk.top/gtgxwpawmf.html

[S24] C：获取本地时间
来源：http://hz.nanxinkj.top/gttfhhjyxr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jianghu66.top/gtpaerrvsy.html

[S25] C：内存拷贝
来源：http://hz.sxryk.cn/gtysxcrpva.html

memcpy(dst, src, n);
来源：http://hz.hfpthk.cn/gtbkxdzjsu.html

[S26] C：内存清零
来源：http://hz.cqqwz.cn/gtyiabwzok.html

memset(a, 0, sizeof a);
来源：http://hz.yongpay.top/gtihatyysj.html

[S27] C：定义常量
来源：http://hz.gogol.net.cn/gthyhlamiy.html

const double PI = 3.14159;
来源：http://hz.shangyingyoupin.top/gtlaciabyy.html

[S28] C：静态变量
来源：http://hz.aizwys.cn/gtnrvplimn.html

static int counter = 0;
来源：http://hz.yj20258.top/gtcmaeztpt.html

[S29] C：变参函数
来源：http://hz.birdmap.top/gtxfjgtznb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.smart0.xyz/gtfkwakyoe.html

[S30] C：头文件保护
来源：http://hz.nanxinkj.top/gtgdnrwadx.html

#ifndef X_H
来源：http://hz.snrcjt.cn/gtczrjyzaj.html

#define X_H
来源：http://hz.0kj1m.cn/gtgwwbtkkf.html

#endif
来源：http://hz.jinqigufen.top/gtwgjvxgyw.html

[S31] C++：Hello World
来源：http://hz.cheryme.top/gtlfffztvy.html

#include <iostream>
来源：http://hz.cashguo.top/gtgumxjojh.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.cucudq.cn/gtywammuyr.html

[S32] C++：字符串
来源：http://hz.chenjidiqi.icu/gtbwmzluuw.html

std::string s = "hi";  s += "!";
来源：http://hz.shzxlz.cn/gthhkcsyer.html

[S33] C++：vector 增删
来源：http://hz.hnqzz.top/gtmtgjnhqp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.dianchejie.cn/gtrspaihmf.html

[S34] C++：遍历 vector
来源：http://hz.tian-w.cn/gtcyxbydxn.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.hnqzz.top/gtmfjbomah.html

[S35] C++：map
来源：http://hz.zdqjudy.top/gtueydqjvp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.chenzaomai.com/gtzkprqdzu.html

[S36] C++：unordered_map
来源：http://hz.yonumen.top/gtdlrcppsp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.daxiang520.top/gtssddlfnn.html

[S37] C++：set
来源：http://hz.kuanghao11.cn/gtowfuktkx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jianghu66.top/gtjhbnbeyx.html

[S38] C++：排序
来源：http://hz.52xcode.cn/gtvgfcagun.html

std::sort(v.begin(), v.end());
来源：http://hz.hfpthk.cn/gtiaceuurv.html

[S39] C++：自定义比较器排序
来源：http://hz.vqdsnc.cn/gtffrtvick.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.havefunace.top/gtbywhsubn.html

[S40] C++：查找元素
来源：http://hz.yanxiufei.cn/gtxzazbyaf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.cqqwz.cn/gtbsqcypib.html

[S41] C++：类与构造函数
来源：http://hz.chenlongwang.top/gtyapoobfb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hnxiangtu.top/gtysvhgfau.html

[S42] C++：继承与虚函数
来源：http://hz.yj202588.top/gtzbvozedj.html

class B : public Base { public: void f() override {} };
来源：http://hz.fzhhl.top/gtzqpqjdxr.html

[S43] C++：智能指针
来源：http://hz.sysykeji.top/gtvkesdydh.html

auto p = std::make_unique<int>(5);
来源：http://hz.zhengqikj.top/gtpplmmtvz.html

[S44] C++：引用传参
来源：http://hz.jiagoushi.top/gtuhkzdvnz.html

void inc(int &x) { ++x; }
来源：http://hz.jqgufenzy.top/gtahdqeudh.html

[S45] C++：lambda
来源：http://hz.yvedp.cn/gtltgdkvso.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yongpay.top/gtobitkyig.html

[S46] C++：函数模板
来源：http://hz.hfpthk.cn/gtpuzzsibm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.cqqwz.cn/gtvnkghsyo.html

[S47] C++：结构化绑定遍历
来源：http://hz.tianlin.xyz/gtqbzybqly.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.kuanghao11.cn/gtwjqpuyun.html

[S48] C++：逐行读文件
来源：http://hz.mhx1999.top/gtmokqmtbt.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.hnxiangtu.top/gtkkqnpgvy.html

while (std::getline(in, line)) { }
来源：http://hz.hysaishi.cn/gtivaaixpx.html

[S49] C++：写文件
来源：http://hz.hnxiangtu.top/gtbijrkkgw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jinghuilouyu.cn/gtvefewiwv.html

[S50] C++：格式化数字
来源：http://hz.chenzaomai.com/gtxfxderek.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.kuanghao11.cn/gtjpdkozpu.html

[S51] C++：显式类型转换
来源：http://hz.yvedp.cn/gtuylpepjl.html

static_cast<double>(a) / b
来源：http://hz.pycfn.com/gtnmpvvatq.html

[S52] C++：const 与 noexcept
来源：http://hz.cucudq.cn/gttlmpelmg.html

int size() const noexcept { return n_; }
来源：http://hz.sxryk.cn/gtorjcwvwd.html

[S53] C++：移动语义
来源：http://hz.tian-w.cn/gtvitsiiel.html

std::vector<int> w = std::move(v);
来源：http://hz.yangfankeji.com/gthyhodlck.html

[S54] C++：异常处理
来源：http://hz.zhaomingkeji.xyz/gthxgwmmoi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.tanke756.top/gtrixncfdg.html

[S55] C++：结构化绑定
来源：http://hz.jianghu66.top/gtqvsfanbd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.xuanzx.com/gtoucnoljv.html

[S56] C++：optional
来源：http://hz.yj20258.top/gtnibtpwai.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhengqikj.top/gtpjsucspj.html

[S57] C++：编译期常量
来源：http://hz.tianlin.xyz/gtszgqrmgi.html

constexpr int N = 10;
来源：http://hz.gzhubu.top/gtiqbmaooi.html

[S58] C++：命名空间
来源：http://hz.andypj.xyz/gtiufhiefr.html

namespace ns { int f() { return 1; } }
来源：http://hz.yueranfly.top/gtxarrkoqh.html

[S59] C++：静态断言
来源：http://hz.jqgufenzy.top/gtaxcgnern.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zdqjudy.top/gtppflmpaq.html

[S60] C++：遍历并删除元素
来源：http://hz.cashguo.top/gtrgkxhapv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.fzhhl.top/gtdaatjusf.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtaknhohgj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.bjfxy.top/gtdbfjrwyz.html

================================================================================
来源：http://hz.jqgufenzy.top/gtgfvlwguf.html

[T01] Kotlin：Hello World
来源：http://hz.jqgufenzy.top/gtkarhwhkx.html

println("Hello")
来源：http://hz.hnxiangtu.top/gtvbdrapqf.html

[T02] Kotlin：变量
来源：http://hz.ybcxt.top/gtcfqstaoh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.cqqwz.cn/gtoqdxjird.html

[T03] Kotlin：字符串模板
来源：http://hz.nanxinkj.top/gtdzbjbxcx.html

"值: $b"
来源：http://hz.pycfn.com/gtfuxfxdne.html

[T04] Kotlin：空安全
来源：http://hz.gotoacloud.top/gtydmvcagk.html

val n: String? = null;  n?.length
来源：http://hz.jlsjyb.cn/gtparporhf.html

[T05] Kotlin：when 表达式
来源：http://hz.redwolf501.top/gtljfgdmzq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.0kj1m.cn/gtxamdtkow.html

[T06] Kotlin：集合映射
来源：http://hz.xylfe.cn/gtwxpaucca.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.guannengcc.top/gtlsdrgjtl.html

[T07] Kotlin：集合过滤
来源：http://hz.yj20258888.top/gtuhdahlwg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.guowangkeji.top/gtipvxhvww.html

[T08] Kotlin：数据类
来源：http://hz.vqdsnc.cn/gtajcrensm.html

data class User(val name: String, val age: Int)
来源：http://hz.yanxiufei.cn/gtguhthqur.html

[T09] Kotlin：扩展函数
来源：http://hz.nwbrower.top/gtyzfuhhvh.html

fun String.exclaim() = this + "!"
来源：http://hz.tanke756.top/gtdjuqhfqt.html

[T10] Kotlin：默认参数
来源：http://hz.xuanzx.com/gtsxnnfdlc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ehwqpu.com/gtkrstldmw.html

[T11] Kotlin：协程
来源：http://hz.xinyue.icu/gtyhswutzw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.fengsongda.top/gtcwsgepad.html

[T12] Kotlin：解构声明
来源：http://hz.yj20258888.top/gtnfjcnkbt.html

val (a, b) = Pair(1, 2)
来源：http://hz.zhijiandao.cn/gtfppvdafm.html

[T13] Kotlin：只读 Map
来源：http://hz.fzhhl.top/gtbxtzaipu.html

val m = mapOf("a" to 1)
来源：http://hz.kuanghao11.cn/gtmhwfrkcv.html

[T14] Kotlin：循环
来源：http://hz.gaohongyu789.top/gtpfgmcnso.html

for (i in 1..10) println(i)
来源：http://hz.gzhubu.top/gtuudjiccn.html

[T15] Kotlin：接口
来源：http://hz.yuxming.cn/gtwwekbedz.html

interface Shape { fun area(): Double }
来源：http://hz.svipenyu.cn/gtihtkstma.html

[T16] Swift：Hello World
来源：http://hz.hammf.cn/gtldkmtwig.html

print("Hello")
来源：http://hz.redwolf501.top/gtpdgzomtp.html

[T17] Swift：变量与常量
来源：http://hz.chenlongwang.top/gtdfgjizld.html

var a = 1;  let b = 2
来源：http://hz.ydzc1.top/gtnbaxlutp.html

[T18] Swift：字符串插值
来源：http://hz.zhiwuduotai.top/gtqendxvph.html

"值: \(b)"
来源：http://hz.hongshengwenyu.top/gtmgsspigb.html

[T19] Swift：可选绑定
来源：http://hz.sweek.top/gtvgllspdo.html

if let n = opt { print(n) }
来源：http://hz.yj20258.top/gtrhgwogat.html

[T20] Swift：数组操作
来源：http://hz.haohaochexian.top/gtzbrjxhad.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jinqigfzy.top/gtthbsjacj.html

[T21] Swift：遍历
来源：http://hz.daria6918.cn/gtbgzgeqre.html

for x in a { print(x) }
来源：http://hz.nanxinkj.top/gtziwqewsn.html

[T22] Swift：字典
来源：http://hz.tian-w.cn/gtzqwcqurz.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.yongpay.top/gtaxcaonsx.html

[T23] Swift：函数
来源：http://hz.zhongyouzk.top/gtmffxdcvp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.sysykeji.top/gtbzxcgwxt.html

[T24] Swift：闭包
来源：http://hz.aizwys.cn/gtrykcayba.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.shuidangran.top/gtpqccuxhp.html

[T25] Swift：结构体
来源：http://hz.yanxiufei.cn/gtdjcbcplu.html

struct P { var x: Int }
来源：http://hz.hfpthk.cn/gtaqwliyfl.html

[T26] Swift：类与重写
来源：http://hz.zhixingplan.top/gtrtljtsfr.html

class A: Base { override func f() {} }
来源：http://hz.sysykeji.top/gtqmcyfwjz.html

[T27] Swift：错误处理
来源：http://hz.yuanzhike.top/gtxoxeepcr.html

do { try f() } catch { print(error) }
来源：http://hz.jinqigfzy.top/gtznxcldvx.html

[T28] Swift：枚举
来源：http://hz.quarkkingdee.top/gtjosrodmy.html

enum Color { case red, green }
来源：http://hz.gogol.net.cn/gtwdulanmy.html

[T29] Swift：guard 提前返回
来源：http://hz.zhoulong.xyz/gtheqflppp.html

guard let x = opt else { return }
来源：http://hz.zdqjudy.top/gtothewzqa.html

[T30] Swift：协议
来源：http://hz.hfpthk.cn/gtrdxpmtpq.html

protocol Shape { func area() -> Double }
来源：http://hz.bjfxy.top/gtnrpbyfdy.html

[T31] Lua：Hello World
来源：http://hz.pycfn.com/gtodrohhvx.html

print("Hello")
来源：http://hz.guowangkeji.top/gtazkfmbog.html

[T32] Lua：局部变量
来源：http://hz.9152youxi.cn/gtlylkmdsp.html

local a = 1
来源：http://hz.shanyushiyangtech.top/gtlozvwtlt.html

[T33] Lua：表（数组）
来源：http://hz.ywan-chungtsiang.top/gtvlzslxiy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.guannengcc.top/gtlxzcubax.html

[T34] Lua：遍历表
来源：http://hz.nanxinkj.top/gtsafmhlgy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.9152youxi.cn/gtuvsklbci.html

[T35] Lua：字典表
来源：http://hz.chenjidiqi.icu/gtthgqknki.html

local d = { a = 1 };  d.b = 2
来源：http://hz.hnqzz.top/gtpscdtfjq.html

[T36] Lua：函数
来源：http://hz.shuidangran.top/gtnenhtazv.html

function add(a, b) return a + b end
来源：http://hz.shanyushiyangkeji.top/gtrissowar.html

[T37] Lua：字符串拼接
来源：http://hz.svipenyu.cn/gtcrjlvngm.html

"a" .. "b"
来源：http://hz.yueranfly.top/gtqmbpufba.html

[T38] Lua：条件
来源：http://hz.aizwys.cn/gtiuhzjvsx.html

if x > 0 then print("正") end
来源：http://hz.xinyue.icu/gtoeejrrag.html

[T39] Lua：模式匹配
来源：http://hz.haohaochexian.top/gtooambmfq.html

string.find(s, "%d+")
来源：http://hz.nwbrower.top/gtmmcvkmnq.html

[T40] Lua：元表
来源：http://hz.ydzc1.top/gtgszpxpya.html

setmetatable({}, { __index = base })
来源：http://hz.hysaishi.cn/gtvfcdmoeu.html

[T41] Perl：Hello World
来源：http://hz.c1oappe.top/gtfitvwcnj.html

print "Hello\n";
来源：http://hz.yvedp.cn/gtrwrqatjr.html

[T42] Perl：变量类型
来源：http://hz.chenjidiqi.icu/gtrnwyeobo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.ydjk.org.cn/gtrwubsvvp.html

[T43] Perl：字符串插值
来源：http://hz.shangyingyoupin.top/gtpdnormkb.html

"值: $a"
来源：http://hz.yuanzhike.top/gtmkmhxqla.html

[T44] Perl：条件
来源：http://hz.meibo888.top/gtjcbormal.html

if ($a > 0) { print "正"; }
来源：http://hz.svipenyu.cn/gtdklgxakj.html

[T45] Perl：数组遍历
来源：http://hz.hnxiangtu.top/gtbfkmsidn.html

for my $x (@arr) { print $x; }
来源：http://hz.yj20258.top/gteldemfgh.html

[T46] Perl：哈希操作
来源：http://hz.sxryk.cn/gtiiukhpnb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.xuanzx.com/gtfeiemssr.html

[T47] Perl：正则捕获
来源：http://hz.jinghuilouyu.cn/gtgmwcqrwo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.ydjk.org.cn/gthzelafjk.html

[T48] Perl：正则替换
来源：http://hz.dashuyun.cn/gtzgqurlvo.html

$s =~ s/old/new/g;
来源：http://hz.chenjidiqi.icu/gtzacfgthy.html


<!-- 参考信息 -->